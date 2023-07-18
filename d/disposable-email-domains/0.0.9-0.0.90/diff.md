# Comparing `tmp/disposable-email-domains-0.0.9.tar.gz` & `tmp/disposable-email-domains-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/disposable-email-domains-0.0.9.tar", last modified: Fri Apr 28 15:38:42 2017, max compression
+gzip compressed data, was "disposable-email-domains-0.0.90.tar", last modified: Fri May 26 02:48:17 2023, max compression
```

## Comparing `disposable-email-domains-0.0.9.tar` & `disposable-email-domains-0.0.90.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 di         (501) staff       (20)        0 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/
-drwxr-xr-x   0 di         (501) staff       (20)        0 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/bin/
--rwxr-xr-x   0 di         (501) staff       (20)      702 2016-10-19 20:35:33.000000 disposable-email-domains-0.0.9/bin/check_for_differences
--rw-r--r--   0 di         (501) staff       (20)      441 2016-10-19 20:35:33.000000 disposable-email-domains-0.0.9/bin/parse_source_data
--rwxr-xr-x   0 di         (501) staff       (20)       83 2016-12-07 23:27:55.000000 disposable-email-domains-0.0.9/bin/prerelease
--rwxr-xr-x   0 di         (501) staff       (20)       79 2016-12-07 23:27:55.000000 disposable-email-domains-0.0.9/bin/release
--rwxr-xr-x   0 di         (501) staff       (20)      277 2016-12-07 23:27:55.000000 disposable-email-domains-0.0.9/bin/update
--rw-r--r--   0 di         (501) staff       (20)      284 2016-10-19 19:25:23.000000 disposable-email-domains-0.0.9/CONTRIBUTING.md
-drwxr-xr-x   0 di         (501) staff       (20)        0 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/disposable_email_domains/
--rw-r--r--   0 di         (501) staff       (20)    47196 2017-04-28 15:38:34.000000 disposable-email-domains-0.0.9/disposable_email_domains/__init__.py
-drwxr-xr-x   0 di         (501) staff       (20)        0 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/disposable_email_domains.egg-info/
--rw-r--r--   0 di         (501) staff       (20)        1 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/disposable_email_domains.egg-info/dependency_links.txt
--rw-r--r--   0 di         (501) staff       (20)     1855 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/disposable_email_domains.egg-info/PKG-INFO
--rw-r--r--   0 di         (501) staff       (20)       22 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/disposable_email_domains.egg-info/requires.txt
--rw-r--r--   0 di         (501) staff       (20)      502 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/disposable_email_domains.egg-info/SOURCES.txt
--rw-r--r--   0 di         (501) staff       (20)       25 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/disposable_email_domains.egg-info/top_level.txt
--rw-r--r--   0 di         (501) staff       (20)     1080 2016-10-19 19:25:23.000000 disposable-email-domains-0.0.9/LICENSE.txt
--rw-r--r--   0 di         (501) staff       (20)      105 2016-10-19 20:35:33.000000 disposable-email-domains-0.0.9/MANIFEST.in
--rw-r--r--   0 di         (501) staff       (20)     1855 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/PKG-INFO
--rw-r--r--   0 di         (501) staff       (20)      855 2016-11-29 21:36:57.000000 disposable-email-domains-0.0.9/README.rst
--rw-r--r--   0 di         (501) staff       (20)       67 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/setup.cfg
--rw-r--r--   0 di         (501) staff       (20)     1158 2017-04-28 15:38:34.000000 disposable-email-domains-0.0.9/setup.py
-drwxr-xr-x   0 di         (501) staff       (20)        0 2017-04-28 15:38:42.000000 disposable-email-domains-0.0.9/source_data/
--rw-r--r--   0 di         (501) staff       (20)    28682 2017-04-28 15:38:34.000000 disposable-email-domains-0.0.9/source_data/disposable_email_blacklist.conf
--rw-r--r--   0 di         (501) staff       (20)     2115 2017-04-28 15:30:09.000000 disposable-email-domains-0.0.9/source_data/whitelist.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/bin/check_for_differences
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/bin/parse_source_data
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/bin/prerelease
+-rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/bin/release
+-rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/bin/update
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/disposable_email_domains/
+-rw-r--r--   0 runner    (1001) docker     (123)    74207 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/disposable_email_domains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-26 02:48:17.000000 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-26 02:48:17.000000 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:48:17.000000 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 02:48:17.000000 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 02:48:17.000000 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/source_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/source_data/allowlist.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    45996 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/source_data/disposable_email_blocklist.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/tests/test_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/tests/test_blocklist.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `disposable-email-domains-0.0.9/disposable_email_domains.egg-info/PKG-INFO` & `disposable-email-domains-0.0.90/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: disposable-email-domains
-Version: 0.0.9
+Version: 0.0.90
 Summary: A set of disposable email domains
-Home-page: https://github.com/di/disposable-email-domains
+Home-page: https://github.com/disposable-email-domains/disposable-email-domains
 Author: Dustin Ingram
 Author-email: github@dustingram.com
 License: MIT
-Description: Disposable Email Domains
-        ========================
-        
-        This module provides a set of known disposable email domains.
-        
-        Usage
-        -----
-        
-        The blacklist is a Python ``set`` containing all domains in the blacklist:
-        
-        ::
-        
-            >>> from disposable_email_domains import blacklist
-            >>> 'bearsarefuzzy.com' in blacklist
-            True
-        
-        The domains are guaranteed to be fully lowercased and stripped of whitespace.
-        
-        Source
-        ------
-        
-        The source of this list is the `disposable-email-domains`_ project.
-        
-        .. _disposable-email-domains: https://github.com/martenson/disposable-email-domains
-        
-        This module attempts to provide a mirror of that project as a Python module.
-        
-        If you feel a domain should or shouldn't be on the blacklist, you are
-        encouraged to make a pull request against the `source repository`_.
-        
-        .. _source repository: https://github.com/martenson/disposable-email-domains
-        
-Keywords: disposable email domains blacklist
-Platform: UNKNOWN
+Keywords: disposable email domains blocklist
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+# Disposable Email Domains
+
+This module provides a set of known disposable email domains.
+
+## Usage
+
+The blocklist is a Python `set` containing all domains in the blocklist:
+
+```python
+>>> from disposable_email_domains import blocklist
+>>> 'bearsarefuzzy.com' in blocklist
+True
+```
+
+The domains are guaranteed to be fully lowercased and stripped of whitespace.
+
+## Source
+
+The source of this list is the [disposable-email-domains][1] project.
+
+This module attempts to provide a mirror of that project as a Python module.
+
+If you feel a domain should or shouldn't be on the blocklist, you are
+encouraged to make a pull request against the [source repository][2]
+
+[1]: https://github.com/disposable-email-domains/disposable-email-domains
+[2]: https://github.com/disposable-email-domains/disposable-email-domains
```

### Comparing `disposable-email-domains-0.0.9/LICENSE.txt` & `disposable-email-domains-0.0.90/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.9/PKG-INFO` & `disposable-email-domains-0.0.90/disposable_email_domains.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: disposable-email-domains
-Version: 0.0.9
+Version: 0.0.90
 Summary: A set of disposable email domains
-Home-page: https://github.com/di/disposable-email-domains
+Home-page: https://github.com/disposable-email-domains/disposable-email-domains
 Author: Dustin Ingram
 Author-email: github@dustingram.com
 License: MIT
-Description: Disposable Email Domains
-        ========================
-        
-        This module provides a set of known disposable email domains.
-        
-        Usage
-        -----
-        
-        The blacklist is a Python ``set`` containing all domains in the blacklist:
-        
-        ::
-        
-            >>> from disposable_email_domains import blacklist
-            >>> 'bearsarefuzzy.com' in blacklist
-            True
-        
-        The domains are guaranteed to be fully lowercased and stripped of whitespace.
-        
-        Source
-        ------
-        
-        The source of this list is the `disposable-email-domains`_ project.
-        
-        .. _disposable-email-domains: https://github.com/martenson/disposable-email-domains
-        
-        This module attempts to provide a mirror of that project as a Python module.
-        
-        If you feel a domain should or shouldn't be on the blacklist, you are
-        encouraged to make a pull request against the `source repository`_.
-        
-        .. _source repository: https://github.com/martenson/disposable-email-domains
-        
-Keywords: disposable email domains blacklist
-Platform: UNKNOWN
+Keywords: disposable email domains blocklist
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+# Disposable Email Domains
+
+This module provides a set of known disposable email domains.
+
+## Usage
+
+The blocklist is a Python `set` containing all domains in the blocklist:
+
+```python
+>>> from disposable_email_domains import blocklist
+>>> 'bearsarefuzzy.com' in blocklist
+True
+```
+
+The domains are guaranteed to be fully lowercased and stripped of whitespace.
+
+## Source
+
+The source of this list is the [disposable-email-domains][1] project.
+
+This module attempts to provide a mirror of that project as a Python module.
+
+If you feel a domain should or shouldn't be on the blocklist, you are
+encouraged to make a pull request against the [source repository][2]
+
+[1]: https://github.com/disposable-email-domains/disposable-email-domains
+[2]: https://github.com/disposable-email-domains/disposable-email-domains
```

### Comparing `disposable-email-domains-0.0.9/README.rst` & `disposable-email-domains-0.0.90/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-Disposable Email Domains
-========================
+# Disposable Email Domains
 
 This module provides a set of known disposable email domains.
 
-Usage
------
+## Usage
 
-The blacklist is a Python ``set`` containing all domains in the blacklist:
+The blocklist is a Python `set` containing all domains in the blocklist:
 
-::
-
-    >>> from disposable_email_domains import blacklist
-    >>> 'bearsarefuzzy.com' in blacklist
-    True
+```python
+>>> from disposable_email_domains import blocklist
+>>> 'bearsarefuzzy.com' in blocklist
+True
+```
 
 The domains are guaranteed to be fully lowercased and stripped of whitespace.
 
-Source
-------
-
-The source of this list is the `disposable-email-domains`_ project.
+## Source
 
-.. _disposable-email-domains: https://github.com/martenson/disposable-email-domains
+The source of this list is the [disposable-email-domains][1] project.
 
 This module attempts to provide a mirror of that project as a Python module.
 
-If you feel a domain should or shouldn't be on the blacklist, you are
-encouraged to make a pull request against the `source repository`_.
+If you feel a domain should or shouldn't be on the blocklist, you are
+encouraged to make a pull request against the [source repository][2]
 
-.. _source repository: https://github.com/martenson/disposable-email-domains
+[1]: https://github.com/disposable-email-domains/disposable-email-domains
+[2]: https://github.com/disposable-email-domains/disposable-email-domains
```

### Comparing `disposable-email-domains-0.0.9/setup.py` & `disposable-email-domains-0.0.90/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from setuptools import setup
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
-__version__ = '0.0.9'
+__version__ = "0.0.90"
 
-with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='disposable-email-domains',
+    name="disposable-email-domains",
     version=__version__,
-    description='A set of disposable email domains',
+    description="A set of disposable email domains",
     long_description=long_description,
-    url='https://github.com/di/disposable-email-domains',
-    author='Dustin Ingram',
-    author_email='github@dustingram.com',
-    license='MIT',
+    long_description_content_type="text/markdown",
+    url="https://github.com/disposable-email-domains/disposable-email-domains",
+    author="Dustin Ingram",
+    author_email="github@dustingram.com",
+    license="MIT",
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
-    keywords='disposable email domains blacklist',
-    packages=['disposable_email_domains'],
+    keywords="disposable email domains blocklist",
+    packages=["disposable_email_domains"],
     extras_require={
-        'dev': ['check-manifest'],
+        "dev": ["check-manifest"],
     },
 )
```

### Comparing `disposable-email-domains-0.0.9/source_data/whitelist.conf` & `disposable-email-domains-0.0.90/source_data/allowlist.conf`

 * *Files 2% similar despite different names*

```diff
@@ -112,52 +112,60 @@
 mailsent.net
 mailservice.ms
 mailup.net
 mailworks.org
 memeware.net
 ml1.net
 mm.st
+mozmail.com
 myfastmail.com
 mymacmail.com
 naver.com
 neverbox.com
 nigge.rs
 nospammail.net
+nus.edu.sg
+onet.pl
 ownmail.net
 petml.com
 postinbox.com
 postpro.net
 proinbox.com
 promessage.com
 qq.com
 realemail.net
 reallyfast.biz
 reallyfast.info
 recursor.net
 redchan.it
+ruffrey.com
 rushpost.com
 safe-mail.net
 sent.as
 sent.at
 sent.com
 shitposting.agency
+shitware.nl
 sibmail.com
+sneakemail.com
+snkmail.com
 spamcannon.com
 spamcannon.net
 spamgourmet.com
 spamgourmet.net
 spamgourmet.org
 speedpost.net
 speedymail.org
 ssl-mail.com
 swift-mail.com
 tfwno.gf
 the-fastest.net
 the-quickest.com
 theinternetemail.com
+tweakly.net
 veryfast.biz
 veryspeedy.net
 waifu.club
 warpmail.net
 xoxy.net
 xsmail.com
 yahoo.com.ph
```

