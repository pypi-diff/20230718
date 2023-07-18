# Comparing `tmp/slapcache-0.1.7.tar.gz` & `tmp/slapcache-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slapcache-0.1.7.tar", last modified: Wed Mar 30 10:40:31 2022, max compression
+gzip compressed data, was "slapcache-0.1.9.tar", last modified: Thu Jun  2 14:33:41 2022, max compression
```

## Comparing `slapcache-0.1.7.tar` & `slapcache-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2022-03-30 10:40:31.611856 slapcache-0.1.7/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1053 2022-03-30 10:40:26.000000 slapcache-0.1.7/CHANGES.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)       68 2019-02-04 11:35:29.000000 slapcache-0.1.7/MANIFEST.in
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1689 2022-03-30 10:40:31.611856 slapcache-0.1.7/PKG-INFO
--rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-02-04 11:35:29.000000 slapcache-0.1.7/README.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)       38 2022-03-30 10:40:31.611856 slapcache-0.1.7/setup.cfg
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1115 2022-03-30 10:40:26.000000 slapcache-0.1.7/setup.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2022-03-30 10:40:31.603856 slapcache-0.1.7/slapcache/
--rw-r--r--   0 tomo      (1000) tomo      (1000)      244 2019-02-04 11:35:29.000000 slapcache-0.1.7/slapcache/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     3569 2019-07-15 15:35:56.000000 slapcache-0.1.7/slapcache/conf.py
--rwxr-xr-x   0 tomo      (1000) tomo      (1000)     2416 2021-03-15 10:25:00.000000 slapcache-0.1.7/slapcache/download.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     9419 2022-03-30 10:40:26.000000 slapcache-0.1.7/slapcache/signature.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2022-03-30 10:40:31.607856 slapcache-0.1.7/slapcache/template/
--rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-02-04 11:35:29.000000 slapcache-0.1.7/slapcache/template/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1040 2022-03-30 10:40:26.000000 slapcache-0.1.7/slapcache/template/update.cfg.in
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2022-03-30 10:40:31.611856 slapcache-0.1.7/slapcache/test/
--rw-r--r--   0 tomo      (1000) tomo      (1000)    12968 2020-11-03 16:23:03.000000 slapcache-0.1.7/slapcache/test/test_signature.py
--rwxr-xr-x   0 tomo      (1000) tomo      (1000)     2815 2020-11-03 17:08:19.000000 slapcache-0.1.7/slapcache/upload.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2022-03-30 10:40:31.607856 slapcache-0.1.7/slapcache.egg-info/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1689 2022-03-30 10:40:31.000000 slapcache-0.1.7/slapcache.egg-info/PKG-INFO
--rw-r--r--   0 tomo      (1000) tomo      (1000)      519 2022-03-30 10:40:31.000000 slapcache-0.1.7/slapcache.egg-info/SOURCES.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2022-03-30 10:40:31.000000 slapcache-0.1.7/slapcache.egg-info/dependency_links.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)      145 2022-03-30 10:40:31.000000 slapcache-0.1.7/slapcache.egg-info/entry_points.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)       10 2022-03-30 10:40:31.000000 slapcache-0.1.7/slapcache.egg-info/namespace_packages.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2019-07-15 15:07:56.000000 slapcache-0.1.7/slapcache.egg-info/not-zip-safe
--rw-r--r--   0 tomo      (1000) tomo      (1000)       44 2022-03-30 10:40:31.000000 slapcache-0.1.7/slapcache.egg-info/requires.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)       10 2022-03-30 10:40:31.000000 slapcache-0.1.7/slapcache.egg-info/top_level.txt
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2022-06-02 14:33:41.220034 slapcache-0.1.9/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1309 2022-06-02 14:32:12.000000 slapcache-0.1.9/CHANGES.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)       68 2019-02-04 11:35:29.000000 slapcache-0.1.9/MANIFEST.in
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2025 2022-06-02 14:33:41.220034 slapcache-0.1.9/PKG-INFO
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-02-04 11:35:29.000000 slapcache-0.1.9/README.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)       38 2022-06-02 14:33:41.220034 slapcache-0.1.9/setup.cfg
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1115 2022-06-02 14:32:31.000000 slapcache-0.1.9/setup.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2022-06-02 14:33:41.212034 slapcache-0.1.9/slapcache/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      244 2019-02-04 11:35:29.000000 slapcache-0.1.9/slapcache/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     3569 2019-07-15 15:35:56.000000 slapcache-0.1.9/slapcache/conf.py
+-rwxr-xr-x   0 tomo      (1000) tomo      (1000)     2416 2021-03-15 10:25:00.000000 slapcache-0.1.9/slapcache/download.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     9497 2022-06-02 14:28:33.000000 slapcache-0.1.9/slapcache/signature.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2022-06-02 14:33:41.216034 slapcache-0.1.9/slapcache/template/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        0 2019-02-04 11:35:29.000000 slapcache-0.1.9/slapcache/template/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1084 2022-06-02 14:29:26.000000 slapcache-0.1.9/slapcache/template/update.cfg.in
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2022-06-02 14:33:41.216034 slapcache-0.1.9/slapcache/test/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)    11511 2022-06-02 14:28:33.000000 slapcache-0.1.9/slapcache/test/test_signature.py
+-rwxr-xr-x   0 tomo      (1000) tomo      (1000)     2815 2020-11-03 17:08:19.000000 slapcache-0.1.9/slapcache/upload.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2022-06-02 14:33:41.216034 slapcache-0.1.9/slapcache.egg-info/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2025 2022-06-02 14:33:40.000000 slapcache-0.1.9/slapcache.egg-info/PKG-INFO
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      519 2022-06-02 14:33:40.000000 slapcache-0.1.9/slapcache.egg-info/SOURCES.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2022-06-02 14:33:40.000000 slapcache-0.1.9/slapcache.egg-info/dependency_links.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      145 2022-06-02 14:33:40.000000 slapcache-0.1.9/slapcache.egg-info/entry_points.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)       10 2022-06-02 14:33:40.000000 slapcache-0.1.9/slapcache.egg-info/namespace_packages.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2019-07-15 15:07:56.000000 slapcache-0.1.9/slapcache.egg-info/not-zip-safe
+-rw-r--r--   0 tomo      (1000) tomo      (1000)       44 2022-06-02 14:33:40.000000 slapcache-0.1.9/slapcache.egg-info/requires.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)       10 2022-06-02 14:33:40.000000 slapcache-0.1.9/slapcache.egg-info/top_level.txt
```

### Comparing `slapcache-0.1.7/CHANGES.txt` & `slapcache-0.1.9/CHANGES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes
 ========
 
+0.1.9 (2022-06-02)
+------------------
+
+ * Add missing "download-dir-url" entry in generated /etc/opt/slapcache.cfg [Thomas Gambier]
+
+0.1.8 (2022-03-31)
+------------------
+
+ * fix upload command after new release of slapos.libnetworkcache [Thomas Gambier]
+
 0.1.7 (2022-03-30)
 ------------------
 
  * inform user about dropped option signature_private_key_file [Łukasz Nowak]
  * expose SHA512SUM on successful upload [Łukasz Nowak]
  * update shacache default URL [Łukasz Nowak]
  * fix tests after the signature-private-key-file option change [Thomas Gambier]
```

### Comparing `slapcache-0.1.7/PKG-INFO` & `slapcache-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 Metadata-Version: 1.1
 Name: slapcache
-Version: 0.1.7
+Version: 0.1.9
 Summary: SlapOS Cache Utils
 Home-page: http://www.slapos.org
 Author: VIFIB
 Author-email: UNKNOWN
 License: GPLv3
 Description: 
         Changes
         ========
         
+        0.1.9 (2022-06-02)
+        ------------------
+        
+         * Add missing "download-dir-url" entry in generated /etc/opt/slapcache.cfg [Thomas Gambier]
+        
+        0.1.8 (2022-03-31)
+        ------------------
+        
+         * fix upload command after new release of slapos.libnetworkcache [Thomas Gambier]
+        
         0.1.7 (2022-03-30)
         ------------------
         
          * inform user about dropped option signature_private_key_file [Łukasz Nowak]
          * expose SHA512SUM on successful upload [Łukasz Nowak]
          * update shacache default URL [Łukasz Nowak]
          * fix tests after the signature-private-key-file option change [Thomas Gambier]
```

### Comparing `slapcache-0.1.7/setup.py` & `slapcache-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '0.1.7'
+version = '0.1.9'
 name = 'slapcache'
 long_description = open("README.txt").read() + "\n" + \
     open("CHANGES.txt").read() + "\n"
 
 setup(name=name,
       version=version,
       description="SlapOS Cache Utils",
```

### Comparing `slapcache-0.1.7/slapcache/conf.py` & `slapcache-0.1.9/slapcache/conf.py`

 * *Files identical despite different names*

### Comparing `slapcache-0.1.7/slapcache/download.py` & `slapcache-0.1.9/slapcache/download.py`

 * *Files identical despite different names*

### Comparing `slapcache-0.1.7/slapcache/signature.py` & `slapcache-0.1.9/slapcache/signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     # backward compatibility
     metadata_dict.setdefault('file', 'notused')
     metadata_dict.setdefault('urlmd5', 'notused')
 
     # convert '' into None in order to call nc nicely
     with NetworkcacheClient(self.cache_url, self.dir_url,
           signature_private_key_file=self.signature_private_key_file or None,
+          signature_certificate_list=self.signature_certificate_list or None,
           shacache_ca_file=self.shacache_ca_file or None,
           shacache_cert_file=self.shacache_cert_file or None,
           shacache_key_file=self.shacache_key_file or None,
           shadir_cert_file=self.shadir_cert_file or None,
           shadir_key_file=self.shadir_key_file or None,
           shadir_ca_file=self.shadir_ca_file or None,
```

### Comparing `slapcache-0.1.7/slapcache/template/update.cfg.in` & `slapcache-0.1.9/slapcache/template/update.cfg.in`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [shacache]
 key = %(key)s
 
 [networkcache]
 download-binary-cache-url = http://shacache.nxdcdn.com
 download-cache-url = https://shacache.nxdcdn.com
 download-binary-dir-url = http://shadir.nxdcdn.com
+download-dir-url = http://shadir.nxdcdn.com
 
 # Standard Signature handled by SlapOS Administrators
 signature-certificate-list =
   -----BEGIN CERTIFICATE-----
   MIIB8DCCAVmgAwIBAgIJAPFf61p8y809MA0GCSqGSIb3DQEBBQUAMBAxDjAMBgNV
   BAMMBUNPTVAtMCAXDTE0MDIxNzE2NDgxN1oYDzIxMTQwMTI0MTY0ODE3WjAQMQ4w
   DAYDVQQDDAVDT01QLTCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAsiqCyuv1
```

### Comparing `slapcache-0.1.7/slapcache/test/test_signature.py` & `slapcache-0.1.9/slapcache/test/test_signature.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,41 +7,14 @@
 from slapcache import signature
 from slapos.libnetworkcache import NetworkcacheClient
 from optparse import Values
 import slapos.signature, time, difflib, tempfile, unittest, os
 def _fake_call(self, *args, **kw):
   self.last_call = (args, kw)
 
-CONFIGURATION_FILE = """
-
-[networkcache]
-download-binary-cache-url = http://www.shacache.org/shacache
-download-cache-url = https://www.shacache.org/shacache
-download-binary-dir-url = http://www.shacache.org/shadir
-
-signature-certificate-list =
-  -----BEGIN CERTIFICATE-----
-  MIIB8DCCAVmgAwIBAgIJAPFf61p8y809MA0GCSqGSIb3DQEBBQUAMBAxDjAMBgNV
-  BAMMBUNPTVAtMCAXDTE0MDIxNzE2NDgxN1oYDzIxMTQwMTI0MTY0ODE3WjAQMQ4w
-  DAYDVQQDDAVDT01QLTCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAsiqCyuv1
-  HO9FmtwnMbEa1/u8Dn7T0k7hVKYXVQYof+59Ltbb3cA3nLjFSJDr/wQT6N89MccS
-  PneRzkWqZKL06Kmj+N+XJfRyVaTz1qQtNzjdbYkO6RgQq+fvq2CO0+PSnL6NttLU
-  /a9nQMcVm7wZ8kmY+AG5LbVo8lmxDD16Wq0CAwEAAaNQME4wHQYDVR0OBBYEFEVi
-  YyWHF3W7/O4NaTjn4lElLpp7MB8GA1UdIwQYMBaAFEViYyWHF3W7/O4NaTjn4lEl
-  Lpp7MAwGA1UdEwQFMAMBAf8wDQYJKoZIhvcNAQEFBQADgYEAgIPGoxhUa16AgjZx
-  Jr1kUrs8Fg3ig8eRFQlBSLYfANIUxcQ2ScFAkmsvwXY3Md7uaSvMJsEl2jcjdmdi
-  eSreNkx85j9GtMLY/2cv0kF4yAQNRtibtDkbg6fRNkmUopDosJNVf79l1GKX8JFL
-  zZBOFdOaLYY/6dLRwiTUKHU6su8=
-  -----END CERTIFICATE-----
-
-[shacache]
-key = slapos-upgrade-testing-key-with-config-file
-
-"""
-
 UPGRADE_KEY = """[debian-default]
 repository-list = 
 	main = http://ftp.fr.debian.org/debian/ wheezy main
 	main-src = http://ftp.fr.debian.org/debian/ wheezy main
 	update = http://ftp.fr.debian.org/debian/ wheezy-updates main
 	update-src = http://ftp.fr.debian.org/debian/ wheezy-updates main
 	slapos = http://download.opensuse.org/repositories/home:/VIFIBnexedi:/branches:/home:/VIFIBnexedi/Debian_7.0/ ./
@@ -126,16 +99,15 @@
 [system]
 reboot = 2011-10-10
 upgrade = 2014-06-04
 
 """
 
 
-SIGNATURE = """
------BEGIN CERTIFICATE-----
+SIGNATURE = """-----BEGIN CERTIFICATE-----
 MIIB8DCCAVmgAwIBAgIJAPFf61p8y809MA0GCSqGSIb3DQEBBQUAMBAxDjAMBgNV
 BAMMBUNPTVAtMCAXDTE0MDIxNzE2NDgxN1oYDzIxMTQwMTI0MTY0ODE3WjAQMQ4w
 DAYDVQQDDAVDT01QLTCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAsiqCyuv1
 HO9FmtwnMbEa1/u8Dn7T0k7hVKYXVQYof+59Ltbb3cA3nLjFSJDr/wQT6N89MccS
 PneRzkWqZKL06Kmj+N+XJfRyVaTz1qQtNzjdbYkO6RgQq+fvq2CO0+PSnL6NttLU
 /a9nQMcVm7wZ8kmY+AG5LbVo8lmxDD16Wq0CAwEAAaNQME4wHQYDVR0OBBYEFEVi
 YyWHF3W7/O4NaTjn4lElLpp7MB8GA1UdIwQYMBaAFEViYyWHF3W7/O4NaTjn4lEl
@@ -146,30 +118,14 @@
 -----END CERTIFICATE-----"""
 BASE_UPDATE_CFG_DATA = """
 
 [networkcache]
 download-binary-cache-url = http://www.shacache.org/shacache
 download-cache-url = https://www.shacache.org/shacache
 download-binary-dir-url = http://www.shacache.org/shadir
-
-signature-certificate-list = 
-  -----BEGIN CERTIFICATE-----
-  MIIB8DCCAVmgAwIBAgIJAPFf61p8y809MA0GCSqGSIb3DQEBBQUAMBAxDjAMBgNV
-  BAMMBUNPTVAtMCAXDTE0MDIxNzE2NDgxN1oYDzIxMTQwMTI0MTY0ODE3WjAQMQ4w
-  DAYDVQQDDAVDT01QLTCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAsiqCyuv1
-  HO9FmtwnMbEa1/u8Dn7T0k7hVKYXVQYof+59Ltbb3cA3nLjFSJDr/wQT6N89MccS
-  PneRzkWqZKL06Kmj+N+XJfRyVaTz1qQtNzjdbYkO6RgQq+fvq2CO0+PSnL6NttLU
-  /a9nQMcVm7wZ8kmY+AG5LbVo8lmxDD16Wq0CAwEAAaNQME4wHQYDVR0OBBYEFEVi
-  YyWHF3W7/O4NaTjn4lElLpp7MB8GA1UdIwQYMBaAFEViYyWHF3W7/O4NaTjn4lEl
-  Lpp7MAwGA1UdEwQFMAMBAf8wDQYJKoZIhvcNAQEFBQADgYEAgIPGoxhUa16AgjZx
-  Jr1kUrs8Fg3ig8eRFQlBSLYfANIUxcQ2ScFAkmsvwXY3Md7uaSvMJsEl2jcjdmdi
-  eSreNkx85j9GtMLY/2cv0kF4yAQNRtibtDkbg6fRNkmUopDosJNVf79l1GKX8JFL
-  zZBOFdOaLYY/6dLRwiTUKHU6su8=
-  -----END CERTIFICATE-----
-
 """
 UPDATE_CFG_DATA = """
 [shacache]
 key = slapos-upgrade-testing-key-with-config-file-invalid
 
 """ + BASE_UPDATE_CFG_DATA
 UPDATE_UPLOAD_CFG_DATA = """
@@ -180,15 +136,14 @@
 VALID_UPDATE_CFG_DATA = """
 [shacache]
 key = 'slapos-upgrade-testing-key-with-config-file-valid' 
 
 """ + BASE_UPDATE_CFG_DATA
 UPDATE_CFG_WITH_UPLOAD_DATA = UPDATE_CFG_DATA + """
 signature-private-key-file = /etc/opt/slapos/signature.key
-signature-certificate-file = /etc/opt/slapos/signature.cert
 upload-cache-url = https://www.shacache.org/shacache
 shacache-cert-file = /etc/opt/slapos/shacache.crt
 shacache-key-file = /etc/opt/slapos/shacache.key
 upload-dir-url = https://www.shacache.org/shadir
 shadir-cert-file = /etc/opt/slapos/shacache.crt
 shadir-key-file = /etc/opt/slapos/shacache.key
 """
@@ -213,17 +168,20 @@
     def _createConfigurationFile(self):
         with open('/tmp/test_signature_000000_configuration.cfg', 'w') as (configuration_file):
             configuration_file.write(VALID_UPDATE_CFG_DATA)
         return '/tmp/test_signature_000000_configuration.cfg'
 
     def test_basic_configuration(self):
         info, self.configuration_file_path = tempfile.mkstemp()
-        open(self.configuration_file_path, 'w').write(UPDATE_CFG_DATA)
+        configuration_content = UPDATE_CFG_DATA + """
+signature-certificate-list = %(certificate)s
+""" % {'certificate': '\n'.join('  ' + l if l.strip() else '\n' for l in SIGNATURE.splitlines())}
+        print(configuration_content)
+        open(self.configuration_file_path, 'w').write(configuration_content)
         shacache = signature.NetworkCache(self.configuration_file_path)
-        print(self.configuration_file_path)
         self.assertEqual(shacache.download_binary_cache_url, 'http://www.shacache.org/shacache')
         self.assertEqual(shacache.download_cache_url, 'https://www.shacache.org/shacache')
         self.assertEqual(shacache.download_binary_dir_url, 'http://www.shacache.org/shadir')
         self.assertEqual(shacache.signature_certificate_list, SIGNATURE)
         self.assertEqual(shacache.directory_key, 'slapos-upgrade-testing-key-with-config-file-invalid')
         self.assertEqual(shacache.dir_url, None)
         self.assertEqual(shacache.cache_url, None)
@@ -232,15 +190,18 @@
         self.assertEqual(shacache.shacache_key_file, None)
         self.assertEqual(shacache.shadir_cert_file, None)
         self.assertEqual(shacache.shadir_key_file, None)
         return
 
     def test_basic_configuration_with_upload(self):
         info, self.configuration_file_path = tempfile.mkstemp()
-        open(self.configuration_file_path, 'w').write(UPDATE_CFG_WITH_UPLOAD_DATA)
+        configuration_content = UPDATE_CFG_WITH_UPLOAD_DATA + """
+signature-certificate-list = %(certificate)s
+""" % {'certificate': '\n'.join('  ' + l if l.strip() else '\n' for l in SIGNATURE.splitlines())}
+        open(self.configuration_file_path, 'w').write(configuration_content)
         shacache = signature.NetworkCache(self.configuration_file_path)
         self.assertEqual(shacache.download_binary_cache_url, 'http://www.shacache.org/shacache')
         self.assertEqual(shacache.download_cache_url, 'https://www.shacache.org/shacache')
         self.assertEqual(shacache.download_binary_dir_url, 'http://www.shacache.org/shadir')
         self.assertEqual(shacache.signature_certificate_list, SIGNATURE)
         self.assertEqual(shacache.directory_key, 'slapos-upgrade-testing-key-with-config-file-invalid')
         self.assertEqual(shacache.dir_url, 'https://www.shacache.org/shadir')
@@ -282,23 +243,27 @@
             os.remove(signature_certificate_file)
         signature_private_key_file = '/tmp/signature_private_key_file_demo_test'
         if os.path.exists(signature_private_key_file):
             os.remove(signature_private_key_file)
         slapos.signature.generateCertificate(signature_certificate_file, signature_private_key_file, 'COMP-123A')
         configuration_content = UPDATE_UPLOAD_CFG_DATA + """
 signature-private-key-file = %(signature_private_key_file)s
-signature-certificate-file = %(signature_certificate_file)s
 upload-cache-url = https://www.shacache.org/shacache
 shacache-cert-file = %(tempfile)s
 shacache-key-file = %(tempfile)s
 upload-dir-url = https://www.shacache.org/shadir
 shadir-cert-file = %(tempfile)s
 shadir-key-file = %(tempfile)s
-""" % {'tempfile': _fake_signature_path, 'signature_certificate_file': signature_certificate_file, 
-           'signature_private_key_file': signature_private_key_file}
+signature-certificate-list =
+  %(certificate)s
+""" % {
+        'tempfile': _fake_signature_path,
+        'signature_private_key_file': signature_private_key_file,
+        'certificate': ''.join('  ' + l if l.strip() else '\n' for l in open(signature_certificate_file, 'r').readlines())
+        }
         open(self.configuration_file_path, 'w').write(configuration_content)
         open(_fake_signature_path, 'w').write('# XXX ...')
         shacache = signature.NetworkCache(self.configuration_file_path)
         metadata_dict = {'timestamp': time.time()}
         shacache.upload(path=path, metadata_dict=metadata_dict)
 
     def test_signature_strategy(self):
```

### Comparing `slapcache-0.1.7/slapcache/upload.py` & `slapcache-0.1.9/slapcache/upload.py`

 * *Files identical despite different names*

### Comparing `slapcache-0.1.7/slapcache.egg-info/PKG-INFO` & `slapcache-0.1.9/slapcache.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 Metadata-Version: 1.1
 Name: slapcache
-Version: 0.1.7
+Version: 0.1.9
 Summary: SlapOS Cache Utils
 Home-page: http://www.slapos.org
 Author: VIFIB
 Author-email: UNKNOWN
 License: GPLv3
 Description: 
         Changes
         ========
         
+        0.1.9 (2022-06-02)
+        ------------------
+        
+         * Add missing "download-dir-url" entry in generated /etc/opt/slapcache.cfg [Thomas Gambier]
+        
+        0.1.8 (2022-03-31)
+        ------------------
+        
+         * fix upload command after new release of slapos.libnetworkcache [Thomas Gambier]
+        
         0.1.7 (2022-03-30)
         ------------------
         
          * inform user about dropped option signature_private_key_file [Łukasz Nowak]
          * expose SHA512SUM on successful upload [Łukasz Nowak]
          * update shacache default URL [Łukasz Nowak]
          * fix tests after the signature-private-key-file option change [Thomas Gambier]
```

### Comparing `slapcache-0.1.7/slapcache.egg-info/SOURCES.txt` & `slapcache-0.1.9/slapcache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

