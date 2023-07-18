# Comparing `tmp/nics-2.8.4.tar.gz` & `tmp/nics-3.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-j2pr5lfj/nics-2.8.4.tar", last modified: Thu Jul 13 18:36:06 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-odb5mm82/nics-3.0.0b0.tar", last modified: Tue Jul 18 18:04:44 2023, max compression
```

## Comparing `nics-2.8.4.tar` & `nics-3.0.0b0.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 18:35:58.000000 nics-2.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 18:35:58.000000 nics-2.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-13 18:36:06.000000 nics-2.8.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 18:35:58.000000 nics-2.8.4/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/404.md
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/1 - Page1.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/docs/tree/2 - Pages/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/2 - Pages/baz.md
--rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/2 - Pages/logo200.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/docs/tree/7 - FAQs/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/7 - FAQs/1 - Question1.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/7 - FAQs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/8 - Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/9 - About.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/_sass/main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/_sass/sass-code-highlight.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/wizard/workflow_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-13 18:35:58.000000 nics-2.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-13 18:35:58.000000 nics-2.8.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 18:36:06.000000 nics-2.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 18:35:58.000000 nics-2.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 18:04:37.000000 nics-3.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 18:04:37.000000 nics-3.0.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-18 18:04:44.000000 nics-3.0.0b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/cmd_init/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/ensure_nics_env_can_be_installed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/get_user_details.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/cmd_init/loading/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/loading/copy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/loading/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/loading/workflow_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/print_outro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/cmd_upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_upgrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/settings.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/template/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/1 - Page1.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/template/tree/2 - Pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/2 - Pages/logo200.png
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/2 - Pages/page.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/template/tree/7 - FAQs/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/7 - FAQs/1 - Question1.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/7 - FAQs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/8 - Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/9 - About.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/utils/ensure_a_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/utils/favicon_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/utils/is_nics_initialized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/utils/page404_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics_compiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics_compiler/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics_compiler/compiler/customize/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/custom_config_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/custom_constants_sass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/custom_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/custom_nav_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-18 18:04:37.000000 nics-3.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-18 18:04:37.000000 nics-3.0.0b0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 18:04:44.000000 nics-3.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 18:04:37.000000 nics-3.0.0b0/setup.py
```

### Comparing `nics-2.8.4/LICENSE` & `nics-3.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-2.8.4/PKG-INFO` & `nics-3.0.0b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.8.4
+Version: 3.0.0b0
 Summary: Automated markdown-based documentation page workflow
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
@@ -18,37 +18,37 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Now I Can Sleep
 
-A minimalist, readable, easy-to-configure, and markdown-based automated documentation workflow for GitHub repositories.
+Minimal settings, markdown-based automated documentation workflow for GitHub repositories.
 
 ```txt
-🐈BEFORE🐈
+Manual workflow:
 
            ┌──────────>  Make changes  ────────────┐
            |                                       v
 
     Deploy docs-page                       Update docs-files
 
            ^                                       │
            └─────────  Rebuild docs-page  <────────┘
 
 
 
-🐾with NICS🐾
+With NICS:
 
            ┌──────────>  Make changes  ────────────┐
            |                                       |
            └─────────  Update docs-files  <────────┘
 ```
 
-![nics' banner](https://raw.githubusercontent.com/nvfp/now-i-can-sleep/master/assets/logo200.png)
+![NICS' banner](https://raw.githubusercontent.com/nvfp/now-i-can-sleep/master/assets/logo200.png)
 
 [![Rebuild docs](https://github.com/nvfp/now-i-can-sleep/actions/workflows/rebuild-docs.yml/badge.svg)](https://github.com/nvfp/now-i-can-sleep/actions/workflows/rebuild-docs.yml)
 [![pypi version](https://img.shields.io/pypi/v/nics?logo=pypi)](https://pypi.org/project/nics/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
```

### Comparing `nics-2.8.4/nics/main/_template/docs/tree/2 - Pages/logo200.png` & `nics-3.0.0b0/nics/main/template/tree/2 - Pages/logo200.png`

 * *Files identical despite different names*

### Comparing `nics-2.8.4/nics/main/compile/update_404_and_favicon.py` & `nics-3.0.0b0/nics_compiler/compiler/customize/custom_favicon.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import shutil
 
 from mykit.kit.utils import printer
 
+from nics.main.utils.favicon_maker import create_favicon_svg_file
 
-def update_404_and_favicon(C_404, C_ICON, D_404, D_ICON):
+
+def custom_favicon(C_404, C_ICON, D_404, D_ICON):
 
     ## 404 page
     printer(f"DEBUG: Attempting to copy '404.md'.")
     if os.path.isfile(C_404):
         printer(f'DEBUG: Rewriting 404.md from {repr(C_404)} to {repr(D_404)}.')
         text = (
             '---\n'
```

### Comparing `nics-2.8.4/nics/main/compile/update_docs_tree.py` & `nics-3.0.0b0/nics_compiler/compiler/customize/update_docs_tree.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.4/nics/main/compile/update_header.py` & `nics-3.0.0b0/nics_compiler/compiler/customize/custom_nav_html.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,8 +48,24 @@
     text += (
                 '</div>'
             '</div>'
         '</header>'
     )
 
     with open(D_HEADER, 'w') as f: f.write(text)
-    printer(f'INFO: Updated header {repr(D_HEADER)}.')
+    printer(f'INFO: Updated header {repr(D_HEADER)}.')
+
+
+
+
+def get_text():
+    text = '<nav>'
+    text += '</nav>'
+    return text
+
+
+def custom_nav_html(container, dock, lowercase_the_url):
+    printer(f'DEBUG: Rewriting _includes/nav.html file.')
+
+    text = get_text()
+    with open(os.path.join(dock, '_includes', 'nav.html'), 'w') as f:
+        f.write(text)
```

### Comparing `nics-2.8.4/nics.egg-info/PKG-INFO` & `nics-3.0.0b0/nics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.8.4
+Version: 3.0.0b0
 Summary: Automated markdown-based documentation page workflow
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
@@ -18,37 +18,37 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Now I Can Sleep
 
-A minimalist, readable, easy-to-configure, and markdown-based automated documentation workflow for GitHub repositories.
+Minimal settings, markdown-based automated documentation workflow for GitHub repositories.
 
 ```txt
-🐈BEFORE🐈
+Manual workflow:
 
            ┌──────────>  Make changes  ────────────┐
            |                                       v
 
     Deploy docs-page                       Update docs-files
 
            ^                                       │
            └─────────  Rebuild docs-page  <────────┘
 
 
 
-🐾with NICS🐾
+With NICS:
 
            ┌──────────>  Make changes  ────────────┐
            |                                       |
            └─────────  Update docs-files  <────────┘
 ```
 
-![nics' banner](https://raw.githubusercontent.com/nvfp/now-i-can-sleep/master/assets/logo200.png)
+![NICS' banner](https://raw.githubusercontent.com/nvfp/now-i-can-sleep/master/assets/logo200.png)
 
 [![Rebuild docs](https://github.com/nvfp/now-i-can-sleep/actions/workflows/rebuild-docs.yml/badge.svg)](https://github.com/nvfp/now-i-can-sleep/actions/workflows/rebuild-docs.yml)
 [![pypi version](https://img.shields.io/pypi/v/nics?logo=pypi)](https://pypi.org/project/nics/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
```

### Comparing `nics-2.8.4/pyproject.toml` & `nics-3.0.0b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "2.8.4"
+version = "3.0.0b0"
 description = "Automated markdown-based documentation page workflow"
 readme = "readme.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
@@ -28,14 +28,15 @@
 
 
 [tool.setuptools.packages.find]
 exclude = [
     "archive*",
     "assets*",
     "docs*",
+    "nics-compiler*",
     "tests*",
 ]
 
 
 [project.urls]
 Documentation = "https://nvfp.github.io/now-i-can-sleep/docs"
 "Report bugs" = "https://github.com/nvfp/now-i-can-sleep/issues"
```

### Comparing `nics-2.8.4/readme.md` & `nics-3.0.0b0/readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Now I Can Sleep
 
-A minimalist, readable, easy-to-configure, and markdown-based automated documentation workflow for GitHub repositories.
+Minimal settings, markdown-based automated documentation workflow for GitHub repositories.
 
 ```txt
-🐈BEFORE🐈
+Manual workflow:
 
            ┌──────────>  Make changes  ────────────┐
            |                                       v
 
     Deploy docs-page                       Update docs-files
 
            ^                                       │
            └─────────  Rebuild docs-page  <────────┘
 
 
 
-🐾with NICS🐾
+With NICS:
 
            ┌──────────>  Make changes  ────────────┐
            |                                       |
            └─────────  Update docs-files  <────────┘
 ```
 
-![nics' banner](https://raw.githubusercontent.com/nvfp/now-i-can-sleep/master/assets/logo200.png)
+![NICS' banner](https://raw.githubusercontent.com/nvfp/now-i-can-sleep/master/assets/logo200.png)
 
 [![Rebuild docs](https://github.com/nvfp/now-i-can-sleep/actions/workflows/rebuild-docs.yml/badge.svg)](https://github.com/nvfp/now-i-can-sleep/actions/workflows/rebuild-docs.yml)
 [![pypi version](https://img.shields.io/pypi/v/nics?logo=pypi)](https://pypi.org/project/nics/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
```

