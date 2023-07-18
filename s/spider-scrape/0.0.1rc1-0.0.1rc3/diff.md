# Comparing `tmp/spider_scrape-0.0.1rc1.tar.gz` & `tmp/spider_scrape-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider_scrape-0.0.1rc1.tar", max compression
+gzip compressed data, was "spider_scrape-0.0.1rc3.tar", max compression
```

## Comparing `spider_scrape-0.0.1rc1.tar` & `spider_scrape-0.0.1rc3.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0     1118 2023-07-15 08:54:14.722895 spider_scrape-0.0.1rc1/LICENSE
--rw-r--r--   0        0        0      373 2023-07-15 09:50:26.814148 spider_scrape-0.0.1rc1/README.md
--rw-r--r--   0        0        0      323 2023-07-15 10:09:42.223368 spider_scrape-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0      190 2023-07-15 09:49:37.256196 spider_scrape-0.0.1rc1/spider_scrape/__init__.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 spider_scrape-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     1118 2023-07-15 10:16:29.599632 spider_scrape-0.0.1rc3/LICENSE
+-rw-r--r--   0        0        0      379 2023-07-15 10:16:29.599729 spider_scrape-0.0.1rc3/README.md
+-rw-r--r--   0        0        0      841 2023-07-18 19:56:25.269492 spider_scrape-0.0.1rc3/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-07-15 10:16:29.600047 spider_scrape-0.0.1rc3/spider_scrape/__init__.py
+-rw-r--r--   0        0        0     1747 2023-07-16 11:47:32.921523 spider_scrape-0.0.1rc3/spider_scrape/arango_db.py
+-rw-r--r--   0        0        0     1712 2023-07-18 19:53:25.133023 spider_scrape-0.0.1rc3/spider_scrape/bs.py
+-rw-r--r--   0        0        0      455 2023-07-16 11:47:32.914044 spider_scrape-0.0.1rc3/spider_scrape/db.py
+-rw-r--r--   0        0        0      746 2023-07-16 11:47:09.633283 spider_scrape-0.0.1rc3/spider_scrape/scraper.py
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 spider_scrape-0.0.1rc3/PKG-INFO
```

### Comparing `spider_scrape-0.0.1rc1/LICENSE` & `spider_scrape-0.0.1rc3/LICENSE`

 * *Files identical despite different names*

