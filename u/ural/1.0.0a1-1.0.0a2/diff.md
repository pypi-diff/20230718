# Comparing `tmp/ural-1.0.0a1.tar.gz` & `tmp/ural-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ural-1.0.0a1.tar", last modified: Mon Jul 17 11:03:20 2023, max compression
+gzip compressed data, was "dist/ural-1.0.0a2.tar", last modified: Tue Jul 18 13:46:25 2023, max compression
```

## Comparing `ural-1.0.0a1.tar` & `ural-1.0.0a2.tar`

### file list

```diff
@@ -1,94 +1,96 @@
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-07-17 11:03:20.000000 ural-1.0.0a1/
--rw-r--r--   0 Yomgui     (501) staff       (20)    65115 2023-07-17 11:03:20.000000 ural-1.0.0a1/PKG-INFO
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/
--rw-r--r--   0 Yomgui     (501) staff       (20)    65115 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/PKG-INFO
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/zip-safe
--rw-r--r--   0 Yomgui     (501) staff       (20)     1872 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/SOURCES.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       43 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/requires.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        5 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/top_level.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/dependency_links.txt
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural/
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural/lru/
--rw-r--r--   0 Yomgui     (501) staff       (20)      966 2023-02-26 16:51:20.000000 ural-1.0.0a1/ural/lru/trie.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      298 2023-02-26 16:51:20.000000 ural-1.0.0a1/ural/lru/stems.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     1384 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/lru/conversion.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      637 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/lru/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      150 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/lru/conversion.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     2816 2023-02-26 16:51:20.000000 ural-1.0.0a1/ural/lru/stems.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1970 2023-02-26 16:51:20.000000 ural-1.0.0a1/ural/lru/trie.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      478 2023-02-25 09:51:53.000000 ural-1.0.0a1/ural/lru/serialization.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      121 2023-02-25 16:45:24.000000 ural-1.0.0a1/ural/lru/serialization.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)   195604 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/tld_data.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      550 2023-02-25 16:32:31.000000 ural-1.0.0a1/ural/twitter.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     2013 2023-07-15 07:16:51.000000 ural-1.0.0a1/ural/is_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)       88 2023-02-25 16:15:45.000000 ural-1.0.0a1/ural/should_resolve.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     9788 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/youtube.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     3065 2023-07-15 11:26:13.000000 ural-1.0.0a1/ural/patterns.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      138 2023-02-25 15:39:15.000000 ural-1.0.0a1/ural/has_special_host.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     1543 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/could_be_rss.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1508 2023-07-15 10:52:43.000000 ural-1.0.0a1/ural/format_url.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     4857 2023-02-25 10:06:33.000000 ural-1.0.0a1/ural/is_typo_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1485 2023-07-15 10:51:13.000000 ural-1.0.0a1/ural/urls_from_html.py
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural/classes/
--rw-r--r--   0 Yomgui     (501) staff       (20)     5238 2023-02-25 09:51:53.000000 ural-1.0.0a1/ural/classes/trie_dict.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      328 2023-02-25 20:51:29.000000 ural-1.0.0a1/ural/classes/hostname_trie_set.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)       44 2022-11-03 11:31:14.000000 ural-1.0.0a1/ural/classes/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1030 2023-02-25 16:43:56.000000 ural-1.0.0a1/ural/classes/trie_dict.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     1468 2023-02-25 20:53:15.000000 ural-1.0.0a1/ural/classes/hostname_trie_set.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     3857 2023-02-26 12:31:27.000000 ural-1.0.0a1/ural/classes/suffix_trie.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      446 2023-02-25 20:56:18.000000 ural-1.0.0a1/ural/classes/suffix_trie.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      734 2023-02-25 09:51:53.000000 ural-1.0.0a1/ural/is_homepage.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     3712 2023-03-11 16:28:18.000000 ural-1.0.0a1/ural/telegram.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      594 2023-02-26 20:00:25.000000 ural-1.0.0a1/ural/should_follow_href.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     2341 2023-07-15 11:18:40.000000 ural-1.0.0a1/ural/infer_redirection.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     2163 2023-02-25 14:40:59.000000 ural-1.0.0a1/ural/facebook.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)       93 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/could_be_rss.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     1302 2023-07-15 13:15:05.000000 ural-1.0.0a1/ural/canonicalize_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      719 2023-02-25 15:37:43.000000 ural-1.0.0a1/ural/google.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     1533 2023-07-15 12:38:29.000000 ural-1.0.0a1/ural/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      742 2023-02-25 20:40:43.000000 ural-1.0.0a1/ural/get_hostname.py
--rw-r--r--   0 Yomgui     (501) staff       (20)       39 2023-02-25 16:14:40.000000 ural-1.0.0a1/ural/is_homepage.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     3779 2023-03-11 16:28:18.000000 ural-1.0.0a1/ural/google.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      931 2023-02-25 09:51:53.000000 ural-1.0.0a1/ural/force_protocol.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      143 2023-02-25 20:43:43.000000 ural-1.0.0a1/ural/get_hostname.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      631 2023-02-25 16:38:38.000000 ural-1.0.0a1/ural/youtube.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     1030 2023-02-25 20:10:18.000000 ural-1.0.0a1/ural/should_resolve.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     2889 2023-07-15 13:25:42.000000 ural-1.0.0a1/ural/fingerprint_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1168 2023-07-15 13:13:06.000000 ural-1.0.0a1/ural/utils.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      289 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/types.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)    11953 2023-03-11 16:28:18.000000 ural-1.0.0a1/ural/facebook.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      709 2023-02-26 19:32:09.000000 ural-1.0.0a1/ural/could_be_html.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      176 2023-02-25 16:17:21.000000 ural-1.0.0a1/ural/is_url.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      599 2023-03-02 12:55:19.000000 ural-1.0.0a1/ural/instagram.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)       39 2023-02-25 16:16:15.000000 ural-1.0.0a1/ural/is_typo_url.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      537 2019-10-04 20:55:44.000000 ural-1.0.0a1/ural/strip_protocol.py
--rw-r--r--   0 Yomgui     (501) staff       (20)       63 2023-02-25 14:00:44.000000 ural-1.0.0a1/ural/ensure_protocol.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     4146 2023-07-15 13:17:26.000000 ural-1.0.0a1/ural/utils.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     3367 2023-03-11 16:28:18.000000 ural-1.0.0a1/ural/twitter.py
--rw-r--r--   0 Yomgui     (501) staff       (20)    11499 2023-07-17 11:00:36.000000 ural-1.0.0a1/ural/normalize_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)       99 2023-07-15 13:02:03.000000 ural-1.0.0a1/ural/canonicalize_url.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)    22337 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/is_shortened_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      592 2023-02-25 16:31:00.000000 ural-1.0.0a1/ural/telegram.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)       47 2023-02-26 19:56:28.000000 ural-1.0.0a1/ural/should_follow_href.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      167 2023-07-15 10:23:50.000000 ural-1.0.0a1/ural/urls_from_html.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      864 2023-02-25 10:12:21.000000 ural-1.0.0a1/ural/ensure_protocol.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     3285 2023-03-11 16:28:18.000000 ural-1.0.0a1/ural/instagram.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      198 2023-02-25 20:18:35.000000 ural-1.0.0a1/ural/exceptions.py
--rw-r--r--   0 Yomgui     (501) staff       (20)       62 2023-02-25 14:00:50.000000 ural-1.0.0a1/ural/force_protocol.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)     1244 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/urls_from_text.py
--rw-r--r--   0 Yomgui     (501) staff       (20)       87 2023-02-26 17:47:23.000000 ural-1.0.0a1/ural/could_be_html.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      908 2023-02-25 15:39:17.000000 ural-1.0.0a1/ural/has_special_host.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      394 2023-02-26 17:08:42.000000 ural-1.0.0a1/ural/tld.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)       81 2023-02-25 14:43:13.000000 ural-1.0.0a1/ural/urls_from_text.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)       41 2023-02-25 16:22:37.000000 ural-1.0.0a1/ural/strip_protocol.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      407 2023-02-25 20:05:32.000000 ural-1.0.0a1/ural/__main__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     5438 2023-02-26 09:49:32.000000 ural-1.0.0a1/ural/tld.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     3612 2023-07-15 10:51:43.000000 ural-1.0.0a1/ural/format_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     3090 2023-02-26 19:56:02.000000 ural-1.0.0a1/ural/data.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1481 2023-07-17 11:00:36.000000 ural-1.0.0a1/ural/normalize_url.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)      330 2023-07-15 13:26:15.000000 ural-1.0.0a1/ural/fingerprint_url.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)       90 2023-02-25 16:15:29.000000 ural-1.0.0a1/ural/is_shortened_url.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)       60 2023-02-25 15:42:33.000000 ural-1.0.0a1/ural/infer_redirection.pyi
--rw-r--r--   0 Yomgui     (501) staff       (20)    50214 2023-07-17 11:01:14.000000 ural-1.0.0a1/README.md
--rw-r--r--   0 Yomgui     (501) staff       (20)      908 2023-07-17 11:03:01.000000 ural-1.0.0a1/setup.py
--rw-r--r--   0 Yomgui     (501) staff       (20)       38 2023-07-17 11:03:20.000000 ural-1.0.0a1/setup.cfg
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 13:46:25.000000 ural-1.0.0a2/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    65598 2023-07-18 13:46:25.000000 ural-1.0.0a2/PKG-INFO
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    50638 2023-07-18 12:36:11.000000 ural-1.0.0a2/README.md
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       38 2023-07-18 13:46:25.000000 ural-1.0.0a2/setup.cfg
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      927 2023-07-18 13:46:11.000000 ural-1.0.0a2/setup.py
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1533 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/__init__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      407 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/__main__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2357 2023-07-18 13:39:28.000000 ural-1.0.0a2/ural/canonicalize_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      119 2023-07-18 12:18:41.000000 ural-1.0.0a2/ural/canonicalize_url.pyi
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural/classes/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       44 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/classes/__init__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1468 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/classes/hostname_trie_set.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      328 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/classes/hostname_trie_set.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3857 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/classes/suffix_trie.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      446 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/classes/suffix_trie.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5238 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/classes/trie_dict.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1030 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/classes/trie_dict.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      709 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/could_be_html.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       87 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/could_be_html.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1543 2023-07-13 08:17:56.000000 ural-1.0.0a2/ural/could_be_rss.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       93 2023-07-13 08:13:03.000000 ural-1.0.0a2/ural/could_be_rss.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3090 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/data.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      864 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/ensure_protocol.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       63 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/ensure_protocol.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      198 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/exceptions.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    11953 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/facebook.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2163 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/facebook.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2889 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/fingerprint_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      330 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/fingerprint_url.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      931 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/force_protocol.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       62 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/force_protocol.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3612 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/format_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1508 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/format_url.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      742 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/get_hostname.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      143 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/get_hostname.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3779 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/google.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      719 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/google.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      908 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/has_special_host.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      138 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/has_special_host.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2341 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/infer_redirection.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       60 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/infer_redirection.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3285 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/instagram.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      599 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/instagram.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      734 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/is_homepage.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       39 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_homepage.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    22337 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_shortened_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       90 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_shortened_url.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4857 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_typo_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       39 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_typo_url.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2013 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/is_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      176 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/is_url.pyi
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural/lru/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      637 2023-07-13 09:11:57.000000 ural-1.0.0a2/ural/lru/__init__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1384 2023-07-13 09:12:01.000000 ural-1.0.0a2/ural/lru/conversion.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      150 2023-07-13 09:11:43.000000 ural-1.0.0a2/ural/lru/conversion.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      478 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/lru/serialization.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      121 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/lru/serialization.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2816 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/lru/stems.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      298 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/lru/stems.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1970 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/lru/trie.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      966 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/lru/trie.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12086 2023-07-18 13:39:28.000000 ural-1.0.0a2/ural/normalize_url.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1493 2023-07-18 12:19:02.000000 ural-1.0.0a2/ural/normalize_url.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3065 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/patterns.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4211 2023-07-18 13:11:34.000000 ural-1.0.0a2/ural/quote.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      549 2023-07-18 13:11:34.000000 ural-1.0.0a2/ural/quote.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      594 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/should_follow_href.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       47 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/should_follow_href.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1030 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/should_resolve.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       88 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/should_resolve.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      537 2023-02-21 11:43:13.000000 ural-1.0.0a2/ural/strip_protocol.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       41 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/strip_protocol.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3712 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/telegram.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      592 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/telegram.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5438 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/tld.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      394 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/tld.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)   195604 2023-07-12 09:14:42.000000 ural-1.0.0a2/ural/tld_data.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3367 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/twitter.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      550 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/twitter.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      289 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/types.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1485 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/urls_from_html.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      167 2023-07-18 08:06:29.000000 ural-1.0.0a2/ural/urls_from_html.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1244 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/urls_from_text.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       81 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/urls_from_text.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4208 2023-07-18 12:11:47.000000 ural-1.0.0a2/ural/utils.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1266 2023-07-18 11:44:02.000000 ural-1.0.0a2/ural/utils.pyi
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     9788 2023-07-12 09:12:27.000000 ural-1.0.0a2/ural/youtube.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      631 2023-07-12 08:48:04.000000 ural-1.0.0a2/ural/youtube.pyi
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    65598 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/PKG-INFO
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1901 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/SOURCES.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/dependency_links.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       43 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/requires.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        5 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/top_level.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-07-18 13:46:25.000000 ural-1.0.0a2/ural.egg-info/zip-safe
```

### Comparing `ural-1.0.0a1/PKG-INFO` & `ural-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ural
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A helper library full of URL-related heuristics.
 Home-page: http://github.com/medialab/ural
-Author: Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel
+Author: Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel, César Pichon
 Author-email: guillaume.plique@sciencespo.fr
-License: MIT
+License: GPL-3.0
 Description: [![Build Status](https://github.com/medialab/ural/workflows/Tests/badge.svg)](https://github.com/medialab/ural/actions)
         
         # Ural
         
         A helper library full of URL-related heuristics.
         
         ## Installation
@@ -174,14 +174,19 @@
         ```python
         from ural import canonicalize_url
         
         canonicalize_url('www.LEMONDE.fr')
         >>> 'https://lemonde.fr'
         ```
         
+        *Arguments*
+        
+        * **url** *string*: url to canonicalize.
+        * **quoted** *?bool* [`False`]: by default the function will unquote the url as much as possible all while keeping the url safe. If this kwarg is set to `True`, the function will instead quote the url as much as possible all while ensuring nothing will be double-quoted.
+        
         ---
         
         ### could_be_html
         
         Function returning whether the url could return HTML.
         
         ```python
@@ -716,15 +721,15 @@
         * **sort_query** *?bool* [`True`]: whether to sort query items.
         * **strip_authentication** *?bool* [`True`]: whether to strip authentication.
         * **strip_fragment** *?bool|str* [`'except-routing'`]: whether to strip the url's fragment. If set to `except-routing`, will only strip the fragment if the fragment is not deemed to be js routing (i.e. if it contains a `/`).
         * **strip_index** *?bool* [`True`]: whether to strip trailing index.
         * **strip_irrelevant_subdomains** *?bool* [`False`]: whether to strip irrelevant subdomains such as `www` etc.
         * **strip_protocol** *?bool* [`True`]: whether to strip the url's protocol.
         * **strip_trailing_slash** *?bool* [`True`]: whether to strip trailing slash.
-        * **unsplit** *?bool* [`True`]: whether to return a stringified version of the normalized url or directly the `SplitResult` instance worked on by the normalization process.
+        * **quoted** *?bool* [`False`]: by default the function will unquote the url as much as possible all while keeping the url safe. If this kwarg is set to `True`, the function will instead quote the url as much as possible all while ensuring nothing will be double-quoted.
         
         ---
         
         ### should_follow_href
         
         Function returning whether the given href should be followed (usually from a crawler's context). This means it will filter out anchors, and url having a scheme which is not http/https.
```

### Comparing `ural-1.0.0a1/ural.egg-info/PKG-INFO` & `ural-1.0.0a2/ural.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ural
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A helper library full of URL-related heuristics.
 Home-page: http://github.com/medialab/ural
-Author: Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel
+Author: Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel, César Pichon
 Author-email: guillaume.plique@sciencespo.fr
-License: MIT
+License: GPL-3.0
 Description: [![Build Status](https://github.com/medialab/ural/workflows/Tests/badge.svg)](https://github.com/medialab/ural/actions)
         
         # Ural
         
         A helper library full of URL-related heuristics.
         
         ## Installation
@@ -174,14 +174,19 @@
         ```python
         from ural import canonicalize_url
         
         canonicalize_url('www.LEMONDE.fr')
         >>> 'https://lemonde.fr'
         ```
         
+        *Arguments*
+        
+        * **url** *string*: url to canonicalize.
+        * **quoted** *?bool* [`False`]: by default the function will unquote the url as much as possible all while keeping the url safe. If this kwarg is set to `True`, the function will instead quote the url as much as possible all while ensuring nothing will be double-quoted.
+        
         ---
         
         ### could_be_html
         
         Function returning whether the url could return HTML.
         
         ```python
@@ -716,15 +721,15 @@
         * **sort_query** *?bool* [`True`]: whether to sort query items.
         * **strip_authentication** *?bool* [`True`]: whether to strip authentication.
         * **strip_fragment** *?bool|str* [`'except-routing'`]: whether to strip the url's fragment. If set to `except-routing`, will only strip the fragment if the fragment is not deemed to be js routing (i.e. if it contains a `/`).
         * **strip_index** *?bool* [`True`]: whether to strip trailing index.
         * **strip_irrelevant_subdomains** *?bool* [`False`]: whether to strip irrelevant subdomains such as `www` etc.
         * **strip_protocol** *?bool* [`True`]: whether to strip the url's protocol.
         * **strip_trailing_slash** *?bool* [`True`]: whether to strip trailing slash.
-        * **unsplit** *?bool* [`True`]: whether to return a stringified version of the normalized url or directly the `SplitResult` instance worked on by the normalization process.
+        * **quoted** *?bool* [`False`]: by default the function will unquote the url as much as possible all while keeping the url safe. If this kwarg is set to `True`, the function will instead quote the url as much as possible all while ensuring nothing will be double-quoted.
         
         ---
         
         ### should_follow_href
         
         Function returning whether the given href should be followed (usually from a crawler's context). This means it will filter out anchors, and url having a scheme which is not http/https.
```

### Comparing `ural-1.0.0a1/ural.egg-info/SOURCES.txt` & `ural-1.0.0a2/ural.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 ural/is_typo_url.py
 ural/is_typo_url.pyi
 ural/is_url.py
 ural/is_url.pyi
 ural/normalize_url.py
 ural/normalize_url.pyi
 ural/patterns.py
+ural/quote.py
+ural/quote.pyi
 ural/should_follow_href.py
 ural/should_follow_href.pyi
 ural/should_resolve.py
 ural/should_resolve.pyi
 ural/strip_protocol.py
 ural/strip_protocol.pyi
 ural/telegram.py
```

### Comparing `ural-1.0.0a1/ural/lru/trie.pyi` & `ural-1.0.0a2/ural/lru/trie.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/lru/conversion.py` & `ural-1.0.0a2/ural/lru/conversion.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/lru/__init__.py` & `ural-1.0.0a2/ural/lru/__init__.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/lru/stems.py` & `ural-1.0.0a2/ural/lru/stems.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/lru/trie.py` & `ural-1.0.0a2/ural/lru/trie.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/tld_data.py` & `ural-1.0.0a2/ural/tld_data.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/twitter.pyi` & `ural-1.0.0a2/ural/twitter.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/is_url.py` & `ural-1.0.0a2/ural/is_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/youtube.py` & `ural-1.0.0a2/ural/youtube.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/patterns.py` & `ural-1.0.0a2/ural/patterns.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/could_be_rss.py` & `ural-1.0.0a2/ural/could_be_rss.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/format_url.pyi` & `ural-1.0.0a2/ural/format_url.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/is_typo_url.py` & `ural-1.0.0a2/ural/is_typo_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/urls_from_html.py` & `ural-1.0.0a2/ural/urls_from_html.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/classes/trie_dict.py` & `ural-1.0.0a2/ural/classes/trie_dict.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/classes/trie_dict.pyi` & `ural-1.0.0a2/ural/classes/trie_dict.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/classes/hostname_trie_set.py` & `ural-1.0.0a2/ural/classes/hostname_trie_set.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/classes/suffix_trie.py` & `ural-1.0.0a2/ural/classes/suffix_trie.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/is_homepage.py` & `ural-1.0.0a2/ural/is_homepage.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/telegram.py` & `ural-1.0.0a2/ural/telegram.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/should_follow_href.py` & `ural-1.0.0a2/ural/should_follow_href.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/infer_redirection.py` & `ural-1.0.0a2/ural/infer_redirection.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/facebook.pyi` & `ural-1.0.0a2/ural/facebook.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/google.pyi` & `ural-1.0.0a2/ural/google.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/__init__.py` & `ural-1.0.0a2/ural/__init__.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/get_hostname.py` & `ural-1.0.0a2/ural/get_hostname.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/google.py` & `ural-1.0.0a2/ural/google.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/force_protocol.py` & `ural-1.0.0a2/ural/force_protocol.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/youtube.pyi` & `ural-1.0.0a2/ural/youtube.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/should_resolve.py` & `ural-1.0.0a2/ural/should_resolve.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/fingerprint_url.py` & `ural-1.0.0a2/ural/fingerprint_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/utils.pyi` & `ural-1.0.0a2/ural/utils.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Optional, Dict, List, Union, overload
+from typing import Optional, Dict, List, Tuple, Iterator, Iterable, Union, overload
 from urllib.parse import SplitResult
 from ural.types import AnyUrlTarget, Literal, QueryArgValue
 
-def space_aware_unquote(string: str, replacement: str = ...) -> str: ...
 def urlsplit(url: str) -> SplitResult: ...
 def safe_urlsplit(url: AnyUrlTarget, scheme: Optional[str] = ...) -> SplitResult: ...
 def pathsplit(urlpath: str) -> List[str]: ...
 def urlpathsplit(url: AnyUrlTarget) -> List[str]: ...
 def normpath(urlpath: str, drop_consecutive_slashes: bool = True) -> str: ...
 def attempt_to_decode_idna(string: str) -> str: ...
 @overload
@@ -22,7 +21,9 @@
 ) -> str: ...
 def unsplit_netloc(
     username: Optional[str],
     password: Optional[str],
     hostname: Optional[str],
     port: Optional[Union[str, int]],
 ) -> str: ...
+def safe_qsl_iter(query: str) -> Iterator[Tuple[str, Optional[str]]]: ...
+def safe_serialize_qsl(qsl: Iterable[Tuple[str, Optional[str]]]): ...
```

### Comparing `ural-1.0.0a1/ural/facebook.py` & `ural-1.0.0a2/ural/facebook.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/could_be_html.py` & `ural-1.0.0a2/ural/could_be_html.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/instagram.pyi` & `ural-1.0.0a2/ural/instagram.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/strip_protocol.py` & `ural-1.0.0a2/ural/strip_protocol.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/utils.py` & `ural-1.0.0a2/ural/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,53 +16,44 @@
 except NameError:
     pass
 
 # PY2/PY3 compatible urlparse
 try:
     from urllib.parse import (
         parse_qs,
-        parse_qsl,
         quote,
         unquote,
         urljoin,
         urlsplit,
         urlunsplit,
         SplitResult,
     )
 except ImportError:
     from urllib import unquote, quote as original_quote
 
-    ALWAYS_SAFE = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789_.-~"
-
     def quote(string, safe="/"):
         if isinstance(string, unicode):
-            safe_set = set(ord(c) for c in ALWAYS_SAFE)
-
-            for c in safe:
-                safe_set.add(ord(c))
-
-            chars = [
-                c if ord(c) in safe_set else "%{:02X}".format(ord(c)) for c in string
-            ]
-
-            return "".join(chars)
+            return original_quote(string.encode("utf-8"), safe)
 
         return original_quote(string, safe)
 
-    from urlparse import parse_qs, parse_qsl, urljoin, urlsplit, urlunsplit, SplitResult
+    from urlparse import (
+        parse_qs,
+        urljoin,
+        urlsplit,
+        urlunsplit,
+        SplitResult,
+    )
 
 MISTAKES_RE = re.compile(r"&amp(?:%3B|;)", re.I)
 
+# NOTE: one of the kwargs below is not so aptly named quote...
 unshadowed_quote = quote
 
 
-def space_aware_unquote(string, replacement="%20"):
-    return unquote(string).replace(" ", replacement)
-
-
 def safe_urlsplit(url, scheme="http"):
     if isinstance(url, SplitResult):
         return url
 
     if not re.match(PROTOCOL_RE, url):
         url = scheme + "://" + url
 
@@ -188,7 +179,26 @@
 
     if auth:
         hostname = auth + "@" + hostname
     if port:
         hostname += ":" + str(port)
 
     return hostname
+
+
+def safe_qsl_iter(query):
+    for item in query.split("&"):
+        if "=" not in item:
+            yield item, None
+        else:
+            yield tuple(item.split("=", 1))
+
+
+def safe_serialize_query_item(item):
+    if item[1] is None:
+        return item[0]
+
+    return "%s=%s" % item
+
+
+def safe_serialize_qsl(qsl):
+    return "&".join(safe_serialize_query_item(item) for item in qsl)
```

### Comparing `ural-1.0.0a1/ural/twitter.py` & `ural-1.0.0a2/ural/twitter.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/normalize_url.py` & `ural-1.0.0a2/ural/normalize_url.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,33 @@
 #
 import re
 from os.path import splitext
 
 from ural.ensure_protocol import ensure_protocol
 from ural.infer_redirection import infer_redirection as resolve
 from ural.utils import (
-    parse_qsl,
+    safe_qsl_iter,
+    safe_serialize_qsl,
     urlsplit,
     urlunsplit,
     unsplit_netloc,
     decode_punycode_hostname,
-    space_aware_unquote,
     normpath,
     fix_common_query_mistakes,
     SplitResult,
 )
+from ural.quote import (
+    safely_unquote_auth_item,
+    safely_unquote_path,
+    safely_unquote_qsl,
+    safely_unquote_fragment,
+    safely_quote,
+    safely_quote_qsl,
+    upper_quoted,
+)
 from ural.patterns import PROTOCOL_RE, CONTROL_CHARS_RE
 
 IRRELEVANT_QUERY_PATTERN = r"^(?:__twitter_impression|_guc_consent_skip|guccounter|fb_action_types|(?:php|asp|j)?sessionid|fb_action_ids|fb_source|echobox|feature|recruiter|_unique_id|twclid|mibextid|campaignid|adgroupid|cn-reloaded|ao_noptimize|mkt_tok|fbclid|igshid|refid|gclid|mc_cid|mc_eid|__tn__|_ft_|dclid|wpamp|fref|usqp|ncid|mtm_.+|utm_.+%s|s?een|cftoken|cfid|sid|xt(?:loc|ref|cr|np|or|s)|at_.+|_ga)$"
 
 IRRELEVANT_SUBDOMAIN_PATTERN = r"\b(?:www\d?|mobile%s|m)\."
 
 AMP_QUERY_PATTERN = r"|amp_.+|amp"
@@ -89,19 +98,19 @@
         or k == "cbrd"
         or k == "ucbcb"
         or k == "ab_channel",
     ),
 ]
 
 
-def stringify_qs(item):
-    if item[1] == "":
-        return item[0]
+def coerce_empty_query_item(item):
+    if item[1].strip() == "":
+        return item[0], None
 
-    return "%s=%s" % item
+    return item
 
 
 def should_strip_query_item(
     item, normalize_amp=True, query_item_filter=None, domain_filter=None
 ):
     key = item[0].lower()
 
@@ -171,33 +180,32 @@
         return None
 
     return normalize_hostname(splitted.hostname, normalize_amp=normalize_amp)
 
 
 # NOTE: normalize_url is not suited to be able to process already splitted urls,
 # because of mutliple string preprocessing tricks and redirection inferrence
-# NOTE: we force an unquoted version of the url because unquoting multiple times
-# is safe, while the contrary is not. Also, unquoted urls are more readable to
-# humans. Note that We still keep whitespace as %20 like most web browsers. Also,
-# we unquote only once, like browsers do. We could do it recursively but it
-# feels somewhat dangerous.
+# NOTE: query filter run before quoting shenanigans because targeted pattern
+# are not subject to escaping, usually
 def normalize_url(
     url,
-    unsplit=True,
     sort_query=True,
     strip_authentication=True,
     strip_trailing_slash=True,
     strip_index=True,
     strip_protocol=True,
     strip_irrelevant_subdomains=True,
     strip_fragment="except-routing",
-    query_item_filter=None,
     normalize_amp=True,
     fix_common_mistakes=True,
     infer_redirection=True,
+    # NOTE: following arguments currently undocumented
+    unsplit=True,
+    quoted=False,
+    query_item_filter=None,
 ):
     """
     Function normalizing the given url by stripping it of usually
     non-discriminant parts such as irrelevant query items or sub-domains etc.
 
     This is a very useful utility when attempting to match similar urls
     written slightly differently when shared on social media etc.
@@ -234,14 +242,16 @@
     original_url_arg = url
 
     if infer_redirection:
         url = resolve(url)
 
     url = CONTROL_CHARS_RE.sub("", url)
     url = url.strip()
+    url = upper_quoted(url)
+
     has_protocol = PROTOCOL_RE.match(url)
 
     # Ensuring scheme so parsing works correctly
     if not has_protocol:
         url = "http://" + url
 
     # Parsing
@@ -285,51 +295,50 @@
 
     # Dropping index:
     if strip_index:
         segments = path.rsplit("/", 1)
 
         if len(segments) != 0:
             last_segment = segments[-1]
-            filename, ext = splitext(last_segment)
+            filename, _ = splitext(last_segment)
 
-            if filename == "index":
+            if filename == "index" or filename == "default":
                 segments.pop()
                 path = "/".join(segments)
 
     # Dropping irrelevant query items
+    qsl = []
+
     if query:
         domain_filter = None
 
         if splitted.hostname:
             domain_filter = next(
                 (
                     f
                     for d, f in PER_DOMAIN_QUERY_FILTERS
                     if splitted.hostname.endswith(d)
                 ),
                 None,
             )
 
-        qsl = parse_qsl(query, keep_blank_values=True)
         qsl = [
-            stringify_qs(item)
-            for item in qsl
+            coerce_empty_query_item(item)
+            for item in safe_qsl_iter(query)
             if not should_strip_query_item(
                 item,
                 normalize_amp=normalize_amp,
                 query_item_filter=query_item_filter,
                 domain_filter=domain_filter,
             )
         ]
 
         if sort_query:
             qsl = sorted(qsl)
 
-        query = "&".join(qsl)
-
     # Dropping fragment if it's not routing
     if fragment and strip_fragment:
         if strip_fragment is True or not should_strip_fragment(fragment):
             fragment = ""
 
     # Always dropping trailing slash with empty query & fragment
     if path == "/" and not fragment and not query:
@@ -356,18 +365,43 @@
     if normalize_amp and hostname and hostname.startswith("amp-"):
         hostname = hostname[4:]
 
     # Dropping trailing slash
     if strip_trailing_slash and path.endswith("/"):
         path = path.rstrip("/")
 
-    # Unquoting
-    path = space_aware_unquote(path)
-    query = space_aware_unquote(query)
-    fragment = space_aware_unquote(fragment)
+    # Quoting
+    if user:
+        if quoted:
+            user = safely_quote(user)
+        else:
+            user = safely_unquote_auth_item(user)
+
+    if password:
+        if quoted:
+            password = safely_quote(password)
+        else:
+            password = safely_unquote_auth_item(password)
+
+    if quoted:
+        path = safely_quote(path)
+    else:
+        path = safely_unquote_path(path)
+
+    if quoted:
+        qsl = safely_quote_qsl(qsl)
+    else:
+        qsl = safely_unquote_qsl(qsl)
+
+    query = safe_serialize_qsl(qsl)
+
+    if quoted:
+        fragment = safely_quote(fragment)
+    else:
+        fragment = safely_unquote_fragment(fragment)
 
     # Result
     netloc = unsplit_netloc(user, password, hostname, port)
     result = SplitResult(scheme, netloc.lower(), path, query, fragment)
 
     if not unsplit:
         return result
```

### Comparing `ural-1.0.0a1/ural/is_shortened_url.py` & `ural-1.0.0a2/ural/is_shortened_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/telegram.pyi` & `ural-1.0.0a2/ural/telegram.pyi`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/ensure_protocol.py` & `ural-1.0.0a2/ural/ensure_protocol.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/instagram.py` & `ural-1.0.0a2/ural/instagram.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/urls_from_text.py` & `ural-1.0.0a2/ural/urls_from_text.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/has_special_host.py` & `ural-1.0.0a2/ural/has_special_host.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/tld.py` & `ural-1.0.0a2/ural/tld.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/format_url.py` & `ural-1.0.0a2/ural/format_url.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/data.py` & `ural-1.0.0a2/ural/data.py`

 * *Files identical despite different names*

### Comparing `ural-1.0.0a1/ural/normalize_url.pyi` & `ural-1.0.0a2/ural/normalize_url.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from typing import Union, Optional, Callable, overload
 from ural.types import AnyUrlTarget, Literal
 from urllib.parse import SplitResult
 
 @overload
 def normalize_url(
     url: str,
-    unsplit: Literal[False] = ...,
     sort_query: bool = ...,
     strip_authentication: bool = ...,
     strip_trailing_slash: bool = ...,
     strip_index: bool = ...,
     strip_protocol: bool = ...,
     strip_irrelevant_subdomains: bool = ...,
     strip_fragment: Union[bool, Literal["except-routing"]] = ...,
-    query_item_filter: Optional[Callable[[str, str], bool]] = ...,
     normalize_amp: bool = ...,
     fix_common_mistakes: bool = ...,
     infer_redirection: bool = ...,
     quoted: bool = ...,
-) -> SplitResult: ...
+    #
+    unsplit: Literal[True] = ...,
+    query_item_filter: Optional[Callable[[str, str], bool]] = ...,
+) -> str: ...
 @overload
 def normalize_url(
     url: str,
-    unsplit: Literal[True] = ...,
     sort_query: bool = ...,
     strip_authentication: bool = ...,
     strip_trailing_slash: bool = ...,
     strip_index: bool = ...,
     strip_protocol: bool = ...,
     strip_irrelevant_subdomains: bool = ...,
     strip_fragment: Union[bool, Literal["except-routing"]] = ...,
-    query_item_filter: Optional[Callable[[str, str], bool]] = ...,
     normalize_amp: bool = ...,
     fix_common_mistakes: bool = ...,
     infer_redirection: bool = ...,
     quoted: bool = ...,
-) -> str: ...
+    #
+    unsplit: Literal[False] = ...,
+    query_item_filter: Optional[Callable[[str, str], bool]] = ...,
+) -> SplitResult: ...
 def normalize_hostname(hostname: str, normalize_amp: bool = True) -> str: ...
 def get_normalized_hostname(
     url: AnyUrlTarget,
     normalize_amp: bool = True,
     infer_redirection: bool = True,
 ) -> str: ...
```

### Comparing `ural-1.0.0a1/README.md` & `ural-1.0.0a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,19 @@
 ```python
 from ural import canonicalize_url
 
 canonicalize_url('www.LEMONDE.fr')
 >>> 'https://lemonde.fr'
 ```
 
+*Arguments*
+
+* **url** *string*: url to canonicalize.
+* **quoted** *?bool* [`False`]: by default the function will unquote the url as much as possible all while keeping the url safe. If this kwarg is set to `True`, the function will instead quote the url as much as possible all while ensuring nothing will be double-quoted.
+
 ---
 
 ### could_be_html
 
 Function returning whether the url could return HTML.
 
 ```python
@@ -708,15 +713,15 @@
 * **sort_query** *?bool* [`True`]: whether to sort query items.
 * **strip_authentication** *?bool* [`True`]: whether to strip authentication.
 * **strip_fragment** *?bool|str* [`'except-routing'`]: whether to strip the url's fragment. If set to `except-routing`, will only strip the fragment if the fragment is not deemed to be js routing (i.e. if it contains a `/`).
 * **strip_index** *?bool* [`True`]: whether to strip trailing index.
 * **strip_irrelevant_subdomains** *?bool* [`False`]: whether to strip irrelevant subdomains such as `www` etc.
 * **strip_protocol** *?bool* [`True`]: whether to strip the url's protocol.
 * **strip_trailing_slash** *?bool* [`True`]: whether to strip trailing slash.
-* **unsplit** *?bool* [`True`]: whether to return a stringified version of the normalized url or directly the `SplitResult` instance worked on by the normalization process.
+* **quoted** *?bool* [`False`]: by default the function will unquote the url as much as possible all while keeping the url safe. If this kwarg is set to `True`, the function will instead quote the url as much as possible all while ensuring nothing will be double-quoted.
 
 ---
 
 ### should_follow_href
 
 Function returning whether the given href should be followed (usually from a crawler's context). This means it will filter out anchors, and url having a scheme which is not http/https.
```

### Comparing `ural-1.0.0a1/setup.py` & `ural-1.0.0a2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="ural",
-    version="1.0.0-a1",
+    version="1.0.0-a2",
     description="A helper library full of URL-related heuristics.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/medialab/ural",
-    license="MIT",
-    author="Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel",
+    author="Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel, César Pichon",
     author_email="guillaume.plique@sciencespo.fr",
     keywords="url",
+    license="GPL-3.0",
     python_requires=">=2.7",
     packages=find_packages(exclude=["scripts", "test"]),
     package_data={"docs": ["README.md"], "ural": ["*.pyi", "**/*.pyi"]},
     install_requires=[],
     extras_require={":python_version<'3.8'": ["typing_extensions"]},
     zip_safe=True,
 )
```

