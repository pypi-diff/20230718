# Comparing `tmp/human_readable-1.3.3.tar.gz` & `tmp/human_readable-1.3.4.tar.gz`

## Comparing `human_readable-1.3.3.tar` & `human_readable-1.3.4.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 human_readable-1.3.3/.cookiecutter.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 human_readable-1.3.3/.flake8
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 human_readable-1.3.3/.gitattributes
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 human_readable-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 human_readable-1.3.3/.readthedocs.yml
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 human_readable-1.3.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 human_readable-1.3.3/CONTRIBUTING.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 human_readable-1.3.3/bandit.yml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 human_readable-1.3.3/codecov.yml
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/labels.yml
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/release-drafter.yml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/workflows/constraints.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/workflows/hatch-constraints.txt
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/workflows/labeler.yml
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/codeofconduct.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/conf.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/contributing.md
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/index.md
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/license.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/requirements.txt
--rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/usage.md
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/__init__.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/files.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/i18n.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/lists.py
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/numbers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/py.typed
--rw-r--r--   0        0        0    28493 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/times.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/de_DE/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/en_ABBR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/es_ES/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/fa_IR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/fi_FI/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/fr_FR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/id_ID/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/it_IT/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/ja_JP/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/ko_KR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/nl_NL/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/pl_PL/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/pt_BR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/pt_PT/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/ru_RU/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/sk_SK/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/tr_TR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/uk_UA/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/vi_VI/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/zh_CN/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/zh_TW/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/conftest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/en_ABBR/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/en_ABBR/test_numbers.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/en_ABBR/test_times.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/fr_FR/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/fr_FR/test_numbers.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/pt_BR/__init__.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/pt_BR/test_numbers.py
--rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/pt_BR/test_times.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/ru_RU/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/ru_RU/test_numbers.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/ru_RU/test_times.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/__init__.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/test_files.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/test_i18n.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/test_lists.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/test_numbers.py
--rw-r--r--   0        0        0    21943 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/test_times.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 human_readable-1.3.3/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 human_readable-1.3.3/LICENSE
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 human_readable-1.3.3/README.md
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 human_readable-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 human_readable-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 human_readable-1.3.4/.cookiecutter.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 human_readable-1.3.4/.flake8
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 human_readable-1.3.4/.gitattributes
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 human_readable-1.3.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 human_readable-1.3.4/.readthedocs.yml
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 human_readable-1.3.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 human_readable-1.3.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 human_readable-1.3.4/bandit.yml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 human_readable-1.3.4/codecov.yml
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 human_readable-1.3.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 human_readable-1.3.4/.github/labels.yml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 human_readable-1.3.4/.github/release-drafter.yml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 human_readable-1.3.4/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 human_readable-1.3.4/.github/workflows/hatch-constraints.txt
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 human_readable-1.3.4/.github/workflows/labeler.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 human_readable-1.3.4/.github/workflows/release-dev.yml
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 human_readable-1.3.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 human_readable-1.3.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 human_readable-1.3.4/docs/codeofconduct.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 human_readable-1.3.4/docs/conf.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 human_readable-1.3.4/docs/contributing.md
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 human_readable-1.3.4/docs/index.md
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 human_readable-1.3.4/docs/license.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 human_readable-1.3.4/docs/requirements.txt
+-rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 human_readable-1.3.4/docs/usage.md
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/__init__.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/files.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/i18n.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/lists.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/numbers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/py.typed
+-rw-r--r--   0        0        0    28493 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/times.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/de_DE/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/en_ABBR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/es_ES/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/fa_IR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/fi_FI/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/fr_FR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/id_ID/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/it_IT/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/ja_JP/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/ko_KR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/nl_NL/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/pl_PL/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/pt_BR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/pt_PT/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/ru_RU/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/sk_SK/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/tr_TR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/uk_UA/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/vi_VI/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/zh_CN/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 human_readable-1.3.4/src/human_readable/locale/zh_TW/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/conftest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/en_ABBR/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/en_ABBR/test_numbers.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/en_ABBR/test_times.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/fr_FR/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/fr_FR/test_numbers.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/pt_BR/__init__.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/pt_BR/test_numbers.py
+-rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/pt_BR/test_times.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/ru_RU/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/ru_RU/test_numbers.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/functional/ru_RU/test_times.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/unit/test_files.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/unit/test_i18n.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/unit/test_lists.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/unit/test_numbers.py
+-rw-r--r--   0        0        0    21943 2020-02-02 00:00:00.000000 human_readable-1.3.4/tests/unit/test_times.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 human_readable-1.3.4/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 human_readable-1.3.4/LICENSE
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 human_readable-1.3.4/README.md
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 human_readable-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 human_readable-1.3.4/PKG-INFO
```

### Comparing `human_readable-1.3.3/.pre-commit-config.yaml` & `human_readable-1.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/CODE_OF_CONDUCT.md` & `human_readable-1.3.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/CONTRIBUTING.md` & `human_readable-1.3.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/.github/labels.yml` & `human_readable-1.3.4/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/.github/release-drafter.yml` & `human_readable-1.3.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/.github/workflows/tests.yml` & `human_readable-1.3.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/docs/usage.md` & `human_readable-1.3.4/docs/usage.md`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/__init__.py` & `human_readable-1.3.4/src/human_readable/__init__.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/files.py` & `human_readable-1.3.4/src/human_readable/files.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/i18n.py` & `human_readable-1.3.4/src/human_readable/i18n.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/lists.py` & `human_readable-1.3.4/src/human_readable/lists.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/numbers.py` & `human_readable-1.3.4/src/human_readable/numbers.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/times.py` & `human_readable-1.3.4/src/human_readable/times.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/de_DE/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/de_DE/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/en_ABBR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/en_ABBR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/es_ES/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/es_ES/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/fa_IR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/fa_IR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/fi_FI/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/fi_FI/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/fr_FR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/fr_FR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/id_ID/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/id_ID/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/it_IT/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/it_IT/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/ja_JP/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/ja_JP/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/ko_KR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/ko_KR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/nl_NL/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/nl_NL/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/pl_PL/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/pl_PL/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/pt_BR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/pt_BR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/pt_PT/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/pt_PT/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/ru_RU/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/ru_RU/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/sk_SK/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/sk_SK/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/tr_TR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/tr_TR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/uk_UA/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/uk_UA/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/vi_VI/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/vi_VI/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/zh_CN/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/zh_CN/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/src/human_readable/locale/zh_TW/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.4/src/human_readable/locale/zh_TW/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/tests/functional/conftest.py` & `human_readable-1.3.4/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/tests/functional/en_ABBR/test_times.py` & `human_readable-1.3.4/tests/functional/en_ABBR/test_times.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/tests/functional/pt_BR/test_numbers.py` & `human_readable-1.3.4/tests/functional/pt_BR/test_numbers.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/tests/functional/pt_BR/test_times.py` & `human_readable-1.3.4/tests/functional/pt_BR/test_times.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/tests/functional/ru_RU/test_times.py` & `human_readable-1.3.4/tests/functional/ru_RU/test_times.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/tests/unit/test_files.py` & `human_readable-1.3.4/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/tests/unit/test_i18n.py` & `human_readable-1.3.4/tests/unit/test_i18n.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/tests/unit/test_lists.py` & `human_readable-1.3.4/tests/unit/test_lists.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/tests/unit/test_numbers.py` & `human_readable-1.3.4/tests/unit/test_numbers.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/tests/unit/test_times.py` & `human_readable-1.3.4/tests/unit/test_times.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/LICENSE` & `human_readable-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/README.md` & `human_readable-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.3/pyproject.toml` & `human_readable-1.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 [project]
 name = "human-readable"
-version = "1.3.3"
+dynamic = ["version"]
 description = "Human Readable"
 authors = [
   { name = "staticdev", email = "staticdev-support@proton.me"}
 ]
-license = "MIT"
+license = {text = "MIT"}
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.8"
 dependencies = []
 
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.version.raw-options]
+local_scheme = "no-local-version"
+
 [project.urls]
 homepage = "https://github.com/staticdev/human-readable"
 repository = "https://github.com/staticdev/human-readable"
 documentation = "https://human-readable.readthedocs.io"
 changelog = "https://github.com/staticdev/human-readable/releases"
 
 [tool.hatch.envs.default]
@@ -196,9 +202,9 @@
 
 [tool.hatch.build]
 exclude = [
   "src/human_readable/locale/**/*.po",
 ]
 
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
```

### Comparing `human_readable-1.3.3/PKG-INFO` & `human_readable-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: human-readable
-Version: 1.3.3
+Version: 1.3.4
 Summary: Human Readable
 Project-URL: homepage, https://github.com/staticdev/human-readable
 Project-URL: repository, https://github.com/staticdev/human-readable
 Project-URL: documentation, https://human-readable.readthedocs.io
 Project-URL: changelog, https://github.com/staticdev/human-readable/releases
 Author-email: staticdev <staticdev-support@proton.me>
-License-Expression: MIT
+License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

