# Comparing `tmp/dgp-oauth2-1.0.7.tar.gz` & `tmp/dgp-oauth2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgp-oauth2-1.0.7.tar", last modified: Tue Sep  6 16:13:09 2022, max compression
+gzip compressed data, was "dgp-oauth2-1.1.0.tar", last modified: Tue Jul 18 18:45:58 2023, max compression
```

## Comparing `dgp-oauth2-1.0.7.tar` & `dgp-oauth2-1.1.0.tar`

### file list

```diff
@@ -1,194 +1,451 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.186859 dgp-oauth2-1.0.7/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.103670 dgp-oauth2-1.0.7/.tox/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.103767 dgp-oauth2-1.0.7/.tox/py37/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.103860 dgp-oauth2-1.0.7/.tox/py37/lib/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.103957 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.113310 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.119782 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask-1.1.2.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       42 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask-1.1.2.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)        6 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask-1.1.2.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.120380 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask_Cors-3.0.9.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       11 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask_Cors-3.0.9.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.121226 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask_Jsonpify-1.5.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       15 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask_Jsonpify-1.5.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.121879 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask_OAuthlib-0.9.6.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       15 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask_OAuthlib-0.9.6.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.122530 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask_Session-0.3.2.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       14 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Flask_Session-0.3.2.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.123679 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Jinja2-2.11.2.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       61 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Jinja2-2.11.2.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)        7 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Jinja2-2.11.2.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.124230 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/MarkupSafe-1.1.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       11 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/MarkupSafe-1.1.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.125451 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/PyJWT-1.7.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       45 2020-09-24 15:22:26.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/PyJWT-1.7.1.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)        4 2020-09-24 15:22:26.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/PyJWT-1.7.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.126409 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/SQLAlchemy-1.3.19.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       11 2020-09-24 15:22:26.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/SQLAlchemy-1.3.19.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.127066 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Werkzeug-0.16.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/Werkzeug-0.16.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.127884 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/attrs-20.2.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        5 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/attrs-20.2.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.129143 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/cachelib-0.1.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/cachelib-0.1.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.129750 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/certifi-2020.6.20.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        8 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/certifi-2020.6.20.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.130930 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/cffi-1.14.3.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       76 2020-09-24 15:22:26.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/cffi-1.14.3.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)       19 2020-09-24 15:22:26.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/cffi-1.14.3.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.133532 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/chardet-3.0.4.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       60 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/chardet-3.0.4.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)     1375 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/chardet-3.0.4.dist-info/metadata.json
--rw-r--r--   0 adam       (501) staff       (20)        8 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/chardet-3.0.4.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.134002 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/click-7.1.2.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        6 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/click-7.1.2.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.136447 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/coverage-5.3.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)    10174 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/coverage-5.3.dist-info/LICENSE.txt
--rw-r--r--   0 adam       (501) staff       (20)      123 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/coverage-5.3.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/coverage-5.3.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.138732 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/coveralls-2.1.2.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)     1077 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/coveralls-2.1.2.dist-info/LICENSE.txt
--rw-r--r--   0 adam       (501) staff       (20)       50 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/coveralls-2.1.2.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/coveralls-2.1.2.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.139451 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/cryptography-3.1.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       31 2020-09-24 15:22:26.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/cryptography-3.1.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.140071 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/dgp_oauth2/
--rw-r--r--   0 adam       (501) staff       (20)        6 2022-04-25 07:48:29.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/dgp_oauth2/VERSION
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.141329 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/dgp_oauth2-0.2.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)      114 2022-04-25 07:48:29.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/dgp_oauth2-0.2.0.dist-info/direct_url.json
--rw-r--r--   0 adam       (501) staff       (20)       55 2022-04-25 07:48:29.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/dgp_oauth2-0.2.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.141965 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/docopt-0.6.2.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        7 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/docopt-0.6.2.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.142417 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/idna-2.10.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        5 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/idna-2.10.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.143058 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/importlib_metadata-2.0.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       19 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/importlib_metadata-2.0.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.143685 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/iniconfig-1.0.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/iniconfig-1.0.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.144414 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/itsdangerous-1.1.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       13 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/itsdangerous-1.1.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.146319 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/mccabe-0.6.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       47 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/mccabe-0.6.1.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)     1218 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/mccabe-0.6.1.dist-info/metadata.json
--rw-r--r--   0 adam       (501) staff       (20)        7 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/mccabe-0.6.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.146750 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/more_itertools-8.5.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       15 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/more_itertools-8.5.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.148048 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/oauthlib-2.1.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)     1534 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/oauthlib-2.1.0.dist-info/LICENSE.txt
--rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/oauthlib-2.1.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.148587 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/packaging-20.4.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/packaging-20.4.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.109560 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pip/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.150915 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pip/_vendor/
--rw-r--r--   0 adam       (501) staff       (20)      437 2020-09-24 15:22:01.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pip/_vendor/vendor.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.150482 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pip-20.2.2.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)     1090 2020-09-24 15:22:01.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pip-20.2.2.dist-info/LICENSE.txt
--rw-r--r--   0 adam       (501) staff       (20)      125 2020-09-24 15:22:01.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pip-20.2.2.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)        4 2020-09-24 15:22:01.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pip-20.2.2.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.151559 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pluggy-0.13.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        7 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pluggy-0.13.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.152212 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/psycopg2_binary-2.8.6.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:26.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/psycopg2_binary-2.8.6.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.110236 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.110468 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.154130 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/apipkg-1.4.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)      779 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/apipkg-1.4.dist-info/metadata.json
--rw-r--r--   0 adam       (501) staff       (20)        7 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/apipkg-1.4.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.155107 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig-1.0.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)      950 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig-1.0.0.dist-info/metadata.json
--rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig-1.0.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.152832 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py-1.9.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        3 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py-1.9.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.157522 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pycodestyle-2.6.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       51 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pycodestyle-2.6.0.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pycodestyle-2.6.0.dist-info/namespace_packages.txt
--rw-r--r--   0 adam       (501) staff       (20)       12 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pycodestyle-2.6.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.157989 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pycparser-2.20.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:26.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pycparser-2.20.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.111145 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pydocstyle/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.160280 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pydocstyle/data/
--rw-r--r--   0 adam       (501) staff       (20)     1813 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pydocstyle/data/imperatives.txt
--rw-r--r--   0 adam       (501) staff       (20)     1451 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pydocstyle/data/imperatives_blacklist.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.159166 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pydocstyle-5.1.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       52 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pydocstyle-5.1.1.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)       11 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pydocstyle-5.1.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.161335 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pyflakes-2.2.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       48 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pyflakes-2.2.0.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pyflakes-2.2.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.162605 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pylama-7.7.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       81 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pylama-7.7.1.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)       13 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pylama-7.7.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.163236 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pyparsing-2.4.7.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pyparsing-2.4.7.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.164551 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pytest-6.0.2.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       78 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pytest-6.0.2.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)       15 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pytest-6.0.2.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.165811 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pytest_cov-2.10.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       63 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pytest_cov-2.10.1.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)       11 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pytest_cov-2.10.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.167716 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)      582 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/LICENSE.txt
--rw-r--r--   0 adam       (501) staff       (20)     1843 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/metadata.json
--rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.169409 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests_mock-1.3.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)     1232 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests_mock-1.3.0.dist-info/metadata.json
--rw-r--r--   0 adam       (501) staff       (20)       46 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests_mock-1.3.0.dist-info/pbr.json
--rw-r--r--   0 adam       (501) staff       (20)       14 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests_mock-1.3.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.169886 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests_oauthlib-1.1.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       18 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests_oauthlib-1.1.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.172416 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/setuptools-49.6.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)      239 2020-09-24 15:22:01.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/setuptools-49.6.0.dist-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)     3143 2020-09-24 15:22:01.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/setuptools-49.6.0.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)       54 2020-09-24 15:22:01.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/setuptools-49.6.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.172828 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/six-1.15.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        4 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/six-1.15.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.173448 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/snowballstemmer-2.0.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)       16 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/snowballstemmer-2.0.0.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.175190 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)     1252 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/LICENSE.txt
--rw-r--r--   0 adam       (501) staff       (20)     1185 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/metadata.json
--rw-r--r--   0 adam       (501) staff       (20)        5 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.176160 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/urllib3-1.25.10.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)     1115 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/urllib3-1.25.10.dist-info/LICENSE.txt
--rw-r--r--   0 adam       (501) staff       (20)        8 2020-09-24 15:22:25.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/urllib3-1.25.10.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.178045 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/wheel-0.35.1.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)     1125 2020-09-24 15:22:01.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/wheel-0.35.1.dist-info/LICENSE.txt
--rw-r--r--   0 adam       (501) staff       (20)      108 2020-09-24 15:22:01.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/wheel-0.35.1.dist-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)        6 2020-09-24 15:22:01.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/wheel-0.35.1.dist-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.178453 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/zipp-3.2.0.dist-info/
--rw-r--r--   0 adam       (501) staff       (20)        5 2020-09-24 15:22:24.000000 dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/zipp-3.2.0.dist-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      329 2020-09-24 15:29:01.000000 dgp-oauth2-1.0.7/.travis.yml
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.179037 dgp-oauth2-1.0.7/.vscode/
--rw-r--r--   0 adam       (501) staff       (20)      147 2022-04-25 07:21:05.000000 dgp-oauth2-1.0.7/.vscode/settings.json
--rw-r--r--   0 adam       (501) staff       (20)      194 2020-09-24 11:02:14.000000 dgp-oauth2-1.0.7/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)      402 2020-09-24 11:02:14.000000 dgp-oauth2-1.0.7/Makefile
--rw-r--r--   0 adam       (501) staff       (20)     5586 2022-09-06 16:13:09.186571 dgp-oauth2-1.0.7/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     3645 2020-09-24 15:19:20.000000 dgp-oauth2-1.0.7/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.183151 dgp-oauth2-1.0.7/dgp_oauth2/
--rw-r--r--   0 adam       (501) staff       (20)        6 2022-09-06 16:12:57.000000 dgp-oauth2-1.0.7/dgp_oauth2/VERSION
--rw-r--r--   0 adam       (501) staff       (20)       63 2020-09-24 11:02:14.000000 dgp-oauth2-1.0.7/dgp_oauth2/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     3405 2022-09-06 16:11:04.000000 dgp-oauth2-1.0.7/dgp_oauth2/blueprint.py
--rw-r--r--   0 adam       (501) staff       (20)    13073 2022-05-07 07:54:35.000000 dgp-oauth2-1.0.7/dgp_oauth2/controllers.py
--rw-r--r--   0 adam       (501) staff       (20)      951 2020-09-24 11:02:14.000000 dgp-oauth2-1.0.7/dgp_oauth2/credentials.py
--rw-r--r--   0 adam       (501) staff       (20)      739 2022-05-07 06:05:14.000000 dgp-oauth2-1.0.7/dgp_oauth2/extensions.py
--rw-r--r--   0 adam       (501) staff       (20)      737 2020-09-24 11:02:14.000000 dgp-oauth2-1.0.7/dgp_oauth2/lib.py
--rw-r--r--   0 adam       (501) staff       (20)      268 2022-05-07 06:04:12.000000 dgp-oauth2-1.0.7/dgp_oauth2/logger.py
--rw-r--r--   0 adam       (501) staff       (20)     4221 2022-09-06 16:10:30.000000 dgp-oauth2-1.0.7/dgp_oauth2/models.py
--rw-r--r--   0 adam       (501) staff       (20)      608 2022-05-07 06:05:25.000000 dgp-oauth2-1.0.7/dgp_oauth2/permissions.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.185370 dgp-oauth2-1.0.7/dgp_oauth2.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     5586 2022-09-06 16:13:08.000000 dgp-oauth2-1.0.7/dgp_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     7915 2022-09-06 16:13:09.000000 dgp-oauth2-1.0.7/dgp_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2022-09-06 16:13:08.000000 dgp-oauth2-1.0.7/dgp_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2020-09-24 15:22:00.000000 dgp-oauth2-1.0.7/dgp_oauth2.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)      196 2022-09-06 16:13:08.000000 dgp-oauth2-1.0.7/dgp_oauth2.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       55 2022-09-06 16:13:08.000000 dgp-oauth2-1.0.7/dgp_oauth2.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      164 2020-09-24 11:02:14.000000 dgp-oauth2-1.0.7/pylama.ini
--rw-r--r--   0 adam       (501) staff       (20)       85 2020-09-24 11:02:14.000000 dgp-oauth2-1.0.7/requirements.dev.txt
--rw-r--r--   0 adam       (501) staff       (20)      117 2020-09-24 15:19:26.000000 dgp-oauth2-1.0.7/requirements.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.185680 dgp-oauth2-1.0.7/sample_extension/
--rw-r--r--   0 adam       (501) staff       (20)      206 2020-09-24 11:02:14.000000 dgp-oauth2-1.0.7/sample_extension/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2022-09-06 16:13:09.186088 dgp-oauth2-1.0.7/sample_permission_provider/
--rw-r--r--   0 adam       (501) staff       (20)      114 2020-09-24 11:02:14.000000 dgp-oauth2-1.0.7/sample_permission_provider/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)       38 2022-09-06 16:13:09.186956 dgp-oauth2-1.0.7/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1838 2020-09-24 15:21:20.000000 dgp-oauth2-1.0.7/setup.py
--rw-r--r--   0 adam       (501) staff       (20)      476 2020-09-24 15:25:40.000000 dgp-oauth2-1.0.7/tox.ini
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.916694 dgp-oauth2-1.1.0/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.628535 dgp-oauth2-1.1.0/.tox/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.571923 dgp-oauth2-1.1.0/.tox/py310/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.572100 dgp-oauth2-1.1.0/.tox/py310/lib/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.572371 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.589435 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.653577 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Flask-2.3.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       41 2023-07-18 18:18:11.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Flask-2.3.2.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        6 2023-07-18 18:18:11.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Flask-2.3.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.653997 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Flask_Cors-4.0.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Flask_Cors-4.0.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.654432 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Flask_Jsonpify-1.5.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       15 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Flask_Jsonpify-1.5.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.654862 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Flask_OAuthlib-0.9.6.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       15 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Flask_OAuthlib-0.9.6.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.655698 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Jinja2-3.1.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       59 2023-07-18 18:18:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Jinja2-3.1.2.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-18 18:18:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Jinja2-3.1.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.656185 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/MarkupSafe-2.1.3.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/MarkupSafe-2.1.3.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.656729 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/PyJWT-2.7.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        4 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/PyJWT-2.7.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.657152 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/SQLAlchemy-2.0.19.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-18 18:12:11.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/SQLAlchemy-2.0.19.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.657568 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Werkzeug-2.3.6.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:18:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/Werkzeug-2.3.6.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.657973 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/blinker-1.6.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        8 2023-07-18 18:18:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/blinker-1.6.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.658567 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/cachelib-0.10.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:12:11.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/cachelib-0.10.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.658985 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        8 2023-07-18 18:12:11.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.659753 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/cffi-1.15.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       75 2023-07-18 18:12:12.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/cffi-1.15.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       19 2023-07-18 18:12:12.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/cffi-1.15.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.660650 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/charset_normalizer-3.2.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       76 2023-07-18 18:12:11.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/charset_normalizer-3.2.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       19 2023-07-18 18:12:11.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/charset_normalizer-3.2.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.661074 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/click-8.1.5.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        6 2023-07-18 18:18:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/click-8.1.5.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.662565 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/coverage-6.5.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)    10174 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/coverage-6.5.0.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)      123 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/coverage-6.5.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/coverage-6.5.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.664276 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/coveralls-3.3.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1058 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/coveralls-3.3.1.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)       50 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/coveralls-3.3.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       10 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/coveralls-3.3.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.664923 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/cryptography-41.0.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       13 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/cryptography-41.0.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.665468 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/dgp_oauth2/
+-rw-r--r--   0 adam       (501) staff       (20)        6 2023-07-18 18:37:31.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/dgp_oauth2/VERSION
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.667258 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/dgp_oauth2-1.0.7.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)      114 2023-07-18 18:37:31.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/dgp_oauth2-1.0.7.dist-info/direct_url.json
+-rw-r--r--   0 adam       (501) staff       (20)       55 2023-07-18 18:37:31.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/dgp_oauth2-1.0.7.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.667958 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/docopt-0.6.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-18 18:12:09.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/docopt-0.6.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.668643 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/greenlet-2.0.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/greenlet-2.0.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.669558 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/itsdangerous-2.1.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       13 2023-07-18 18:18:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/itsdangerous-2.1.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.671429 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/mccabe-0.7.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       47 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/mccabe-0.7.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/mccabe-0.7.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.673581 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/oauthlib-2.1.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1534 2023-07-18 18:12:09.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/oauthlib-2.1.0.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:12:09.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/oauthlib-2.1.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.578287 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pip/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.677000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pip/_vendor/
+-rw-r--r--   0 adam       (501) staff       (20)      482 2023-07-18 18:11:36.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pip/_vendor/vendor.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.676068 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pip-22.1.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1093 2023-07-18 18:11:36.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pip-22.1.2.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)      125 2023-07-18 18:11:36.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pip-22.1.2.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        4 2023-07-18 18:11:36.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pip-22.1.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.677780 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pluggy-1.2.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pluggy-1.2.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.678819 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/psycopg2_binary-2.9.6.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/psycopg2_binary-2.9.6.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.682050 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pycodestyle-2.10.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       50 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pycodestyle-2.10.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       12 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pycodestyle-2.10.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.683260 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pycparser-2.21.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       10 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pycparser-2.21.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.580018 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pydocstyle/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.685977 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pydocstyle/data/
+-rw-r--r--   0 adam       (501) staff       (20)     1821 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pydocstyle/data/imperatives.txt
+-rw-r--r--   0 adam       (501) staff       (20)     1443 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pydocstyle/data/imperatives_blacklist.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.684179 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pydocstyle-6.3.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       50 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pydocstyle-6.3.0.dist-info/entry_points.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.687306 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pyflakes-3.0.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       47 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pyflakes-3.0.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pyflakes-3.0.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.688734 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pylama-8.4.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       81 2023-07-18 18:12:12.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pylama-8.4.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-18 18:12:12.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pylama-8.4.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.690173 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pytest-7.4.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       77 2023-07-18 18:12:12.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pytest-7.4.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       18 2023-07-18 18:12:12.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pytest-7.4.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.691721 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pytest_cov-4.1.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       42 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pytest_cov-4.1.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/pytest_cov-4.1.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.692530 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/requests-2.31.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:12:12.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/requests-2.31.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.695134 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/requests_mock-1.3.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1232 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/requests_mock-1.3.0.dist-info/metadata.json
+-rw-r--r--   0 adam       (501) staff       (20)       46 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/requests_mock-1.3.0.dist-info/pbr.json
+-rw-r--r--   0 adam       (501) staff       (20)       14 2023-07-18 18:12:13.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/requests_mock-1.3.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.696333 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/requests_oauthlib-1.1.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       18 2023-07-18 18:12:12.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/requests_oauthlib-1.1.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.698206 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/setuptools-62.6.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     2674 2023-07-18 18:11:35.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/setuptools-62.6.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       41 2023-07-18 18:11:35.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/setuptools-62.6.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.698958 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/six-1.16.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        4 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/six-1.16.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.699741 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/snowballstemmer-2.2.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       16 2023-07-18 18:12:09.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/snowballstemmer-2.2.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.588674 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/sqlalchemy/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.700432 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/sqlalchemy/dialects/
+-rw-r--r--   0 adam       (501) staff       (20)     8239 2023-07-18 18:12:11.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.589147 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.701131 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/licenses/
+-rw-r--r--   0 adam       (501) staff       (20)     1093 2023-07-18 18:12:10.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.703074 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/wheel-0.37.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1125 2023-07-18 18:11:35.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/wheel-0.37.1.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)      108 2023-07-18 18:11:35.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/wheel-0.37.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        6 2023-07-18 18:11:35.000000 dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/wheel-0.37.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.593858 dgp-oauth2-1.1.0/.tox/py37/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.594109 dgp-oauth2-1.1.0/.tox/py37/lib/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.594363 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.628068 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.704283 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask-1.1.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       42 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask-1.1.2.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        6 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask-1.1.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.704827 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask_Cors-3.0.9.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       11 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask_Cors-3.0.9.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.705394 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask_Jsonpify-1.5.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       15 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask_Jsonpify-1.5.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.706048 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask_OAuthlib-0.9.6.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       15 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask_OAuthlib-0.9.6.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.706655 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask_Session-0.3.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       14 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Flask_Session-0.3.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.707766 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Jinja2-2.11.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       61 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Jinja2-2.11.2.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Jinja2-2.11.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.708323 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/MarkupSafe-1.1.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       11 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/MarkupSafe-1.1.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.709412 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/PyJWT-1.7.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       45 2020-09-24 15:22:26.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/PyJWT-1.7.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        4 2020-09-24 15:22:26.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/PyJWT-1.7.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.709998 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/SQLAlchemy-1.3.19.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       11 2020-09-24 15:22:26.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/SQLAlchemy-1.3.19.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.710663 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Werkzeug-0.16.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/Werkzeug-0.16.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.711377 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/attrs-20.2.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/attrs-20.2.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.712009 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/cachelib-0.1.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/cachelib-0.1.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.712717 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/certifi-2020.6.20.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        8 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/certifi-2020.6.20.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.714443 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/cffi-1.14.3.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       76 2020-09-24 15:22:26.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/cffi-1.14.3.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       19 2020-09-24 15:22:26.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/cffi-1.14.3.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.717611 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/chardet-3.0.4.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       60 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/chardet-3.0.4.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)     1375 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/chardet-3.0.4.dist-info/metadata.json
+-rw-r--r--   0 adam       (501) staff       (20)        8 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/chardet-3.0.4.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.718291 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/click-7.1.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        6 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/click-7.1.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.720359 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/coverage-5.3.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)    10174 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/coverage-5.3.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)      123 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/coverage-5.3.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/coverage-5.3.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.722448 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/coveralls-2.1.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1077 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/coveralls-2.1.2.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)       50 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/coveralls-2.1.2.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/coveralls-2.1.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.723240 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/cryptography-3.1.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       31 2020-09-24 15:22:26.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/cryptography-3.1.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.723828 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/dgp_oauth2/
+-rw-r--r--   0 adam       (501) staff       (20)        6 2022-04-25 07:48:29.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/dgp_oauth2/VERSION
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.724932 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/dgp_oauth2-0.2.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)      114 2022-04-25 07:48:29.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/dgp_oauth2-0.2.0.dist-info/direct_url.json
+-rw-r--r--   0 adam       (501) staff       (20)       55 2022-04-25 07:48:29.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/dgp_oauth2-0.2.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.725503 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/docopt-0.6.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        7 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/docopt-0.6.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.726105 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/idna-2.10.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/idna-2.10.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.726746 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/importlib_metadata-2.0.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       19 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/importlib_metadata-2.0.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.727292 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/iniconfig-1.0.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/iniconfig-1.0.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.727781 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/itsdangerous-1.1.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       13 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/itsdangerous-1.1.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.740977 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/mccabe-0.6.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       47 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/mccabe-0.6.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)     1218 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/mccabe-0.6.1.dist-info/metadata.json
+-rw-r--r--   0 adam       (501) staff       (20)        7 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/mccabe-0.6.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.750531 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/more_itertools-8.5.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       15 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/more_itertools-8.5.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.757269 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/oauthlib-2.1.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1534 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/oauthlib-2.1.0.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/oauthlib-2.1.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.758233 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/packaging-20.4.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/packaging-20.4.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.617123 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pip/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.762697 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pip/_vendor/
+-rw-r--r--   0 adam       (501) staff       (20)      437 2020-09-24 15:22:01.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pip/_vendor/vendor.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.761950 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pip-20.2.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1090 2020-09-24 15:22:01.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pip-20.2.2.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)      125 2020-09-24 15:22:01.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pip-20.2.2.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        4 2020-09-24 15:22:01.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pip-20.2.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.763553 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pluggy-0.13.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        7 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pluggy-0.13.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.764543 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/psycopg2_binary-2.8.6.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:26.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/psycopg2_binary-2.8.6.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.621289 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.621797 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.766333 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/apipkg-1.4.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)      779 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/apipkg-1.4.dist-info/metadata.json
+-rw-r--r--   0 adam       (501) staff       (20)        7 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/apipkg-1.4.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.767582 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig-1.0.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)      950 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig-1.0.0.dist-info/metadata.json
+-rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig-1.0.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.765093 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py-1.9.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        3 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py-1.9.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.769794 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pycodestyle-2.6.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       51 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pycodestyle-2.6.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pycodestyle-2.6.0.dist-info/namespace_packages.txt
+-rw-r--r--   0 adam       (501) staff       (20)       12 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pycodestyle-2.6.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.770593 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pycparser-2.20.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:26.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pycparser-2.20.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.623237 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pydocstyle/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.774153 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pydocstyle/data/
+-rw-r--r--   0 adam       (501) staff       (20)     1813 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pydocstyle/data/imperatives.txt
+-rw-r--r--   0 adam       (501) staff       (20)     1451 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pydocstyle/data/imperatives_blacklist.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.772733 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pydocstyle-5.1.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       52 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pydocstyle-5.1.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       11 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pydocstyle-5.1.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.775656 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pyflakes-2.2.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       48 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pyflakes-2.2.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pyflakes-2.2.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.777197 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pylama-7.7.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       81 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pylama-7.7.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       13 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pylama-7.7.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.778097 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pyparsing-2.4.7.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       10 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pyparsing-2.4.7.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.779982 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pytest-6.0.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       78 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pytest-6.0.2.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       15 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pytest-6.0.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.781688 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pytest_cov-2.10.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       63 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pytest_cov-2.10.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       11 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pytest_cov-2.10.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.784110 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)      582 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)     1843 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/metadata.json
+-rw-r--r--   0 adam       (501) staff       (20)        9 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.786694 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests_mock-1.3.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1232 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests_mock-1.3.0.dist-info/metadata.json
+-rw-r--r--   0 adam       (501) staff       (20)       46 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests_mock-1.3.0.dist-info/pbr.json
+-rw-r--r--   0 adam       (501) staff       (20)       14 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests_mock-1.3.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.787536 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests_oauthlib-1.1.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       18 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests_oauthlib-1.1.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.811909 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/setuptools-49.6.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)      239 2020-09-24 15:22:01.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/setuptools-49.6.0.dist-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)     3143 2020-09-24 15:22:01.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/setuptools-49.6.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       54 2020-09-24 15:22:01.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/setuptools-49.6.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.812672 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/six-1.15.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        4 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/six-1.15.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.813383 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/snowballstemmer-2.0.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       16 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/snowballstemmer-2.0.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.816174 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1252 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)     1185 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/metadata.json
+-rw-r--r--   0 adam       (501) staff       (20)        5 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.818725 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/urllib3-1.25.10.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1115 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/urllib3-1.25.10.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)        8 2020-09-24 15:22:25.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/urllib3-1.25.10.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.821096 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/wheel-0.35.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1125 2020-09-24 15:22:01.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/wheel-0.35.1.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)      108 2020-09-24 15:22:01.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/wheel-0.35.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        6 2020-09-24 15:22:01.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/wheel-0.35.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.822086 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/zipp-3.2.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2020-09-24 15:22:24.000000 dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/zipp-3.2.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.628732 dgp-oauth2-1.1.0/.tox/py39/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.628917 dgp-oauth2-1.1.0/.tox/py39/lib/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.629179 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.645138 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.823697 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Flask-2.3.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       41 2023-07-18 18:17:52.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Flask-2.3.2.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        6 2023-07-18 18:17:52.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Flask-2.3.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.824349 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Flask_Cors-4.0.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-18 18:11:26.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Flask_Cors-4.0.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.825102 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Flask_Jsonpify-1.5.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       15 2023-07-18 18:11:26.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Flask_Jsonpify-1.5.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.825892 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Flask_OAuthlib-0.9.6.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       15 2023-07-18 18:11:26.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Flask_OAuthlib-0.9.6.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.827311 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Jinja2-3.1.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       59 2023-07-18 18:17:51.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Jinja2-3.1.2.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-18 18:17:51.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Jinja2-3.1.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.828375 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/MarkupSafe-2.1.3.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/MarkupSafe-2.1.3.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.854970 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/PyJWT-2.7.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        4 2023-07-18 18:11:20.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/PyJWT-2.7.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.856340 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/SQLAlchemy-2.0.19.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-18 18:11:22.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/SQLAlchemy-2.0.19.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.857273 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Werkzeug-2.3.6.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:17:51.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/Werkzeug-2.3.6.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.858285 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/blinker-1.6.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        8 2023-07-18 18:17:52.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/blinker-1.6.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.859415 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/cachelib-0.10.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:11:22.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/cachelib-0.10.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.860064 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/certifi-2023.5.7.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        8 2023-07-18 18:11:22.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/certifi-2023.5.7.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.862870 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/cffi-1.15.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       75 2023-07-18 18:11:24.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/cffi-1.15.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       19 2023-07-18 18:11:24.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/cffi-1.15.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.865457 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/charset_normalizer-3.2.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       76 2023-07-18 18:11:22.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/charset_normalizer-3.2.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       19 2023-07-18 18:11:22.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/charset_normalizer-3.2.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.866947 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/click-8.1.5.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        6 2023-07-18 18:17:52.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/click-8.1.5.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.869616 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/coverage-6.5.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)    10174 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/coverage-6.5.0.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)      122 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/coverage-6.5.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/coverage-6.5.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.872188 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/coveralls-3.3.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1058 2023-07-18 18:11:26.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/coveralls-3.3.1.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)       50 2023-07-18 18:11:26.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/coveralls-3.3.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       10 2023-07-18 18:11:26.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/coveralls-3.3.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.873095 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/cryptography-41.0.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       13 2023-07-18 18:11:26.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/cryptography-41.0.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.873876 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/dgp_oauth2/
+-rw-r--r--   0 adam       (501) staff       (20)        6 2023-07-18 18:37:22.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/dgp_oauth2/VERSION
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.875816 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/dgp_oauth2-1.0.7.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)      114 2023-07-18 18:37:22.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/dgp_oauth2-1.0.7.dist-info/direct_url.json
+-rw-r--r--   0 adam       (501) staff       (20)       55 2023-07-18 18:37:22.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/dgp_oauth2-1.0.7.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.876500 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/docopt-0.6.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-18 18:11:20.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/docopt-0.6.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.877346 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/greenlet-2.0.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/greenlet-2.0.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.878334 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/importlib_metadata-6.8.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       19 2023-07-18 18:17:52.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/importlib_metadata-6.8.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.879204 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/itsdangerous-2.1.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       13 2023-07-18 18:17:51.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/itsdangerous-2.1.2.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.881034 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/mccabe-0.7.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       47 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/mccabe-0.7.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/mccabe-0.7.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.882798 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/oauthlib-2.1.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1534 2023-07-18 18:11:20.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/oauthlib-2.1.0.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:11:20.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/oauthlib-2.1.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.638444 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pip/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.885286 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pip/_vendor/
+-rw-r--r--   0 adam       (501) staff       (20)      469 2023-07-18 18:10:46.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pip/_vendor/vendor.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.884609 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pip-22.3.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1093 2023-07-18 18:10:46.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pip-22.3.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)      125 2023-07-18 18:10:46.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pip-22.3.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        4 2023-07-18 18:10:46.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pip-22.3.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.886002 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pluggy-1.2.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pluggy-1.2.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.886765 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/psycopg2_binary-2.9.6.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/psycopg2_binary-2.9.6.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.888132 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pycodestyle-2.10.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       50 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pycodestyle-2.10.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       12 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pycodestyle-2.10.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.888717 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pycparser-2.21.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       10 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pycparser-2.21.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.640600 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pydocstyle/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.890414 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pydocstyle/data/
+-rw-r--r--   0 adam       (501) staff       (20)     1821 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pydocstyle/data/imperatives.txt
+-rw-r--r--   0 adam       (501) staff       (20)     1443 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pydocstyle/data/imperatives_blacklist.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.889305 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pydocstyle-6.3.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       50 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pydocstyle-6.3.0.dist-info/entry_points.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.891541 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pyflakes-3.0.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       47 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pyflakes-3.0.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:11:21.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pyflakes-3.0.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.892732 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pylama-8.4.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       81 2023-07-18 18:11:24.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pylama-8.4.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-18 18:11:24.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pylama-8.4.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.893686 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pytest-7.4.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       77 2023-07-18 18:11:24.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pytest-7.4.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       18 2023-07-18 18:11:24.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pytest-7.4.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.894739 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pytest_cov-4.1.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       42 2023-07-18 18:11:25.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pytest_cov-4.1.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-18 18:11:25.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/pytest_cov-4.1.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.895672 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/requests-2.31.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-18 18:11:24.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/requests-2.31.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.897887 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/requests_mock-1.3.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1232 2023-07-18 18:11:25.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/requests_mock-1.3.0.dist-info/metadata.json
+-rw-r--r--   0 adam       (501) staff       (20)       46 2023-07-18 18:11:25.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/requests_mock-1.3.0.dist-info/pbr.json
+-rw-r--r--   0 adam       (501) staff       (20)       14 2023-07-18 18:11:25.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/requests_mock-1.3.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.898706 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/requests_oauthlib-1.1.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       18 2023-07-18 18:11:24.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/requests_oauthlib-1.1.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.900038 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/setuptools-65.5.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     2740 2023-07-18 18:10:46.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       41 2023-07-18 18:10:46.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/setuptools-65.5.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.900506 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/six-1.16.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        4 2023-07-18 18:11:20.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/six-1.16.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.900978 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/snowballstemmer-2.2.0.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)       16 2023-07-18 18:11:20.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/snowballstemmer-2.2.0.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.644167 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/sqlalchemy/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.901554 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/sqlalchemy/dialects/
+-rw-r--r--   0 adam       (501) staff       (20)     8239 2023-07-18 18:11:22.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.644654 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/urllib3-2.0.3.dist-info/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.902179 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/urllib3-2.0.3.dist-info/licenses/
+-rw-r--r--   0 adam       (501) staff       (20)     1093 2023-07-18 18:11:20.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.903758 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/wheel-0.37.1.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)     1125 2023-07-18 18:10:46.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/wheel-0.37.1.dist-info/LICENSE.txt
+-rw-r--r--   0 adam       (501) staff       (20)      108 2023-07-18 18:10:46.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/wheel-0.37.1.dist-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)        6 2023-07-18 18:10:46.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/wheel-0.37.1.dist-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.904215 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/zipp-3.16.2.dist-info/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2023-07-18 18:17:51.000000 dgp-oauth2-1.1.0/.tox/py39/lib/python3.9/site-packages/zipp-3.16.2.dist-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      329 2020-09-24 15:29:01.000000 dgp-oauth2-1.1.0/.travis.yml
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.904700 dgp-oauth2-1.1.0/.vscode/
+-rw-r--r--   0 adam       (501) staff       (20)      147 2022-04-25 07:21:05.000000 dgp-oauth2-1.1.0/.vscode/settings.json
+-rw-r--r--   0 adam       (501) staff       (20)     1143 2020-09-24 15:20:50.000000 dgp-oauth2-1.1.0/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      194 2020-09-24 11:02:14.000000 dgp-oauth2-1.1.0/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)      402 2020-09-24 11:02:14.000000 dgp-oauth2-1.1.0/Makefile
+-rw-r--r--   0 adam       (501) staff       (20)     4405 2023-07-18 18:45:58.916347 dgp-oauth2-1.1.0/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     3645 2020-09-24 15:19:20.000000 dgp-oauth2-1.1.0/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.909462 dgp-oauth2-1.1.0/dgp_oauth2/
+-rw-r--r--   0 adam       (501) staff       (20)        6 2023-07-18 18:37:42.000000 dgp-oauth2-1.1.0/dgp_oauth2/VERSION
+-rw-r--r--   0 adam       (501) staff       (20)       63 2020-09-24 11:02:14.000000 dgp-oauth2-1.1.0/dgp_oauth2/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     3405 2022-09-06 16:11:04.000000 dgp-oauth2-1.1.0/dgp_oauth2/blueprint.py
+-rw-r--r--   0 adam       (501) staff       (20)    13167 2023-07-18 18:37:10.000000 dgp-oauth2-1.1.0/dgp_oauth2/controllers.py
+-rw-r--r--   0 adam       (501) staff       (20)     1029 2023-07-18 18:10:06.000000 dgp-oauth2-1.1.0/dgp_oauth2/credentials.py
+-rw-r--r--   0 adam       (501) staff       (20)      739 2022-05-07 06:05:14.000000 dgp-oauth2-1.1.0/dgp_oauth2/extensions.py
+-rw-r--r--   0 adam       (501) staff       (20)      737 2020-09-24 11:02:14.000000 dgp-oauth2-1.1.0/dgp_oauth2/lib.py
+-rw-r--r--   0 adam       (501) staff       (20)      268 2022-05-07 06:04:12.000000 dgp-oauth2-1.1.0/dgp_oauth2/logger.py
+-rw-r--r--   0 adam       (501) staff       (20)     4183 2023-07-18 18:29:04.000000 dgp-oauth2-1.1.0/dgp_oauth2/models.py
+-rw-r--r--   0 adam       (501) staff       (20)      608 2022-05-07 06:05:25.000000 dgp-oauth2-1.1.0/dgp_oauth2/permissions.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.912443 dgp-oauth2-1.1.0/dgp_oauth2.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     4405 2023-07-18 18:45:57.000000 dgp-oauth2-1.1.0/dgp_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)    19239 2023-07-18 18:45:58.000000 dgp-oauth2-1.1.0/dgp_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-18 18:45:57.000000 dgp-oauth2-1.1.0/dgp_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2020-09-24 15:22:00.000000 dgp-oauth2-1.1.0/dgp_oauth2.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)      196 2023-07-18 18:45:57.000000 dgp-oauth2-1.1.0/dgp_oauth2.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       55 2023-07-18 18:45:57.000000 dgp-oauth2-1.1.0/dgp_oauth2.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      164 2020-09-24 11:02:14.000000 dgp-oauth2-1.1.0/pylama.ini
+-rw-r--r--   0 adam       (501) staff       (20)       85 2020-09-24 11:02:14.000000 dgp-oauth2-1.1.0/requirements.dev.txt
+-rw-r--r--   0 adam       (501) staff       (20)      107 2023-07-18 18:15:37.000000 dgp-oauth2-1.1.0/requirements.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.913011 dgp-oauth2-1.1.0/sample_extension/
+-rw-r--r--   0 adam       (501) staff       (20)      206 2020-09-24 11:02:14.000000 dgp-oauth2-1.1.0/sample_extension/__init__.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.913658 dgp-oauth2-1.1.0/sample_permission_provider/
+-rw-r--r--   0 adam       (501) staff       (20)      114 2020-09-24 11:02:14.000000 dgp-oauth2-1.1.0/sample_permission_provider/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-18 18:45:58.916820 dgp-oauth2-1.1.0/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     1838 2020-09-24 15:21:20.000000 dgp-oauth2-1.1.0/setup.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-18 18:45:58.915526 dgp-oauth2-1.1.0/tests/
+-rw-r--r--   0 adam       (501) staff       (20)     1117 2023-07-18 18:34:21.000000 dgp-oauth2-1.1.0/tests/test_extensions_controllers.py
+-rw-r--r--   0 adam       (501) staff       (20)     2783 2023-07-18 18:31:24.000000 dgp-oauth2-1.1.0/tests/test_permission_controllers.py
+-rw-r--r--   0 adam       (501) staff       (20)    21290 2023-07-18 18:28:29.000000 dgp-oauth2-1.1.0/tests/test_user_controllers.py
+-rw-r--r--   0 adam       (501) staff       (20)      477 2023-07-18 18:18:19.000000 dgp-oauth2-1.1.0/tox.ini
```

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/chardet-3.0.4.dist-info/metadata.json` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/chardet-3.0.4.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/coverage-5.3.dist-info/LICENSE.txt` & `dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/coverage-6.5.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/coveralls-2.1.2.dist-info/LICENSE.txt` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/coveralls-2.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/mccabe-0.6.1.dist-info/metadata.json` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/mccabe-0.6.1.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/oauthlib-2.1.0.dist-info/LICENSE.txt` & `dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/oauthlib-2.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pip-20.2.2.dist-info/LICENSE.txt` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pip-20.2.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/apipkg-1.4.dist-info/metadata.json` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/apipkg-1.4.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig-1.0.0.dist-info/metadata.json` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig-1.0.0.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pydocstyle/data/imperatives.txt` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pydocstyle/data/imperatives.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/pydocstyle/data/imperatives_blacklist.txt` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/pydocstyle/data/imperatives_blacklist.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/LICENSE.txt` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/metadata.json` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/requests-2.24.0.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/requests_mock-1.3.0.dist-info/metadata.json` & `dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/requests_mock-1.3.0.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/setuptools-49.6.0.dist-info/entry_points.txt` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/setuptools-49.6.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/LICENSE.txt` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/metadata.json` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/toml-0.10.1.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/urllib3-1.25.10.dist-info/LICENSE.txt` & `dgp-oauth2-1.1.0/.tox/py37/lib/python3.7/site-packages/urllib3-1.25.10.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/.tox/py37/lib/python3.7/site-packages/wheel-0.35.1.dist-info/LICENSE.txt` & `dgp-oauth2-1.1.0/.tox/py310/lib/python3.10/site-packages/wheel-0.37.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/PKG-INFO` & `dgp-oauth2-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,172 @@
 Metadata-Version: 2.1
 Name: dgp-oauth2
-Version: 1.0.7
+Version: 1.1.0
 Summary: {{ DESCRIPTION }}
 Home-page: https://github.com/dataspot/dgp-oauth2
 Author: Adam Kariv, Open Knowledge (International), Datopian
 License: MIT
-Description: # Oauth2 Flask Service
-        
-        [![Build Status](https://travis-ci.org/datahq/auth.svg?branch=master)](https://travis-ci.org/dataspot/dgp-oauth2)
-        
-        A generic OAuth2 authentication service and user permission manager.
-        
-        Based off [OpenSpending auth service](https://github.com/openspending/os-conductor).
-        
-        ## Quick start
-        
-        ### Clone the repo and install
-        
-        `make install`
-        
-        ### Run tests
-        
-        `make test`
-        
-        ### Run server
-        
-        `python server.py`
-        
-        ## Env Vars
-        - `PRIVATE_KEY` & `PUBLIC_KEY` an RSA key-pair in PEM format.
-          See `tools/generate_key_pair.sh` for more info.
-        - `GOOGLE_KEY` & `GOOGLE_SECRET`: OAuth credentials for authenticating with Google
-        - `GITHUB_KEY` & `GITHUB_SECRET`: OAuth credentials for authenticating with Github
-        - `DATABASE_URL`: A SQLAlchemy compatible database connection string (where user data is stored)
-        - `EXTERNAL_ADDRESS`: The hostname where this service is located on
-        - `ALLOWED_SERVICES`:
-            Which permissions providers are available. A `;` delimited list of provider identifiers.
-            Each provider identifier takes the form of `[alias:]provider`, where `provider` is the name of a Python module
-            which exports a `get_permissions(service, userid)` function.
-        - `INSTALLED_EXTENSIONS`:
-            List of installed extensions. A `;` delimited list of `extension` - the name of a Python modules which exports one or all of these functions
-            - `on_new_user(user_info)`
-            - `on_user_login(user_info)`
-            - `on_user_logout(user_info)`
-        
-        
-        ## API
-        
-        ### Check an authentication token's validity
-        `/auth/check`
-        
-        **Method:** `GET`
-        
-        **Query Parameters:**
-        
-         - `jwt` - authentication token
-         - `next` - URL to redirect to when finished authentication
-        
-        **Returns:**
-        
-        If authenticated:
-        
-        ```json
-        {
-            "authenticated": true,
-            "profile": {
-                "id": "<user-id>",
-                "name": "<user-name>",
-                "email": "<user-email>",
-                "avatar_url": "<url-for-user's-profile-photo>",
-                "idhash": "<unique-id-of-the-user>",
-                "username": "<user-selected-id>" # If user has a username
-            }
-        }
-        ```
-        
-        If not:
-        
-        ```json
-        {
-            "authenticated": false,
-            "providers": {
-                "google": {
-                    "url": "<url-for-logging-in-with-the-Google-provider>"
-                },
-                "github": {
-                    "url": "<url-for-logging-in-with-the-Github-provider>"
-                },
-            }
-        }
-        ```
-        
-        When the authentication flow is finished, the caller will be redirected to the `next` URL with an extra query parameter
-        `jwt` which contains the authentication token. The caller should cache this token for further interactions with the API.
-        
-        ### Get permission for a service
-        `/auth/authorize`
-        
-        **Method:** `GET`
-        
-        **Query Parameters:**
-        
-         - `jwt` - user token (received from `/user/check`)
-         - `service` - the relevant service (e.g. `storage-service`)
-        
-        **Returns:**
-        
-        ```json
-        {
-            "token": "<token-for-the-relevant-service>"
-            "userid": "<unique-id-of-the-user>",
-            "permissions": {
-                "permission-x": true,
-                "permission-y": false
-            },
-            "service": "<relevant-service>"
-        }
-        ```
-        
-        ### Change the username
-        `/auth/update`
-        
-        **Method:** `POST`
-        
-        **Query Parameters:**
-        
-         - `jwt` - authentication token (received from `/user/check`)
-         - `username` - A new username for the user profile (this action is only allowed once)
-        
-        **Returns:**
-        
-        ```json
-        {
-            "success": true,
-            "error": "<error-message-if-applicable>"
-        }
-        ```
-        
-        __Note__: trying to update other user profile fields like `email` will fail silently and return
-        
-        ```json
-        {
-            "success": true
-        }
-        ```
-        
-        ### Receive authorization public key
-        `/auth/public-key`
-        
-        **Method:** `GET`
-        
-        **Returns:**
-        
-        The service's public key in PEM format.
-        
-        Can be used by services to validate that the permission token is authentic.
 Keywords: data,authentication,oauth2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: develop
+License-File: LICENSE
+
+# Oauth2 Flask Service
+
+[![Build Status](https://travis-ci.org/datahq/auth.svg?branch=master)](https://travis-ci.org/dataspot/dgp-oauth2)
+
+A generic OAuth2 authentication service and user permission manager.
+
+Based off [OpenSpending auth service](https://github.com/openspending/os-conductor).
+
+## Quick start
+
+### Clone the repo and install
+
+`make install`
+
+### Run tests
+
+`make test`
+
+### Run server
+
+`python server.py`
+
+## Env Vars
+- `PRIVATE_KEY` & `PUBLIC_KEY` an RSA key-pair in PEM format.
+  See `tools/generate_key_pair.sh` for more info.
+- `GOOGLE_KEY` & `GOOGLE_SECRET`: OAuth credentials for authenticating with Google
+- `GITHUB_KEY` & `GITHUB_SECRET`: OAuth credentials for authenticating with Github
+- `DATABASE_URL`: A SQLAlchemy compatible database connection string (where user data is stored)
+- `EXTERNAL_ADDRESS`: The hostname where this service is located on
+- `ALLOWED_SERVICES`:
+    Which permissions providers are available. A `;` delimited list of provider identifiers.
+    Each provider identifier takes the form of `[alias:]provider`, where `provider` is the name of a Python module
+    which exports a `get_permissions(service, userid)` function.
+- `INSTALLED_EXTENSIONS`:
+    List of installed extensions. A `;` delimited list of `extension` - the name of a Python modules which exports one or all of these functions
+    - `on_new_user(user_info)`
+    - `on_user_login(user_info)`
+    - `on_user_logout(user_info)`
+
+
+## API
+
+### Check an authentication token's validity
+`/auth/check`
+
+**Method:** `GET`
+
+**Query Parameters:**
+
+ - `jwt` - authentication token
+ - `next` - URL to redirect to when finished authentication
+
+**Returns:**
+
+If authenticated:
+
+```json
+{
+    "authenticated": true,
+    "profile": {
+        "id": "<user-id>",
+        "name": "<user-name>",
+        "email": "<user-email>",
+        "avatar_url": "<url-for-user's-profile-photo>",
+        "idhash": "<unique-id-of-the-user>",
+        "username": "<user-selected-id>" # If user has a username
+    }
+}
+```
+
+If not:
+
+```json
+{
+    "authenticated": false,
+    "providers": {
+        "google": {
+            "url": "<url-for-logging-in-with-the-Google-provider>"
+        },
+        "github": {
+            "url": "<url-for-logging-in-with-the-Github-provider>"
+        },
+    }
+}
+```
+
+When the authentication flow is finished, the caller will be redirected to the `next` URL with an extra query parameter
+`jwt` which contains the authentication token. The caller should cache this token for further interactions with the API.
+
+### Get permission for a service
+`/auth/authorize`
+
+**Method:** `GET`
+
+**Query Parameters:**
+
+ - `jwt` - user token (received from `/user/check`)
+ - `service` - the relevant service (e.g. `storage-service`)
+
+**Returns:**
+
+```json
+{
+    "token": "<token-for-the-relevant-service>"
+    "userid": "<unique-id-of-the-user>",
+    "permissions": {
+        "permission-x": true,
+        "permission-y": false
+    },
+    "service": "<relevant-service>"
+}
+```
+
+### Change the username
+`/auth/update`
+
+**Method:** `POST`
+
+**Query Parameters:**
+
+ - `jwt` - authentication token (received from `/user/check`)
+ - `username` - A new username for the user profile (this action is only allowed once)
+
+**Returns:**
+
+```json
+{
+    "success": true,
+    "error": "<error-message-if-applicable>"
+}
+```
+
+__Note__: trying to update other user profile fields like `email` will fail silently and return
+
+```json
+{
+    "success": true
+}
+```
+
+### Receive authorization public key
+`/auth/public-key`
+
+**Method:** `GET`
+
+**Returns:**
+
+The service's public key in PEM format.
+
+Can be used by services to validate that the permission token is authentic.
+
```

### Comparing `dgp-oauth2-1.0.7/README.md` & `dgp-oauth2-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/dgp_oauth2/blueprint.py` & `dgp-oauth2-1.1.0/dgp_oauth2/blueprint.py`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/dgp_oauth2/controllers.py` & `dgp-oauth2-1.1.0/dgp_oauth2/controllers.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,21 +69,21 @@
             'AUTH CONTROLLERS:' + 
             (' google' if has_google else '') + 
             (' github' if has_github else '') + 
             (' fake' if self.enable_fake else '')
         )
 
     # Public methods
-    def authenticate(self, token, next, callback_url, private_key):
+    def authenticate(self, token, next, callback_url, private_token):
         """Check if user is authenticated
         """
         logger.info('AUTH CONTROLLERS: authenticate %s %s %s' % (token is not None, next, callback_url))
         if token is not None:
             try:
-                token = jwt.decode(token, private_key)
+                token = jwt.decode(token, private_token, algorithms=['HS256'])
             except jwt.InvalidTokenError:
                 logger.info('AUTH CONTROLLERS: invalid token %r' % token)
                 token = None
 
             if token is not None:
                 userid = token['userid']
                 user = self.models.get_user(userid)
@@ -100,34 +100,34 @@
         state = {
             'next': next,
             'exp': datetime.datetime.utcnow() + datetime.timedelta(minutes=10),
             'nbf': datetime.datetime.utcnow()
         }
         for provider, params in self.remote_apps.items():
             pstate = dict(provider=provider, **state)
-            pstate = jwt.encode(pstate, private_key)
+            pstate = jwt.encode(pstate, private_token)
             login_url = params['app'] \
                 .authorize(callback=callback_url, state=pstate).headers['Location']
             providers[provider] = {'url': login_url}
         if self.enable_fake:
-            providers = self._fake_providers(next, private_key)
+            providers = self._fake_providers(next, private_token)
         ret = {
             'authenticated': False,
             'providers': providers
         }
         return ret
 
 
-    def update(self, token, username, private_key):
+    def update(self, token, username, private_token):
         """Update a user
         """
         err = None
         if token is not None:
             try:
-                token = jwt.decode(token, private_key)
+                token = jwt.decode(token, private_token, algorithms=['HS256'])
             except jwt.InvalidTokenError:
                 token = None
                 err = 'Not authenticated'
         else:
             err = 'No token'
 
         if token is not None:
@@ -150,49 +150,48 @@
         ret = {'success': err is None}
         if err is not None:
             ret['error'] = err
 
         return ret
 
 
-    def authorize(self, token, service, private_key):
+    def authorize(self, token, service, private_key, private_token):
         """Return user authorization for a service
         """
         if token is not None and service is not None:
             try:
-                token = jwt.decode(token, private_key)
+                token = jwt.decode(token, private_token, algorithms=['HS256'])
             except jwt.InvalidTokenError:
                 token = None
 
             if token is not None:
                 userid = token['userid']
                 permissions = get_token(service, userid)
                 ret = {
                     'userid': userid,
                     'permissions': permissions,
                     'service': service
                 }
-                token = jwt.encode(ret, private_key, algorithm='RS256')\
-                           .decode('ascii')
+                token = jwt.encode(ret, private_key, algorithm='RS256')
                 ret['token'] = token
                 return ret
 
         ret = {
             'permissions': {}
         }
         return ret
 
 
-    def oauth_callback(self, state, callback_url, private_key,
+    def oauth_callback(self, state, callback_url, private_token,
                        set_session=lambda k, v: None):
         """Callback from OAuth
         """
         logger.info('AUTH CONTROLLERS: oauth_callback %s' % state)
         try:
-            state = jwt.decode(state, private_key)
+            state = jwt.decode(state, private_token, algorithms=['HS256'])
         except jwt.InvalidTokenError:
             state = {}
         logger.info('AUTH CONTROLLERS: oauth_callback decoded %r' % state)
 
         resp = None
 
         provider = state.get('provider')
@@ -203,15 +202,15 @@
                 resp = app.authorized_response()
             except OAuthException as e:
                 resp = e
             if isinstance(resp, OAuthException):
                 logger.error("OAuthException: %r", resp.data, exc_info=resp)
                 resp = None
         access_token = resp.get('access_token') if resp is not None else None
-        next_url = self._next_url(state, access_token, private_key)
+        next_url = self._next_url(state, access_token, private_token)
         logger.info('AUTH CONTROLLERS: oauth_callback next_url %s %s -> %s' % (state, access_token, next_url))
         return next_url
 
 
     def resolve_username(self, username):
         """Return userid for given username. If not exist, return None.
         """
@@ -264,39 +263,39 @@
                     response['email'] = email['email']
                     break
                 if email.get('primary'):
                     response['email'] = email['email']
         return response
 
 
-    def _fake_providers(self, next, private_key):
+    def _fake_providers(self, next, private_token):
         ret = dict()
         for provider in ('google', 'github'):
-            token = self._get_token_from_userid(self.models.FAKE_USER_ID, private_key)
+            token = self._get_token_from_userid(self.models.FAKE_USER_ID, private_token)
             next = self._update_next_url(next, token)
             ret[provider] = dict(url=next)
         self.models.create_or_get_user(
             self.models.FAKE_USER_ID,
             self.models.FAKE_USER_RECORD['name'],
             self.models.FAKE_USER_RECORD['username'],
             self.models.FAKE_USER_RECORD['email'],
             self.models.FAKE_USER_RECORD['avatar_url'],
         )
         return ret
 
 
-    def _next_url(self, state, access_token, private_key):
+    def _next_url(self, state, access_token, private_token):
         next_url = '/'
         provider = state.get('provider')
         next_url = state.get('next', next_url)
         if access_token is not None and provider is not None:
             logger.info('Got ACCESS TOKEN %r', access_token)
             profile = self._get_user_profile(provider, access_token)
             logger.info('Got PROFILE %r', profile)
-            client_token = self._get_token_from_profile(provider, profile, private_key)
+            client_token = self._get_token_from_profile(provider, profile, private_token)
             # Add client token to redirect url
             next_url = self._update_next_url(next_url, client_token)
 
         return next_url
 
 
     def _update_next_url(self, next_url, client_token):
@@ -309,37 +308,37 @@
 
         url_parts[4] = urlparse.urlencode(query)
 
         next_url = urlparse.urlunparse(url_parts)
         return next_url
 
 
-    def _get_token_from_profile(self, provider, profile, private_key):
+    def _get_token_from_profile(self, provider, profile, private_token):
         norm_profile = self._normalize_profile(provider, profile)
         if norm_profile is None:
             return None
         userid = norm_profile['userid']
         name = norm_profile['name']
         username = norm_profile['username']
         email = norm_profile['email']
         avatar_url = norm_profile['avatar_url']
         user = self.models.create_or_get_user(userid, name, username, email, avatar_url)
         if user.get('new'):
             on_new_user(user)
         logger.info('Got USER %r', user)
-        return self._get_token_from_userid(user['id'], private_key)
+        return self._get_token_from_userid(user['id'], private_token)
 
 
-    def _get_token_from_userid(self, userid, private_key):
+    def _get_token_from_userid(self, userid, private_token):
         token = {
             'userid': userid,
             'exp': (datetime.datetime.utcnow() +
                     datetime.timedelta(days=14))
         }
-        client_token = jwt.encode(token, private_key)
+        client_token = jwt.encode(token, private_token)
         return client_token
 
 
     def _normalize_profile(self, provider, profile):
         if profile is None:
             return None
         provider_id = profile['id']
```

### Comparing `dgp-oauth2-1.0.7/dgp_oauth2/credentials.py` & `dgp-oauth2-1.1.0/dgp_oauth2/credentials.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
+import hashlib
 
 # Private/Public key pair
 # -- use tools/generate_key_pair.sh to generate a key pair
 private_key = os.environ.get('PRIVATE_KEY')
 public_key = os.environ.get('PUBLIC_KEY')
 
+private_token = hashlib.sha256(private_key.encode()).digest()
+
 # Google Secrets
 google_key = os.environ.get('GOOGLE_KEY')
 google_secret = os.environ.get('GOOGLE_SECRET')
 
 # Github Secrets
 github_key = os.environ.get('GITHUB_KEY')
 github_secret = os.environ.get('GITHUB_SECRET')
```

### Comparing `dgp-oauth2-1.0.7/dgp_oauth2/extensions.py` & `dgp-oauth2-1.1.0/dgp_oauth2/extensions.py`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/dgp_oauth2/lib.py` & `dgp-oauth2-1.1.0/dgp_oauth2/lib.py`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/dgp_oauth2/models.py` & `dgp-oauth2-1.1.0/dgp_oauth2/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 import datetime
 from hashlib import md5
 
 from contextlib import contextmanager
 
 from sqlalchemy import DateTime
 from sqlalchemy import inspect
-from sqlalchemy.ext.declarative import declarative_base
 
 from sqlalchemy import Column, Unicode, String, create_engine, func
-from sqlalchemy.orm import sessionmaker
+from sqlalchemy.orm import sessionmaker, declarative_base
 
 # ## SQL DB
 Base = declarative_base()
 
 def object_as_dict(obj):
     return {c.key: getattr(obj, c.key)
             for c in inspect(obj).mapper.column_attrs}
```

### Comparing `dgp-oauth2-1.0.7/dgp_oauth2/permissions.py` & `dgp-oauth2-1.1.0/dgp_oauth2/permissions.py`

 * *Files identical despite different names*

### Comparing `dgp-oauth2-1.0.7/dgp_oauth2.egg-info/PKG-INFO` & `dgp-oauth2-1.1.0/dgp_oauth2.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,172 @@
 Metadata-Version: 2.1
 Name: dgp-oauth2
-Version: 1.0.7
+Version: 1.1.0
 Summary: {{ DESCRIPTION }}
 Home-page: https://github.com/dataspot/dgp-oauth2
 Author: Adam Kariv, Open Knowledge (International), Datopian
 License: MIT
-Description: # Oauth2 Flask Service
-        
-        [![Build Status](https://travis-ci.org/datahq/auth.svg?branch=master)](https://travis-ci.org/dataspot/dgp-oauth2)
-        
-        A generic OAuth2 authentication service and user permission manager.
-        
-        Based off [OpenSpending auth service](https://github.com/openspending/os-conductor).
-        
-        ## Quick start
-        
-        ### Clone the repo and install
-        
-        `make install`
-        
-        ### Run tests
-        
-        `make test`
-        
-        ### Run server
-        
-        `python server.py`
-        
-        ## Env Vars
-        - `PRIVATE_KEY` & `PUBLIC_KEY` an RSA key-pair in PEM format.
-          See `tools/generate_key_pair.sh` for more info.
-        - `GOOGLE_KEY` & `GOOGLE_SECRET`: OAuth credentials for authenticating with Google
-        - `GITHUB_KEY` & `GITHUB_SECRET`: OAuth credentials for authenticating with Github
-        - `DATABASE_URL`: A SQLAlchemy compatible database connection string (where user data is stored)
-        - `EXTERNAL_ADDRESS`: The hostname where this service is located on
-        - `ALLOWED_SERVICES`:
-            Which permissions providers are available. A `;` delimited list of provider identifiers.
-            Each provider identifier takes the form of `[alias:]provider`, where `provider` is the name of a Python module
-            which exports a `get_permissions(service, userid)` function.
-        - `INSTALLED_EXTENSIONS`:
-            List of installed extensions. A `;` delimited list of `extension` - the name of a Python modules which exports one or all of these functions
-            - `on_new_user(user_info)`
-            - `on_user_login(user_info)`
-            - `on_user_logout(user_info)`
-        
-        
-        ## API
-        
-        ### Check an authentication token's validity
-        `/auth/check`
-        
-        **Method:** `GET`
-        
-        **Query Parameters:**
-        
-         - `jwt` - authentication token
-         - `next` - URL to redirect to when finished authentication
-        
-        **Returns:**
-        
-        If authenticated:
-        
-        ```json
-        {
-            "authenticated": true,
-            "profile": {
-                "id": "<user-id>",
-                "name": "<user-name>",
-                "email": "<user-email>",
-                "avatar_url": "<url-for-user's-profile-photo>",
-                "idhash": "<unique-id-of-the-user>",
-                "username": "<user-selected-id>" # If user has a username
-            }
-        }
-        ```
-        
-        If not:
-        
-        ```json
-        {
-            "authenticated": false,
-            "providers": {
-                "google": {
-                    "url": "<url-for-logging-in-with-the-Google-provider>"
-                },
-                "github": {
-                    "url": "<url-for-logging-in-with-the-Github-provider>"
-                },
-            }
-        }
-        ```
-        
-        When the authentication flow is finished, the caller will be redirected to the `next` URL with an extra query parameter
-        `jwt` which contains the authentication token. The caller should cache this token for further interactions with the API.
-        
-        ### Get permission for a service
-        `/auth/authorize`
-        
-        **Method:** `GET`
-        
-        **Query Parameters:**
-        
-         - `jwt` - user token (received from `/user/check`)
-         - `service` - the relevant service (e.g. `storage-service`)
-        
-        **Returns:**
-        
-        ```json
-        {
-            "token": "<token-for-the-relevant-service>"
-            "userid": "<unique-id-of-the-user>",
-            "permissions": {
-                "permission-x": true,
-                "permission-y": false
-            },
-            "service": "<relevant-service>"
-        }
-        ```
-        
-        ### Change the username
-        `/auth/update`
-        
-        **Method:** `POST`
-        
-        **Query Parameters:**
-        
-         - `jwt` - authentication token (received from `/user/check`)
-         - `username` - A new username for the user profile (this action is only allowed once)
-        
-        **Returns:**
-        
-        ```json
-        {
-            "success": true,
-            "error": "<error-message-if-applicable>"
-        }
-        ```
-        
-        __Note__: trying to update other user profile fields like `email` will fail silently and return
-        
-        ```json
-        {
-            "success": true
-        }
-        ```
-        
-        ### Receive authorization public key
-        `/auth/public-key`
-        
-        **Method:** `GET`
-        
-        **Returns:**
-        
-        The service's public key in PEM format.
-        
-        Can be used by services to validate that the permission token is authentic.
 Keywords: data,authentication,oauth2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: develop
+License-File: LICENSE
+
+# Oauth2 Flask Service
+
+[![Build Status](https://travis-ci.org/datahq/auth.svg?branch=master)](https://travis-ci.org/dataspot/dgp-oauth2)
+
+A generic OAuth2 authentication service and user permission manager.
+
+Based off [OpenSpending auth service](https://github.com/openspending/os-conductor).
+
+## Quick start
+
+### Clone the repo and install
+
+`make install`
+
+### Run tests
+
+`make test`
+
+### Run server
+
+`python server.py`
+
+## Env Vars
+- `PRIVATE_KEY` & `PUBLIC_KEY` an RSA key-pair in PEM format.
+  See `tools/generate_key_pair.sh` for more info.
+- `GOOGLE_KEY` & `GOOGLE_SECRET`: OAuth credentials for authenticating with Google
+- `GITHUB_KEY` & `GITHUB_SECRET`: OAuth credentials for authenticating with Github
+- `DATABASE_URL`: A SQLAlchemy compatible database connection string (where user data is stored)
+- `EXTERNAL_ADDRESS`: The hostname where this service is located on
+- `ALLOWED_SERVICES`:
+    Which permissions providers are available. A `;` delimited list of provider identifiers.
+    Each provider identifier takes the form of `[alias:]provider`, where `provider` is the name of a Python module
+    which exports a `get_permissions(service, userid)` function.
+- `INSTALLED_EXTENSIONS`:
+    List of installed extensions. A `;` delimited list of `extension` - the name of a Python modules which exports one or all of these functions
+    - `on_new_user(user_info)`
+    - `on_user_login(user_info)`
+    - `on_user_logout(user_info)`
+
+
+## API
+
+### Check an authentication token's validity
+`/auth/check`
+
+**Method:** `GET`
+
+**Query Parameters:**
+
+ - `jwt` - authentication token
+ - `next` - URL to redirect to when finished authentication
+
+**Returns:**
+
+If authenticated:
+
+```json
+{
+    "authenticated": true,
+    "profile": {
+        "id": "<user-id>",
+        "name": "<user-name>",
+        "email": "<user-email>",
+        "avatar_url": "<url-for-user's-profile-photo>",
+        "idhash": "<unique-id-of-the-user>",
+        "username": "<user-selected-id>" # If user has a username
+    }
+}
+```
+
+If not:
+
+```json
+{
+    "authenticated": false,
+    "providers": {
+        "google": {
+            "url": "<url-for-logging-in-with-the-Google-provider>"
+        },
+        "github": {
+            "url": "<url-for-logging-in-with-the-Github-provider>"
+        },
+    }
+}
+```
+
+When the authentication flow is finished, the caller will be redirected to the `next` URL with an extra query parameter
+`jwt` which contains the authentication token. The caller should cache this token for further interactions with the API.
+
+### Get permission for a service
+`/auth/authorize`
+
+**Method:** `GET`
+
+**Query Parameters:**
+
+ - `jwt` - user token (received from `/user/check`)
+ - `service` - the relevant service (e.g. `storage-service`)
+
+**Returns:**
+
+```json
+{
+    "token": "<token-for-the-relevant-service>"
+    "userid": "<unique-id-of-the-user>",
+    "permissions": {
+        "permission-x": true,
+        "permission-y": false
+    },
+    "service": "<relevant-service>"
+}
+```
+
+### Change the username
+`/auth/update`
+
+**Method:** `POST`
+
+**Query Parameters:**
+
+ - `jwt` - authentication token (received from `/user/check`)
+ - `username` - A new username for the user profile (this action is only allowed once)
+
+**Returns:**
+
+```json
+{
+    "success": true,
+    "error": "<error-message-if-applicable>"
+}
+```
+
+__Note__: trying to update other user profile fields like `email` will fail silently and return
+
+```json
+{
+    "success": true
+}
+```
+
+### Receive authorization public key
+`/auth/public-key`
+
+**Method:** `GET`
+
+**Returns:**
+
+The service's public key in PEM format.
+
+Can be used by services to validate that the permission token is authentic.
+
```

### Comparing `dgp-oauth2-1.0.7/setup.py` & `dgp-oauth2-1.1.0/setup.py`

 * *Files identical despite different names*

