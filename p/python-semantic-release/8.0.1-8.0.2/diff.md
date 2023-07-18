# Comparing `tmp/python-semantic-release-8.0.1.tar.gz` & `tmp/python-semantic-release-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-8.0.1.tar", last modified: Mon Jul 17 20:04:47 2023, max compression
+gzip compressed data, was "python-semantic-release-8.0.2.tar", last modified: Tue Jul 18 21:40:50 2023, max compression
```

## Comparing `python-semantic-release-8.0.1.tar` & `python-semantic-release-8.0.2.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.047376 python-semantic-release-8.0.1/
--rw-r--r--   0 root         (0) root         (0)      230 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1084 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      153 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3108 2023-07-17 20:04:47.047376 python-semantic-release-8.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2272 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/README.rst
--rw-r--r--   0 root         (0) root         (0)     4691 2023-07-17 20:04:39.000000 python-semantic-release-8.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.031376 python-semantic-release-8.0.1/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3108 2023-07-17 20:04:47.000000 python-semantic-release-8.0.1/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4221 2023-07-17 20:04:47.000000 python-semantic-release-8.0.1/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 20:04:47.000000 python-semantic-release-8.0.1/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-07-17 20:04:47.000000 python-semantic-release-8.0.1/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      610 2023-07-17 20:04:47.000000 python-semantic-release-8.0.1/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-17 20:04:47.000000 python-semantic-release-8.0.1/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.031376 python-semantic-release-8.0.1/semantic_release/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-17 20:04:39.000000 python-semantic-release-8.0.1/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.031376 python-semantic-release-8.0.1/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      361 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4328 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.035376 python-semantic-release-8.0.1/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.035376 python-semantic-release-8.0.1/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    18649 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    13706 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.035376 python-semantic-release-8.0.1/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      884 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.027376 python-semantic-release-8.0.1/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.035376 python-semantic-release-8.0.1/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.039376 python-semantic-release-8.0.1/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      300 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5595 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     8285 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10146 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     5898 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.039376 python-semantic-release-8.0.1/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      339 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14641 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7267 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3037 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14060 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 20:04:47.047376 python-semantic-release-8.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.027376 python-semantic-release-8.0.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.039376 python-semantic-release-8.0.1/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    20288 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/command_line/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.043376 python-semantic-release-8.0.1/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    45283 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/fixtures/git_repo.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.043376 python-semantic-release-8.0.1/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46838 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12186 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.043376 python-semantic-release-8.0.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.043376 python-semantic-release-8.0.1/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.043376 python-semantic-release-8.0.1/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5005 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     2540 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.043376 python-semantic-release-8.0.1/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.047376 python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.047376 python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    22533 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    23987 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    13407 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:04:47.047376 python-semantic-release-8.0.1/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8947 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9640 2023-07-17 20:03:51.000000 python-semantic-release-8.0.1/tests/unit/semantic_release/version/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      153 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)     4651 2023-07-18 21:40:42.000000 python-semantic-release-8.0.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.645312 python-semantic-release-8.0.2/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      598 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.645312 python-semantic-release-8.0.2/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-18 21:40:43.000000 python-semantic-release-8.0.2/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.649312 python-semantic-release-8.0.2/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.649312 python-semantic-release-8.0.2/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.649312 python-semantic-release-8.0.2/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    18649 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    12975 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.649312 python-semantic-release-8.0.2/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      884 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.641312 python-semantic-release-8.0.2/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.653312 python-semantic-release-8.0.2/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.653312 python-semantic-release-8.0.2/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     8285 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    10146 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.653312 python-semantic-release-8.0.2/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14641 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7267 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14060 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.641312 python-semantic-release-8.0.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.653312 python-semantic-release-8.0.2/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     3631 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    20288 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    45283 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/fixtures/git_repo.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46838 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5005 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    22533 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    23987 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    13407 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8947 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9640 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_version.py
```

### Comparing `python-semantic-release-8.0.1/LICENSE` & `python-semantic-release-8.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/PKG-INFO` & `python-semantic-release-8.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.1
+Version: 8.0.2
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.1/README.rst` & `python-semantic-release-8.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/pyproject.toml` & `python-semantic-release-8.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "8.0.1"
+version = "8.0.2"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.7"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 readme = "README.rst"
 authors = [{ name = "Rolf Erik Lekang", email = "me@rolflekang.com" }]
 dependencies = [
-  "click>=7,<9",
+  "click>=8,<9",
   "gitpython>=3.0.8,<4",
   "requests>=2.25,<3",
   "jinja2>=3.1.2,<4",
   "python-gitlab>=2,<4",
   "tomlkit~=0.10",
   "dotty-dict>=1.3.0,<2",
   "dataclasses==0.8; python_version < '3.7.0'",
@@ -58,15 +58,15 @@
   "pytest-lazy-fixture~=0.6.3",
   "pytest-cov>=4,<5",
   "responses==0.21.0",
   "requests-mock>=1.10.0,<2",
   "types-pytest-lazy-fixture>=0.6.3.3",
 ]
 dev = ["tox", "isort", "black"]
-mypy = ["mypy", "types-requests", "types-click"]
+mypy = ["mypy", "types-requests"]
 
 [tool.pytest.ini_options]
 addopts = [
   "-nauto",
   "-ra",
   "--cache-clear",
   "--cov=semantic_release",
@@ -120,15 +120,15 @@
 deps = .[test]
 commands =
     coverage run -p --source=semantic_release -m pytest -v {posargs:tests}
 
 [testenv:mypy]
 deps = .[mypy]
 commands =
-    mypy --ignore-missing-imports semantic_release
+    mypy semantic_release
 
 [testenv:coverage]
 deps = coverage[toml]
 commands =
     coverage combine
     coverage report -m
     coverage xml
```

### Comparing `python-semantic-release-8.0.1/python_semantic_release.egg-info/PKG-INFO` & `python-semantic-release-8.0.2/python_semantic_release.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.1
+Version: 8.0.2
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.1/python_semantic_release.egg-info/SOURCES.txt` & `python-semantic-release-8.0.2/python_semantic_release.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 tests/unit/semantic_release/changelog/test_default_changelog.py
 tests/unit/semantic_release/changelog/test_release_notes.py
 tests/unit/semantic_release/changelog/test_template.py
 tests/unit/semantic_release/cli/__init__.py
 tests/unit/semantic_release/cli/test_config.py
 tests/unit/semantic_release/cli/test_github_actions_output.py
 tests/unit/semantic_release/cli/test_masking_filter.py
+tests/unit/semantic_release/cli/test_util.py
 tests/unit/semantic_release/cli/test_version.py
 tests/unit/semantic_release/commit_parser/__init__.py
 tests/unit/semantic_release/commit_parser/helper.py
 tests/unit/semantic_release/commit_parser/test_angular.py
 tests/unit/semantic_release/commit_parser/test_emoji.py
 tests/unit/semantic_release/commit_parser/test_scipy.py
 tests/unit/semantic_release/commit_parser/test_tag.py
```

### Comparing `python-semantic-release-8.0.1/python_semantic_release.egg-info/requires.txt` & `python-semantic-release-8.0.2/python_semantic_release.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-click<9,>=7
+click<9,>=8
 gitpython<4,>=3.0.8
 requests<3,>=2.25
 jinja2<4,>=3.1.2
 python-gitlab<4,>=2
 tomlkit~=0.10
 dotty-dict<2,>=1.3.0
 importlib-resources==5.7
@@ -23,15 +23,14 @@
 sphinxcontrib-apidoc==0.3.0
 sphinx-autobuild==2021.03.14
 furo>=2023.3.27
 
 [mypy]
 mypy
 types-requests
-types-click
 
 [test]
 coverage[toml]<7,>=6
 pytest<8,>=7
 pytest-xdist<3,>=2
 pytest-mock<4,>=3
 pytest-lazy-fixture~=0.6.3
```

### Comparing `python-semantic-release-8.0.1/semantic_release/__init__.py` & `python-semantic-release-8.0.2/semantic_release/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from semantic_release.version import (
     Version as Version,
     VersionTranslator as VersionTranslator,
     next_version as next_version,
     tags_and_versions as tags_and_versions,
 )
 
-__version__ = "8.0.1"
+__version__ = "8.0.2"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-8.0.1/semantic_release/changelog/context.py` & `python-semantic-release-8.0.2/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/changelog/release_history.py` & `python-semantic-release-8.0.2/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/changelog/template.py` & `python-semantic-release-8.0.2/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/cli/commands/changelog.py` & `python-semantic-release-8.0.2/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/cli/commands/generate_config.py` & `python-semantic-release-8.0.2/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/cli/commands/main.py` & `python-semantic-release-8.0.2/semantic_release/cli/commands/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from __future__ import annotations
 
-import json
 import logging
 from pathlib import Path
 
 import click
+from click.core import ParameterSource
 from git import InvalidGitRepositoryError
 from git.repo.base import Repo
 from rich.console import Console
 from rich.logging import RichHandler
 
 import semantic_release
 from semantic_release.cli.commands.generate_config import generate_config
 from semantic_release.cli.config import (
     GlobalCommandLineOptions,
     RawConfig,
     RuntimeContext,
-    read_toml,
 )
 from semantic_release.cli.const import DEFAULT_CONFIG_FILE
-from semantic_release.cli.util import rprint
+from semantic_release.cli.util import load_raw_config_file, rprint
 from semantic_release.errors import InvalidConfiguration, NotAReleaseBranch
 
 FORMAT = "[%(name)s] %(levelname)s %(module)s.%(funcName)s: %(message)s"
 
 
 @click.group(
     context_settings={
@@ -37,15 +36,15 @@
 )
 @click.option(
     "-c",
     "--config",
     "config_file",
     default=DEFAULT_CONFIG_FILE,
     help="Specify a configuration file for semantic-release to use",
-    type=click.Path(exists=True),
+    type=click.Path(),
 )
 @click.option("--noop", "noop", is_flag=True, help="Run semantic-release in no-op mode")
 @click.option(
     "-v",
     "--verbose",
     "verbosity",
     help="Set logging verbosity",
@@ -119,27 +118,34 @@
         noop=noop,
         verbosity=verbosity,
         config_file=config_file,
         strict=strict,
     )
     log.debug("global cli options: %s", cli_options)
 
-    try:
-        if config_file.endswith(".toml"):
-            log.info(f"Loading TOML configuration from {config_file}")
-            config_text = read_toml(config_file)
-        elif config_file.endswith(".json"):
-            log.info(f"Loading JSON configuration from {config_file}")
-            raw_text = (Path() / config_file).resolve().read_text(encoding="utf-8")
-            config_text = json.loads(raw_text)["semantic_release"]
-        else:
-            *_, suffix = config_file.split(".")
-            ctx.fail(f"{suffix!r} is not a supported configuration format")
-    except (FileNotFoundError, InvalidConfiguration) as exc:
-        ctx.fail(str(exc))
+    config_path = Path(config_file)
+    # default no config loaded
+    config_text = {}
+    if not config_path.exists():
+        if ctx.get_parameter_source("config_file") not in (
+            ParameterSource.DEFAULT,
+            ParameterSource.DEFAULT_MAP,
+        ):
+            ctx.fail(f"File {config_file} does not exist")
+
+        log.info(
+            "configuration file %s not found, using default configuration",
+            config_file,
+        )
+
+    else:
+        try:
+            config_text = load_raw_config_file(config_path)
+        except InvalidConfiguration as exc:
+            ctx.fail(str(exc))
 
     raw_config = RawConfig.parse_obj(config_text)
     try:
         runtime = RuntimeContext.from_raw_config(
             raw_config, repo=repo, global_cli_options=cli_options
         )
     except NotAReleaseBranch as exc:
```

### Comparing `python-semantic-release-8.0.1/semantic_release/cli/commands/publish.py` & `python-semantic-release-8.0.2/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/cli/commands/version.py` & `python-semantic-release-8.0.2/semantic_release/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/cli/common.py` & `python-semantic-release-8.0.2/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/cli/config.py` & `python-semantic-release-8.0.2/semantic_release/cli/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os
 import re
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Any, ClassVar, Dict, List, Optional, Tuple, Union
 
-import tomlkit
 from git import Actor
 from git.repo.base import Repo
 from jinja2 import Environment
 from pydantic import BaseModel
 from typing_extensions import Literal
 
 from semantic_release.changelog import environment
@@ -37,35 +36,14 @@
     TomlVersionDeclaration,
     VersionDeclarationABC,
 )
 
 log = logging.getLogger(__name__)
 
 
-def read_toml(path: str) -> dict[str, Any]:
-    raw_text = (Path() / path).resolve().read_text(encoding="utf-8")
-    try:
-        toml_text = tomlkit.loads(raw_text)
-    except tomlkit.exceptions.TOMLKitError as exc:
-        raise InvalidConfiguration(f"File {path!r} contains invalid TOML") from exc
-
-    # Look for [tool.semantic_release]
-    cfg_text = toml_text.get("tool", {}).get("semantic_release")
-    if cfg_text is not None:
-        return cfg_text
-    # Look for [semantic_release]
-    cfg_text = toml_text.get("semantic_release")
-    if cfg_text is not None:
-        return cfg_text
-
-    raise InvalidConfiguration(
-        f"Missing keys 'tool.semantic_release' or 'semantic_release' in {path}"
-    )
-
-
 class HvcsClient(str, Enum):
     GITHUB = "github"
     GITLAB = "gitlab"
     GITEA = "gitea"
 
 
 class EnvConfigVar(BaseModel):
```

### Comparing `python-semantic-release-8.0.1/semantic_release/cli/github_actions_output.py` & `python-semantic-release-8.0.2/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/cli/masking_filter.py` & `python-semantic-release-8.0.2/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/commit_parser/__init__.py` & `python-semantic-release-8.0.2/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/commit_parser/_base.py` & `python-semantic-release-8.0.2/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/commit_parser/angular.py` & `python-semantic-release-8.0.2/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/commit_parser/emoji.py` & `python-semantic-release-8.0.2/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/commit_parser/scipy.py` & `python-semantic-release-8.0.2/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/commit_parser/tag.py` & `python-semantic-release-8.0.2/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/commit_parser/token.py` & `python-semantic-release-8.0.2/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/commit_parser/util.py` & `python-semantic-release-8.0.2/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/const.py` & `python-semantic-release-8.0.2/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/data/templates/CHANGELOG.md.j2` & `python-semantic-release-8.0.2/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/enums.py` & `python-semantic-release-8.0.2/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/errors.py` & `python-semantic-release-8.0.2/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/helpers.py` & `python-semantic-release-8.0.2/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/hvcs/_base.py` & `python-semantic-release-8.0.2/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/hvcs/gitea.py` & `python-semantic-release-8.0.2/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/hvcs/github.py` & `python-semantic-release-8.0.2/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/hvcs/gitlab.py` & `python-semantic-release-8.0.2/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/hvcs/token_auth.py` & `python-semantic-release-8.0.2/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/hvcs/util.py` & `python-semantic-release-8.0.2/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/version/algorithm.py` & `python-semantic-release-8.0.2/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/version/declaration.py` & `python-semantic-release-8.0.2/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/version/translator.py` & `python-semantic-release-8.0.2/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/semantic_release/version/version.py` & `python-semantic-release-8.0.2/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/command_line/test_changelog.py` & `python-semantic-release-8.0.2/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/command_line/test_generate_config.py` & `python-semantic-release-8.0.2/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/command_line/test_help.py` & `python-semantic-release-8.0.2/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/command_line/test_main.py` & `python-semantic-release-8.0.2/tests/command_line/test_publish.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-import pytest
-
-from semantic_release import __version__
-from semantic_release.cli import main
-
-
-def test_main_prints_version_and_exits(cli_runner):
-    result = cli_runner.invoke(main, ["--version"])
-    assert result.exit_code == 0
-    assert result.output == f"semantic-release, version {__version__}\n"
-
-
-@pytest.mark.parametrize("args", [[], ["--help"]])
-def test_main_prints_help_text(cli_runner, args):
-    result = cli_runner.invoke(main, args)
-    assert result.exit_code == 0
+from unittest import mock
 
+import pytest
 
-def test_not_a_release_branch_exit_code(repo_with_git_flow_angular_commits, cli_runner):
-    # Run anything that doesn't trigger the help text
-    repo_with_git_flow_angular_commits.git.checkout("-b", "branch-does-not-exist")
-    result = cli_runner.invoke(main, ["version", "--no-commit"])
-    assert result.exit_code == 0
+from semantic_release.cli import main, publish
+from semantic_release.hvcs import Github
+from semantic_release.version import tags_and_versions
 
 
-def test_not_a_release_branch_exit_code_with_strict(
-    repo_with_git_flow_angular_commits, cli_runner
+@pytest.mark.parametrize("cmd_args", [(), ("--tag", "latest")])
+def test_publish_latest_uses_latest_tag(
+    repo_with_single_branch_angular_commits,
+    cli_runner,
+    cmd_args,
 ):
-    # Run anything that doesn't trigger the help text
-    repo_with_git_flow_angular_commits.git.checkout("-b", "branch-does-not-exist")
-    result = cli_runner.invoke(main, ["--strict", "version", "--no-commit"])
-    assert result.exit_code != 0
+    with mock.patch.object(Github, "upload_dists") as mocked_upload_dists, mock.patch(
+        "semantic_release.cli.commands.publish.tags_and_versions",
+        return_value=([("v1.0.0", "1.0.0")]),
+    ) as mock_tags_and_versions:
+        result = cli_runner.invoke(main, [publish.name, *cmd_args])
+        assert result.exit_code == 0
+
+    mock_tags_and_versions.assert_called_once()
+    mocked_upload_dists.assert_called_once_with(tag="v1.0.0", dist_glob="dist/*")
+
+
+def test_publish_to_tag_uses_tag(repo_with_single_branch_angular_commits, cli_runner):
+    tag = "v99.999.9999+build.1234"
+    with mock.patch.object(Github, "upload_dists") as mocked_upload_dists, mock.patch(
+        "semantic_release.cli.commands.publish.tags_and_versions",
+        return_value=([("v1.0.0", "1.0.0")]),
+    ) as mock_tags_and_versions:
+        result = cli_runner.invoke(main, [publish.name, "--tag", tag])
+        assert result.exit_code == 0
+
+    mock_tags_and_versions.assert_not_called()
+    assert mocked_upload_dists.called_once_with(tag=tag, dist_glob="dist/*")
```

### Comparing `python-semantic-release-8.0.1/tests/command_line/test_version.py` & `python-semantic-release-8.0.2/tests/command_line/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/fixtures/commit_parsers.py` & `python-semantic-release-8.0.2/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/fixtures/example_project.py` & `python-semantic-release-8.0.2/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/fixtures/git_repo.py` & `python-semantic-release-8.0.2/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/fixtures/scipy.py` & `python-semantic-release-8.0.2/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/scenario/test_next_version.py` & `python-semantic-release-8.0.2/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/scenario/test_release_history.py` & `python-semantic-release-8.0.2/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/scenario/test_template_render.py` & `python-semantic-release-8.0.2/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/changelog/test_release_notes.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/changelog/test_template.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/cli/test_config.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/cli/test_masking_filter.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/cli/test_version.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/test_angular.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/test_tag.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/commit_parser/test_token.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test__base.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test_gitea.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test_github.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/version/test_algorithm.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/version/test_declaration.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/version/test_translator.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.1/tests/unit/semantic_release/version/test_version.py` & `python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

