# Comparing `tmp/render_engine-2023.7.4a5.tar.gz` & `tmp/render_engine-2023.7.4a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.7.4a5.tar", last modified: Tue Jul 18 03:44:38 2023, max compression
+gzip compressed data, was "render_engine-2023.7.4a6.tar", last modified: Tue Jul 18 04:25:08 2023, max compression
```

## Comparing `render_engine-2023.7.4a5.tar` & `render_engine-2023.7.4a6.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.792951 render_engine-2023.7.4a5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.776951 render_engine-2023.7.4a5/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.780951 render_engine-2023.7.4a5/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.780951 render_engine-2023.7.4a5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.github/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.780951 render_engine-2023.7.4a5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.780951 render_engine-2023.7.4a5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.780951 render_engine-2023.7.4a5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 03:44:38.792951 render_engine-2023.7.4a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.780951 render_engine-2023.7.4a5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.780951 render_engine-2023.7.4a5/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.784951 render_engine-2023.7.4a5/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/assets/render-engine-init-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.784951 render_engine-2023.7.4a5/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.784951 render_engine-2023.7.4a5/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/getting-started/building-your-site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/getting-started/creating-your-app.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/parsers.md
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/docs/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:44:38.792951 render_engine-2023.7.4a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.784951 render_engine-2023.7.4a5/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.788951 render_engine-2023.7.4a5/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.788951 render_engine-2023.7.4a5/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.788951 render_engine-2023.7.4a5/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/parsers/markdown/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.788951 render_engine-2023.7.4a5/src/render_engine/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/plugins/clean_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/plugins/site_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.792951 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9578 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.788951 render_engine-2023.7.4a5/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 03:44:38.000000 render_engine-2023.7.4a5/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-18 03:44:38.000000 render_engine-2023.7.4a5/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:44:38.000000 render_engine-2023.7.4a5/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 03:44:38.000000 render_engine-2023.7.4a5/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 03:44:38.000000 render_engine-2023.7.4a5/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 03:44:38.000000 render_engine-2023.7.4a5/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.792951 render_engine-2023.7.4a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/create_app_check_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/create_app_check_file_no_site_vars.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.792951 render_engine-2023.7.4a5/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.792951 render_engine-2023.7.4a5/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:44:38.792951 render_engine-2023.7.4a5/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-18 03:44:22.000000 render_engine-2023.7.4a5/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.305494 render_engine-2023.7.4a6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.293494 render_engine-2023.7.4a6/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.293494 render_engine-2023.7.4a6/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.293494 render_engine-2023.7.4a6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.293494 render_engine-2023.7.4a6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.297494 render_engine-2023.7.4a6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.297494 render_engine-2023.7.4a6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 04:25:08.305494 render_engine-2023.7.4a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.297494 render_engine-2023.7.4a6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.297494 render_engine-2023.7.4a6/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.297494 render_engine-2023.7.4a6/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/assets/render-engine-init-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.297494 render_engine-2023.7.4a6/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.297494 render_engine-2023.7.4a6/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/getting-started/building-your-site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/getting-started/creating-your-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/docs/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:25:08.305494 render_engine-2023.7.4a6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.297494 render_engine-2023.7.4a6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.301494 render_engine-2023.7.4a6/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.301494 render_engine-2023.7.4a6/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.301494 render_engine-2023.7.4a6/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/parsers/markdown/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.301494 render_engine-2023.7.4a6/src/render_engine/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/plugins/clean_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/plugins/site_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.301494 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.301494 render_engine-2023.7.4a6/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 04:25:08.000000 render_engine-2023.7.4a6/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-18 04:25:08.000000 render_engine-2023.7.4a6/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:25:08.000000 render_engine-2023.7.4a6/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 04:25:08.000000 render_engine-2023.7.4a6/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 04:25:08.000000 render_engine-2023.7.4a6/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 04:25:08.000000 render_engine-2023.7.4a6/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.305494 render_engine-2023.7.4a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/create_app_check_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/create_app_check_file_no_site_vars.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.305494 render_engine-2023.7.4a6/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.305494 render_engine-2023.7.4a6/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:25:08.305494 render_engine-2023.7.4a6/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-18 04:24:53.000000 render_engine-2023.7.4a6/tests/test_site.py
```

### Comparing `render_engine-2023.7.4a5/.chglog/CHANGELOG.tpl.md` & `render_engine-2023.7.4a6/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/.chglog/config.yml` & `render_engine-2023.7.4a6/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/.devcontainer/devcontainer.json` & `render_engine-2023.7.4a6/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.7.4a6/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/.github/CONTRIBUTION.md` & `render_engine-2023.7.4a6/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/.github/FUNDING.yml` & `render_engine-2023.7.4a6/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/.github/LICENSE` & `render_engine-2023.7.4a6/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/.github/dependabot.yml` & `render_engine-2023.7.4a6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/.github/workflows/publish.yml` & `render_engine-2023.7.4a6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/.gitignore` & `render_engine-2023.7.4a6/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/PKG-INFO` & `render_engine-2023.7.4a6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine
-Version: 2023.7.4a5
+Version: 2023.7.4a6
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.7.4a5/README.md` & `render_engine-2023.7.4a6/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/changelog.md` & `render_engine-2023.7.4a6/changelog.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/archive.md` & `render_engine-2023.7.4a6/docs/docs/archive.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/assets/create-app-help.png` & `render_engine-2023.7.4a6/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/assets/render-engine-init-help.png` & `render_engine-2023.7.4a6/docs/docs/assets/render-engine-init-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/assets/render-engine-init.png` & `render_engine-2023.7.4a6/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/cli.md` & `render_engine-2023.7.4a6/docs/docs/cli.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/contributing/pages.md` & `render_engine-2023.7.4a6/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/custom_collections.md` & `render_engine-2023.7.4a6/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/getting-started/building-your-site.md` & `render_engine-2023.7.4a6/docs/docs/getting-started/building-your-site.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.7.4a6/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.7.4a6/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/getting-started/installation.md` & `render_engine-2023.7.4a6/docs/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/getting-started/layout.md` & `render_engine-2023.7.4a6/docs/docs/getting-started/layout.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/index.md` & `render_engine-2023.7.4a6/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/page.md` & `render_engine-2023.7.4a6/docs/docs/page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/parsers.md` & `render_engine-2023.7.4a6/docs/docs/parsers.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/plugins.md` & `render_engine-2023.7.4a6/docs/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/docs/templates.md` & `render_engine-2023.7.4a6/docs/docs/templates.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/docs/mkdocs.yml` & `render_engine-2023.7.4a6/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/pyproject.toml` & `render_engine-2023.7.4a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/requirements.txt` & `render_engine-2023.7.4a6/requirements.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/.DS_Store` & `render_engine-2023.7.4a6/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/.DS_Store` & `render_engine-2023.7.4a6/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/_base_object.py` & `render_engine-2023.7.4a6/src/render_engine/_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/archive.py` & `render_engine-2023.7.4a6/src/render_engine/archive.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/blog.py` & `render_engine-2023.7.4a6/src/render_engine/blog.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/cli.py` & `render_engine-2023.7.4a6/src/render_engine/cli.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/collection.py` & `render_engine-2023.7.4a6/src/render_engine/collection.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/engine.py` & `render_engine-2023.7.4a6/src/render_engine/engine.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/feeds.py` & `render_engine-2023.7.4a6/src/render_engine/feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/hookspecs.py` & `render_engine-2023.7.4a6/src/render_engine/hookspecs.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/links.py` & `render_engine-2023.7.4a6/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/page.py` & `render_engine-2023.7.4a6/src/render_engine/page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/parsers/.DS_Store` & `render_engine-2023.7.4a6/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.7.4a6/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/parsers/base_parsers.py` & `render_engine-2023.7.4a6/src/render_engine/parsers/base_parsers.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.7.4a6/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/parsers/markdown/__init__.py` & `render_engine-2023.7.4a6/src/render_engine/parsers/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/plugins/clean_output.py` & `render_engine-2023.7.4a6/src/render_engine/plugins/clean_output.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/plugins/site_map.py` & `render_engine-2023.7.4a6/src/render_engine/plugins/site_map.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.7.4a6/src/render_engine/render_engine_templates/create_app_py.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.7.4a6/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.7.4a6/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.7.4a6/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/src/render_engine/site.py` & `render_engine-2023.7.4a6/src/render_engine/site.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,18 @@
         self.subcollections = defaultdict(lambda: {"pages": []})
         self.engine.globals.update(self.site_vars)
         
         # Manage Plugins
         self._pm = pluggy.PluginManager(project_name=_PROJECT_NAME)
         self._pm.add_hookspecs(SiteSpecs)
 
+    def update_site_vars(self, **kwargs) -> None:
+        self.site_vars.update(**kwargs)
+        self.engine.globals.update(self.site_vars)
+
 
     def register_plugins(self, *plugins, **settings: dict[str, typing.Any]) -> None:
         """Register plugins with the site
         
         parameters:
             plugins: list of plugins to register
             settings: settings to pass into the plugins
@@ -88,14 +92,15 @@
     def register_themes(self, *themes) -> None:
         """Register a theme with the site"""
         for theme in themes:
             logging.info(f"Registering theme: {theme}")
             self.engine.loader.loaders.insert(0, theme)
 
 
+
     def collection(self, Collection: type[Collection]) -> Collection:
         """
         Add the collection to the route list to be rendered later.
 
         This is the primary way to add a collection to the site and 
         can either be called on an uninstantiated class or on the class definition as a decorator.
 
@@ -240,14 +245,16 @@
 
             pre_build_task = progress.add_task("Loading Pre-Build Plugins", total=1)
             self._pm.hook.pre_build_site(
                 site=self,
                 settings=self.site_settings.get('plugins', {})
                 ) #type: ignore
 
+
+            self.engine.globals.update(self.site_vars)
             # Parse Route List
             task_add_route = progress.add_task(
                 "[blue]Adding Routes", total=len(self.route_list)
             )
 
             if pathlib.Path(self.static_path).exists():
                 self._render_static()
```

### Comparing `render_engine-2023.7.4a5/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.7.4a6/src/render_engine.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine
-Version: 2023.7.4a5
+Version: 2023.7.4a6
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.7.4a5/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.7.4a6/src/render_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/tests/conftest.py` & `render_engine-2023.7.4a6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/tests/create_app_check_file.txt` & `render_engine-2023.7.4a6/tests/create_app_check_file.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/tests/test_base_object.py` & `render_engine-2023.7.4a6/tests/test_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/tests/test_base_parser.py` & `render_engine-2023.7.4a6/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/tests/test_collections.py` & `render_engine-2023.7.4a6/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/tests/test_create_app.py` & `render_engine-2023.7.4a6/tests/test_create_app.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/tests/test_feeds.py` & `render_engine-2023.7.4a6/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/tests/test_page.py` & `render_engine-2023.7.4a6/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/tests/test_plugins.py` & `render_engine-2023.7.4a6/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a5/tests/test_site.py` & `render_engine-2023.7.4a6/tests/test_site.py`

 * *Files identical despite different names*
