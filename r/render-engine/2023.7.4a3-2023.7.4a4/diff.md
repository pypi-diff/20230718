# Comparing `tmp/render_engine-2023.7.4a3.tar.gz` & `tmp/render_engine-2023.7.4a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.7.4a3.tar", last modified: Tue Jul 18 02:09:47 2023, max compression
+gzip compressed data, was "render_engine-2023.7.4a4.tar", last modified: Tue Jul 18 03:24:29 2023, max compression
```

## Comparing `render_engine-2023.7.4a3.tar` & `render_engine-2023.7.4a4.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.358816 render_engine-2023.7.4a3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.350816 render_engine-2023.7.4a3/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.350816 render_engine-2023.7.4a3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.350816 render_engine-2023.7.4a3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.github/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.350816 render_engine-2023.7.4a3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.350816 render_engine-2023.7.4a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.350816 render_engine-2023.7.4a3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 02:09:47.358816 render_engine-2023.7.4a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.350816 render_engine-2023.7.4a3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.350816 render_engine-2023.7.4a3/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.354816 render_engine-2023.7.4a3/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/assets/render-engine-init-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.354816 render_engine-2023.7.4a3/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.354816 render_engine-2023.7.4a3/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/getting-started/building-your-site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/getting-started/creating-your-app.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/parsers.md
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/docs/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 02:09:47.358816 render_engine-2023.7.4a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.354816 render_engine-2023.7.4a3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.354816 render_engine-2023.7.4a3/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.354816 render_engine-2023.7.4a3/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.358816 render_engine-2023.7.4a3/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/parsers/markdown/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.358816 render_engine-2023.7.4a3/src/render_engine/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/plugins/clean_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/plugins/site_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.358816 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.354816 render_engine-2023.7.4a3/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 02:09:47.000000 render_engine-2023.7.4a3/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-18 02:09:47.000000 render_engine-2023.7.4a3/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:09:47.000000 render_engine-2023.7.4a3/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 02:09:47.000000 render_engine-2023.7.4a3/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 02:09:47.000000 render_engine-2023.7.4a3/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 02:09:47.000000 render_engine-2023.7.4a3/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.358816 render_engine-2023.7.4a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/create_app_check_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/create_app_check_file_no_site_vars.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.358816 render_engine-2023.7.4a3/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.358816 render_engine-2023.7.4a3/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:09:47.358816 render_engine-2023.7.4a3/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-18 02:09:33.000000 render_engine-2023.7.4a3/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.174140 render_engine-2023.7.4a4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.162140 render_engine-2023.7.4a4/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.162140 render_engine-2023.7.4a4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.162140 render_engine-2023.7.4a4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.162140 render_engine-2023.7.4a4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.162140 render_engine-2023.7.4a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.162140 render_engine-2023.7.4a4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 03:24:29.174140 render_engine-2023.7.4a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.162140 render_engine-2023.7.4a4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.166140 render_engine-2023.7.4a4/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.166140 render_engine-2023.7.4a4/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/assets/render-engine-init-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.166140 render_engine-2023.7.4a4/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.166140 render_engine-2023.7.4a4/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/getting-started/building-your-site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/getting-started/creating-your-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/docs/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:24:29.174140 render_engine-2023.7.4a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.166140 render_engine-2023.7.4a4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.170140 render_engine-2023.7.4a4/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.170140 render_engine-2023.7.4a4/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.170140 render_engine-2023.7.4a4/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/parsers/markdown/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.170140 render_engine-2023.7.4a4/src/render_engine/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/plugins/clean_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/plugins/site_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.174140 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.170140 render_engine-2023.7.4a4/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 03:24:29.000000 render_engine-2023.7.4a4/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-18 03:24:29.000000 render_engine-2023.7.4a4/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:24:29.000000 render_engine-2023.7.4a4/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 03:24:29.000000 render_engine-2023.7.4a4/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 03:24:29.000000 render_engine-2023.7.4a4/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 03:24:29.000000 render_engine-2023.7.4a4/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.174140 render_engine-2023.7.4a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/create_app_check_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/create_app_check_file_no_site_vars.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.174140 render_engine-2023.7.4a4/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.174140 render_engine-2023.7.4a4/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:24:29.174140 render_engine-2023.7.4a4/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-18 03:24:14.000000 render_engine-2023.7.4a4/tests/test_site.py
```

### Comparing `render_engine-2023.7.4a3/.chglog/CHANGELOG.tpl.md` & `render_engine-2023.7.4a4/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/.chglog/config.yml` & `render_engine-2023.7.4a4/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/.devcontainer/devcontainer.json` & `render_engine-2023.7.4a4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.7.4a4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/.github/CONTRIBUTION.md` & `render_engine-2023.7.4a4/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/.github/FUNDING.yml` & `render_engine-2023.7.4a4/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/.github/LICENSE` & `render_engine-2023.7.4a4/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/.github/dependabot.yml` & `render_engine-2023.7.4a4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/.github/workflows/publish.yml` & `render_engine-2023.7.4a4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/.gitignore` & `render_engine-2023.7.4a4/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/PKG-INFO` & `render_engine-2023.7.4a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine
-Version: 2023.7.4a3
+Version: 2023.7.4a4
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.7.4a3/README.md` & `render_engine-2023.7.4a4/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/changelog.md` & `render_engine-2023.7.4a4/changelog.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/archive.md` & `render_engine-2023.7.4a4/docs/docs/archive.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/assets/create-app-help.png` & `render_engine-2023.7.4a4/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/assets/render-engine-init-help.png` & `render_engine-2023.7.4a4/docs/docs/assets/render-engine-init-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/assets/render-engine-init.png` & `render_engine-2023.7.4a4/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/cli.md` & `render_engine-2023.7.4a4/docs/docs/cli.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/contributing/pages.md` & `render_engine-2023.7.4a4/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/custom_collections.md` & `render_engine-2023.7.4a4/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/getting-started/building-your-site.md` & `render_engine-2023.7.4a4/docs/docs/getting-started/building-your-site.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.7.4a4/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.7.4a4/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/getting-started/installation.md` & `render_engine-2023.7.4a4/docs/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/getting-started/layout.md` & `render_engine-2023.7.4a4/docs/docs/getting-started/layout.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/index.md` & `render_engine-2023.7.4a4/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/page.md` & `render_engine-2023.7.4a4/docs/docs/page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/parsers.md` & `render_engine-2023.7.4a4/docs/docs/parsers.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/plugins.md` & `render_engine-2023.7.4a4/docs/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/docs/templates.md` & `render_engine-2023.7.4a4/docs/docs/templates.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/docs/mkdocs.yml` & `render_engine-2023.7.4a4/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/pyproject.toml` & `render_engine-2023.7.4a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/requirements.txt` & `render_engine-2023.7.4a4/requirements.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/.DS_Store` & `render_engine-2023.7.4a4/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/.DS_Store` & `render_engine-2023.7.4a4/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/_base_object.py` & `render_engine-2023.7.4a4/src/render_engine/_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/archive.py` & `render_engine-2023.7.4a4/src/render_engine/archive.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/blog.py` & `render_engine-2023.7.4a4/src/render_engine/blog.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/cli.py` & `render_engine-2023.7.4a4/src/render_engine/cli.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/collection.py` & `render_engine-2023.7.4a4/src/render_engine/collection.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/engine.py` & `render_engine-2023.7.4a4/src/render_engine/engine.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/feeds.py` & `render_engine-2023.7.4a4/src/render_engine/feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/hookspecs.py` & `render_engine-2023.7.4a4/src/render_engine/hookspecs.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/links.py` & `render_engine-2023.7.4a4/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/page.py` & `render_engine-2023.7.4a4/src/render_engine/page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/parsers/.DS_Store` & `render_engine-2023.7.4a4/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.7.4a4/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/parsers/base_parsers.py` & `render_engine-2023.7.4a4/src/render_engine/parsers/base_parsers.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.7.4a4/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/parsers/markdown/__init__.py` & `render_engine-2023.7.4a4/src/render_engine/parsers/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/plugins/clean_output.py` & `render_engine-2023.7.4a4/src/render_engine/plugins/clean_output.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/plugins/site_map.py` & `render_engine-2023.7.4a4/src/render_engine/plugins/site_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from render_engine.site import Site
 
 
 
 class SiteMap:
     """Generate a sitemap.xml file"""
 
+    default_settings = {
+        "template": "sitemap.xml",
+        "output_path": "sitemap.xml",
+        "map_item_pattern": "*.html",
+    }
+
     @hook_impl
     def post_build_site(
         site: Site,
-        settings: dict[str, typing.Any] = {
-            "SiteMap": {
-                "template": "sitemap.xml",
-                "output_path": "sitemap.xml",
-                "map_pattern": "*.html",
-            },
-        }
+        settings: dict[str, typing.Any],
         ):
         """Generate a sitemap.xml file.
         
         parameters: 
             site: The site object
             settings: The settings for the site
                 template: The template to use for the sitemap.xml file
```

### Comparing `render_engine-2023.7.4a3/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.7.4a4/src/render_engine/render_engine_templates/create_app_py.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.7.4a4/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.7.4a4/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.7.4a4/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine/site.py` & `render_engine-2023.7.4a4/src/render_engine/site.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.7.4a4/src/render_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine
-Version: 2023.7.4a3
+Version: 2023.7.4a4
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.7.4a3/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.7.4a4/src/render_engine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 src/render_engine/parsers/.DS_Store
 src/render_engine/parsers/README.md
 src/render_engine/parsers/README_TEMPLATE.md
 src/render_engine/parsers/__init__.py
 src/render_engine/parsers/base_parsers.py
 src/render_engine/parsers/markdown/README.md
 src/render_engine/parsers/markdown/__init__.py
+src/render_engine/plugins/__init__.py
 src/render_engine/plugins/clean_output.py
 src/render_engine/plugins/site_map.py
 src/render_engine/render_engine_templates/__init__.py
 src/render_engine/render_engine_templates/base.html
 src/render_engine/render_engine_templates/base_collection_path.md
 src/render_engine/render_engine_templates/content.html
 src/render_engine/render_engine_templates/create_app_py.txt
```

### Comparing `render_engine-2023.7.4a3/tests/conftest.py` & `render_engine-2023.7.4a4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/tests/create_app_check_file.txt` & `render_engine-2023.7.4a4/tests/create_app_check_file.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/tests/test_base_object.py` & `render_engine-2023.7.4a4/tests/test_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/tests/test_base_parser.py` & `render_engine-2023.7.4a4/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/tests/test_collections.py` & `render_engine-2023.7.4a4/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/tests/test_create_app.py` & `render_engine-2023.7.4a4/tests/test_create_app.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/tests/test_feeds.py` & `render_engine-2023.7.4a4/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/tests/test_page.py` & `render_engine-2023.7.4a4/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/tests/test_plugins.py` & `render_engine-2023.7.4a4/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a3/tests/test_site.py` & `render_engine-2023.7.4a4/tests/test_site.py`

 * *Files identical despite different names*

