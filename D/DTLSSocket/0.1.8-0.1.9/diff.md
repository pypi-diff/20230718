# Comparing `tmp/DTLSSocket-0.1.8.tar.gz` & `tmp/DTLSSocket-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DTLSSocket-0.1.8.tar", last modified: Fri Dec  7 18:34:37 2018, max compression
+gzip compressed data, was "dist/DTLSSocket-0.1.9.tar", last modified: Fri Dec  7 19:58:50 2018, max compression
```

## Comparing `DTLSSocket-0.1.8.tar` & `DTLSSocket-0.1.9.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/
-drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket/
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     4962 2018-12-07 17:55:42.000000 DTLSSocket-0.1.8/DTLSSocket/DTLSSocket.py
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)       49 2018-12-07 17:55:42.000000 DTLSSocket-0.1.8/DTLSSocket/__init__.py
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     9461 2018-12-07 17:55:42.000000 DTLSSocket-0.1.8/DTLSSocket/dtls.pyx
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3370 2018-12-07 17:55:42.000000 DTLSSocket-0.1.8/DTLSSocket/tdtls.pxd
-drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2471 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/ABOUT.md
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3677 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/CONTRIBUTING.md
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      798 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/LICENSE
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3572 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/Makefile.in
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      842 2018-12-07 18:28:48.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/README
-drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/aes/
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1713 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/aes/Makefile.in
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    59392 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/aes/rijndael.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2631 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/aes/rijndael.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2881 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/alert.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     8662 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/ccm.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2628 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/ccm.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3353 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/configure.ac
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    15446 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/crypto.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    13408 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/crypto.h
-drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/doc/
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    65464 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/doc/Doxyfile.in
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      671 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/doc/Makefile.in
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)   126287 2018-12-07 18:28:48.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    26646 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3927 2018-12-07 17:56:07.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls_config.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     8084 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls_debug.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3929 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls_debug.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1687 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls_time.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1534 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls_time.h
-drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/ecc/
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2147 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/ecc/Makefile.in
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     4179 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/ecc/ecc.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2200 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/ecc/test_helper.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     4073 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/global.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3903 2018-12-07 18:28:48.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/hmac.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     4707 2018-12-07 18:28:48.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/hmac.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2763 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/netq.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3428 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/netq.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3577 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/numeric.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2160 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/peer.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     4341 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/peer.h
-drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/platform-specific/
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      475 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/platform-specific/Makefile.in
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2046 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/platform-specific/platform.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2404 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/prng.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2168 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/session.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1857 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/session.h
-drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/sha2/
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1890 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/sha2/Makefile.in
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    12045 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/sha2/README
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    33510 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/sha2/sha2.c
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     7232 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/sha2/sha2.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1922 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/state.h
-drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/tests/
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1877 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/tests/Makefile.in
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1134 2018-12-07 17:56:05.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/tinydtls.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    77655 2018-12-07 18:28:48.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/uthash.h
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    81494 2018-12-07 18:28:48.000000 DTLSSocket-0.1.8/DTLSSocket/tinydtls/utlist.h
-drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket.egg-info/
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      308 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket.egg-info/PKG-INFO
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1778 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket.egg-info/SOURCES.txt
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)        1 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket.egg-info/dependency_links.txt
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)       11 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/DTLSSocket.egg-info/top_level.txt
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1495 2018-12-07 17:55:42.000000 DTLSSocket-0.1.8/LICENSE
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      180 2018-12-07 17:55:42.000000 DTLSSocket-0.1.8/MANIFEST.in
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      308 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/PKG-INFO
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      407 2018-12-07 17:55:42.000000 DTLSSocket-0.1.8/README
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)       38 2018-12-07 18:34:37.000000 DTLSSocket-0.1.8/setup.cfg
--rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2307 2018-12-07 18:34:36.000000 DTLSSocket-0.1.8/setup.py
+drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/
+drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket/
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     4962 2017-05-03 09:16:57.000000 DTLSSocket-0.1.9/DTLSSocket/DTLSSocket.py
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)       49 2017-05-03 09:15:01.000000 DTLSSocket-0.1.9/DTLSSocket/__init__.py
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)   434048 2017-12-15 23:26:40.000000 DTLSSocket-0.1.9/DTLSSocket/dtls.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     9461 2017-04-25 17:44:41.000000 DTLSSocket-0.1.9/DTLSSocket/dtls.pyx
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3370 2017-04-25 17:44:02.000000 DTLSSocket-0.1.9/DTLSSocket/tdtls.pxd
+drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2471 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/ABOUT.md
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3677 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/CONTRIBUTING.md
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      798 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/LICENSE
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3572 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/Makefile.in
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      842 2018-12-07 19:55:36.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/README
+drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/aes/
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1713 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/aes/Makefile.in
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    59392 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/aes/rijndael.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2631 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/aes/rijndael.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2881 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/alert.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     8662 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/ccm.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2628 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/ccm.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3353 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/configure.ac
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    15446 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/crypto.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    13408 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/crypto.h
+drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/doc/
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    65464 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/doc/Doxyfile.in
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      671 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/doc/Makefile.in
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)   126287 2018-12-07 19:55:36.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    26646 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3927 2017-04-26 09:19:32.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls_config.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     8084 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls_debug.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3929 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls_debug.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1687 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls_time.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1534 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls_time.h
+drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/ecc/
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2147 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/ecc/Makefile.in
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     4179 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/ecc/ecc.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2200 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/ecc/test_helper.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     4073 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/global.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3903 2018-12-07 19:55:36.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/hmac.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     4707 2018-12-07 19:55:36.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/hmac.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2763 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/netq.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3428 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/netq.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     3577 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/numeric.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2160 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/peer.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     4341 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/peer.h
+drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/platform-specific/
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      475 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/platform-specific/Makefile.in
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2046 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/platform-specific/platform.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2404 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/prng.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2168 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/session.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1857 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/session.h
+drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/sha2/
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1890 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/sha2/Makefile.in
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    12045 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/sha2/README
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    33510 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/sha2/sha2.c
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     7232 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/sha2/sha2.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1922 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/state.h
+drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/tests/
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1877 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/tests/Makefile.in
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1134 2017-04-26 09:19:23.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/tinydtls.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    77655 2018-12-07 19:55:36.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/uthash.h
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)    81494 2018-12-07 19:55:36.000000 DTLSSocket-0.1.9/DTLSSocket/tinydtls/utlist.h
+drwxr-xr-x   0 kabelaffe   (500) kabelaffe  (1000)        0 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket.egg-info/
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      308 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket.egg-info/PKG-INFO
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1829 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket.egg-info/SOURCES.txt
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)        1 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket.egg-info/dependency_links.txt
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)        7 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket.egg-info/requires.txt
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)       11 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/DTLSSocket.egg-info/top_level.txt
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     1495 2017-05-02 12:40:00.000000 DTLSSocket-0.1.9/LICENSE
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      180 2017-09-15 09:03:54.000000 DTLSSocket-0.1.9/MANIFEST.in
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      308 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/PKG-INFO
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)      407 2017-05-03 10:17:49.000000 DTLSSocket-0.1.9/README
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)       38 2018-12-07 19:58:50.000000 DTLSSocket-0.1.9/setup.cfg
+-rw-r--r--   0 kabelaffe   (500) kabelaffe  (1000)     2406 2018-12-07 19:54:07.000000 DTLSSocket-0.1.9/setup.py
```

### Comparing `DTLSSocket-0.1.8/DTLSSocket/DTLSSocket.py` & `DTLSSocket-0.1.9/DTLSSocket/DTLSSocket.py`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/dtls.pyx` & `DTLSSocket-0.1.9/DTLSSocket/dtls.pyx`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tdtls.pxd` & `DTLSSocket-0.1.9/DTLSSocket/tdtls.pxd`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/ABOUT.md` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/ABOUT.md`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/CONTRIBUTING.md` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/LICENSE` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/LICENSE`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/Makefile.in` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/Makefile.in`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/README` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/README`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/aes/Makefile.in` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/aes/Makefile.in`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/aes/rijndael.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/aes/rijndael.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/aes/rijndael.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/aes/rijndael.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/alert.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/alert.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/ccm.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/ccm.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/ccm.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/ccm.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/configure.ac` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/configure.ac`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/crypto.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/crypto.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/crypto.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/crypto.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/doc/Doxyfile.in` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/doc/Makefile.in` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/doc/Makefile.in`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls_config.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls_config.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls_debug.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls_debug.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls_debug.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls_debug.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls_time.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls_time.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/dtls_time.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/dtls_time.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/ecc/Makefile.in` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/ecc/Makefile.in`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/ecc/ecc.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/ecc/ecc.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/ecc/test_helper.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/ecc/test_helper.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/global.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/global.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/hmac.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/hmac.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/hmac.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/hmac.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/netq.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/netq.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/netq.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/netq.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/numeric.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/numeric.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/peer.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/peer.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/peer.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/peer.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/platform-specific/platform.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/platform-specific/platform.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/prng.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/prng.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/session.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/session.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/session.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/session.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/sha2/Makefile.in` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/sha2/Makefile.in`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/sha2/README` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/sha2/README`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/sha2/sha2.c` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/sha2/sha2.c`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/sha2/sha2.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/sha2/sha2.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/state.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/state.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/tests/Makefile.in` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/tests/Makefile.in`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/tinydtls.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/tinydtls.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/uthash.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/uthash.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket/tinydtls/utlist.h` & `DTLSSocket-0.1.9/DTLSSocket/tinydtls/utlist.h`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/DTLSSocket.egg-info/SOURCES.txt` & `DTLSSocket-0.1.9/DTLSSocket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 MANIFEST.in
 README
 setup.py
 DTLSSocket/DTLSSocket.py
 DTLSSocket/__init__.py
+DTLSSocket/dtls.c
 DTLSSocket/dtls.pyx
 DTLSSocket/tdtls.pxd
 DTLSSocket.egg-info/PKG-INFO
 DTLSSocket.egg-info/SOURCES.txt
 DTLSSocket.egg-info/dependency_links.txt
+DTLSSocket.egg-info/requires.txt
 DTLSSocket.egg-info/top_level.txt
 DTLSSocket/tinydtls/ABOUT.md
 DTLSSocket/tinydtls/CONTRIBUTING.md
 DTLSSocket/tinydtls/LICENSE
 DTLSSocket/tinydtls/Makefile.in
 DTLSSocket/tinydtls/README
 DTLSSocket/tinydtls/alert.h
```

### Comparing `DTLSSocket-0.1.8/LICENSE` & `DTLSSocket-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `DTLSSocket-0.1.8/setup.py` & `DTLSSocket-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,23 @@
             run_command(["git", "submodule", "update", "--init"])
         for command in commands:
             run_command(command)
         build_ext.run(self)
 
 setup(
     name="DTLSSocket",
-    version='0.1.8',
+    version='0.1.9',
     description = "DTLSSocket is a cython wrapper for tinydtls with a Socket like interface",
     author      = "Jannis Konrad",
     author_email= "Jannis.Konrad@h-brs.de",
     url         = "https://git.fslab.de/jkonra2m/tinydtls-cython",
     py_modules  = [ "DTLSSocket.DTLSSocket"],
     cmdclass    = {"build_ext": prepare_tinydtls},
-    setup_requires = [ "cython", ],
+    setup_requires = ['setuptools>=18.0','Cython'],
+    install_requires = ['Cython'],
     ext_modules = [Extension("DTLSSocket.dtls",
                 [
                  "DTLSSocket/dtls.pyx",
                  "DTLSSocket/tinydtls/ccm.c",
                  "DTLSSocket/tinydtls/crypto.c",
                  "DTLSSocket/tinydtls/dtls.c",
                  "DTLSSocket/tinydtls/dtls_debug.c",
@@ -47,12 +48,12 @@
                  "DTLSSocket/tinydtls/sha2/sha2.c"
                  ],
                 include_dirs=['DTLSSocket/tinydtls'],
                 define_macros=[('DTLSv12', '1'),
                                ('WITH_SHA256', '1'),
                                ('DTLS_CHECK_CONTENTTYPE', '1'),
                                ('_GNU_SOURCE', '1'),
-			       ('NDEBUG', '1'),
-				],
+                                ('NDEBUG', '1'),
+                              ],
 #                undef_macros = [ "NDEBUG" ],
                 ),]
     )
```

