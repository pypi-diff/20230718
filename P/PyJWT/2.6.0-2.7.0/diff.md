# Comparing `tmp/PyJWT-2.6.0.tar.gz` & `tmp/PyJWT-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyJWT-2.6.0.tar", last modified: Thu Oct 20 01:08:45 2022, max compression
+gzip compressed data, was "dist/PyJWT-2.7.0.tar", last modified: Tue May  9 20:04:10 2023, max compression
```

## Comparing `PyJWT-2.6.0.tar` & `PyJWT-2.7.0.tar`

### file list

```diff
@@ -1,88 +1,90 @@
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.271692 PyJWT-2.6.0/
--rw-r--r--   0 jpadilla   (501) staff       (20)      908 2022-10-20 00:40:43.000000 PyJWT-2.6.0/.pre-commit-config.yaml
--rw-r--r--   0 jpadilla   (501) staff       (20)      322 2020-11-02 12:48:30.000000 PyJWT-2.6.0/AUTHORS.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)    28577 2022-10-20 01:08:19.000000 PyJWT-2.6.0/CHANGELOG.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)     3272 2019-10-20 23:19:00.000000 PyJWT-2.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jpadilla   (501) staff       (20)     1085 2022-05-12 18:31:26.000000 PyJWT-2.6.0/LICENSE
--rw-r--r--   0 jpadilla   (501) staff       (20)      309 2021-01-12 03:01:03.000000 PyJWT-2.6.0/MANIFEST.in
--rw-r--r--   0 jpadilla   (501) staff       (20)     3836 2022-10-20 01:08:45.272015 PyJWT-2.6.0/PKG-INFO
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.209050 PyJWT-2.6.0/PyJWT.egg-info/
--rw-r--r--   0 jpadilla   (501) staff       (20)     3836 2022-10-20 01:08:44.000000 PyJWT-2.6.0/PyJWT.egg-info/PKG-INFO
--rw-r--r--   0 jpadilla   (501) staff       (20)     1873 2022-10-20 01:08:45.000000 PyJWT-2.6.0/PyJWT.egg-info/SOURCES.txt
--rw-r--r--   0 jpadilla   (501) staff       (20)        1 2022-10-20 01:08:44.000000 PyJWT-2.6.0/PyJWT.egg-info/dependency_links.txt
--rw-r--r--   0 jpadilla   (501) staff       (20)        1 2022-09-17 14:01:39.000000 PyJWT-2.6.0/PyJWT.egg-info/not-zip-safe
--rw-r--r--   0 jpadilla   (501) staff       (20)      277 2022-10-20 01:08:44.000000 PyJWT-2.6.0/PyJWT.egg-info/requires.txt
--rw-r--r--   0 jpadilla   (501) staff       (20)        4 2022-10-20 01:08:44.000000 PyJWT-2.6.0/PyJWT.egg-info/top_level.txt
--rw-r--r--   0 jpadilla   (501) staff       (20)     2336 2022-09-20 10:55:34.000000 PyJWT-2.6.0/README.rst
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.219760 PyJWT-2.6.0/docs/
--rw-r--r--   0 jpadilla   (501) staff       (20)     7405 2018-11-26 03:04:17.000000 PyJWT-2.6.0/docs/Makefile
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.220723 PyJWT-2.6.0/docs/_static/
--rw-r--r--   0 jpadilla   (501) staff       (20)      363 2018-11-26 03:04:17.000000 PyJWT-2.6.0/docs/_static/theme_overrides.css
--rw-r--r--   0 jpadilla   (501) staff       (20)     3538 2022-07-19 02:16:21.000000 PyJWT-2.6.0/docs/algorithms.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)     7518 2022-09-20 10:55:34.000000 PyJWT-2.6.0/docs/api.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)       30 2021-01-12 03:01:03.000000 PyJWT-2.6.0/docs/changelog.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)     3914 2022-05-12 18:31:26.000000 PyJWT-2.6.0/docs/conf.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      621 2020-12-20 00:01:37.000000 PyJWT-2.6.0/docs/faq.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)     2018 2022-09-20 10:55:34.000000 PyJWT-2.6.0/docs/index.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)      791 2021-08-08 19:55:24.000000 PyJWT-2.6.0/docs/installation.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)       24 2020-06-19 14:24:04.000000 PyJWT-2.6.0/docs/requirements-docs.txt
--rw-r--r--   0 jpadilla   (501) staff       (20)    11752 2022-05-12 18:31:26.000000 PyJWT-2.6.0/docs/usage.rst
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.230894 PyJWT-2.6.0/jwt/
--rw-r--r--   0 jpadilla   (501) staff       (20)     1604 2022-10-20 01:08:19.000000 PyJWT-2.6.0/jwt/__init__.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    23688 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/algorithms.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     3653 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/api_jwk.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    10653 2022-09-20 11:00:07.000000 PyJWT-2.6.0/jwt/api_jws.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    10059 2022-10-20 00:40:19.000000 PyJWT-2.6.0/jwt/api_jwt.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      963 2022-05-12 18:31:26.000000 PyJWT-2.6.0/jwt/exceptions.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     1692 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/help.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      944 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/jwk_set_cache.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     3553 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/jwks_client.py
--rw-r--r--   0 jpadilla   (501) staff       (20)        0 2020-12-20 00:01:37.000000 PyJWT-2.6.0/jwt/py.typed
--rw-r--r--   0 jpadilla   (501) staff       (20)     3973 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/utils.py
--rw-r--r--   0 jpadilla   (501) staff       (20)       59 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/warnings.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      448 2022-09-20 10:55:34.000000 PyJWT-2.6.0/pyproject.toml
--rw-r--r--   0 jpadilla   (501) staff       (20)     1384 2022-10-20 01:08:45.273726 PyJWT-2.6.0/setup.cfg
--rwxr-xr-x   0 jpadilla   (501) staff       (20)       62 2020-06-19 15:14:56.000000 PyJWT-2.6.0/setup.py
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.243403 PyJWT-2.6.0/tests/
--rw-r--r--   0 jpadilla   (501) staff       (20)        0 2018-11-26 03:04:17.000000 PyJWT-2.6.0/tests/__init__.py
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.270980 PyJWT-2.6.0/tests/keys/
--rw-r--r--   0 jpadilla   (501) staff       (20)     1488 2020-12-21 16:55:46.000000 PyJWT-2.6.0/tests/keys/__init__.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      245 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_ec_key_P-256.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      308 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/jwk_ec_key_P-384.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      380 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/jwk_ec_key_P-521.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      250 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_ec_key_secp256k1.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      191 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_ec_pub_P-256.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      233 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/jwk_ec_pub_P-384.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      281 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/jwk_ec_pub_P-521.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      196 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_ec_pub_secp256k1.json
--rw-rw-r--   0 jpadilla   (501) staff       (20)      171 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/jwk_hmac.json
--rw-r--r--   0 jpadilla   (501) staff       (20)     1470 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/keys/jwk_keyset_only_unknown_alg.json
--rw-r--r--   0 jpadilla   (501) staff       (20)     2926 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/keys/jwk_keyset_with_unknown_alg.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      143 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_okp_key_Ed25519.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      270 2021-10-06 10:37:16.000000 PyJWT-2.6.0/tests/keys/jwk_okp_key_Ed448.json
--rw-r--r--   0 jpadilla   (501) staff       (20)       90 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_okp_pub_Ed25519.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      183 2021-10-06 10:37:16.000000 PyJWT-2.6.0/tests/keys/jwk_okp_pub_Ed448.json
--rw-rw-r--   0 jpadilla   (501) staff       (20)     1745 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/jwk_rsa_key.json
--rw-rw-r--   0 jpadilla   (501) staff       (20)      461 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/jwk_rsa_pub.json
--rw-rw-r--   0 jpadilla   (501) staff       (20)      451 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/testkey2_rsa.pub.pem
--rw-r--r--   0 jpadilla   (501) staff       (20)      241 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/testkey_ec.priv
--rw-r--r--   0 jpadilla   (501) staff       (20)      178 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/testkey_ec.pub
--rw-r--r--   0 jpadilla   (501) staff       (20)      209 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/keys/testkey_ec_secp192r1.priv
--rw-r--r--   0 jpadilla   (501) staff       (20)      161 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/testkey_ec_ssh.pub
--rw-r--r--   0 jpadilla   (501) staff       (20)      119 2020-08-24 14:15:08.000000 PyJWT-2.6.0/tests/keys/testkey_ed25519
--rw-r--r--   0 jpadilla   (501) staff       (20)       81 2020-08-24 14:15:07.000000 PyJWT-2.6.0/tests/keys/testkey_ed25519.pub
--rw-rw-r--   0 jpadilla   (501) staff       (20)      247 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/testkey_pkcs1.pub.pem
--rw-rw-r--   0 jpadilla   (501) staff       (20)     1281 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/testkey_rsa.cer
--rw-r--r--   0 jpadilla   (501) staff       (20)     1679 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/testkey_rsa.priv
--rw-rw-r--   0 jpadilla   (501) staff       (20)      401 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/testkey_rsa.pub
--rw-r--r--   0 jpadilla   (501) staff       (20)     5022 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/test_advisory.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    38285 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/test_algorithms.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     9699 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/test_api_jwk.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    29203 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/test_api_jws.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    25097 2022-10-20 00:40:19.000000 PyJWT-2.6.0/tests/test_api_jwt.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      213 2019-10-22 15:57:44.000000 PyJWT-2.6.0/tests/test_exceptions.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    12895 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/test_jwks_client.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      625 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/test_jwt.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      897 2020-12-20 00:01:37.000000 PyJWT-2.6.0/tests/test_utils.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      722 2021-10-06 10:37:16.000000 PyJWT-2.6.0/tests/utils.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     1427 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tox.ini
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2023-05-09 20:04:10.466741 PyJWT-2.7.0/
+-rw-r--r--   0 jpadilla   (501) staff       (20)      961 2023-05-09 14:57:33.000000 PyJWT-2.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 jpadilla   (501) staff       (20)      322 2020-11-02 12:48:30.000000 PyJWT-2.7.0/AUTHORS.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)    31111 2023-05-09 19:04:15.000000 PyJWT-2.7.0/CHANGELOG.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3272 2019-10-20 23:19:00.000000 PyJWT-2.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1085 2022-05-12 18:31:26.000000 PyJWT-2.7.0/LICENSE
+-rw-r--r--   0 jpadilla   (501) staff       (20)      309 2021-01-12 03:01:03.000000 PyJWT-2.7.0/MANIFEST.in
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3887 2023-05-09 20:04:10.467066 PyJWT-2.7.0/PKG-INFO
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2023-05-09 20:04:10.416185 PyJWT-2.7.0/PyJWT.egg-info/
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3887 2023-05-09 20:04:10.000000 PyJWT-2.7.0/PyJWT.egg-info/PKG-INFO
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1915 2023-05-09 20:04:10.000000 PyJWT-2.7.0/PyJWT.egg-info/SOURCES.txt
+-rw-r--r--   0 jpadilla   (501) staff       (20)        1 2023-05-09 20:04:10.000000 PyJWT-2.7.0/PyJWT.egg-info/dependency_links.txt
+-rw-r--r--   0 jpadilla   (501) staff       (20)        1 2022-09-17 14:01:39.000000 PyJWT-2.7.0/PyJWT.egg-info/not-zip-safe
+-rw-r--r--   0 jpadilla   (501) staff       (20)      323 2023-05-09 20:04:10.000000 PyJWT-2.7.0/PyJWT.egg-info/requires.txt
+-rw-r--r--   0 jpadilla   (501) staff       (20)        4 2023-05-09 20:04:10.000000 PyJWT-2.7.0/PyJWT.egg-info/top_level.txt
+-rw-r--r--   0 jpadilla   (501) staff       (20)     2336 2022-09-20 10:55:34.000000 PyJWT-2.7.0/README.rst
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2023-05-09 20:04:10.424264 PyJWT-2.7.0/docs/
+-rw-r--r--   0 jpadilla   (501) staff       (20)     7405 2018-11-26 03:04:17.000000 PyJWT-2.7.0/docs/Makefile
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2023-05-09 20:04:10.425048 PyJWT-2.7.0/docs/_static/
+-rw-r--r--   0 jpadilla   (501) staff       (20)      363 2018-11-26 03:04:17.000000 PyJWT-2.7.0/docs/_static/theme_overrides.css
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3538 2022-07-19 02:16:21.000000 PyJWT-2.7.0/docs/algorithms.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)     7518 2022-09-20 10:55:34.000000 PyJWT-2.7.0/docs/api.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)       30 2021-01-12 03:01:03.000000 PyJWT-2.7.0/docs/changelog.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3928 2023-05-09 13:25:05.000000 PyJWT-2.7.0/docs/conf.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      621 2020-12-20 00:01:37.000000 PyJWT-2.7.0/docs/faq.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)     2018 2022-09-20 10:55:34.000000 PyJWT-2.7.0/docs/index.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)      791 2021-08-08 19:55:24.000000 PyJWT-2.7.0/docs/installation.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)       24 2020-06-19 14:24:04.000000 PyJWT-2.7.0/docs/requirements-docs.txt
+-rw-r--r--   0 jpadilla   (501) staff       (20)    14216 2023-05-09 13:25:05.000000 PyJWT-2.7.0/docs/usage.rst
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2023-05-09 20:04:10.431425 PyJWT-2.7.0/jwt/
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1604 2023-05-09 14:55:28.000000 PyJWT-2.7.0/jwt/__init__.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    29800 2023-05-09 19:04:14.000000 PyJWT-2.7.0/jwt/algorithms.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     4196 2023-05-09 19:02:14.000000 PyJWT-2.7.0/jwt/api_jwk.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    11099 2023-05-09 13:25:05.000000 PyJWT-2.7.0/jwt/api_jws.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    11825 2023-05-09 13:25:05.000000 PyJWT-2.7.0/jwt/api_jwt.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1046 2023-05-09 13:25:05.000000 PyJWT-2.7.0/jwt/exceptions.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1749 2023-05-09 13:25:05.000000 PyJWT-2.7.0/jwt/help.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      959 2023-05-09 13:25:05.000000 PyJWT-2.7.0/jwt/jwk_set_cache.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     4050 2023-05-09 13:25:05.000000 PyJWT-2.7.0/jwt/jwks_client.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)        0 2020-12-20 00:01:37.000000 PyJWT-2.7.0/jwt/py.typed
+-rw-r--r--   0 jpadilla   (501) staff       (20)       99 2023-05-09 13:25:05.000000 PyJWT-2.7.0/jwt/types.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3903 2023-05-09 13:25:05.000000 PyJWT-2.7.0/jwt/utils.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)       59 2022-09-20 10:55:34.000000 PyJWT-2.7.0/jwt/warnings.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      704 2023-05-09 19:04:14.000000 PyJWT-2.7.0/pyproject.toml
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1486 2023-05-09 20:04:10.468314 PyJWT-2.7.0/setup.cfg
+-rwxr-xr-x   0 jpadilla   (501) staff       (20)       62 2020-06-19 15:14:56.000000 PyJWT-2.7.0/setup.py
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2023-05-09 20:04:10.442337 PyJWT-2.7.0/tests/
+-rw-r--r--   0 jpadilla   (501) staff       (20)        0 2018-11-26 03:04:17.000000 PyJWT-2.7.0/tests/__init__.py
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2023-05-09 20:04:10.465957 PyJWT-2.7.0/tests/keys/
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1488 2020-12-21 16:55:46.000000 PyJWT-2.7.0/tests/keys/__init__.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      245 2021-04-28 11:23:40.000000 PyJWT-2.7.0/tests/keys/jwk_ec_key_P-256.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      308 2020-08-24 16:22:55.000000 PyJWT-2.7.0/tests/keys/jwk_ec_key_P-384.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      380 2020-08-24 16:22:55.000000 PyJWT-2.7.0/tests/keys/jwk_ec_key_P-521.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      250 2021-04-28 11:23:40.000000 PyJWT-2.7.0/tests/keys/jwk_ec_key_secp256k1.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      191 2021-04-28 11:23:40.000000 PyJWT-2.7.0/tests/keys/jwk_ec_pub_P-256.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      233 2020-08-24 16:22:55.000000 PyJWT-2.7.0/tests/keys/jwk_ec_pub_P-384.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      281 2020-08-24 16:22:55.000000 PyJWT-2.7.0/tests/keys/jwk_ec_pub_P-521.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      196 2021-04-28 11:23:40.000000 PyJWT-2.7.0/tests/keys/jwk_ec_pub_secp256k1.json
+-rw-rw-r--   0 jpadilla   (501) staff       (20)      171 2020-04-08 13:53:03.000000 PyJWT-2.7.0/tests/keys/jwk_hmac.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1470 2022-09-20 10:55:34.000000 PyJWT-2.7.0/tests/keys/jwk_keyset_only_unknown_alg.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)     2926 2022-09-20 10:55:34.000000 PyJWT-2.7.0/tests/keys/jwk_keyset_with_unknown_alg.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      143 2021-04-28 11:23:40.000000 PyJWT-2.7.0/tests/keys/jwk_okp_key_Ed25519.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      270 2021-10-06 10:37:16.000000 PyJWT-2.7.0/tests/keys/jwk_okp_key_Ed448.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)       90 2021-04-28 11:23:40.000000 PyJWT-2.7.0/tests/keys/jwk_okp_pub_Ed25519.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      183 2021-10-06 10:37:16.000000 PyJWT-2.7.0/tests/keys/jwk_okp_pub_Ed448.json
+-rw-rw-r--   0 jpadilla   (501) staff       (20)     1745 2020-04-08 13:53:03.000000 PyJWT-2.7.0/tests/keys/jwk_rsa_key.json
+-rw-rw-r--   0 jpadilla   (501) staff       (20)      461 2020-04-08 13:53:03.000000 PyJWT-2.7.0/tests/keys/jwk_rsa_pub.json
+-rw-rw-r--   0 jpadilla   (501) staff       (20)      451 2020-04-08 13:53:03.000000 PyJWT-2.7.0/tests/keys/testkey2_rsa.pub.pem
+-rw-r--r--   0 jpadilla   (501) staff       (20)      241 2020-08-24 16:22:55.000000 PyJWT-2.7.0/tests/keys/testkey_ec.priv
+-rw-r--r--   0 jpadilla   (501) staff       (20)      178 2020-08-24 16:22:55.000000 PyJWT-2.7.0/tests/keys/testkey_ec.pub
+-rw-r--r--   0 jpadilla   (501) staff       (20)      209 2022-09-20 10:55:34.000000 PyJWT-2.7.0/tests/keys/testkey_ec_secp192r1.priv
+-rw-r--r--   0 jpadilla   (501) staff       (20)      161 2020-08-24 16:22:55.000000 PyJWT-2.7.0/tests/keys/testkey_ec_ssh.pub
+-rw-r--r--   0 jpadilla   (501) staff       (20)      119 2020-08-24 14:15:08.000000 PyJWT-2.7.0/tests/keys/testkey_ed25519
+-rw-r--r--   0 jpadilla   (501) staff       (20)       81 2020-08-24 14:15:07.000000 PyJWT-2.7.0/tests/keys/testkey_ed25519.pub
+-rw-rw-r--   0 jpadilla   (501) staff       (20)      247 2020-04-08 13:53:03.000000 PyJWT-2.7.0/tests/keys/testkey_pkcs1.pub.pem
+-rw-rw-r--   0 jpadilla   (501) staff       (20)     1281 2020-04-08 13:53:03.000000 PyJWT-2.7.0/tests/keys/testkey_rsa.cer
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1679 2020-08-24 16:22:55.000000 PyJWT-2.7.0/tests/keys/testkey_rsa.priv
+-rw-rw-r--   0 jpadilla   (501) staff       (20)      401 2020-04-08 13:53:03.000000 PyJWT-2.7.0/tests/keys/testkey_rsa.pub
+-rw-r--r--   0 jpadilla   (501) staff       (20)     5091 2023-05-09 13:25:05.000000 PyJWT-2.7.0/tests/test_advisory.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    41068 2023-05-09 19:04:14.000000 PyJWT-2.7.0/tests/test_algorithms.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     9966 2023-05-09 13:25:05.000000 PyJWT-2.7.0/tests/test_api_jwk.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    29772 2023-05-09 13:25:05.000000 PyJWT-2.7.0/tests/test_api_jws.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    25396 2023-05-09 13:25:05.000000 PyJWT-2.7.0/tests/test_api_jwt.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1237 2023-05-09 13:25:05.000000 PyJWT-2.7.0/tests/test_compressed_jwt.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      213 2019-10-22 15:57:44.000000 PyJWT-2.7.0/tests/test_exceptions.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    15220 2023-05-09 13:25:05.000000 PyJWT-2.7.0/tests/test_jwks_client.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      625 2020-08-24 16:22:55.000000 PyJWT-2.7.0/tests/test_jwt.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      923 2023-05-09 13:25:05.000000 PyJWT-2.7.0/tests/test_utils.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      722 2021-10-06 10:37:16.000000 PyJWT-2.7.0/tests/utils.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1427 2022-09-20 10:55:34.000000 PyJWT-2.7.0/tox.ini
```

### Comparing `PyJWT-2.6.0/.pre-commit-config.yaml` & `PyJWT-2.7.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
         args: ["--target-version=py37"]
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
         args: ["--target-version=py37"]
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
-        language_version: python3.8
+        language_version: python3.9
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: debug-statements
 
   - repo: https://github.com/mgedmin/check-manifest
-    rev: "0.48"
+    rev: "0.49"
     hooks:
       - id: check-manifest
         args: [--no-build-isolation]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v0.982"
+    rev: "v1.2.0"
     hooks:
       - id: mypy
+        additional_dependencies: [cryptography>=3.4.0]
```

### Comparing `PyJWT-2.6.0/CHANGELOG.rst` & `PyJWT-2.7.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,62 @@
 Changelog
 =========
 
 All notable changes to this project will be documented in this file.
 This project adheres to `Semantic Versioning <https://semver.org/>`__.
 
-`Unreleased <https://github.com/jpadilla/pyjwt/compare/2.6.0...HEAD>`__
+`Unreleased <https://github.com/jpadilla/pyjwt/compare/2.7.0...HEAD>`__
 -----------------------------------------------------------------------
 
 Changed
 ~~~~~~~
 
 Fixed
 ~~~~~
 
 Added
 ~~~~~
 
+`v2.7.0 <https://github.com/jpadilla/pyjwt/compare/2.6.0...2.7.0>`__
+-----------------------------------------------------------------------
+
+Changed
+~~~~~~~
+
+- Changed the error message when the token audience doesn't match the expected audience by @irdkwmnsb `#809 <https://github.com/jpadilla/pyjwt/pull/809>`__
+- Improve error messages when cryptography isn't installed by @Viicos in `#846 <https://github.com/jpadilla/pyjwt/pull/846>`__
+- Make `Algorithm` an abstract base class by @Viicos in `#845 <https://github.com/jpadilla/pyjwt/pull/845>`__
+- ignore invalid keys in a jwks by @timw6n in `#863 <https://github.com/jpadilla/pyjwt/pull/863>`__
+
+Fixed
+~~~~~
+
+- Add classifier for Python 3.11 by @eseifert in `#818 <https://github.com/jpadilla/pyjwt/pull/818>`__
+- Fix ``_validate_iat`` validation by @Viicos in `#847 <https://github.com/jpadilla/pyjwt/pull/847>`__
+- fix: use datetime.datetime.timestamp function to have a milliseconds by @daillouf `#821 <https://github.com/jpadilla/pyjwt/pull/821>`__
+- docs: correct mistake in the changelog about verify param by @gbillig in `#866 <https://github.com/jpadilla/pyjwt/pull/866>`__
+
+Added
+~~~~~
+
+- Add ``compute_hash_digest`` as a method of ``Algorithm`` objects, which uses
+  the underlying hash algorithm to compute a digest. If there is no appropriate
+  hash algorithm, a ``NotImplementedError`` will be raised in `#775 <https://github.com/jpadilla/pyjwt/pull/775>`__
+- Add optional ``headers`` argument to ``PyJWKClient``. If provided, the headers
+  will be included in requests that the client uses when fetching the JWK set by @thundercat1 in `#823 <https://github.com/jpadilla/pyjwt/pull/823>`__
+- Add PyJWT._{de,en}code_payload hooks by @akx in `#829 <https://github.com/jpadilla/pyjwt/pull/829>`__
+- Add `sort_headers` parameter to `api_jwt.encode` by @evroon in `#832 <https://github.com/jpadilla/pyjwt/pull/832>`__
+- Make mypy configuration stricter and improve typing by @akx in `#830 <https://github.com/jpadilla/pyjwt/pull/830>`__
+- Add more types by @Viicos in `#843 <https://github.com/jpadilla/pyjwt/pull/843>`__
+- Add a timeout for PyJWKClient requests by @daviddavis in `#875 <https://github.com/jpadilla/pyjwt/pull/875>`__
+- Add client connection error exception by @daviddavis in `#876 <https://github.com/jpadilla/pyjwt/pull/876>`__
+- Add complete types to take all allowed keys into account by @Viicos in `#873 <https://github.com/jpadilla/pyjwt/pull/873>`__
+- Add `as_dict` option to `Algorithm.to_jwk` by @fluxth in `#881 <https://github.com/jpadilla/pyjwt/pull/881>`__
+
+
 `v2.6.0 <https://github.com/jpadilla/pyjwt/compare/2.5.0...2.6.0>`__
 -----------------------------------------------------------------------
 
 Changed
 ~~~~~~~
 
 - bump up cryptography >= 3.4.0 by @jpadilla in `#807 <https://github.com/jpadilla/pyjwt/pull/807>`_
@@ -246,15 +283,15 @@
 ``jwt.decode(encoded, key, algorithms=["HS256"], options={"require_exp": True})``,
 use
 ``jwt.decode(encoded, key, algorithms=["HS256"], options={"require": ["exp"]})``.
 
 And the old v1.x syntax
 ``jwt.decode(token, verify=False)``
 is now:
-``jwt.decode(jwt=token, key='secret', algorithms=['HS256'], options={"verify_signature": False, "verify_exp": True})``
+``jwt.decode(jwt=token, key='secret', algorithms=['HS256'], options={"verify_signature": False})``
 
 Added
 ~~~~~
 
 Introduce better experience for JWKs
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
```

### Comparing `PyJWT-2.6.0/CODE_OF_CONDUCT.md` & `PyJWT-2.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/LICENSE` & `PyJWT-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/PKG-INFO` & `PyJWT-2.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJWT
-Version: 2.6.0
+Version: 2.7.0
 Summary: JSON Web Token implementation in Python
 Home-page: https://github.com/jpadilla/pyjwt
 Author: Jose Padilla
 Author-email: hello@jpadilla.com
 License: MIT
 Description: PyJWT
         =====
@@ -78,14 +78,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: tests
 Provides-Extra: crypto
-Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: tests
+Provides-Extra: dev
```

### Comparing `PyJWT-2.6.0/PyJWT.egg-info/PKG-INFO` & `PyJWT-2.7.0/PyJWT.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJWT
-Version: 2.6.0
+Version: 2.7.0
 Summary: JSON Web Token implementation in Python
 Home-page: https://github.com/jpadilla/pyjwt
 Author: Jose Padilla
 Author-email: hello@jpadilla.com
 License: MIT
 Description: PyJWT
         =====
@@ -78,14 +78,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: tests
 Provides-Extra: crypto
-Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: tests
+Provides-Extra: dev
```

### Comparing `PyJWT-2.6.0/PyJWT.egg-info/SOURCES.txt` & `PyJWT-2.7.0/PyJWT.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,24 @@
 jwt/api_jws.py
 jwt/api_jwt.py
 jwt/exceptions.py
 jwt/help.py
 jwt/jwk_set_cache.py
 jwt/jwks_client.py
 jwt/py.typed
+jwt/types.py
 jwt/utils.py
 jwt/warnings.py
 tests/__init__.py
 tests/test_advisory.py
 tests/test_algorithms.py
 tests/test_api_jwk.py
 tests/test_api_jws.py
 tests/test_api_jwt.py
+tests/test_compressed_jwt.py
 tests/test_exceptions.py
 tests/test_jwks_client.py
 tests/test_jwt.py
 tests/test_utils.py
 tests/utils.py
 tests/keys/__init__.py
 tests/keys/jwk_ec_key_P-256.json
```

### Comparing `PyJWT-2.6.0/README.rst` & `PyJWT-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/docs/Makefile` & `PyJWT-2.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/docs/algorithms.rst` & `PyJWT-2.7.0/docs/algorithms.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/docs/api.rst` & `PyJWT-2.7.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/docs/conf.py` & `PyJWT-2.7.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import re
 
 import sphinx_rtd_theme
 
 
-def read(*parts):
+def read(*parts) -> str:
     """
     Build an absolute path from *parts* and and return the contents of the
     resulting file.  Assume UTF-8 encoding.
     """
     here = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(here, *parts), encoding="utf-8") as f:
         return f.read()
 
 
-def find_version(*file_paths):
+def find_version(*file_paths) -> str:
     """
     Build a path from *file_paths* and search for a ``__version__``
     string inside.
     """
     version_file = read(*file_paths)
     version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
     if version_match:
```

### Comparing `PyJWT-2.6.0/docs/faq.rst` & `PyJWT-2.7.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/docs/index.rst` & `PyJWT-2.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/docs/installation.rst` & `PyJWT-2.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/docs/usage.rst` & `PyJWT-2.7.0/docs/usage.rst`

 * *Files 14% similar despite different names*

```diff
@@ -282,18 +282,90 @@
 .. code-block:: pycon
 
     >>> import jwt
     >>> from jwt import PyJWKClient
     >>> token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImtpZCI6Ik5FRTFRVVJCT1RNNE16STVSa0ZETlRZeE9UVTFNRGcyT0Rnd1EwVXpNVGsxUWpZeVJrUkZRdyJ9.eyJpc3MiOiJodHRwczovL2Rldi04N2V2eDlydS5hdXRoMC5jb20vIiwic3ViIjoiYVc0Q2NhNzl4UmVMV1V6MGFFMkg2a0QwTzNjWEJWdENAY2xpZW50cyIsImF1ZCI6Imh0dHBzOi8vZXhwZW5zZXMtYXBpIiwiaWF0IjoxNTcyMDA2OTU0LCJleHAiOjE1NzIwMDY5NjQsImF6cCI6ImFXNENjYTc5eFJlTFdVejBhRTJINmtEME8zY1hCVnRDIiwiZ3R5IjoiY2xpZW50LWNyZWRlbnRpYWxzIn0.PUxE7xn52aTCohGiWoSdMBZGiYAHwE5FYie0Y1qUT68IHSTXwXVd6hn02HTah6epvHHVKA2FqcFZ4GGv5VTHEvYpeggiiZMgbxFrmTEY0csL6VNkX1eaJGcuehwQCRBKRLL3zKmA5IKGy5GeUnIbpPHLHDxr-GXvgFzsdsyWlVQvPX2xjeaQ217r2PtxDeqjlf66UYl6oY6AqNS8DH3iryCvIfCcybRZkc_hdy-6ZMoKT6Piijvk_aXdm7-QQqKJFHLuEqrVSOuBqqiNfVrG27QzAPuPOxvfXTVLXL2jek5meH6n-VWgrBdoMFH93QEszEDowDAEhQPHVs0xj7SIzA"
     >>> kid = "NEE1QURBOTM4MzI5RkFDNTYxOTU1MDg2ODgwQ0UzMTk1QjYyRkRFQw"
     >>> url = "https://dev-87evx9ru.auth0.com/.well-known/jwks.json"
-    >>> jwks_client = PyJWKClient(url)
+    >>> optional_custom_headers = {"User-agent": "custom-user-agent"}
+    >>> jwks_client = PyJWKClient(url, headers=optional_custom_headers)
     >>> signing_key = jwks_client.get_signing_key_from_jwt(token)
     >>> data = jwt.decode(
     ...     token,
     ...     signing_key.key,
     ...     algorithms=["RS256"],
     ...     audience="https://expenses-api",
     ...     options={"verify_exp": False},
     ... )
     >>> print(data)
     {'iss': 'https://dev-87evx9ru.auth0.com/', 'sub': 'aW4Cca79xReLWUz0aE2H6kD0O3cXBVtC@clients', 'aud': 'https://expenses-api', 'iat': 1572006954, 'exp': 1572006964, 'azp': 'aW4Cca79xReLWUz0aE2H6kD0O3cXBVtC', 'gty': 'client-credentials'}
+
+OIDC Login Flow
+---------------
+
+The following usage demonstrates an OIDC login flow using pyjwt. Further
+reading about the OIDC spec is recommended for implementers.
+
+In particular, this demonstrates validation of the ``at_hash`` claim.
+This claim relies on data from outside of the the JWT for validation. Methods
+are provided which support computation and validation of this claim, but it
+is not built into pyjwt.
+
+.. code-block:: python
+
+    import base64
+    import jwt
+    import requests
+
+
+    # Part 1: setup
+    # get the OIDC config and JWKs to use
+
+    # in OIDC, you must know your client_id (this is the OAuth 2.0 client_id)
+    client_id = ...
+
+    # example of fetching data from your OIDC server
+    # see: https://openid.net/specs/openid-connect-discovery-1_0.html#ProviderConfig
+    oidc_server = ...
+    oidc_config = requests.get(
+        f"https://{oidc_server}/.well-known/openid-configuration"
+    ).json()
+    signing_algos = oidc_config["id_token_signing_alg_values_supported"]
+
+    # setup a PyJWKClient to get the appropriate signing key
+    jwks_client = jwt.PyJWKClient(oidc_config["jwks_uri"])
+
+
+    # Part 2: login / authorization
+    # when a user completes an OIDC login flow, there will be a well-formed
+    # response object to parse/handle
+
+    # data from the login flow
+    # see: https://openid.net/specs/openid-connect-core-1_0.html#TokenResponse
+    token_response = ...
+    id_token = token_response["id_token"]
+    access_token = token_response["access_token"]
+
+
+    # Part 3: decode and validate at_hash
+    # after the login is complete, the id_token needs to be decoded
+    # this is the stage at which an OIDC client must verify the at_hash
+
+    # get signing_key from id_token
+    signing_key = jwks_client.get_signing_key_from_jwt(id_token)
+
+    # now, decode_complete to get payload + header
+    data = jwt.decode_complete(
+        id_token,
+        key=signing_key.key,
+        algorithms=signing_algos,
+        audience=client_id,
+    )
+    payload, header = data["payload"], data["header"]
+
+    # get the pyjwt algorithm object
+    alg_obj = jwt.get_algorithm_by_name(header["alg"])
+
+    # compute at_hash, then validate / assert
+    digest = alg_obj.compute_hash_digest(access_token)
+    at_hash = base64.urlsafe_b64encode(digest[: (len(digest) // 2)]).rstrip("=")
+    assert at_hash == payload["at_hash"]
```

### Comparing `PyJWT-2.6.0/jwt/__init__.py` & `PyJWT-2.7.0/jwt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     PyJWKClientError,
     PyJWKError,
     PyJWKSetError,
     PyJWTError,
 )
 from .jwks_client import PyJWKClient
 
-__version__ = "2.6.0"
+__version__ = "2.7.0"
 
 __title__ = "PyJWT"
 __description__ = "JSON Web Token implementation in Python"
 __url__ = "https://pyjwt.readthedocs.io"
 __uri__ = __url__
 __doc__ = f"{__description__} <{__uri__}>"
```

### Comparing `PyJWT-2.6.0/jwt/api_jws.py` & `PyJWT-2.7.0/jwt/api_jws.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import binascii
 import json
 import warnings
-from typing import Any, Type
+from typing import TYPE_CHECKING, Any
 
 from .algorithms import (
     Algorithm,
     get_default_algorithms,
     has_crypto,
     requires_cryptography,
 )
@@ -16,19 +16,26 @@
     InvalidAlgorithmError,
     InvalidSignatureError,
     InvalidTokenError,
 )
 from .utils import base64url_decode, base64url_encode
 from .warnings import RemovedInPyjwt3Warning
 
+if TYPE_CHECKING:
+    from .algorithms import AllowedPrivateKeys, AllowedPublicKeys
+
 
 class PyJWS:
     header_typ = "JWT"
 
-    def __init__(self, algorithms=None, options=None) -> None:
+    def __init__(
+        self,
+        algorithms: list[str] | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> None:
         self._algorithms = get_default_algorithms()
         self._valid_algs = (
             set(algorithms) if algorithms is not None else set(self._algorithms)
         )
 
         # Remove algorithms that aren't on the whitelist
         for key in list(self._algorithms.keys()):
@@ -92,19 +99,20 @@
                     f"Algorithm '{alg_name}' could not be found. Do you have cryptography installed?"
                 ) from e
             raise NotImplementedError("Algorithm not supported") from e
 
     def encode(
         self,
         payload: bytes,
-        key: str,
+        key: AllowedPrivateKeys | str | bytes,
         algorithm: str | None = "HS256",
         headers: dict[str, Any] | None = None,
-        json_encoder: Type[json.JSONEncoder] | None = None,
+        json_encoder: type[json.JSONEncoder] | None = None,
         is_payload_detached: bool = False,
+        sort_headers: bool = True,
     ) -> str:
         segments = []
 
         # declare a new var to narrow the type for type checkers
         algorithm_: str = algorithm if algorithm is not None else "none"
 
         # Prefer headers values if present to function parameters.
@@ -129,17 +137,16 @@
 
         if is_payload_detached:
             header["b64"] = False
         elif "b64" in header:
             # True is the standard value for b64, so no need for it
             del header["b64"]
 
-        # Fix for headers misorder - issue #715
         json_header = json.dumps(
-            header, separators=(",", ":"), cls=json_encoder, sort_keys=True
+            header, separators=(",", ":"), cls=json_encoder, sort_keys=sort_headers
         ).encode()
 
         segments.append(base64url_encode(json_header))
 
         if is_payload_detached:
             msg_payload = payload
         else:
@@ -160,16 +167,16 @@
             segments[1] = b""
         encoded_string = b".".join(segments)
 
         return encoded_string.decode("utf-8")
 
     def decode_complete(
         self,
-        jwt: str,
-        key: str = "",
+        jwt: str | bytes,
+        key: AllowedPublicKeys | str | bytes = "",
         algorithms: list[str] | None = None,
         options: dict[str, Any] | None = None,
         detached_payload: bytes | None = None,
         **kwargs,
     ) -> dict[str, Any]:
         if kwargs:
             warnings.warn(
@@ -205,45 +212,45 @@
             "payload": payload,
             "header": header,
             "signature": signature,
         }
 
     def decode(
         self,
-        jwt: str,
-        key: str = "",
+        jwt: str | bytes,
+        key: AllowedPublicKeys | str | bytes = "",
         algorithms: list[str] | None = None,
         options: dict[str, Any] | None = None,
         detached_payload: bytes | None = None,
         **kwargs,
-    ) -> str:
+    ) -> Any:
         if kwargs:
             warnings.warn(
                 "passing additional kwargs to decode() is deprecated "
                 "and will be removed in pyjwt version 3. "
                 f"Unsupported kwargs: {tuple(kwargs.keys())}",
                 RemovedInPyjwt3Warning,
             )
         decoded = self.decode_complete(
             jwt, key, algorithms, options, detached_payload=detached_payload
         )
         return decoded["payload"]
 
-    def get_unverified_header(self, jwt: str | bytes) -> dict:
+    def get_unverified_header(self, jwt: str | bytes) -> dict[str, Any]:
         """Returns back the JWT header parameters as a dict()
 
         Note: The signature is not verified so the header parameters
         should not be fully trusted until signature verification is complete
         """
         headers = self._load(jwt)[2]
         self._validate_headers(headers)
 
         return headers
 
-    def _load(self, jwt: str | bytes) -> tuple[bytes, bytes, dict, bytes]:
+    def _load(self, jwt: str | bytes) -> tuple[bytes, bytes, dict[str, Any], bytes]:
         if isinstance(jwt, str):
             jwt = jwt.encode("utf-8")
 
         if not isinstance(jwt, bytes):
             raise DecodeError(f"Invalid token type. Token must be a {bytes}")
 
         try:
@@ -276,39 +283,41 @@
             raise DecodeError("Invalid crypto padding") from err
 
         return (payload, signing_input, header, signature)
 
     def _verify_signature(
         self,
         signing_input: bytes,
-        header: dict,
+        header: dict[str, Any],
         signature: bytes,
-        key: str = "",
+        key: AllowedPublicKeys | str | bytes = "",
         algorithms: list[str] | None = None,
     ) -> None:
-
-        alg = header.get("alg")
+        try:
+            alg = header["alg"]
+        except KeyError:
+            raise InvalidAlgorithmError("Algorithm not specified")
 
         if not alg or (algorithms is not None and alg not in algorithms):
             raise InvalidAlgorithmError("The specified alg value is not allowed")
 
         try:
             alg_obj = self.get_algorithm_by_name(alg)
         except NotImplementedError as e:
             raise InvalidAlgorithmError("Algorithm not supported") from e
-        key = alg_obj.prepare_key(key)
+        prepared_key = alg_obj.prepare_key(key)
 
-        if not alg_obj.verify(signing_input, key, signature):
+        if not alg_obj.verify(signing_input, prepared_key, signature):
             raise InvalidSignatureError("Signature verification failed")
 
     def _validate_headers(self, headers: dict[str, Any]) -> None:
         if "kid" in headers:
             self._validate_kid(headers["kid"])
 
-    def _validate_kid(self, kid: str) -> None:
+    def _validate_kid(self, kid: Any) -> None:
         if not isinstance(kid, str):
             raise InvalidTokenError("Key ID header parameter must be a string")
 
 
 _jws_global_obj = PyJWS()
 encode = _jws_global_obj.encode
 decode_complete = _jws_global_obj.decode_complete
```

### Comparing `PyJWT-2.6.0/jwt/api_jwt.py` & `PyJWT-2.7.0/jwt/api_jwt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,124 @@
 from __future__ import annotations
 
 import json
 import warnings
 from calendar import timegm
-from collections.abc import Iterable, Mapping
+from collections.abc import Iterable
 from datetime import datetime, timedelta, timezone
-from typing import Any, Dict, List, Optional, Type, Union
+from typing import TYPE_CHECKING, Any
 
 from . import api_jws
 from .exceptions import (
     DecodeError,
     ExpiredSignatureError,
     ImmatureSignatureError,
     InvalidAudienceError,
     InvalidIssuedAtError,
     InvalidIssuerError,
     MissingRequiredClaimError,
 )
 from .warnings import RemovedInPyjwt3Warning
 
+if TYPE_CHECKING:
+    from .algorithms import AllowedPrivateKeys, AllowedPublicKeys
+
 
 class PyJWT:
-    def __init__(self, options=None):
+    def __init__(self, options: dict[str, Any] | None = None) -> None:
         if options is None:
             options = {}
-        self.options = {**self._get_default_options(), **options}
+        self.options: dict[str, Any] = {**self._get_default_options(), **options}
 
     @staticmethod
-    def _get_default_options() -> Dict[str, Union[bool, List[str]]]:
+    def _get_default_options() -> dict[str, bool | list[str]]:
         return {
             "verify_signature": True,
             "verify_exp": True,
             "verify_nbf": True,
             "verify_iat": True,
             "verify_aud": True,
             "verify_iss": True,
             "require": [],
         }
 
     def encode(
         self,
-        payload: Dict[str, Any],
-        key: str,
-        algorithm: Optional[str] = "HS256",
-        headers: Optional[Dict[str, Any]] = None,
-        json_encoder: Optional[Type[json.JSONEncoder]] = None,
+        payload: dict[str, Any],
+        key: AllowedPrivateKeys | str | bytes,
+        algorithm: str | None = "HS256",
+        headers: dict[str, Any] | None = None,
+        json_encoder: type[json.JSONEncoder] | None = None,
+        sort_headers: bool = True,
     ) -> str:
-        # Check that we get a mapping
-        if not isinstance(payload, Mapping):
+        # Check that we get a dict
+        if not isinstance(payload, dict):
             raise TypeError(
-                "Expecting a mapping object, as JWT only supports "
+                "Expecting a dict object, as JWT only supports "
                 "JSON objects as payloads."
             )
 
         # Payload
         payload = payload.copy()
         for time_claim in ["exp", "iat", "nbf"]:
             # Convert datetime to a intDate value in known time-format claims
             if isinstance(payload.get(time_claim), datetime):
                 payload[time_claim] = timegm(payload[time_claim].utctimetuple())
 
-        json_payload = json.dumps(
-            payload, separators=(",", ":"), cls=json_encoder
-        ).encode("utf-8")
+        json_payload = self._encode_payload(
+            payload,
+            headers=headers,
+            json_encoder=json_encoder,
+        )
 
-        return api_jws.encode(json_payload, key, algorithm, headers, json_encoder)
+        return api_jws.encode(
+            json_payload,
+            key,
+            algorithm,
+            headers,
+            json_encoder,
+            sort_headers=sort_headers,
+        )
+
+    def _encode_payload(
+        self,
+        payload: dict[str, Any],
+        headers: dict[str, Any] | None = None,
+        json_encoder: type[json.JSONEncoder] | None = None,
+    ) -> bytes:
+        """
+        Encode a given payload to the bytes to be signed.
+
+        This method is intended to be overridden by subclasses that need to
+        encode the payload in a different way, e.g. compress the payload.
+        """
+        return json.dumps(
+            payload,
+            separators=(",", ":"),
+            cls=json_encoder,
+        ).encode("utf-8")
 
     def decode_complete(
         self,
-        jwt: str,
-        key: str = "",
-        algorithms: Optional[List[str]] = None,
-        options: Optional[Dict[str, Any]] = None,
+        jwt: str | bytes,
+        key: AllowedPublicKeys | str | bytes = "",
+        algorithms: list[str] | None = None,
+        options: dict[str, Any] | None = None,
         # deprecated arg, remove in pyjwt3
-        verify: Optional[bool] = None,
+        verify: bool | None = None,
         # could be used as passthrough to api_jws, consider removal in pyjwt3
-        detached_payload: Optional[bytes] = None,
+        detached_payload: bytes | None = None,
         # passthrough arguments to _validate_claims
         # consider putting in options
-        audience: Optional[Union[str, Iterable[str]]] = None,
-        issuer: Optional[str] = None,
-        leeway: Union[int, float, timedelta] = 0,
+        audience: str | Iterable[str] | None = None,
+        issuer: str | None = None,
+        leeway: float | timedelta = 0,
         # kwargs
-        **kwargs,
-    ) -> Dict[str, Any]:
+        **kwargs: Any,
+    ) -> dict[str, Any]:
         if kwargs:
             warnings.warn(
                 "passing additional kwargs to decode_complete() is deprecated "
                 "and will be removed in pyjwt version 3. "
                 f"Unsupported kwargs: {tuple(kwargs.keys())}",
                 RemovedInPyjwt3Warning,
             )
@@ -121,47 +152,58 @@
             jwt,
             key=key,
             algorithms=algorithms,
             options=options,
             detached_payload=detached_payload,
         )
 
-        try:
-            payload = json.loads(decoded["payload"])
-        except ValueError as e:
-            raise DecodeError(f"Invalid payload string: {e}")
-        if not isinstance(payload, dict):
-            raise DecodeError("Invalid payload string: must be a json object")
+        payload = self._decode_payload(decoded)
 
         merged_options = {**self.options, **options}
         self._validate_claims(
             payload, merged_options, audience=audience, issuer=issuer, leeway=leeway
         )
 
         decoded["payload"] = payload
         return decoded
 
+    def _decode_payload(self, decoded: dict[str, Any]) -> Any:
+        """
+        Decode the payload from a JWS dictionary (payload, signature, header).
+
+        This method is intended to be overridden by subclasses that need to
+        decode the payload in a different way, e.g. decompress compressed
+        payloads.
+        """
+        try:
+            payload = json.loads(decoded["payload"])
+        except ValueError as e:
+            raise DecodeError(f"Invalid payload string: {e}")
+        if not isinstance(payload, dict):
+            raise DecodeError("Invalid payload string: must be a json object")
+        return payload
+
     def decode(
         self,
-        jwt: str,
-        key: str = "",
-        algorithms: Optional[List[str]] = None,
-        options: Optional[Dict[str, Any]] = None,
+        jwt: str | bytes,
+        key: AllowedPublicKeys | str | bytes = "",
+        algorithms: list[str] | None = None,
+        options: dict[str, Any] | None = None,
         # deprecated arg, remove in pyjwt3
-        verify: Optional[bool] = None,
+        verify: bool | None = None,
         # could be used as passthrough to api_jws, consider removal in pyjwt3
-        detached_payload: Optional[bytes] = None,
+        detached_payload: bytes | None = None,
         # passthrough arguments to _validate_claims
         # consider putting in options
-        audience: Optional[Union[str, Iterable[str]]] = None,
-        issuer: Optional[str] = None,
-        leeway: Union[int, float, timedelta] = 0,
+        audience: str | Iterable[str] | None = None,
+        issuer: str | None = None,
+        leeway: float | timedelta = 0,
         # kwargs
-        **kwargs,
-    ) -> Dict[str, Any]:
+        **kwargs: Any,
+    ) -> Any:
         if kwargs:
             warnings.warn(
                 "passing additional kwargs to decode() is deprecated "
                 "and will be removed in pyjwt version 3. "
                 f"Unsupported kwargs: {tuple(kwargs.keys())}",
                 RemovedInPyjwt3Warning,
             )
@@ -174,24 +216,31 @@
             detached_payload=detached_payload,
             audience=audience,
             issuer=issuer,
             leeway=leeway,
         )
         return decoded["payload"]
 
-    def _validate_claims(self, payload, options, audience=None, issuer=None, leeway=0):
+    def _validate_claims(
+        self,
+        payload: dict[str, Any],
+        options: dict[str, Any],
+        audience=None,
+        issuer=None,
+        leeway: float | timedelta = 0,
+    ) -> None:
         if isinstance(leeway, timedelta):
             leeway = leeway.total_seconds()
 
         if audience is not None and not isinstance(audience, (str, Iterable)):
             raise TypeError("audience must be a string, iterable or None")
 
         self._validate_required_claims(payload, options)
 
-        now = timegm(datetime.now(tz=timezone.utc).utctimetuple())
+        now = datetime.now(tz=timezone.utc).timestamp()
 
         if "iat" in payload and options["verify_iat"]:
             self._validate_iat(payload, now, leeway)
 
         if "nbf" in payload and options["verify_nbf"]:
             self._validate_nbf(payload, now, leeway)
 
@@ -200,47 +249,69 @@
 
         if options["verify_iss"]:
             self._validate_iss(payload, issuer)
 
         if options["verify_aud"]:
             self._validate_aud(payload, audience)
 
-    def _validate_required_claims(self, payload, options):
+    def _validate_required_claims(
+        self,
+        payload: dict[str, Any],
+        options: dict[str, Any],
+    ) -> None:
         for claim in options["require"]:
             if payload.get(claim) is None:
                 raise MissingRequiredClaimError(claim)
 
-    def _validate_iat(self, payload, now, leeway):
-        iat = payload["iat"]
+    def _validate_iat(
+        self,
+        payload: dict[str, Any],
+        now: float,
+        leeway: float,
+    ) -> None:
         try:
-            int(iat)
+            iat = int(payload["iat"])
         except ValueError:
             raise InvalidIssuedAtError("Issued At claim (iat) must be an integer.")
         if iat > (now + leeway):
             raise ImmatureSignatureError("The token is not yet valid (iat)")
 
-    def _validate_nbf(self, payload, now, leeway):
+    def _validate_nbf(
+        self,
+        payload: dict[str, Any],
+        now: float,
+        leeway: float,
+    ) -> None:
         try:
             nbf = int(payload["nbf"])
         except ValueError:
             raise DecodeError("Not Before claim (nbf) must be an integer.")
 
         if nbf > (now + leeway):
             raise ImmatureSignatureError("The token is not yet valid (nbf)")
 
-    def _validate_exp(self, payload, now, leeway):
+    def _validate_exp(
+        self,
+        payload: dict[str, Any],
+        now: float,
+        leeway: float,
+    ) -> None:
         try:
             exp = int(payload["exp"])
         except ValueError:
             raise DecodeError("Expiration Time claim (exp) must be an" " integer.")
 
         if exp <= (now - leeway):
             raise ExpiredSignatureError("Signature has expired")
 
-    def _validate_aud(self, payload, audience):
+    def _validate_aud(
+        self,
+        payload: dict[str, Any],
+        audience: str | Iterable[str] | None,
+    ) -> None:
         if audience is None:
             if "aud" not in payload or not payload["aud"]:
                 return
             # Application did not specify an audience, but
             # the token has the 'aud' claim
             raise InvalidAudienceError("Invalid audience")
 
@@ -258,17 +329,17 @@
         if any(not isinstance(c, str) for c in audience_claims):
             raise InvalidAudienceError("Invalid claim format in token")
 
         if isinstance(audience, str):
             audience = [audience]
 
         if all(aud not in audience_claims for aud in audience):
-            raise InvalidAudienceError("Invalid audience")
+            raise InvalidAudienceError("Audience doesn't match")
 
-    def _validate_iss(self, payload, issuer):
+    def _validate_iss(self, payload: dict[str, Any], issuer: Any) -> None:
         if issuer is None:
             return
 
         if "iss" not in payload:
             raise MissingRequiredClaimError("iss")
 
         if payload["iss"] != issuer:
```

### Comparing `PyJWT-2.6.0/jwt/exceptions.py` & `PyJWT-2.7.0/jwt/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,24 +43,28 @@
 
 
 class InvalidAlgorithmError(InvalidTokenError):
     pass
 
 
 class MissingRequiredClaimError(InvalidTokenError):
-    def __init__(self, claim):
+    def __init__(self, claim: str) -> None:
         self.claim = claim
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'Token is missing the "{self.claim}" claim'
 
 
 class PyJWKError(PyJWTError):
     pass
 
 
 class PyJWKSetError(PyJWTError):
     pass
 
 
 class PyJWKClientError(PyJWTError):
     pass
+
+
+class PyJWKClientConnectionError(PyJWKClientError):
+    pass
```

### Comparing `PyJWT-2.6.0/jwt/help.py` & `PyJWT-2.7.0/jwt/help.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import sys
 from typing import Dict
 
 from . import __version__ as pyjwt_version
 
 try:
     import cryptography
+
+    cryptography_version = cryptography.__version__
 except ModuleNotFoundError:
-    cryptography = None
+    cryptography_version = ""
 
 
 def info() -> Dict[str, Dict[str, str]]:
     """
     Generate information for a bug report.
     Based on the requests package help utility module.
     """
@@ -25,15 +27,15 @@
         platform_info = {"system": "Unknown", "release": "Unknown"}
 
     implementation = platform.python_implementation()
 
     if implementation == "CPython":
         implementation_version = platform.python_version()
     elif implementation == "PyPy":
-        pypy_version_info = getattr(sys, "pypy_version_info")
+        pypy_version_info = sys.pypy_version_info  # type: ignore[attr-defined]
         implementation_version = (
             f"{pypy_version_info.major}."
             f"{pypy_version_info.minor}."
             f"{pypy_version_info.micro}"
         )
         if pypy_version_info.releaselevel != "final":
             implementation_version = "".join(
@@ -44,15 +46,15 @@
 
     return {
         "platform": platform_info,
         "implementation": {
             "name": implementation,
             "version": implementation_version,
         },
-        "cryptography": {"version": getattr(cryptography, "__version__", "")},
+        "cryptography": {"version": cryptography_version},
         "pyjwt": {"version": pyjwt_version},
     }
 
 
 def main() -> None:
     """Pretty-print the bug information as JSON."""
     print(json.dumps(info(), sort_keys=True, indent=2))
```

### Comparing `PyJWT-2.6.0/jwt/jwk_set_cache.py` & `PyJWT-2.7.0/jwt/jwk_set_cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import time
 from typing import Optional
 
 from .api_jwk import PyJWKSet, PyJWTSetWithTimestamp
 
 
 class JWKSetCache:
-    def __init__(self, lifespan: int):
+    def __init__(self, lifespan: int) -> None:
         self.jwk_set_with_timestamp: Optional[PyJWTSetWithTimestamp] = None
         self.lifespan = lifespan
 
-    def put(self, jwk_set: PyJWKSet):
+    def put(self, jwk_set: PyJWKSet) -> None:
         if jwk_set is not None:
             self.jwk_set_with_timestamp = PyJWTSetWithTimestamp(jwk_set)
         else:
             # clear cache
             self.jwk_set_with_timestamp = None
 
     def get(self) -> Optional[PyJWKSet]:
         if self.jwk_set_with_timestamp is None or self.is_expired():
             return None
 
         return self.jwk_set_with_timestamp.get_jwk_set()
 
     def is_expired(self) -> bool:
-
         return (
             self.jwk_set_with_timestamp is not None
             and self.lifespan > -1
             and time.monotonic()
             > self.jwk_set_with_timestamp.get_timestamp() + self.lifespan
         )
```

### Comparing `PyJWT-2.6.0/jwt/jwks_client.py` & `PyJWT-2.7.0/jwt/jwks_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import json
 import urllib.request
 from functools import lru_cache
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional
 from urllib.error import URLError
 
 from .api_jwk import PyJWK, PyJWKSet
 from .api_jwt import decode_complete as decode_token
-from .exceptions import PyJWKClientError
+from .exceptions import PyJWKClientConnectionError, PyJWKClientError
 from .jwk_set_cache import JWKSetCache
 
 
 class PyJWKClient:
     def __init__(
         self,
         uri: str,
         cache_keys: bool = False,
         max_cached_keys: int = 16,
         cache_jwk_set: bool = True,
         lifespan: int = 300,
+        headers: Optional[Dict[str, Any]] = None,
+        timeout: int = 30,
     ):
+        if headers is None:
+            headers = {}
         self.uri = uri
         self.jwk_set_cache: Optional[JWKSetCache] = None
+        self.headers = headers
+        self.timeout = timeout
 
         if cache_jwk_set:
             # Init jwt set cache with default or given lifespan.
             # Default lifespan is 300 seconds (5 minutes).
             if lifespan <= 0:
                 raise PyJWKClientError(
                     f'Lifespan must be greater than 0, the input is "{lifespan}"'
@@ -37,32 +43,38 @@
             # Cache signing keys
             # Ignore mypy (https://github.com/python/mypy/issues/2427)
             self.get_signing_key = lru_cache(maxsize=max_cached_keys)(self.get_signing_key)  # type: ignore
 
     def fetch_data(self) -> Any:
         jwk_set: Any = None
         try:
-            with urllib.request.urlopen(self.uri) as response:
+            r = urllib.request.Request(url=self.uri, headers=self.headers)
+            with urllib.request.urlopen(r, timeout=self.timeout) as response:
                 jwk_set = json.load(response)
-        except URLError as e:
-            raise PyJWKClientError(f'Fail to fetch data from the url, err: "{e}"')
+        except (URLError, TimeoutError) as e:
+            raise PyJWKClientConnectionError(
+                f'Fail to fetch data from the url, err: "{e}"'
+            )
         else:
             return jwk_set
         finally:
             if self.jwk_set_cache is not None:
                 self.jwk_set_cache.put(jwk_set)
 
     def get_jwk_set(self, refresh: bool = False) -> PyJWKSet:
         data = None
         if self.jwk_set_cache is not None and not refresh:
             data = self.jwk_set_cache.get()
 
         if data is None:
             data = self.fetch_data()
 
+        if not isinstance(data, dict):
+            raise PyJWKClientError("The JWKS endpoint did not return a JSON object")
+
         return PyJWKSet.from_dict(data)
 
     def get_signing_keys(self, refresh: bool = False) -> List[PyJWK]:
         jwk_set = self.get_jwk_set(refresh)
         signing_keys = [
             jwk_set_key
             for jwk_set_key in jwk_set.keys
```

### Comparing `PyJWT-2.6.0/jwt/utils.py` & `PyJWT-2.7.0/jwt/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,35 @@
 try:
     from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurve
     from cryptography.hazmat.primitives.asymmetric.utils import (
         decode_dss_signature,
         encode_dss_signature,
     )
 except ModuleNotFoundError:
-    EllipticCurve = None
+    pass
 
 
-def force_bytes(value: Union[str, bytes]) -> bytes:
+def force_bytes(value: Union[bytes, str]) -> bytes:
     if isinstance(value, str):
         return value.encode("utf-8")
     elif isinstance(value, bytes):
         return value
     else:
         raise TypeError("Expected a string value")
 
 
-def base64url_decode(input: Union[str, bytes]) -> bytes:
-    if isinstance(input, str):
-        input = input.encode("ascii")
+def base64url_decode(input: Union[bytes, str]) -> bytes:
+    input_bytes = force_bytes(input)
 
-    rem = len(input) % 4
+    rem = len(input_bytes) % 4
 
     if rem > 0:
-        input += b"=" * (4 - rem)
+        input_bytes += b"=" * (4 - rem)
 
-    return base64.urlsafe_b64decode(input)
+    return base64.urlsafe_b64decode(input_bytes)
 
 
 def base64url_encode(input: bytes) -> bytes:
     return base64.urlsafe_b64encode(input).replace(b"=", b"")
 
 
 def to_base64url_uint(val: int) -> bytes:
@@ -46,19 +45,16 @@
 
     if len(int_bytes) == 0:
         int_bytes = b"\x00"
 
     return base64url_encode(int_bytes)
 
 
-def from_base64url_uint(val: Union[str, bytes]) -> int:
-    if isinstance(val, str):
-        val = val.encode("ascii")
-
-    data = base64url_decode(val)
+def from_base64url_uint(val: Union[bytes, str]) -> int:
+    data = base64url_decode(force_bytes(val))
     return int.from_bytes(data, byteorder="big")
 
 
 def number_to_bytes(num: int, num_bytes: int) -> bytes:
     padded_hex = "%0*x" % (2 * num_bytes, num)
     return binascii.a2b_hex(padded_hex.encode("ascii"))
 
@@ -74,34 +70,34 @@
     while remaining != 0:
         remaining >>= 8
         byte_length += 1
 
     return val.to_bytes(byte_length, "big", signed=False)
 
 
-def der_to_raw_signature(der_sig: bytes, curve: EllipticCurve) -> bytes:
+def der_to_raw_signature(der_sig: bytes, curve: "EllipticCurve") -> bytes:
     num_bits = curve.key_size
     num_bytes = (num_bits + 7) // 8
 
     r, s = decode_dss_signature(der_sig)
 
     return number_to_bytes(r, num_bytes) + number_to_bytes(s, num_bytes)
 
 
-def raw_to_der_signature(raw_sig: bytes, curve: EllipticCurve) -> bytes:
+def raw_to_der_signature(raw_sig: bytes, curve: "EllipticCurve") -> bytes:
     num_bits = curve.key_size
     num_bytes = (num_bits + 7) // 8
 
     if len(raw_sig) != 2 * num_bytes:
         raise ValueError("Invalid signature")
 
     r = bytes_to_number(raw_sig[:num_bytes])
     s = bytes_to_number(raw_sig[num_bytes:])
 
-    return encode_dss_signature(r, s)
+    return bytes(encode_dss_signature(r, s))
 
 
 # Based on https://github.com/hynek/pem/blob/7ad94db26b0bc21d10953f5dbad3acfdfacf57aa/src/pem/_core.py#L224-L252
 _PEMS = {
     b"CERTIFICATE",
     b"TRUSTED CERTIFICATE",
     b"PRIVATE KEY",
```

### Comparing `PyJWT-2.6.0/setup.cfg` & `PyJWT-2.7.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,24 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Utilities
 
 [options]
 zip_safe = false
 include_package_data = true
 python_requires = >=3.7
 packages = find:
+install_requires = 
+	typing_extensions; python_version<="3.7"
 
 [options.package_data]
 * = py.typed
 
 [options.extras_require]
 docs = 
 	sphinx>=4.5.0,<5.0.0
```

### Comparing `PyJWT-2.6.0/tests/keys/__init__.py` & `PyJWT-2.7.0/tests/keys/__init__.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/tests/keys/jwk_keyset_only_unknown_alg.json` & `PyJWT-2.7.0/tests/keys/jwk_keyset_only_unknown_alg.json`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/tests/keys/jwk_keyset_with_unknown_alg.json` & `PyJWT-2.7.0/tests/keys/jwk_keyset_with_unknown_alg.json`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/tests/keys/jwk_rsa_key.json` & `PyJWT-2.7.0/tests/keys/jwk_rsa_key.json`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/tests/keys/testkey_rsa.cer` & `PyJWT-2.7.0/tests/keys/testkey_rsa.cer`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/tests/keys/testkey_rsa.priv` & `PyJWT-2.7.0/tests/keys/testkey_rsa.priv`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/tests/test_advisory.py` & `PyJWT-2.7.0/tests/test_advisory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 import jwt
+from jwt.algorithms import get_default_algorithms
 from jwt.exceptions import InvalidKeyError
 
 from .utils import crypto_required
 
 priv_key_bytes = b"""-----BEGIN PRIVATE KEY-----
 MC4CAQAwBQYDK2VwBCIEIIbBhdo2ah7X32i50GOzrCr4acZTe6BezUdRIixjTAdL
 -----END PRIVATE KEY-----"""
@@ -46,26 +47,28 @@
         # encoded_good = jwt.encode({"test": 1234}, priv_key_bytes, algorithm="EdDSA")
         encoded_good = "eyJ0eXAiOiJKV1QiLCJhbGciOiJFZERTQSJ9.eyJ0ZXN0IjoxMjM0fQ.M5y1EEavZkHSlj9i8yi9nXKKyPBSAUhDRTOYZi3zZY11tZItDaR3qwAye8pc74_lZY3Ogt9KPNFbVOSGnUBHDg"
 
         # Using HMAC with the public key to trick the receiver to think that the
         # public key is a HMAC secret
         encoded_bad = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0ZXN0IjoxMjM0fQ.6ulDpqSlbHmQ8bZXhZRLFko9SwcHrghCwh8d-exJEE4"
 
+        algorithm_names = list(get_default_algorithms())
+
         # Both of the jwt tokens are validated as valid
         jwt.decode(
             encoded_good,
             pub_key_bytes,
-            algorithms=jwt.algorithms.get_default_algorithms(),
+            algorithms=algorithm_names,
         )
 
         with pytest.raises(InvalidKeyError):
             jwt.decode(
                 encoded_bad,
                 pub_key_bytes,
-                algorithms=jwt.algorithms.get_default_algorithms(),
+                algorithms=algorithm_names,
             )
 
         # Of course the receiver should specify ed25519 algorithm to be used if
         # they specify ed25519 public key. However, if other algorithms are used,
         # the POC does not work
         # HMAC specifies illegal strings for the HMAC secret in jwt/algorithms.py
         #
@@ -96,20 +99,21 @@
         # encoded_good = jwt.encode({"test": 1234}, ssh_priv_key_bytes, algorithm="ES256")
         encoded_good = "eyJhbGciOiJFUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0ZXN0IjoxMjM0fQ.NX42mS8cNqYoL3FOW9ZcKw8Nfq2mb6GqJVADeMA1-kyHAclilYo_edhdM_5eav9tBRQTlL0XMeu_WFE_mz3OXg"
 
         # Using HMAC with the ssh public key to trick the receiver to think that the public key is a HMAC secret
         # encoded_bad = jwt.encode({"test": 1234}, ssh_key_bytes, algorithm="HS256")
         encoded_bad = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0ZXN0IjoxMjM0fQ.5eYfbrbeGYmWfypQ6rMWXNZ8bdHcqKng5GPr9MJZITU"
 
+        algorithm_names = list(get_default_algorithms())
         # Both of the jwt tokens are validated as valid
         jwt.decode(
             encoded_good,
             ssh_key_bytes,
-            algorithms=jwt.algorithms.get_default_algorithms(),
+            algorithms=algorithm_names,
         )
 
         with pytest.raises(InvalidKeyError):
             jwt.decode(
                 encoded_bad,
                 ssh_key_bytes,
-                algorithms=jwt.algorithms.get_default_algorithms(),
+                algorithms=algorithm_names,
             )
```

### Comparing `PyJWT-2.6.0/tests/test_algorithms.py` & `PyJWT-2.7.0/tests/test_algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 import base64
 import json
+from typing import Any, cast
 
 import pytest
 
-from jwt.algorithms import Algorithm, HMACAlgorithm, NoneAlgorithm, has_crypto
+from jwt.algorithms import HMACAlgorithm, NoneAlgorithm, has_crypto
 from jwt.exceptions import InvalidKeyError
 from jwt.utils import base64url_decode
 
 from .keys import load_ec_pub_key_p_521, load_hmac_key, load_rsa_pub_key
 from .utils import crypto_required, key_path
 
 if has_crypto:
+    from cryptography.hazmat.primitives.asymmetric.ec import (
+        EllipticCurvePrivateKey,
+        EllipticCurvePublicKey,
+    )
+    from cryptography.hazmat.primitives.asymmetric.ed448 import (
+        Ed448PrivateKey,
+        Ed448PublicKey,
+    )
+    from cryptography.hazmat.primitives.asymmetric.ed25519 import (
+        Ed25519PrivateKey,
+        Ed25519PublicKey,
+    )
+    from cryptography.hazmat.primitives.asymmetric.rsa import (
+        RSAPrivateKey,
+        RSAPublicKey,
+    )
+
     from jwt.algorithms import ECAlgorithm, OKPAlgorithm, RSAAlgorithm, RSAPSSAlgorithm
 
 
 class TestAlgorithms:
-    def test_algorithm_should_throw_exception_if_prepare_key_not_impl(self):
-        algo = Algorithm()
-
-        with pytest.raises(NotImplementedError):
-            algo.prepare_key("test")
-
-    def test_algorithm_should_throw_exception_if_sign_not_impl(self):
-        algo = Algorithm()
-
-        with pytest.raises(NotImplementedError):
-            algo.sign("message", "key")
-
-    def test_algorithm_should_throw_exception_if_verify_not_impl(self):
-        algo = Algorithm()
-
-        with pytest.raises(NotImplementedError):
-            algo.verify("message", "key", "signature")
-
-    def test_algorithm_should_throw_exception_if_to_jwk_not_impl(self):
-        algo = Algorithm()
+    def test_none_algorithm_should_throw_exception_if_key_is_not_none(self):
+        algo = NoneAlgorithm()
 
-        with pytest.raises(NotImplementedError):
-            algo.from_jwk("value")
+        with pytest.raises(InvalidKeyError):
+            algo.prepare_key("123")
 
-    def test_algorithm_should_throw_exception_if_from_jwk_not_impl(self):
-        algo = Algorithm()
+    def test_none_algorithm_should_throw_exception_on_to_jwk(self):
+        algo = NoneAlgorithm()
 
         with pytest.raises(NotImplementedError):
-            algo.to_jwk("value")
+            algo.to_jwk("dummy")  # Using a dummy argument as is it not relevant
 
-    def test_none_algorithm_should_throw_exception_if_key_is_not_none(self):
+    def test_none_algorithm_should_throw_exception_on_from_jwk(self):
         algo = NoneAlgorithm()
 
-        with pytest.raises(InvalidKeyError):
-            algo.prepare_key("123")
+        with pytest.raises(NotImplementedError):
+            algo.from_jwk({})  # Using a dummy argument as is it not relevant
 
     def test_hmac_should_reject_nonstring_key(self):
         algo = HMACAlgorithm(HMACAlgorithm.SHA256)
 
         with pytest.raises(TypeError) as context:
-            algo.prepare_key(object())
+            algo.prepare_key(object())  # type: ignore[arg-type]
 
         exception = context.value
         assert str(exception) == "Expected a string value"
 
     def test_hmac_should_accept_unicode_key(self):
         algo = HMACAlgorithm(HMACAlgorithm.SHA256)
 
@@ -87,19 +87,23 @@
 
         with open(key_path("jwk_hmac.json")) as keyfile:
             key = algo.from_jwk(keyfile.read())
 
         signature = algo.sign(b"Hello World!", key)
         assert algo.verify(b"Hello World!", key, signature)
 
-    def test_hmac_to_jwk_returns_correct_values(self):
+    @pytest.mark.parametrize("as_dict", (False, True))
+    def test_hmac_to_jwk_returns_correct_values(self, as_dict):
         algo = HMACAlgorithm(HMACAlgorithm.SHA256)
-        key = algo.to_jwk("secret")
+        key: Any = algo.to_jwk("secret", as_dict=as_dict)
+
+        if not as_dict:
+            key = json.loads(key)
 
-        assert json.loads(key) == {"kty": "oct", "k": "c2VjcmV0"}
+        assert key == {"kty": "oct", "k": "c2VjcmV0"}
 
     def test_hmac_from_jwk_should_raise_exception_if_not_hmac_key(self):
         algo = HMACAlgorithm(HMACAlgorithm.SHA256)
 
         with open(key_path("jwk_rsa_pub.json")) as keyfile:
             with pytest.raises(InvalidKeyError):
                 algo.from_jwk(keyfile.read())
@@ -126,15 +130,15 @@
             algo.prepare_key(rsa_key.read())
 
     @crypto_required
     def test_rsa_should_reject_non_string_key(self):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with pytest.raises(TypeError):
-            algo.prepare_key(None)
+            algo.prepare_key(None)  # type: ignore[arg-type]
 
     @crypto_required
     def test_rsa_verify_should_return_false_if_signature_invalid(self):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         message = b"Hello World!"
 
@@ -146,35 +150,35 @@
             b"fHJnNUzAEUOXS0WahHVb57D30pcgIji9z923q90p5c7E2cU8V+E1qe8NdCA"
             b"APCDzZZ9zQ/dgcMVaBrGrgimrcLbPjueOKFgSO+SSjIElKA=="
         )
 
         sig += b"123"  # Signature is now invalid
 
         with open(key_path("testkey_rsa.pub")) as keyfile:
-            pub_key = algo.prepare_key(keyfile.read())
+            pub_key = cast(RSAPublicKey, algo.prepare_key(keyfile.read()))
 
         result = algo.verify(message, pub_key, sig)
         assert not result
 
     @crypto_required
     def test_ec_jwk_public_and_private_keys_should_parse_and_verify(self):
         tests = {
             "P-256": ECAlgorithm.SHA256,
             "P-384": ECAlgorithm.SHA384,
             "P-521": ECAlgorithm.SHA512,
             "secp256k1": ECAlgorithm.SHA256,
         }
-        for (curve, hash) in tests.items():
+        for curve, hash in tests.items():
             algo = ECAlgorithm(hash)
 
             with open(key_path(f"jwk_ec_pub_{curve}.json")) as keyfile:
-                pub_key = algo.from_jwk(keyfile.read())
+                pub_key = cast(EllipticCurvePublicKey, algo.from_jwk(keyfile.read()))
 
             with open(key_path(f"jwk_ec_key_{curve}.json")) as keyfile:
-                priv_key = algo.from_jwk(keyfile.read())
+                priv_key = cast(EllipticCurvePrivateKey, algo.from_jwk(keyfile.read()))
 
             signature = algo.sign(b"Hello World!", priv_key)
             assert algo.verify(b"Hello World!", pub_key, signature)
 
     @crypto_required
     def test_ec_jwk_fails_on_invalid_json(self):
         algo = ECAlgorithm(ECAlgorithm.SHA512)
@@ -226,106 +230,125 @@
         for curve in ("P-256", "P-384", "P-521", "secp256k1"):
             with pytest.raises(InvalidKeyError):
                 algo.from_jwk(
                     f'{{"kty": "EC", "crv": "{curve}", "x": "dGVzdA==", "y": "dGVzdA=="}}'
                 )
 
         # EC private key length invalid
-        for (curve, point) in valid_points.items():
+        for curve, point in valid_points.items():
             with pytest.raises(InvalidKeyError):
                 algo.from_jwk(
                     f'{{"kty": "EC", "crv": "{curve}", "x": "{point["x"]}", "y": "{point["y"]}", "d": "dGVzdA=="}}'
                 )
 
     @crypto_required
     def test_ec_private_key_to_jwk_works_with_from_jwk(self):
         algo = ECAlgorithm(ECAlgorithm.SHA256)
 
         with open(key_path("testkey_ec.priv")) as ec_key:
-            orig_key = algo.prepare_key(ec_key.read())
+            orig_key = cast(EllipticCurvePrivateKey, algo.prepare_key(ec_key.read()))
 
-        parsed_key = algo.from_jwk(algo.to_jwk(orig_key))
+        parsed_key = cast(EllipticCurvePrivateKey, algo.from_jwk(algo.to_jwk(orig_key)))
         assert parsed_key.private_numbers() == orig_key.private_numbers()
         assert (
             parsed_key.private_numbers().public_numbers
             == orig_key.private_numbers().public_numbers
         )
 
     @crypto_required
     def test_ec_public_key_to_jwk_works_with_from_jwk(self):
         algo = ECAlgorithm(ECAlgorithm.SHA256)
 
         with open(key_path("testkey_ec.pub")) as ec_key:
-            orig_key = algo.prepare_key(ec_key.read())
+            orig_key = cast(EllipticCurvePublicKey, algo.prepare_key(ec_key.read()))
 
-        parsed_key = algo.from_jwk(algo.to_jwk(orig_key))
+        parsed_key = cast(EllipticCurvePublicKey, algo.from_jwk(algo.to_jwk(orig_key)))
         assert parsed_key.public_numbers() == orig_key.public_numbers()
 
     @crypto_required
-    def test_ec_to_jwk_returns_correct_values_for_public_key(self):
+    @pytest.mark.parametrize("as_dict", (False, True))
+    def test_ec_to_jwk_returns_correct_values_for_public_key(self, as_dict):
         algo = ECAlgorithm(ECAlgorithm.SHA256)
 
         with open(key_path("testkey_ec.pub")) as keyfile:
             pub_key = algo.prepare_key(keyfile.read())
 
-        key = algo.to_jwk(pub_key)
+        key: Any = algo.to_jwk(pub_key, as_dict=as_dict)
+
+        if not as_dict:
+            key = json.loads(key)
 
         expected = {
             "kty": "EC",
             "crv": "P-256",
             "x": "HzAcUWSlGBHcuf3y3RiNrWI-pE6-dD2T7fIzg9t6wEc",
             "y": "t2G02kbWiOqimYfQAfnARdp2CTycsJPhwA8rn1Cn0SQ",
         }
 
-        assert json.loads(key) == expected
+        assert key == expected
 
     @crypto_required
-    def test_ec_to_jwk_returns_correct_values_for_private_key(self):
+    @pytest.mark.parametrize("as_dict", (False, True))
+    def test_ec_to_jwk_returns_correct_values_for_private_key(self, as_dict):
         algo = ECAlgorithm(ECAlgorithm.SHA256)
 
         with open(key_path("testkey_ec.priv")) as keyfile:
             priv_key = algo.prepare_key(keyfile.read())
 
-        key = algo.to_jwk(priv_key)
+        key: Any = algo.to_jwk(priv_key, as_dict=as_dict)
+
+        if not as_dict:
+            key = json.loads(key)
 
         expected = {
             "kty": "EC",
             "crv": "P-256",
             "x": "HzAcUWSlGBHcuf3y3RiNrWI-pE6-dD2T7fIzg9t6wEc",
             "y": "t2G02kbWiOqimYfQAfnARdp2CTycsJPhwA8rn1Cn0SQ",
             "d": "2nninfu2jMHDwAbn9oERUhRADS6duQaJEadybLaa0YQ",
         }
 
-        assert json.loads(key) == expected
+        assert key == expected
 
     @crypto_required
     def test_ec_to_jwk_raises_exception_on_invalid_key(self):
         algo = ECAlgorithm(ECAlgorithm.SHA256)
 
         with pytest.raises(InvalidKeyError):
-            algo.to_jwk({"not": "a valid key"})
+            algo.to_jwk({"not": "a valid key"})  # type: ignore[call-overload]
 
     @crypto_required
-    def test_ec_to_jwk_with_valid_curves(self):
+    @pytest.mark.parametrize("as_dict", (False, True))
+    def test_ec_to_jwk_with_valid_curves(self, as_dict):
         tests = {
             "P-256": ECAlgorithm.SHA256,
             "P-384": ECAlgorithm.SHA384,
             "P-521": ECAlgorithm.SHA512,
             "secp256k1": ECAlgorithm.SHA256,
         }
-        for (curve, hash) in tests.items():
+        for curve, hash in tests.items():
             algo = ECAlgorithm(hash)
 
             with open(key_path(f"jwk_ec_pub_{curve}.json")) as keyfile:
                 pub_key = algo.from_jwk(keyfile.read())
-                assert json.loads(algo.to_jwk(pub_key))["crv"] == curve
+                jwk: Any = algo.to_jwk(pub_key, as_dict=as_dict)
+
+                if not as_dict:
+                    jwk = json.loads(jwk)
+
+                assert jwk["crv"] == curve
 
             with open(key_path(f"jwk_ec_key_{curve}.json")) as keyfile:
                 priv_key = algo.from_jwk(keyfile.read())
-                assert json.loads(algo.to_jwk(priv_key))["crv"] == curve
+                jwk = algo.to_jwk(priv_key, as_dict=as_dict)
+
+                if not as_dict:
+                    jwk = json.loads(jwk)
+
+                assert jwk["crv"] == curve
 
     @crypto_required
     def test_ec_to_jwk_with_invalid_curve(self):
         algo = ECAlgorithm(ECAlgorithm.SHA256)
 
         with open(key_path("testkey_ec_secp192r1.priv")) as keyfile:
             priv_key = algo.prepare_key(keyfile.read())
@@ -334,44 +357,44 @@
             algo.to_jwk(priv_key)
 
     @crypto_required
     def test_rsa_jwk_public_and_private_keys_should_parse_and_verify(self):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with open(key_path("jwk_rsa_pub.json")) as keyfile:
-            pub_key = algo.from_jwk(keyfile.read())
+            pub_key = cast(RSAPublicKey, algo.from_jwk(keyfile.read()))
 
         with open(key_path("jwk_rsa_key.json")) as keyfile:
-            priv_key = algo.from_jwk(keyfile.read())
+            priv_key = cast(RSAPrivateKey, algo.from_jwk(keyfile.read()))
 
         signature = algo.sign(b"Hello World!", priv_key)
         assert algo.verify(b"Hello World!", pub_key, signature)
 
     @crypto_required
     def test_rsa_private_key_to_jwk_works_with_from_jwk(self):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with open(key_path("testkey_rsa.priv")) as rsa_key:
-            orig_key = algo.prepare_key(rsa_key.read())
+            orig_key = cast(RSAPrivateKey, algo.prepare_key(rsa_key.read()))
 
-        parsed_key = algo.from_jwk(algo.to_jwk(orig_key))
+        parsed_key = cast(RSAPrivateKey, algo.from_jwk(algo.to_jwk(orig_key)))
         assert parsed_key.private_numbers() == orig_key.private_numbers()
         assert (
             parsed_key.private_numbers().public_numbers
             == orig_key.private_numbers().public_numbers
         )
 
     @crypto_required
     def test_rsa_public_key_to_jwk_works_with_from_jwk(self):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with open(key_path("testkey_rsa.pub")) as rsa_key:
-            orig_key = algo.prepare_key(rsa_key.read())
+            orig_key = cast(RSAPublicKey, algo.prepare_key(rsa_key.read()))
 
-        parsed_key = algo.from_jwk(algo.to_jwk(orig_key))
+        parsed_key = cast(RSAPublicKey, algo.from_jwk(algo.to_jwk(orig_key)))
         assert parsed_key.public_numbers() == orig_key.public_numbers()
 
     @crypto_required
     def test_rsa_jwk_private_key_with_other_primes_is_invalid(self):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with open(key_path("jwk_rsa_key.json")) as keyfile:
@@ -394,22 +417,24 @@
 
     @crypto_required
     def test_rsa_jwk_private_key_can_recover_prime_factors(self):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with open(key_path("jwk_rsa_key.json")) as keyfile:
             keybytes = keyfile.read()
-            control_key = algo.from_jwk(keybytes).private_numbers()
+            control_key = cast(RSAPrivateKey, algo.from_jwk(keybytes)).private_numbers()
 
             keydata = json.loads(keybytes)
             delete_these = ["p", "q", "dp", "dq", "qi"]
             for field in delete_these:
                 del keydata[field]
 
-            parsed_key = algo.from_jwk(json.dumps(keydata)).private_numbers()
+            parsed_key = cast(
+                RSAPrivateKey, algo.from_jwk(json.dumps(keydata))
+            ).private_numbers()
 
         assert control_key.d == parsed_key.d
         assert control_key.p == parsed_key.p
         assert control_key.q == parsed_key.q
         assert control_key.dmp1 == parsed_key.dmp1
         assert control_key.dmq1 == parsed_key.dmq1
         assert control_key.iqmp == parsed_key.iqmp
@@ -434,45 +459,53 @@
             algo.from_jwk("{not-a-real-key")
 
         # Missing key parts
         with pytest.raises(InvalidKeyError):
             algo.from_jwk('{"kty": "RSA"}')
 
     @crypto_required
-    def test_rsa_to_jwk_returns_correct_values_for_public_key(self):
+    @pytest.mark.parametrize("as_dict", (False, True))
+    def test_rsa_to_jwk_returns_correct_values_for_public_key(self, as_dict):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with open(key_path("testkey_rsa.pub")) as keyfile:
             pub_key = algo.prepare_key(keyfile.read())
 
-        key = algo.to_jwk(pub_key)
+        key: Any = algo.to_jwk(pub_key, as_dict=as_dict)
+
+        if not as_dict:
+            key = json.loads(key)
 
         expected = {
             "e": "AQAB",
             "key_ops": ["verify"],
             "kty": "RSA",
             "n": (
                 "1HgzBfJv2cOjQryCwe8NEelriOTNFWKZUivevUrRhlqcmZJdCvuCJRr-xCN-"
                 "OmO8qwgJJR98feNujxVg-J9Ls3_UOA4HcF9nYH6aqVXELAE8Hk_ALvxi96ms"
                 "1DDuAvQGaYZ-lANxlvxeQFOZSbjkz_9mh8aLeGKwqJLp3p-OhUBQpwvAUAPg"
                 "82-OUtgTW3nSljjeFr14B8qAneGSc_wl0ni--1SRZUXFSovzcqQOkla3W27r"
                 "rLfrD6LXgj_TsDs4vD1PnIm1zcVenKT7TfYI17bsG_O_Wecwz2Nl19pL7gDo"
                 "sNruF3ogJWNq1Lyn_ijPQnkPLpZHyhvuiycYcI3DiQ"
             ),
         }
-        assert json.loads(key) == expected
+        assert key == expected
 
     @crypto_required
-    def test_rsa_to_jwk_returns_correct_values_for_private_key(self):
+    @pytest.mark.parametrize("as_dict", (False, True))
+    def test_rsa_to_jwk_returns_correct_values_for_private_key(self, as_dict):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with open(key_path("testkey_rsa.priv")) as keyfile:
             priv_key = algo.prepare_key(keyfile.read())
 
-        key = algo.to_jwk(priv_key)
+        key: Any = algo.to_jwk(priv_key, as_dict=as_dict)
+
+        if not as_dict:
+            key = json.loads(key)
 
         expected = {
             "key_ops": ["sign"],
             "kty": "RSA",
             "e": "AQAB",
             "n": (
                 "1HgzBfJv2cOjQryCwe8NEelriOTNFWKZUivevUrRhlqcmZJdCvuCJRr-xCN-"
@@ -512,37 +545,37 @@
             ),
             "dq": (
                 "xxCIuhD0YlWFbUcwFgGdBWcLIm_WCMGj7SB6aGu1VDTLr4Wu10TFWM0TNu"
                 "hc9YPker2gpj5qzAmdAzwcfWSSvXpJTYR43jfulBTMoj8-2o3wCM0anclW"
                 "AuKhin-kc4mh9ssDXRQZwlMymZP0QtaxUDw_nlfVrUCZgO7L1_ZsUTk"
             ),
         }
-        assert json.loads(key) == expected
+        assert key == expected
 
     @crypto_required
     def test_rsa_to_jwk_raises_exception_on_invalid_key(self):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with pytest.raises(InvalidKeyError):
-            algo.to_jwk({"not": "a valid key"})
+            algo.to_jwk({"not": "a valid key"})  # type: ignore[call-overload]
 
     @crypto_required
     def test_rsa_from_jwk_raises_exception_on_invalid_key(self):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with open(key_path("jwk_hmac.json")) as keyfile:
             with pytest.raises(InvalidKeyError):
                 algo.from_jwk(keyfile.read())
 
     @crypto_required
     def test_ec_should_reject_non_string_key(self):
         algo = ECAlgorithm(ECAlgorithm.SHA256)
 
         with pytest.raises(TypeError):
-            algo.prepare_key(None)
+            algo.prepare_key(None)  # type: ignore[arg-type]
 
     @crypto_required
     def test_ec_should_accept_pem_private_key_bytes(self):
         algo = ECAlgorithm(ECAlgorithm.SHA256)
 
         with open(key_path("testkey_ec.priv"), "rb") as ec_key:
             algo.prepare_key(ec_key.read())
@@ -604,19 +637,19 @@
     @crypto_required
     def test_rsa_pss_sign_then_verify_should_return_true(self):
         algo = RSAPSSAlgorithm(RSAPSSAlgorithm.SHA256)
 
         message = b"Hello World!"
 
         with open(key_path("testkey_rsa.priv")) as keyfile:
-            priv_key = algo.prepare_key(keyfile.read())
+            priv_key = cast(RSAPrivateKey, algo.prepare_key(keyfile.read()))
             sig = algo.sign(message, priv_key)
 
         with open(key_path("testkey_rsa.pub")) as keyfile:
-            pub_key = algo.prepare_key(keyfile.read())
+            pub_key = cast(RSAPublicKey, algo.prepare_key(keyfile.read()))
 
         result = algo.verify(message, pub_key, sig)
         assert result
 
     @crypto_required
     def test_rsa_pss_verify_should_return_false_if_signature_invalid(self):
         algo = RSAPSSAlgorithm(RSAPSSAlgorithm.SHA256)
@@ -631,15 +664,15 @@
             b"daOCWqbpZDuLb1imKpmm8Nsm56kAxijMLZnpCcnPgyb7CqG+B93W9GHglA5"
             b"drUeR1gRtO7vqbZMsCAQ4bpjXxwbYyjQlEVuMl73UL6sOWg=="
         )
 
         jwt_sig += b"123"  # Signature is now invalid
 
         with open(key_path("testkey_rsa.pub")) as keyfile:
-            jwt_pub_key = algo.prepare_key(keyfile.read())
+            jwt_pub_key = cast(RSAPublicKey, algo.prepare_key(keyfile.read()))
 
         result = algo.verify(jwt_message, jwt_pub_key, jwt_sig)
         assert not result
 
 
 class TestAlgorithmsRFC7520:
     """
@@ -692,15 +725,15 @@
             b"K3lfWRa-XtL0RnltuYv746iYTh_qHRD68BNt1uSNCrUCTJDt5aAE6x8wW1Kt9eRo4"
             b"QPocSadnHXFxnt8Is9UzpERV0ePPQdLuW3IS_de3xyIrDaLGdjluPxUAhb6L2aXic"
             b"1U12podGU0KLUQSE_oI-ZnmKJ3F4uOZDnd6QZWJushZ41Axf_fcIe8u9ipH84ogor"
             b"ee7vjbU5y18kDquDg"
         )
 
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
-        key = algo.prepare_key(load_rsa_pub_key())
+        key = cast(RSAPublicKey, algo.prepare_key(load_rsa_pub_key()))
 
         result = algo.verify(signing_input, key, signature)
         assert result
 
     @crypto_required
     def test_rsapss_verify_should_return_true_for_test_vector(self):
         """
@@ -723,15 +756,15 @@
             b"g-UD8biiReQFlfz28zGWVsdiNAUf8ZnyPEgVFn442ZdNqiVJRmBqrYRXe8P_ijQ7p"
             b"8Vdz0TTrxUeT3lm8d9shnr2lfJT8ImUjvAA2Xez2Mlp8cBE5awDzT0qI0n6uiP1aC"
             b"N_2_jLAeQTlqRHtfa64QQSUmFAAjVKPbByi7xho0uTOcbH510a6GYmJUAfmWjwZ6o"
             b"D4ifKo8DYM-X72Eaw"
         )
 
         algo = RSAPSSAlgorithm(RSAPSSAlgorithm.SHA384)
-        key = algo.prepare_key(load_rsa_pub_key())
+        key = cast(RSAPublicKey, algo.prepare_key(load_rsa_pub_key()))
 
         result = algo.verify(signing_input, key, signature)
         assert result
 
     @crypto_required
     def test_ec_verify_should_return_true_for_test_vector(self):
         """
@@ -773,40 +806,34 @@
     hello_world_sig = b"Qxa47mk/azzUgmY2StAOguAd4P7YBLpyCfU3JdbaiWnXM4o4WibXwmIHvNYgN3frtE2fcyd8OYEaOiD/KiwkCg=="
     hello_world = b"Hello World!"
 
     def test_okp_ed25519_should_reject_non_string_key(self):
         algo = OKPAlgorithm()
 
         with pytest.raises(InvalidKeyError):
-            algo.prepare_key(None)
+            algo.prepare_key(None)  # type: ignore[arg-type]
 
         with open(key_path("testkey_ed25519")) as keyfile:
             algo.prepare_key(keyfile.read())
 
         with open(key_path("testkey_ed25519.pub")) as keyfile:
             algo.prepare_key(keyfile.read())
 
-    def test_okp_ed25519_should_accept_unicode_key(self):
-        algo = OKPAlgorithm()
-
-        with open(key_path("testkey_ed25519")) as ec_key:
-            algo.prepare_key(ec_key.read())
-
     def test_okp_ed25519_sign_should_generate_correct_signature_value(self):
         algo = OKPAlgorithm()
 
         jwt_message = self.hello_world
 
         expected_sig = base64.b64decode(self.hello_world_sig)
 
         with open(key_path("testkey_ed25519")) as keyfile:
-            jwt_key = algo.prepare_key(keyfile.read())
+            jwt_key = cast(Ed25519PrivateKey, algo.prepare_key(keyfile.read()))
 
         with open(key_path("testkey_ed25519.pub")) as keyfile:
-            jwt_pub_key = algo.prepare_key(keyfile.read())
+            jwt_pub_key = cast(Ed25519PublicKey, algo.prepare_key(keyfile.read()))
 
         algo.sign(jwt_message, jwt_key)
         result = algo.verify(jwt_message, jwt_pub_key, expected_sig)
         assert result
 
     def test_okp_ed25519_verify_should_return_false_if_signature_invalid(self):
         algo = OKPAlgorithm()
@@ -843,53 +870,53 @@
 
         assert jwt_pub_key_first == jwt_pub_key_second
 
     def test_okp_ed25519_jwk_private_key_should_parse_and_verify(self):
         algo = OKPAlgorithm()
 
         with open(key_path("jwk_okp_key_Ed25519.json")) as keyfile:
-            key = algo.from_jwk(keyfile.read())
+            key = cast(Ed25519PrivateKey, algo.from_jwk(keyfile.read()))
 
         signature = algo.sign(b"Hello World!", key)
         assert algo.verify(b"Hello World!", key.public_key(), signature)
 
     def test_okp_ed25519_jwk_private_key_should_parse_and_verify_with_private_key_as_is(
         self,
     ):
         algo = OKPAlgorithm()
 
         with open(key_path("jwk_okp_key_Ed25519.json")) as keyfile:
-            key = algo.from_jwk(keyfile.read())
+            key = cast(Ed25519PrivateKey, algo.from_jwk(keyfile.read()))
 
         signature = algo.sign(b"Hello World!", key)
         assert algo.verify(b"Hello World!", key, signature)
 
     def test_okp_ed25519_jwk_public_key_should_parse_and_verify(self):
         algo = OKPAlgorithm()
 
         with open(key_path("jwk_okp_key_Ed25519.json")) as keyfile:
-            priv_key = algo.from_jwk(keyfile.read())
+            priv_key = cast(Ed25519PrivateKey, algo.from_jwk(keyfile.read()))
 
         with open(key_path("jwk_okp_pub_Ed25519.json")) as keyfile:
-            pub_key = algo.from_jwk(keyfile.read())
+            pub_key = cast(Ed25519PublicKey, algo.from_jwk(keyfile.read()))
 
         signature = algo.sign(b"Hello World!", priv_key)
         assert algo.verify(b"Hello World!", pub_key, signature)
 
     def test_okp_ed25519_jwk_fails_on_invalid_json(self):
         algo = OKPAlgorithm()
 
         with open(key_path("jwk_okp_pub_Ed25519.json")) as keyfile:
             valid_pub = json.loads(keyfile.read())
         with open(key_path("jwk_okp_key_Ed25519.json")) as keyfile:
             valid_key = json.loads(keyfile.read())
 
         # Invalid instance type
         with pytest.raises(InvalidKeyError):
-            algo.from_jwk(123)
+            algo.from_jwk(123)  # type: ignore[arg-type]
 
         # Invalid JSON
         with pytest.raises(InvalidKeyError):
             algo.from_jwk("<this isn't json>")
 
         # Invalid kty, not "OKP"
         v = valid_pub.copy()
@@ -923,82 +950,83 @@
 
         # Invalid d
         v = valid_key.copy()
         v["d"] = "123"
         with pytest.raises(InvalidKeyError):
             algo.from_jwk(v)
 
-    def test_okp_ed25519_to_jwk_works_with_from_jwk(self):
+    @pytest.mark.parametrize("as_dict", (False, True))
+    def test_okp_ed25519_to_jwk_works_with_from_jwk(self, as_dict):
         algo = OKPAlgorithm()
 
         with open(key_path("jwk_okp_key_Ed25519.json")) as keyfile:
-            priv_key_1 = algo.from_jwk(keyfile.read())
+            priv_key_1 = cast(Ed25519PrivateKey, algo.from_jwk(keyfile.read()))
 
         with open(key_path("jwk_okp_pub_Ed25519.json")) as keyfile:
-            pub_key_1 = algo.from_jwk(keyfile.read())
+            pub_key_1 = cast(Ed25519PublicKey, algo.from_jwk(keyfile.read()))
 
-        pub = algo.to_jwk(pub_key_1)
+        pub = algo.to_jwk(pub_key_1, as_dict=as_dict)
         pub_key_2 = algo.from_jwk(pub)
-        pri = algo.to_jwk(priv_key_1)
-        priv_key_2 = algo.from_jwk(pri)
+        pri = algo.to_jwk(priv_key_1, as_dict=as_dict)
+        priv_key_2 = cast(Ed25519PrivateKey, algo.from_jwk(pri))
 
         signature_1 = algo.sign(b"Hello World!", priv_key_1)
         signature_2 = algo.sign(b"Hello World!", priv_key_2)
         assert algo.verify(b"Hello World!", pub_key_2, signature_1)
         assert algo.verify(b"Hello World!", pub_key_2, signature_2)
 
     def test_okp_to_jwk_raises_exception_on_invalid_key(self):
         algo = OKPAlgorithm()
 
         with pytest.raises(InvalidKeyError):
-            algo.to_jwk({"not": "a valid key"})
+            algo.to_jwk({"not": "a valid key"})  # type: ignore[call-overload]
 
     def test_okp_ed448_jwk_private_key_should_parse_and_verify(self):
         algo = OKPAlgorithm()
 
         with open(key_path("jwk_okp_key_Ed448.json")) as keyfile:
-            key = algo.from_jwk(keyfile.read())
+            key = cast(Ed448PrivateKey, algo.from_jwk(keyfile.read()))
 
         signature = algo.sign(b"Hello World!", key)
         assert algo.verify(b"Hello World!", key.public_key(), signature)
 
     def test_okp_ed448_jwk_private_key_should_parse_and_verify_with_private_key_as_is(
         self,
     ):
         algo = OKPAlgorithm()
 
         with open(key_path("jwk_okp_key_Ed448.json")) as keyfile:
-            key = algo.from_jwk(keyfile.read())
+            key = cast(Ed448PrivateKey, algo.from_jwk(keyfile.read()))
 
         signature = algo.sign(b"Hello World!", key)
         assert algo.verify(b"Hello World!", key, signature)
 
     def test_okp_ed448_jwk_public_key_should_parse_and_verify(self):
         algo = OKPAlgorithm()
 
         with open(key_path("jwk_okp_key_Ed448.json")) as keyfile:
-            priv_key = algo.from_jwk(keyfile.read())
+            priv_key = cast(Ed448PrivateKey, algo.from_jwk(keyfile.read()))
 
         with open(key_path("jwk_okp_pub_Ed448.json")) as keyfile:
-            pub_key = algo.from_jwk(keyfile.read())
+            pub_key = cast(Ed448PublicKey, algo.from_jwk(keyfile.read()))
 
         signature = algo.sign(b"Hello World!", priv_key)
         assert algo.verify(b"Hello World!", pub_key, signature)
 
     def test_okp_ed448_jwk_fails_on_invalid_json(self):
         algo = OKPAlgorithm()
 
         with open(key_path("jwk_okp_pub_Ed448.json")) as keyfile:
             valid_pub = json.loads(keyfile.read())
         with open(key_path("jwk_okp_key_Ed448.json")) as keyfile:
             valid_key = json.loads(keyfile.read())
 
         # Invalid instance type
         with pytest.raises(InvalidKeyError):
-            algo.from_jwk(123)
+            algo.from_jwk(123)  # type: ignore[arg-type]
 
         # Invalid JSON
         with pytest.raises(InvalidKeyError):
             algo.from_jwk("<this isn't json>")
 
         # Invalid kty, not "OKP"
         v = valid_pub.copy()
@@ -1032,25 +1060,43 @@
 
         # Invalid d
         v = valid_key.copy()
         v["d"] = "123"
         with pytest.raises(InvalidKeyError):
             algo.from_jwk(v)
 
-    def test_okp_ed448_to_jwk_works_with_from_jwk(self):
+    @pytest.mark.parametrize("as_dict", (False, True))
+    def test_okp_ed448_to_jwk_works_with_from_jwk(self, as_dict):
         algo = OKPAlgorithm()
 
         with open(key_path("jwk_okp_key_Ed448.json")) as keyfile:
-            priv_key_1 = algo.from_jwk(keyfile.read())
+            priv_key_1 = cast(Ed448PrivateKey, algo.from_jwk(keyfile.read()))
 
         with open(key_path("jwk_okp_pub_Ed448.json")) as keyfile:
-            pub_key_1 = algo.from_jwk(keyfile.read())
+            pub_key_1 = cast(Ed448PublicKey, algo.from_jwk(keyfile.read()))
 
-        pub = algo.to_jwk(pub_key_1)
+        pub = algo.to_jwk(pub_key_1, as_dict=as_dict)
         pub_key_2 = algo.from_jwk(pub)
-        pri = algo.to_jwk(priv_key_1)
-        priv_key_2 = algo.from_jwk(pri)
+        pri = algo.to_jwk(priv_key_1, as_dict=as_dict)
+        priv_key_2 = cast(Ed448PrivateKey, algo.from_jwk(pri))
 
         signature_1 = algo.sign(b"Hello World!", priv_key_1)
         signature_2 = algo.sign(b"Hello World!", priv_key_2)
         assert algo.verify(b"Hello World!", pub_key_2, signature_1)
         assert algo.verify(b"Hello World!", pub_key_2, signature_2)
+
+    @crypto_required
+    def test_rsa_can_compute_digest(self):
+        # this is the well-known sha256 hash of "foo"
+        foo_hash = base64.b64decode(b"LCa0a2j/xo/5m0U8HTBBNBNCLXBkg7+g+YpeiGJm564=")
+
+        algo = RSAAlgorithm(RSAAlgorithm.SHA256)
+        computed_hash = algo.compute_hash_digest(b"foo")
+        assert computed_hash == foo_hash
+
+    def test_hmac_can_compute_digest(self):
+        # this is the well-known sha256 hash of "foo"
+        foo_hash = base64.b64decode(b"LCa0a2j/xo/5m0U8HTBBNBNCLXBkg7+g+YpeiGJm564=")
+
+        algo = HMACAlgorithm(HMACAlgorithm.SHA256)
+        computed_hash = algo.compute_hash_digest(b"foo")
+        assert computed_hash == foo_hash
```

### Comparing `PyJWT-2.6.0/tests/test_api_jwk.py` & `PyJWT-2.7.0/tests/test_api_jwk.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pytest
 
 from jwt.algorithms import has_crypto
 from jwt.api_jwk import PyJWK, PyJWKSet
 from jwt.exceptions import InvalidKeyError, PyJWKError, PyJWKSetError
 
-from .utils import crypto_required, key_path
+from .utils import crypto_required, key_path, no_crypto_required
 
 if has_crypto:
     from jwt.algorithms import ECAlgorithm, HMACAlgorithm, OKPAlgorithm, RSAAlgorithm
 
 
 class TestPyJWK:
     @crypto_required
@@ -53,123 +53,113 @@
 
         assert jwk.key_type == "RSA"
         assert jwk.key_id == "keyid-abc123"
         assert jwk.public_key_use == "sig"
 
     @crypto_required
     def test_should_load_key_without_alg_from_dict(self):
-
         with open(key_path("jwk_rsa_pub.json")) as keyfile:
             key_data = json.loads(keyfile.read())
 
         jwk = PyJWK.from_dict(key_data)
 
         assert jwk.key_type == "RSA"
         assert isinstance(jwk.Algorithm, RSAAlgorithm)
         assert jwk.Algorithm.hash_alg == RSAAlgorithm.SHA256
 
     @crypto_required
     def test_should_load_key_from_dict_with_algorithm(self):
-
         with open(key_path("jwk_rsa_pub.json")) as keyfile:
             key_data = json.loads(keyfile.read())
 
         jwk = PyJWK.from_dict(key_data, algorithm="RS256")
 
         assert jwk.key_type == "RSA"
         assert isinstance(jwk.Algorithm, RSAAlgorithm)
         assert jwk.Algorithm.hash_alg == RSAAlgorithm.SHA256
 
     @crypto_required
     def test_should_load_key_ec_p256_from_dict(self):
-
         with open(key_path("jwk_ec_pub_P-256.json")) as keyfile:
             key_data = json.loads(keyfile.read())
 
         jwk = PyJWK.from_dict(key_data)
 
         assert jwk.key_type == "EC"
         assert isinstance(jwk.Algorithm, ECAlgorithm)
         assert jwk.Algorithm.hash_alg == ECAlgorithm.SHA256
 
     @crypto_required
     def test_should_load_key_ec_p384_from_dict(self):
-
         with open(key_path("jwk_ec_pub_P-384.json")) as keyfile:
             key_data = json.loads(keyfile.read())
 
         jwk = PyJWK.from_dict(key_data)
 
         assert jwk.key_type == "EC"
         assert isinstance(jwk.Algorithm, ECAlgorithm)
         assert jwk.Algorithm.hash_alg == ECAlgorithm.SHA384
 
     @crypto_required
     def test_should_load_key_ec_p521_from_dict(self):
-
         with open(key_path("jwk_ec_pub_P-521.json")) as keyfile:
             key_data = json.loads(keyfile.read())
 
         jwk = PyJWK.from_dict(key_data)
 
         assert jwk.key_type == "EC"
         assert isinstance(jwk.Algorithm, ECAlgorithm)
         assert jwk.Algorithm.hash_alg == ECAlgorithm.SHA512
 
     @crypto_required
     def test_should_load_key_ec_secp256k1_from_dict(self):
-
         with open(key_path("jwk_ec_pub_secp256k1.json")) as keyfile:
             key_data = json.loads(keyfile.read())
 
         jwk = PyJWK.from_dict(key_data)
 
         assert jwk.key_type == "EC"
         assert isinstance(jwk.Algorithm, ECAlgorithm)
         assert jwk.Algorithm.hash_alg == ECAlgorithm.SHA256
 
     @crypto_required
     def test_should_load_key_hmac_from_dict(self):
-
         with open(key_path("jwk_hmac.json")) as keyfile:
             key_data = json.loads(keyfile.read())
 
         jwk = PyJWK.from_dict(key_data)
 
         assert jwk.key_type == "oct"
         assert isinstance(jwk.Algorithm, HMACAlgorithm)
         assert jwk.Algorithm.hash_alg == HMACAlgorithm.SHA256
 
     @crypto_required
     def test_should_load_key_hmac_without_alg_from_dict(self):
-
         with open(key_path("jwk_hmac.json")) as keyfile:
             key_data = json.loads(keyfile.read())
 
         del key_data["alg"]
         jwk = PyJWK.from_dict(key_data)
 
         assert jwk.key_type == "oct"
         assert isinstance(jwk.Algorithm, HMACAlgorithm)
         assert jwk.Algorithm.hash_alg == HMACAlgorithm.SHA256
 
     @crypto_required
     def test_should_load_key_okp_without_alg_from_dict(self):
-
         with open(key_path("jwk_okp_pub_Ed25519.json")) as keyfile:
             key_data = json.loads(keyfile.read())
 
         jwk = PyJWK.from_dict(key_data)
 
         assert jwk.key_type == "OKP"
         assert isinstance(jwk.Algorithm, OKPAlgorithm)
 
     @crypto_required
     def test_from_dict_should_throw_exception_if_arg_is_invalid(self):
-
         with open(key_path("jwk_rsa_pub.json")) as keyfile:
             valid_rsa_pub = json.loads(keyfile.read())
         with open(key_path("jwk_ec_pub_P-256.json")) as keyfile:
             valid_ec_pub = json.loads(keyfile.read())
         with open(key_path("jwk_okp_pub_Ed25519.json")) as keyfile:
             valid_okp_pub = json.loads(keyfile.read())
 
@@ -203,14 +193,20 @@
 
         # Missing OKP crv
         v = valid_okp_pub.copy()
         del v["crv"]
         with pytest.raises(InvalidKeyError):
             PyJWK.from_dict(v)
 
+    @no_crypto_required
+    def test_missing_crypto_library_good_error_message(self):
+        with pytest.raises(PyJWKError) as exc:
+            PyJWK({"kty": "dummy"}, algorithm="RS256")
+            assert "cryptography" in str(exc.value)
+
 
 @crypto_required
 class TestPyJWKSet:
     def test_should_load_keys_from_jwk_data_dict(self):
         algo = RSAAlgorithm(RSAAlgorithm.SHA256)
 
         with open(key_path("jwk_rsa_pub.json")) as keyfile:
@@ -289,14 +285,14 @@
             jwks = json.loads(jwks_text)
             assert len(jwks.get("keys")) == 1
             with pytest.raises(PyJWKSetError):
                 _ = PyJWKSet.from_json(jwks_text)
 
     def test_invalid_keys_list(self):
         with pytest.raises(PyJWKSetError) as err:
-            PyJWKSet(keys="string")
+            PyJWKSet(keys="string")  # type: ignore
         assert str(err.value) == "Invalid JWK Set value"
 
     def test_empty_keys_list(self):
         with pytest.raises(PyJWKSetError) as err:
             PyJWKSet(keys=[])
         assert str(err.value) == "The JWK Set did not contain any keys"
```

### Comparing `PyJWT-2.6.0/tests/test_api_jws.py` & `PyJWT-2.7.0/tests/test_api_jws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from decimal import Decimal
 
 import pytest
 
-from jwt.algorithms import Algorithm, has_crypto
+from jwt.algorithms import NoneAlgorithm, has_crypto
 from jwt.api_jws import PyJWS
 from jwt.exceptions import (
     DecodeError,
     InvalidAlgorithmError,
     InvalidSignatureError,
     InvalidTokenError,
 )
@@ -35,18 +35,18 @@
 def payload():
     """Creates a sample jws claimset for use as a payload during tests"""
     return b"hello world"
 
 
 class TestJWS:
     def test_register_algo_does_not_allow_duplicate_registration(self, jws):
-        jws.register_algorithm("AAA", Algorithm())
+        jws.register_algorithm("AAA", NoneAlgorithm())
 
         with pytest.raises(ValueError):
-            jws.register_algorithm("AAA", Algorithm())
+            jws.register_algorithm("AAA", NoneAlgorithm())
 
     def test_register_algo_rejects_non_algorithm_obj(self, jws):
         with pytest.raises(TypeError):
             jws.register_algorithm("AAA123", {})
 
     def test_unregister_algo_removes_algorithm(self, jws):
         supported = jws.get_algorithms()
@@ -78,15 +78,15 @@
     def test_non_object_options_dont_persist(self, jws, payload):
         token = jws.encode(payload, "secret")
 
         jws.decode(token, "secret", options={"verify_signature": False})
 
         assert jws.options["verify_signature"]
 
-    def test_options_must_be_dict(self, jws):
+    def test_options_must_be_dict(self):
         pytest.raises(TypeError, PyJWS, options=object())
         pytest.raises((TypeError, ValueError), PyJWS, options=("something"))
 
     def test_encode_decode(self, jws, payload):
         secret = "secret"
         jws_message = jws.encode(payload, secret, algorithm="HS256")
         decoded_payload = jws.decode(jws_message, secret, algorithms=["HS256"])
@@ -154,15 +154,14 @@
         with pytest.raises(DecodeError) as context:
             jws.decode(example_jws, secret, algorithms=["HS256"])
 
         exception = context.value
         assert str(exception) == "Invalid header string: must be a json object"
 
     def test_encode_algorithm_param_should_be_case_sensitive(self, jws, payload):
-
         jws.encode(payload, "secret", algorithm="HS256")
 
         with pytest.raises(NotImplementedError) as context:
             jws.encode(payload, None, algorithm="hs256")
 
         exception = context.value
         assert str(exception) == "Algorithm not supported"
@@ -410,14 +409,25 @@
         secret = b"\xc2"  # char value that ascii codec cannot decode
         jws_message = jws.encode(payload, secret)
 
         decoded_payload = jws.decode(jws_message, secret, algorithms=["HS256"])
 
         assert decoded_payload == payload
 
+    @pytest.mark.parametrize("sort_headers", (False, True))
+    def test_sorting_of_headers(self, jws, payload, sort_headers):
+        jws_message = jws.encode(
+            payload,
+            key="\xc2",
+            headers={"b": "1", "a": "2"},
+            sort_headers=sort_headers,
+        )
+        header_json = base64url_decode(jws_message.split(".")[0])
+        assert sort_headers == (header_json.index(b'"a"') < header_json.index(b'"b"'))
+
     def test_decode_invalid_header_padding(self, jws):
         example_jws = (
             "aeyJhbGciOiAiSFMyNTYiLCAidHlwIjogIkpXVCJ9"
             ".eyJoZWxsbyI6ICJ3b3JsZCJ9"
             ".tvagLDLoaiJKxOKqpBXSEGy7SYSifZhjntgm9ctpyj8"
         )
         example_secret = "secret"
@@ -519,19 +529,19 @@
 
         with open(key_path("testkey_rsa.pub"), "rb") as rsa_pub_file:
             pub_rsakey = load_ssh_public_key(rsa_pub_file.read())
             jws.decode(jws_message, pub_rsakey, algorithms=[algo])
 
         # string-formatted key
         with open(key_path("testkey_rsa.priv")) as rsa_priv_file:
-            priv_rsakey = rsa_priv_file.read()
+            priv_rsakey = rsa_priv_file.read()  # type: ignore[assignment]
             jws_message = jws.encode(payload, priv_rsakey, algorithm=algo)
 
         with open(key_path("testkey_rsa.pub")) as rsa_pub_file:
-            pub_rsakey = rsa_pub_file.read()
+            pub_rsakey = rsa_pub_file.read()  # type: ignore[assignment]
             jws.decode(jws_message, pub_rsakey, algorithms=[algo])
 
     def test_rsa_related_algorithms(self, jws):
         jws = PyJWS()
         jws_algorithms = jws.get_algorithms()
 
         if has_crypto:
@@ -568,19 +578,19 @@
 
         with open(key_path("testkey_ec.pub"), "rb") as ec_pub_file:
             pub_eckey = load_pem_public_key(ec_pub_file.read())
             jws.decode(jws_message, pub_eckey, algorithms=[algo])
 
         # string-formatted key
         with open(key_path("testkey_ec.priv")) as ec_priv_file:
-            priv_eckey = ec_priv_file.read()
+            priv_eckey = ec_priv_file.read()  # type: ignore[assignment]
             jws_message = jws.encode(payload, priv_eckey, algorithm=algo)
 
         with open(key_path("testkey_ec.pub")) as ec_pub_file:
-            pub_eckey = ec_pub_file.read()
+            pub_eckey = ec_pub_file.read()  # type: ignore[assignment]
             jws.decode(jws_message, pub_eckey, algorithms=[algo])
 
     def test_ecdsa_related_algorithms(self, jws):
         jws = PyJWS()
         jws_algorithms = jws.get_algorithms()
 
         if has_crypto:
```

### Comparing `PyJWT-2.6.0/tests/test_api_jwt.py` & `PyJWT-2.7.0/tests/test_api_jwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,14 @@
                 algorithms=["HS256"],
             )
 
         exception = context.value
         assert str(exception) == "Invalid claim format in token"
 
     def test_encode_bad_type(self, jwt):
-
         types = ["string", tuple(), list(), 42, set()]
 
         for t in types:
             pytest.raises(
                 TypeError,
                 lambda: jwt.encode(t, "secret", algorithms=["HS256"]),
             )
@@ -223,14 +222,21 @@
         payload["iat"] = utc_timestamp() + 10
         secret = "secret"
         jwt_message = jwt.encode(payload, secret)
 
         with pytest.raises(ImmatureSignatureError):
             jwt.decode(jwt_message, secret, algorithms=["HS256"])
 
+    def test_decode_works_if_iat_is_str_of_a_number(self, jwt, payload):
+        payload["iat"] = "1638202770"
+        secret = "secret"
+        jwt_message = jwt.encode(payload, secret)
+        data = jwt.decode(jwt_message, secret, algorithms=["HS256"])
+        assert data["iat"] == "1638202770"
+
     def test_decode_raises_exception_if_nbf_is_not_int(self, jwt):
         # >>> jwt.encode({'nbf': 'not-an-int'}, 'secret')
         example_jwt = (
             "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9."
             "eyJuYmYiOiJub3QtYW4taW50In0."
             "c25hldC8G2ZamC8uKpax9sYMTgdZo3cxrmzFHaAAluw"
         )
@@ -355,16 +361,16 @@
         )
 
     def test_decode_with_expiration_with_leeway(self, jwt, payload):
         payload["exp"] = utc_timestamp() - 2
         secret = "secret"
         jwt_message = jwt.encode(payload, secret)
 
-        # With 3 seconds leeway, should be ok
-        for leeway in (3, timedelta(seconds=3)):
+        # With 5 seconds leeway, should be ok
+        for leeway in (5, timedelta(seconds=5)):
             decoded = jwt.decode(
                 jwt_message, secret, leeway=leeway, algorithms=["HS256"]
             )
             assert decoded == payload
 
         # With 1 seconds, should fail
         for leeway in (1, timedelta(seconds=1)):
```

### Comparing `PyJWT-2.6.0/tests/test_jwks_client.py` & `PyJWT-2.7.0/tests/test_jwks_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from urllib.error import URLError
 
 import pytest
 
 import jwt
 from jwt import PyJWKClient
 from jwt.api_jwk import PyJWK
-from jwt.exceptions import PyJWKClientError
+from jwt.exceptions import PyJWKClientConnectionError, PyJWKClientError
 
 from .utils import crypto_required
 
 RESPONSE_DATA_WITH_MATCHING_KID = {
     "keys": [
         {
             "alg": "RS256",
@@ -74,16 +74,36 @@
             json.dumps(response_data_one),
             json.dumps(response_data_two),
         ]
         urlopen_mock.return_value = response
         yield urlopen_mock
 
 
+@contextlib.contextmanager
+def mocked_timeout():
+    with mock.patch("urllib.request.urlopen") as urlopen_mock:
+        urlopen_mock.side_effect = TimeoutError("timed out")
+        yield urlopen_mock
+
+
 @crypto_required
 class TestPyJWKClient:
+    def test_fetch_data_forwards_headers_to_correct_url(self):
+        url = "https://dev-87evx9ru.auth0.com/.well-known/jwks.json"
+
+        with mocked_success_response(RESPONSE_DATA_WITH_MATCHING_KID) as mock_request:
+            custom_headers = {"User-agent": "my-custom-agent"}
+            jwks_client = PyJWKClient(url, headers=custom_headers)
+            jwk_set = jwks_client.get_jwk_set()
+            request_params = mock_request.call_args[0][0]
+            assert request_params.full_url == url
+            assert request_params.headers == custom_headers
+
+        assert len(jwk_set.keys) == 1
+
     def test_get_jwk_set(self):
         url = "https://dev-87evx9ru.auth0.com/.well-known/jwks.json"
 
         with mocked_success_response(RESPONSE_DATA_WITH_MATCHING_KID):
             jwks_client = PyJWKClient(url)
             jwk_set = jwks_client.get_jwk_set()
 
@@ -259,14 +279,23 @@
 
         with pytest.raises(PyJWKClientError):
             with mocked_failed_response():
                 jwks_client.get_jwk_set(refresh=True)
 
             assert jwks_client.jwk_set_cache is None
 
+    def test_failed_request_should_raise_connection_error(self):
+        token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImtpZCI6Ik5FRTFRVVJCT1RNNE16STVSa0ZETlRZeE9UVTFNRGcyT0Rnd1EwVXpNVGsxUWpZeVJrUkZRdyJ9.eyJpc3MiOiJodHRwczovL2Rldi04N2V2eDlydS5hdXRoMC5jb20vIiwic3ViIjoiYVc0Q2NhNzl4UmVMV1V6MGFFMkg2a0QwTzNjWEJWdENAY2xpZW50cyIsImF1ZCI6Imh0dHBzOi8vZXhwZW5zZXMtYXBpIiwiaWF0IjoxNTcyMDA2OTU0LCJleHAiOjE1NzIwMDY5NjQsImF6cCI6ImFXNENjYTc5eFJlTFdVejBhRTJINmtEME8zY1hCVnRDIiwiZ3R5IjoiY2xpZW50LWNyZWRlbnRpYWxzIn0.PUxE7xn52aTCohGiWoSdMBZGiYAHwE5FYie0Y1qUT68IHSTXwXVd6hn02HTah6epvHHVKA2FqcFZ4GGv5VTHEvYpeggiiZMgbxFrmTEY0csL6VNkX1eaJGcuehwQCRBKRLL3zKmA5IKGy5GeUnIbpPHLHDxr-GXvgFzsdsyWlVQvPX2xjeaQ217r2PtxDeqjlf66UYl6oY6AqNS8DH3iryCvIfCcybRZkc_hdy-6ZMoKT6Piijvk_aXdm7-QQqKJFHLuEqrVSOuBqqiNfVrG27QzAPuPOxvfXTVLXL2jek5meH6n-VWgrBdoMFH93QEszEDowDAEhQPHVs0xj7SIzA"
+        url = "https://dev-87evx9ru.auth0.com/.well-known/jwks.json"
+
+        jwks_client = PyJWKClient(url)
+        with pytest.raises(PyJWKClientConnectionError):
+            with mocked_failed_response():
+                jwks_client.get_signing_key_from_jwt(token)
+
     def test_get_jwt_set_refresh_cache(self):
         url = "https://dev-87evx9ru.auth0.com/.well-known/jwks.json"
         jwks_client = PyJWKClient(url)
 
         kid = "NEE1QURBOTM4MzI5RkFDNTYxOTU1MDg2ODgwQ0UzMTk1QjYyRkRFQw"
 
         # The first call will return response with no matching kid,
@@ -292,7 +321,17 @@
 
     def test_get_jwt_set_invalid_lifespan(self):
         url = "https://dev-87evx9ru.auth0.com/.well-known/jwks.json"
 
         with pytest.raises(PyJWKClientError):
             jwks_client = PyJWKClient(url, lifespan=-1)
             assert jwks_client is None
+
+    def test_get_jwt_set_timeout(self):
+        url = "https://dev-87evx9ru.auth0.com/.well-known/jwks.json"
+        jwks_client = PyJWKClient(url, timeout=5)
+
+        with pytest.raises(PyJWKClientError) as exc:
+            with mocked_timeout():
+                jwks_client.get_jwk_set()
+
+        assert 'Fail to fetch data from the url, err: "timed out"' in str(exc.value)
```

### Comparing `PyJWT-2.6.0/tests/test_jwt.py` & `PyJWT-2.7.0/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/tests/test_utils.py` & `PyJWT-2.7.0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 def test_from_base64url_uint(inputval, expected):
     actual = from_base64url_uint(inputval)
     assert actual == expected
 
 
 def test_force_bytes_raises_error_on_invalid_object():
     with pytest.raises(TypeError):
-        force_bytes({})
+        force_bytes({})  # type: ignore[arg-type]
```

### Comparing `PyJWT-2.6.0/tests/utils.py` & `PyJWT-2.7.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.6.0/tox.ini` & `PyJWT-2.7.0/tox.ini`

 * *Files identical despite different names*

