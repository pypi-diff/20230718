# Comparing `tmp/nonebot_plugin_templates-0.1.1.tar.gz` & `tmp/nonebot_plugin_templates-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_templates-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_templates-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_templates-0.1.1.tar` & `nonebot_plugin_templates-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     5861 2023-07-18 02:38:35.241359 nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/template_types.py
--rw-r--r--   0        0        0     4545 2023-07-18 02:38:35.327079 nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/templates/cards.html
--rw-r--r--   0        0        0     4336 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/templates/colorlist.html
--rw-r--r--   0        0        0     3821 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/templates/menus.html
--rw-r--r--   0        0        0 10968356 2023-07-18 02:38:35.327079 nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/templates/PingFang.ttf
--rw-r--r--   0        0        0     6543 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/templates_render.py
--rw-r--r--   0        0        0      471 2023-07-18 02:38:35.329079 nonebot_plugin_templates-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1667 2023-07-18 02:42:24.784189 nonebot_plugin_templates-0.1.1/README.md
--rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 nonebot_plugin_templates-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      305 2023-07-18 03:41:10.378463 nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/__init__.py
+-rw-r--r--   0        0        0     5861 2023-07-18 02:38:35.241359 nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/template_types.py
+-rw-r--r--   0        0        0     4545 2023-07-18 02:38:35.327079 nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/templates/cards.html
+-rw-r--r--   0        0        0     4336 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/templates/colorlist.html
+-rw-r--r--   0        0        0     3821 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/templates/menus.html
+-rw-r--r--   0        0        0 10968356 2023-07-18 02:38:35.327079 nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/templates/PingFang.ttf
+-rw-r--r--   0        0        0     6543 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/templates_render.py
+-rw-r--r--   0        0        0      471 2023-07-18 03:41:36.492987 nonebot_plugin_templates-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3450 2023-07-18 03:34:04.186661 nonebot_plugin_templates-0.1.2/README.md
+-rw-r--r--   0        0        0     4011 1970-01-01 00:00:00.000000 nonebot_plugin_templates-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/template_types.py` & `nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/template_types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/templates/cards.html` & `nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/templates/cards.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/templates/colorlist.html` & `nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/templates/colorlist.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/templates/menus.html` & `nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/templates/menus.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/templates/PingFang.ttf` & `nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/templates/PingFang.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.1/nonebot_plugin_templates/templates_render.py` & `nonebot_plugin_templates-0.1.2/nonebot_plugin_templates/templates_render.py`

 * *Files identical despite different names*

