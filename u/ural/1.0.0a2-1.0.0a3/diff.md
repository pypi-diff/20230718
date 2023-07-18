# Comparing `tmp/ural-1.0.0a2.tar.gz` & `tmp/ural-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ural-1.0.0a2.tar", last modified: Tue Jul 18 13:46:25 2023, max compression
+gzip compressed data, was "dist/ural-1.0.0a3.tar", last modified: Tue Jul 18 15:17:59 2023, max compression
```

## Comparing `ural-1.0.0a2.tar` & `ural-1.0.0a3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 13:46:25.000000 ural-1.0.0a2/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    65598 2023-07-18 13:46:25.000000 ural-1.0.0a2/PKG-INFO
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    50638 2023-07-18 12:36:11.000000 ural-1.0.0a2/README.md
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       38 2023-07-18 13:46:25.000000 ural-1.0.0a2/setup.cfg
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      927 2023-07-18 13:46:11.000000 ural-1.0.0a2/setup.py
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1533 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      407 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/__main__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2357 2023-07-18 13:39:28.000000 ural-1.0.0a2/ural/canonicalize_url.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      119 2023-07-18 12:18:41.000000 ural-1.0.0a2/ural/canonicalize_url.pyi
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural/classes/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       44 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/classes/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1468 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/classes/hostname_trie_set.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      328 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/classes/hostname_trie_set.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3857 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/classes/suffix_trie.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      446 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/classes/suffix_trie.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5238 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/classes/trie_dict.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1030 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/classes/trie_dict.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      709 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/could_be_html.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       87 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/could_be_html.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1543 2023-07-13 08:17:56.000000 ural-1.0.0a2/ural/could_be_rss.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       93 2023-07-13 08:13:03.000000 ural-1.0.0a2/ural/could_be_rss.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3090 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/data.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      864 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/ensure_protocol.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       63 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/ensure_protocol.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      198 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    11953 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/facebook.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2163 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/facebook.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2889 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/fingerprint_url.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      330 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/fingerprint_url.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      931 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/force_protocol.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       62 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/force_protocol.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3612 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/format_url.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1508 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/format_url.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      742 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/get_hostname.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      143 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/get_hostname.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3779 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/google.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      719 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/google.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      908 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/has_special_host.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      138 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/has_special_host.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2341 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/infer_redirection.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       60 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/infer_redirection.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3285 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/instagram.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      599 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/instagram.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      734 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/is_homepage.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       39 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_homepage.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    22337 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_shortened_url.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       90 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_shortened_url.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4857 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_typo_url.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       39 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_typo_url.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2013 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/is_url.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      176 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_url.pyi
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural/lru/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      637 2023-07-13 09:11:57.000000 ural-1.0.0a2/ural/lru/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1384 2023-07-13 09:12:01.000000 ural-1.0.0a2/ural/lru/conversion.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      150 2023-07-13 09:11:43.000000 ural-1.0.0a2/ural/lru/conversion.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      478 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/lru/serialization.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      121 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/lru/serialization.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2816 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/lru/stems.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      298 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/lru/stems.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1970 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/lru/trie.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      966 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/lru/trie.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12086 2023-07-18 13:39:28.000000 ural-1.0.0a2/ural/normalize_url.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1493 2023-07-18 12:19:02.000000 ural-1.0.0a2/ural/normalize_url.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3065 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/patterns.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4211 2023-07-18 13:11:34.000000 ural-1.0.0a2/ural/quote.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      549 2023-07-18 13:11:34.000000 ural-1.0.0a2/ural/quote.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      594 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/should_follow_href.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       47 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/should_follow_href.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1030 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/should_resolve.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       88 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/should_resolve.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      537 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/strip_protocol.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       41 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/strip_protocol.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3712 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/telegram.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      592 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/telegram.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5438 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/tld.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      394 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/tld.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)   195604 2023-07-12 09:14:42.000000 ural-1.0.0a2/ural/tld_data.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3367 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/twitter.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      550 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/twitter.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      289 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/types.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1485 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/urls_from_html.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      167 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/urls_from_html.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1244 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/urls_from_text.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       81 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/urls_from_text.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4208 2023-07-18 12:11:47.000000 ural-1.0.0a2/ural/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1266 2023-07-18 11:44:02.000000 ural-1.0.0a2/ural/utils.pyi
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     9788 2023-07-12 09:12:27.000000 ural-1.0.0a2/ural/youtube.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      631 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/youtube.pyi
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    65598 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/PKG-INFO
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1901 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/SOURCES.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/dependency_links.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       43 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/requires.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        5 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/top_level.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/zip-safe
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 15:17:59.000000 ural-1.0.0a3/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    66263 2023-07-18 15:17:59.000000 ural-1.0.0a3/PKG-INFO
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    51239 2023-07-18 13:51:37.000000 ural-1.0.0a3/README.md
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       38 2023-07-18 15:17:59.000000 ural-1.0.0a3/setup.cfg
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      927 2023-07-18 15:17:44.000000 ural-1.0.0a3/setup.py
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 15:17:59.000000 ural-1.0.0a3/ural/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1533 2023-07-18 08:06:29.000000 ural-1.0.0a3/ural/__init__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      407 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/__main__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2357 2023-07-18 13:39:28.000000 ural-1.0.0a3/ural/canonicalize_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      119 2023-07-18 12:18:41.000000 ural-1.0.0a3/ural/canonicalize_url.pyi
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 15:17:59.000000 ural-1.0.0a3/ural/classes/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       44 2023-02-21 11:43:13.000000 ural-1.0.0a3/ural/classes/__init__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1468 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/classes/hostname_trie_set.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      328 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/classes/hostname_trie_set.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3857 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/classes/suffix_trie.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      446 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/classes/suffix_trie.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5238 2023-02-21 11:43:13.000000 ural-1.0.0a3/ural/classes/trie_dict.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1030 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/classes/trie_dict.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      709 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/could_be_html.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       87 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/could_be_html.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1543 2023-07-13 08:17:56.000000 ural-1.0.0a3/ural/could_be_rss.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       93 2023-07-13 08:13:03.000000 ural-1.0.0a3/ural/could_be_rss.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3090 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/data.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      864 2023-02-21 11:43:13.000000 ural-1.0.0a3/ural/ensure_protocol.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       63 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/ensure_protocol.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      198 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/exceptions.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    11953 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/facebook.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2163 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/facebook.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2889 2023-07-18 08:06:29.000000 ural-1.0.0a3/ural/fingerprint_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      330 2023-07-18 08:06:29.000000 ural-1.0.0a3/ural/fingerprint_url.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      931 2023-02-21 11:43:13.000000 ural-1.0.0a3/ural/force_protocol.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       62 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/force_protocol.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3612 2023-07-18 08:06:29.000000 ural-1.0.0a3/ural/format_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1508 2023-07-18 08:06:29.000000 ural-1.0.0a3/ural/format_url.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      742 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/get_hostname.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      143 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/get_hostname.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3779 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/google.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      719 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/google.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      908 2023-02-21 11:43:13.000000 ural-1.0.0a3/ural/has_special_host.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      138 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/has_special_host.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2341 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/infer_redirection.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       60 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/infer_redirection.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3285 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/instagram.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      599 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/instagram.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      734 2023-02-21 11:43:13.000000 ural-1.0.0a3/ural/is_homepage.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       39 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/is_homepage.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    22337 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/is_shortened_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       90 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/is_shortened_url.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4857 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/is_typo_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       39 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/is_typo_url.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2013 2023-07-18 08:06:29.000000 ural-1.0.0a3/ural/is_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      176 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/is_url.pyi
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 15:17:59.000000 ural-1.0.0a3/ural/lru/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      637 2023-07-13 09:11:57.000000 ural-1.0.0a3/ural/lru/__init__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1384 2023-07-13 09:12:01.000000 ural-1.0.0a3/ural/lru/conversion.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      150 2023-07-13 09:11:43.000000 ural-1.0.0a3/ural/lru/conversion.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      478 2023-02-21 11:43:13.000000 ural-1.0.0a3/ural/lru/serialization.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      121 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/lru/serialization.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2816 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/lru/stems.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      298 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/lru/stems.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1970 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/lru/trie.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      966 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/lru/trie.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12163 2023-07-18 15:09:49.000000 ural-1.0.0a3/ural/normalize_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1493 2023-07-18 12:19:02.000000 ural-1.0.0a3/ural/normalize_url.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3065 2023-07-18 08:06:29.000000 ural-1.0.0a3/ural/patterns.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4211 2023-07-18 13:11:34.000000 ural-1.0.0a3/ural/quote.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      549 2023-07-18 13:11:34.000000 ural-1.0.0a3/ural/quote.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      594 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/should_follow_href.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       47 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/should_follow_href.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1030 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/should_resolve.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       88 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/should_resolve.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      537 2023-02-21 11:43:13.000000 ural-1.0.0a3/ural/strip_protocol.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       41 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/strip_protocol.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3712 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/telegram.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      592 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/telegram.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5438 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/tld.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      394 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/tld.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)   195604 2023-07-12 09:14:42.000000 ural-1.0.0a3/ural/tld_data.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3367 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/twitter.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      550 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/twitter.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      289 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/types.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1485 2023-07-18 08:06:29.000000 ural-1.0.0a3/ural/urls_from_html.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      167 2023-07-18 08:06:29.000000 ural-1.0.0a3/ural/urls_from_html.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1244 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/urls_from_text.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       81 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/urls_from_text.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4208 2023-07-18 12:11:47.000000 ural-1.0.0a3/ural/utils.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1266 2023-07-18 11:44:02.000000 ural-1.0.0a3/ural/utils.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     9788 2023-07-12 09:12:27.000000 ural-1.0.0a3/ural/youtube.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      631 2023-07-12 08:48:04.000000 ural-1.0.0a3/ural/youtube.pyi
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 15:17:59.000000 ural-1.0.0a3/ural.egg-info/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    66263 2023-07-18 15:17:59.000000 ural-1.0.0a3/ural.egg-info/PKG-INFO
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1901 2023-07-18 15:17:59.000000 ural-1.0.0a3/ural.egg-info/SOURCES.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-07-18 15:17:59.000000 ural-1.0.0a3/ural.egg-info/dependency_links.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       43 2023-07-18 15:17:59.000000 ural-1.0.0a3/ural.egg-info/requires.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        5 2023-07-18 15:17:59.000000 ural-1.0.0a3/ural.egg-info/top_level.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-07-18 15:17:59.000000 ural-1.0.0a3/ural.egg-info/zip-safe
```

### Comparing `ural-1.0.0a2/PKG-INFO` & `ural-1.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 Metadata-Version: 2.1
 Name: ural
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: A helper library full of URL-related heuristics.
 Home-page: http://github.com/medialab/ural
 Author: Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel, César Pichon
 Author-email: guillaume.plique@sciencespo.fr
 License: GPL-3.0
-Description: [![Build Status](https://github.com/medialab/ural/workflows/Tests/badge.svg)](https://github.com/medialab/ural/actions)
+Description: [![Build Status](https://github.com/medialab/ural/workflows/Tests/badge.svg)](https://github.com/medialab/ural/actions) [![DOI](https://zenodo.org/badge/133951636.svg)](https://zenodo.org/badge/latestdoi/133951636)
         
         # Ural
         
-        A helper library full of URL-related heuristics.
+        A python helper library full of URL-related heuristics.
         
         ## Installation
         
         You can install `ural` with pip with the following command:
         
         ```
         pip install ural
         ```
         
+        ## How to cite?
+        
+        `ural` is published on [Zenodo](https://zenodo.org/) as [![DOI](https://zenodo.org/badge/133951636.svg)](https://zenodo.org/badge/latestdoi/133951636)
+        
+        You can cite it thusly:
+        
+        > Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel, & César Pichon. Ural, a python helper library full of URL-related heuristics. (2018). Zenodo. https://doi.org/10.5281/zenodo.8160139
+        
         ## Usage
         
         *Generic functions*
         
         * [canonicalize_url](#canonicalize_url)
         * [could_be_html](#could_be_html)
         * [could_be_rss](#could_be_rss)
```

### Comparing `ural-1.0.0a2/README.md` & `ural-1.0.0a3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-[![Build Status](https://github.com/medialab/ural/workflows/Tests/badge.svg)](https://github.com/medialab/ural/actions)
+[![Build Status](https://github.com/medialab/ural/workflows/Tests/badge.svg)](https://github.com/medialab/ural/actions) [![DOI](https://zenodo.org/badge/133951636.svg)](https://zenodo.org/badge/latestdoi/133951636)
 
 # Ural
 
-A helper library full of URL-related heuristics.
+A python helper library full of URL-related heuristics.
 
 ## Installation
 
 You can install `ural` with pip with the following command:
 
 ```
 pip install ural
 ```
 
+## How to cite?
+
+`ural` is published on [Zenodo](https://zenodo.org/) as [![DOI](https://zenodo.org/badge/133951636.svg)](https://zenodo.org/badge/latestdoi/133951636)
+
+You can cite it thusly:
+
+> Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel, & César Pichon. Ural, a python helper library full of URL-related heuristics. (2018). Zenodo. https://doi.org/10.5281/zenodo.8160139
+
 ## Usage
 
 *Generic functions*
 
 * [canonicalize_url](#canonicalize_url)
 * [could_be_html](#could_be_html)
 * [could_be_rss](#could_be_rss)
```

### Comparing `ural-1.0.0a2/setup.py` & `ural-1.0.0a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="ural",
-    version="1.0.0-a2",
+    version="1.0.0-a3",
     description="A helper library full of URL-related heuristics.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/medialab/ural",
     author="Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel, César Pichon",
     author_email="guillaume.plique@sciencespo.fr",
     keywords="url",
```

### Comparing `ural-1.0.0a2/ural/__init__.py` & `ural-1.0.0a3/ural/__init__.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/canonicalize_url.py` & `ural-1.0.0a3/ural/canonicalize_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/classes/hostname_trie_set.py` & `ural-1.0.0a3/ural/classes/hostname_trie_set.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/classes/suffix_trie.py` & `ural-1.0.0a3/ural/classes/suffix_trie.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/classes/trie_dict.py` & `ural-1.0.0a3/ural/classes/trie_dict.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/classes/trie_dict.pyi` & `ural-1.0.0a3/ural/classes/trie_dict.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/could_be_html.py` & `ural-1.0.0a3/ural/could_be_html.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/could_be_rss.py` & `ural-1.0.0a3/ural/could_be_rss.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/data.py` & `ural-1.0.0a3/ural/data.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/ensure_protocol.py` & `ural-1.0.0a3/ural/ensure_protocol.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/facebook.py` & `ural-1.0.0a3/ural/facebook.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/facebook.pyi` & `ural-1.0.0a3/ural/facebook.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/fingerprint_url.py` & `ural-1.0.0a3/ural/fingerprint_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/force_protocol.py` & `ural-1.0.0a3/ural/force_protocol.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/format_url.py` & `ural-1.0.0a3/ural/format_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/format_url.pyi` & `ural-1.0.0a3/ural/format_url.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/get_hostname.py` & `ural-1.0.0a3/ural/get_hostname.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/google.py` & `ural-1.0.0a3/ural/google.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/google.pyi` & `ural-1.0.0a3/ural/google.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/has_special_host.py` & `ural-1.0.0a3/ural/has_special_host.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/infer_redirection.py` & `ural-1.0.0a3/ural/infer_redirection.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/instagram.py` & `ural-1.0.0a3/ural/instagram.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/instagram.pyi` & `ural-1.0.0a3/ural/instagram.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/is_homepage.py` & `ural-1.0.0a3/ural/is_homepage.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/is_shortened_url.py` & `ural-1.0.0a3/ural/is_shortened_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/is_typo_url.py` & `ural-1.0.0a3/ural/is_typo_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/is_url.py` & `ural-1.0.0a3/ural/is_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/lru/__init__.py` & `ural-1.0.0a3/ural/lru/__init__.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/lru/conversion.py` & `ural-1.0.0a3/ural/lru/conversion.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/lru/stems.py` & `ural-1.0.0a3/ural/lru/stems.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/lru/trie.py` & `ural-1.0.0a3/ural/lru/trie.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/lru/trie.pyi` & `ural-1.0.0a3/ural/lru/trie.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/normalize_url.py` & `ural-1.0.0a3/ural/normalize_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,19 +98,16 @@
         or k == "cbrd"
         or k == "ucbcb"
         or k == "ab_channel",
     ),
 ]
 
 
-def coerce_empty_query_item(item):
-    if item[1].strip() == "":
-        return item[0], None
-
-    return item
+def qsl_sort_key(item):
+    return item[0], item[1] or '', 0 if item[1] is None else 1
 
 
 def should_strip_query_item(
     item, normalize_amp=True, query_item_filter=None, domain_filter=None
 ):
     key = item[0].lower()
 
@@ -317,27 +314,29 @@
                     f
                     for d, f in PER_DOMAIN_QUERY_FILTERS
                     if splitted.hostname.endswith(d)
                 ),
                 None,
             )
 
+        # TODO: what to do of empty query items vs. no valued
+        # TODO: should be dedupe query items?
         qsl = [
-            coerce_empty_query_item(item)
+            item
             for item in safe_qsl_iter(query)
             if not should_strip_query_item(
                 item,
                 normalize_amp=normalize_amp,
                 query_item_filter=query_item_filter,
                 domain_filter=domain_filter,
             )
         ]
 
         if sort_query:
-            qsl = sorted(qsl)
+            qsl = sorted(qsl, key=qsl_sort_key)
 
     # Dropping fragment if it's not routing
     if fragment and strip_fragment:
         if strip_fragment is True or not should_strip_fragment(fragment):
             fragment = ""
 
     # Always dropping trailing slash with empty query & fragment
```

### Comparing `ural-1.0.0a2/ural/normalize_url.pyi` & `ural-1.0.0a3/ural/normalize_url.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/patterns.py` & `ural-1.0.0a3/ural/patterns.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/quote.py` & `ural-1.0.0a3/ural/quote.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/quote.pyi` & `ural-1.0.0a3/ural/quote.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/should_follow_href.py` & `ural-1.0.0a3/ural/should_follow_href.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/should_resolve.py` & `ural-1.0.0a3/ural/should_resolve.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/strip_protocol.py` & `ural-1.0.0a3/ural/strip_protocol.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/telegram.py` & `ural-1.0.0a3/ural/telegram.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/telegram.pyi` & `ural-1.0.0a3/ural/telegram.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/tld.py` & `ural-1.0.0a3/ural/tld.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/tld_data.py` & `ural-1.0.0a3/ural/tld_data.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/twitter.py` & `ural-1.0.0a3/ural/twitter.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/twitter.pyi` & `ural-1.0.0a3/ural/twitter.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/urls_from_html.py` & `ural-1.0.0a3/ural/urls_from_html.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/urls_from_text.py` & `ural-1.0.0a3/ural/urls_from_text.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/utils.py` & `ural-1.0.0a3/ural/utils.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/utils.pyi` & `ural-1.0.0a3/ural/utils.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/youtube.py` & `ural-1.0.0a3/ural/youtube.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural/youtube.pyi` & `ural-1.0.0a3/ural/youtube.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a2/ural.egg-info/PKG-INFO` & `ural-1.0.0a3/ural.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 Metadata-Version: 2.1
 Name: ural
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: A helper library full of URL-related heuristics.
 Home-page: http://github.com/medialab/ural
 Author: Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel, César Pichon
 Author-email: guillaume.plique@sciencespo.fr
 License: GPL-3.0
-Description: [![Build Status](https://github.com/medialab/ural/workflows/Tests/badge.svg)](https://github.com/medialab/ural/actions)
+Description: [![Build Status](https://github.com/medialab/ural/workflows/Tests/badge.svg)](https://github.com/medialab/ural/actions) [![DOI](https://zenodo.org/badge/133951636.svg)](https://zenodo.org/badge/latestdoi/133951636)
         
         # Ural
         
-        A helper library full of URL-related heuristics.
+        A python helper library full of URL-related heuristics.
         
         ## Installation
         
         You can install `ural` with pip with the following command:
         
         ```
         pip install ural
         ```
         
+        ## How to cite?
+        
+        `ural` is published on [Zenodo](https://zenodo.org/) as [![DOI](https://zenodo.org/badge/133951636.svg)](https://zenodo.org/badge/latestdoi/133951636)
+        
+        You can cite it thusly:
+        
+        > Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel, & César Pichon. Ural, a python helper library full of URL-related heuristics. (2018). Zenodo. https://doi.org/10.5281/zenodo.8160139
+        
         ## Usage
         
         *Generic functions*
         
         * [canonicalize_url](#canonicalize_url)
         * [could_be_html](#could_be_html)
         * [could_be_rss](#could_be_rss)
```

### Comparing `ural-1.0.0a2/ural.egg-info/SOURCES.txt` & `ural-1.0.0a3/ural.egg-info/SOURCES.txt`

 * *Files identical despite different names*

