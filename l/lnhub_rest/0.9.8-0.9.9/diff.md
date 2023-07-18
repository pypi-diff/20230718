# Comparing `tmp/lnhub_rest-0.9.8.tar.gz` & `tmp/lnhub_rest-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnhub_rest-0.9.8.tar", last modified: Sun May 28 13:31:31 2023, max compression
+gzip compressed data, was "lnhub_rest-0.9.9.tar", last modified: Sun Jun  4 17:58:31 2023, max compression
```

## Comparing `lnhub_rest-0.9.8.tar` & `lnhub_rest-0.9.9.tar`

### file list

```diff
@@ -1,201 +1,122 @@
--rw-r--r--   0        0        0     1259 2023-01-15 12:17:52.329263 lnhub_rest-0.9.8/.dockerignore
--rw-r--r--   0        0        0     3245 2023-05-25 20:34:20.149969 lnhub_rest-0.9.8/.github/workflows/build.yml
--rw-r--r--   0        0        0     5417 2023-05-25 20:34:20.150136 lnhub_rest-0.9.8/.github/workflows/google-cloudrun-docker-prod.yml
--rw-r--r--   0        0        0     5426 2023-05-25 20:34:20.150292 lnhub_rest-0.9.8/.github/workflows/google-cloudrun-docker-staging.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:17:52.329501 lnhub_rest-0.9.8/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      613 2023-04-18 16:02:04.937767 lnhub_rest-0.9.8/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1212 2023-04-18 16:02:04.938015 lnhub_rest-0.9.8/.gitignore
--rw-r--r--   0        0        0       73 2023-04-18 16:02:04.938253 lnhub_rest-0.9.8/.gitmodules
--rw-r--r--   0        0        0     1772 2023-04-18 16:02:04.938593 lnhub_rest-0.9.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      157 2023-04-18 16:02:04.938840 lnhub_rest-0.9.8/Dockerfile
--rw-r--r--   0        0        0     2442 2023-04-25 15:29:32.847024 lnhub_rest-0.9.8/README.md
--rw-r--r--   0        0        0     1680 2023-04-27 03:39:31.402324 lnhub_rest-0.9.8/docs/00-migrate.ipynb
--rw-r--r--   0        0        0     1189 2023-04-27 03:39:31.402860 lnhub_rest-0.9.8/docs/01-checks/01-check-break-lndb.ipynb
--rw-r--r--   0        0        0     4487 2023-04-27 03:39:31.414955 lnhub_rest-0.9.8/docs/02-account/02-create-account.ipynb
--rw-r--r--   0        0        0     5566 2023-04-27 03:39:31.419067 lnhub_rest-0.9.8/docs/02-account/03-update-account.ipynb
--rw-r--r--   0        0        0     6111 2023-04-27 03:39:31.418992 lnhub_rest-0.9.8/docs/02-account/04-fetch-account.ipynb
--rw-r--r--   0        0        0     9088 2023-04-27 03:39:31.419398 lnhub_rest-0.9.8/docs/02-account/05-rls.ipynb
--rw-r--r--   0        0        0    11110 2023-04-27 04:21:53.504972 lnhub_rest-0.9.8/docs/03-instance/01-init-instance.ipynb
--rw-r--r--   0        0        0     5293 2023-04-27 03:39:31.415575 lnhub_rest-0.9.8/docs/03-instance/02-load-instance.ipynb
--rw-r--r--   0        0        0     6498 2023-04-27 03:39:31.417147 lnhub_rest-0.9.8/docs/03-instance/03-update-instance.ipynb
--rw-r--r--   0        0        0     8667 2023-04-27 03:39:31.417306 lnhub_rest-0.9.8/docs/03-instance/04-delete-instance.ipynb
--rw-r--r--   0        0        0     7001 2023-04-27 03:39:31.420904 lnhub_rest-0.9.8/docs/03-instance/05-fetch-instance.ipynb
--rw-r--r--   0        0        0    19423 2023-04-27 03:39:31.401299 lnhub_rest-0.9.8/docs/03-instance/06-rls.ipynb
--rw-r--r--   0        0        0     3990 2023-04-27 04:21:53.505189 lnhub_rest-0.9.8/docs/04-storage/01-add-storage.ipynb
--rw-r--r--   0        0        0     9837 2023-04-27 03:39:31.421340 lnhub_rest-0.9.8/docs/04-storage/02-rls.ipynb
--rw-r--r--   0        0        0     3894 2023-04-27 03:39:31.415314 lnhub_rest-0.9.8/docs/05-organization/01-create-organization.ipynb
--rw-r--r--   0        0        0     4749 2023-04-27 03:39:31.413247 lnhub_rest-0.9.8/docs/05-organization/02-manage-members.ipynb
--rw-r--r--   0        0        0     5892 2023-04-27 03:39:31.413014 lnhub_rest-0.9.8/docs/05-organization/03-rls.ipynb
--rw-r--r--   0        0        0     5310 2023-04-27 03:39:31.417221 lnhub_rest-0.9.8/docs/06-integration/01-signup-signin.ipynb
--rw-r--r--   0        0        0      125 2023-04-18 16:52:57.348114 lnhub_rest-0.9.8/docs/README.md
--rw-r--r--   0        0        0    25029 2023-05-28 13:31:14.587869 lnhub_rest-0.9.8/docs/changelog.md
--rw-r--r--   0        0        0      520 2023-04-18 16:02:04.943225 lnhub_rest-0.9.8/docs/migrations.md
--rw-r--r--   0        0        0      162 2023-04-18 16:02:04.943589 lnhub_rest-0.9.8/docs/notes/index.md
--rw-r--r--   0        0        0    26418 2023-04-18 16:02:04.943698 lnhub_rest-0.9.8/docs/notes/multiple-sign-ups-same-email.ipynb
--rw-r--r--   0        0        0      137 2023-01-15 12:17:52.330365 lnhub_rest-0.9.8/lamin-project.yaml
--rw-r--r--   0        0        0     3832 2023-04-18 16:53:14.549682 lnhub_rest-0.9.8/lndb/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-14 19:46:06.422201 lnhub_rest-0.9.8/lndb/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-14 19:46:06.422302 lnhub_rest-0.9.8/lndb/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-03-14 19:46:06.422406 lnhub_rest-0.9.8/lndb/.gitignore
--rw-r--r--   0        0        0     1777 2023-04-25 15:29:40.845175 lnhub_rest-0.9.8/lndb/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-14 19:46:06.422598 lnhub_rest-0.9.8/lndb/LICENSE
--rw-r--r--   0        0        0      173 2023-04-18 16:53:14.549987 lnhub_rest-0.9.8/lndb/README.md
--rw-r--r--   0        0        0       52 2023-03-14 19:46:06.422755 lnhub_rest-0.9.8/lndb/docs/api.md
--rw-r--r--   0        0        0    47755 2023-04-27 03:47:05.803728 lnhub_rest-0.9.8/lndb/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-14 19:46:06.423210 lnhub_rest-0.9.8/lndb/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-14 19:46:06.423317 lnhub_rest-0.9.8/lndb/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-04-18 16:53:14.550717 lnhub_rest-0.9.8/lndb/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-04-18 16:53:14.551192 lnhub_rest-0.9.8/lndb/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-25 15:29:40.845949 lnhub_rest-0.9.8/lndb/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-14 19:46:06.423689 lnhub_rest-0.9.8/lndb/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-18 16:53:14.551375 lnhub_rest-0.9.8/lndb/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-18 16:53:14.551472 lnhub_rest-0.9.8/lndb/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-18 16:53:14.551612 lnhub_rest-0.9.8/lndb/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    10370 2023-04-27 04:20:38.053396 lnhub_rest-0.9.8/lndb/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5355 2023-04-25 15:29:40.846776 lnhub_rest-0.9.8/lndb/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     6390 2023-04-25 15:29:40.846861 lnhub_rest-0.9.8/lndb/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3746 2023-04-25 15:29:40.846961 lnhub_rest-0.9.8/lndb/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-04-18 16:53:14.552137 lnhub_rest-0.9.8/lndb/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     2689 2023-04-25 15:29:40.847226 lnhub_rest-0.9.8/lndb/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-03-14 19:46:06.424331 lnhub_rest-0.9.8/lndb/docs/guide/index.md
--rw-r--r--   0        0        0     3158 2023-04-25 15:29:40.847416 lnhub_rest-0.9.8/lndb/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-03-14 19:46:06.424475 lnhub_rest-0.9.8/lndb/docs/index.md
--rw-r--r--   0        0        0      118 2023-03-14 19:46:06.424531 lnhub_rest-0.9.8/lndb/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-04-27 03:47:05.803990 lnhub_rest-0.9.8/lndb/lndb/__init__.py
--rw-r--r--   0        0        0     4507 2023-04-25 15:29:40.847751 lnhub_rest-0.9.8/lndb/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-03-14 19:46:06.424805 lnhub_rest-0.9.8/lndb/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-18 16:53:14.553281 lnhub_rest-0.9.8/lndb/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-04-25 15:29:40.847842 lnhub_rest-0.9.8/lndb/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-18 16:53:14.553610 lnhub_rest-0.9.8/lndb/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-18 16:53:14.553765 lnhub_rest-0.9.8/lndb/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-04-25 15:29:40.848070 lnhub_rest-0.9.8/lndb/lndb/_info.py
--rw-r--r--   0        0        0     6035 2023-04-27 03:52:24.150379 lnhub_rest-0.9.8/lndb/lndb/_init_instance.py
--rw-r--r--   0        0        0     6485 2023-04-27 03:49:23.883095 lnhub_rest-0.9.8/lndb/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-18 16:53:14.554421 lnhub_rest-0.9.8/lndb/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-18 16:53:14.554545 lnhub_rest-0.9.8/lndb/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-04-25 15:29:40.848442 lnhub_rest-0.9.8/lndb/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7644 2023-04-25 15:29:40.848595 lnhub_rest-0.9.8/lndb/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-03-14 19:46:06.425623 lnhub_rest-0.9.8/lndb/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-04-25 15:29:40.848722 lnhub_rest-0.9.8/lndb/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-18 16:53:14.554944 lnhub_rest-0.9.8/lndb/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      803 2023-04-27 04:20:38.053795 lnhub_rest-0.9.8/lndb/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-03-14 19:46:06.425742 lnhub_rest-0.9.8/lndb/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-04-25 15:29:40.849016 lnhub_rest-0.9.8/lndb/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-18 21:34:53.593994 lnhub_rest-0.9.8/lndb/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-03-14 19:46:06.425940 lnhub_rest-0.9.8/lndb/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-03-14 19:46:06.426016 lnhub_rest-0.9.8/lndb/lndb/_settings_store.py
--rw-r--r--   0        0        0     3902 2023-04-25 15:29:40.849262 lnhub_rest-0.9.8/lndb/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-18 16:53:14.555545 lnhub_rest-0.9.8/lndb/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-04-18 16:53:14.555802 lnhub_rest-0.9.8/lndb/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-18 16:53:14.555956 lnhub_rest-0.9.8/lndb/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-03-14 19:46:06.426451 lnhub_rest-0.9.8/lndb/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-03-14 19:46:06.426542 lnhub_rest-0.9.8/lndb/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-18 16:53:14.556103 lnhub_rest-0.9.8/lndb/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8946 2023-04-27 03:49:23.883399 lnhub_rest-0.9.8/lndb/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-04-18 16:53:14.556382 lnhub_rest-0.9.8/lndb/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-03-14 19:46:06.426936 lnhub_rest-0.9.8/lndb/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-18 16:53:14.556505 lnhub_rest-0.9.8/lndb/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-03-14 19:46:06.427111 lnhub_rest-0.9.8/lndb/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-04-18 16:53:14.556633 lnhub_rest-0.9.8/lndb/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     7204 2023-04-25 15:29:40.849676 lnhub_rest-0.9.8/lndb/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-04-25 15:29:40.849829 lnhub_rest-0.9.8/lndb/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-03-14 19:46:06.427525 lnhub_rest-0.9.8/lndb/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-18 16:53:14.557004 lnhub_rest-0.9.8/lndb/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-18 16:53:14.557144 lnhub_rest-0.9.8/lndb/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-03-14 19:46:06.427862 lnhub_rest-0.9.8/lndb/lndb/test/_env.py
--rw-r--r--   0        0        0     3911 2023-04-27 03:52:24.153553 lnhub_rest-0.9.8/lndb/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-18 16:53:14.557417 lnhub_rest-0.9.8/lndb/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-03-14 19:46:06.428161 lnhub_rest-0.9.8/lndb/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-03-14 19:46:06.428239 lnhub_rest-0.9.8/lndb/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-18 16:53:14.557535 lnhub_rest-0.9.8/lndb/noxfile.py
--rw-r--r--   0        0        0     1396 2023-04-27 04:20:38.053974 lnhub_rest-0.9.8/lndb/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-18 16:53:14.557862 lnhub_rest-0.9.8/lndb/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-14 19:46:06.428637 lnhub_rest-0.9.8/lndb/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-18 16:53:14.558657 lnhub_rest-0.9.8/lndb/tests/test_notebooks.py
--rw-r--r--   0        0        0      157 2023-05-28 13:31:08.333660 lnhub_rest-0.9.8/lnhub_rest/__init__.py
--rw-r--r--   0        0        0     7054 2023-04-25 15:29:32.854635 lnhub_rest-0.9.8/lnhub_rest/__main__.py
--rw-r--r--   0        0        0       64 2023-01-15 12:17:52.330585 lnhub_rest-0.9.8/lnhub_rest/_assets/__init__.py
--rw-r--r--   0        0        0      706 2023-05-28 12:36:10.508939 lnhub_rest-0.9.8/lnhub_rest/_assets/_instances.py
--rw-r--r--   0        0        0     1109 2023-05-25 20:34:20.151651 lnhub_rest-0.9.8/lnhub_rest/_assets/_schemas.py
--rw-r--r--   0        0        0     1722 2023-04-18 16:02:04.946281 lnhub_rest-0.9.8/lnhub_rest/_check_breaks_lndb.py
--rw-r--r--   0        0        0     1260 2023-04-25 15:29:32.854787 lnhub_rest-0.9.8/lnhub_rest/_ci.py
--rw-r--r--   0        0        0     5726 2023-04-19 15:57:22.490723 lnhub_rest-0.9.8/lnhub_rest/_clean_ci.py
--rw-r--r--   0        0        0     1626 2023-05-28 12:14:52.784375 lnhub_rest-0.9.8/lnhub_rest/config.py
--rw-r--r--   0        0        0       42 2023-04-18 16:02:04.947562 lnhub_rest-0.9.8/lnhub_rest/core/__init__.py
--rw-r--r--   0        0        0      285 2023-04-18 16:02:04.947641 lnhub_rest-0.9.8/lnhub_rest/core/account/__init__.py
--rw-r--r--   0        0        0     2542 2023-04-21 10:12:34.724799 lnhub_rest-0.9.8/lnhub_rest/core/account/_create_account.py
--rw-r--r--   0        0        0     1062 2023-04-18 16:02:04.947805 lnhub_rest-0.9.8/lnhub_rest/core/account/_crud.py
--rw-r--r--   0        0        0      739 2023-04-19 15:57:22.491329 lnhub_rest-0.9.8/lnhub_rest/core/account/_delete_account.py
--rw-r--r--   0        0        0     3325 2023-04-19 15:57:22.491711 lnhub_rest-0.9.8/lnhub_rest/core/account/_signup_signin.py
--rw-r--r--   0        0        0     1423 2023-04-19 15:57:22.491949 lnhub_rest-0.9.8/lnhub_rest/core/account/_update_account.py
--rw-r--r--   0        0        0       38 2023-04-18 16:02:04.948381 lnhub_rest-0.9.8/lnhub_rest/core/collaborator/__init__.py
--rw-r--r--   0        0        0     3056 2023-04-25 15:29:32.855696 lnhub_rest-0.9.8/lnhub_rest/core/collaborator/_crud.py
--rw-r--r--   0        0        0      243 2023-04-18 16:02:04.948618 lnhub_rest-0.9.8/lnhub_rest/core/instance/__init__.py
--rw-r--r--   0        0        0     1651 2023-04-18 16:02:04.948683 lnhub_rest-0.9.8/lnhub_rest/core/instance/_crud.py
--rw-r--r--   0        0        0     1284 2023-04-19 15:57:22.492340 lnhub_rest-0.9.8/lnhub_rest/core/instance/_delete_instance.py
--rw-r--r--   0        0        0     6096 2023-04-27 04:21:53.505412 lnhub_rest-0.9.8/lnhub_rest/core/instance/_init_instance.py
--rw-r--r--   0        0        0     1532 2023-04-19 15:57:22.492860 lnhub_rest-0.9.8/lnhub_rest/core/instance/_load_instance.py
--rw-r--r--   0        0        0     1067 2023-04-19 15:57:22.493104 lnhub_rest-0.9.8/lnhub_rest/core/instance/_update_instance.py
--rw-r--r--   0        0        0       32 2023-04-18 16:02:04.949819 lnhub_rest-0.9.8/lnhub_rest/core/member/__init__.py
--rw-r--r--   0        0        0     2078 2023-04-18 16:02:04.949894 lnhub_rest-0.9.8/lnhub_rest/core/member/_crud.py
--rw-r--r--   0        0        0       80 2023-04-18 16:02:04.949960 lnhub_rest-0.9.8/lnhub_rest/core/storage/__init__.py
--rw-r--r--   0        0        0     3427 2023-05-28 12:14:52.784992 lnhub_rest-0.9.8/lnhub_rest/core/storage/_add_storage.py
--rw-r--r--   0        0        0     1167 2023-04-18 16:02:04.950097 lnhub_rest-0.9.8/lnhub_rest/core/storage/_crud.py
--rw-r--r--   0        0        0      849 2023-05-25 20:34:20.151769 lnhub_rest-0.9.8/lnhub_rest/main.py
--rw-r--r--   0        0        0       39 2023-04-19 15:57:22.493742 lnhub_rest-0.9.8/lnhub_rest/orm/__init__.py
--rw-r--r--   0        0        0      199 2023-04-25 15:29:32.856194 lnhub_rest-0.9.8/lnhub_rest/orm/_engine.py
--rw-r--r--   0        0        0     1968 2023-04-25 15:29:32.856453 lnhub_rest-0.9.8/lnhub_rest/orm/_sbclient.py
--rw-r--r--   0        0        0      239 2023-05-25 20:34:20.152255 lnhub_rest-0.9.8/lnhub_rest/routers/__init__.py
--rw-r--r--   0        0        0     4661 2023-04-25 15:29:32.856734 lnhub_rest-0.9.8/lnhub_rest/routers/account.py
--rw-r--r--   0        0        0      538 2023-04-18 16:02:04.951096 lnhub_rest-0.9.8/lnhub_rest/routers/ci.py
--rw-r--r--   0        0        0     2313 2023-05-25 20:34:20.152366 lnhub_rest-0.9.8/lnhub_rest/routers/collaborator.py
--rw-r--r--   0        0        0      408 2023-04-18 16:02:04.951160 lnhub_rest-0.9.8/lnhub_rest/routers/dev.py
--rw-r--r--   0        0        0     5233 2023-04-25 15:29:32.856998 lnhub_rest-0.9.8/lnhub_rest/routers/instance.py
--rw-r--r--   0        0        0     2617 2023-04-18 16:02:04.951432 lnhub_rest-0.9.8/lnhub_rest/routers/organization.py
--rw-r--r--   0        0        0     1074 2023-04-19 15:57:22.494317 lnhub_rest-0.9.8/lnhub_rest/routers/utils.py
--rw-r--r--   0        0        0      249 2023-04-18 16:02:04.952299 lnhub_rest-0.9.8/lnhub_rest/schema/__init__.py
--rw-r--r--   0        0        0     4986 2023-04-18 16:02:04.952431 lnhub_rest-0.9.8/lnhub_rest/schema/_core.py
--rw-r--r--   0        0        0      270 2023-02-15 16:43:38.796706 lnhub_rest-0.9.8/lnhub_rest/schema/_timestamps.py
--rw-r--r--   0        0        0      262 2023-04-18 16:02:04.952506 lnhub_rest-0.9.8/lnhub_rest/schema/_type.py
--rw-r--r--   0        0        0      252 2023-02-15 16:43:38.796850 lnhub_rest-0.9.8/lnhub_rest/schema/_users.py
--rw-r--r--   0        0        0     1079 2023-04-18 16:02:04.952789 lnhub_rest-0.9.8/lnhub_rest/schema/_versions.py
--rw-r--r--   0        0        0      674 2023-04-18 16:01:55.110061 lnhub_rest-0.9.8/lnhub_rest/schema/alembic.ini
--rw-r--r--   0        0        0       40 2023-04-25 15:29:32.857365 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/__init__.py
--rw-r--r--   0        0        0     6020 2023-04-18 16:02:04.953355 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/clone.py
--rw-r--r--   0        0        0     3033 2023-04-25 15:29:32.857603 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/env.py
--rw-r--r--   0        0        0     1193 2023-04-18 16:02:04.953923 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0     1319 2023-04-18 16:02:04.953987 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1667 2023-04-18 16:02:04.954047 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0       39 2023-04-18 16:02:04.954171 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/__init__.py
--rw-r--r--   0        0        0     3940 2023-04-18 16:02:04.954327 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0      639 2023-04-18 16:02:04.954391 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
--rw-r--r--   0        0        0      214 2023-04-18 16:02:04.954454 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
--rw-r--r--   0        0        0      192 2023-04-18 16:02:04.954511 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
--rw-r--r--   0        0        0     7619 2023-04-18 16:02:04.954572 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1408 2023-04-18 16:02:04.954855 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0      880 2023-04-18 16:02:04.955067 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
--rw-r--r--   0        0        0       33 2023-04-18 16:02:04.955245 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/__init__.py
--rw-r--r--   0        0        0      542 2023-01-15 12:17:52.331616 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/script.py.mako
--rw-r--r--   0        0        0     5258 2023-04-25 15:29:32.857771 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/testing.py
--rw-r--r--   0        0        0     9882 2023-04-18 16:52:57.349405 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
--rw-r--r--   0        0        0      624 2023-04-18 16:52:57.349781 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
--rw-r--r--   0        0        0      918 2023-04-18 16:02:04.956279 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
--rw-r--r--   0        0        0      575 2023-04-18 16:02:04.956348 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
--rw-r--r--   0        0        0      542 2023-04-18 16:02:04.956406 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
--rw-r--r--   0        0        0     1199 2023-04-18 16:02:04.956469 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
--rw-r--r--   0        0        0      733 2023-04-18 16:02:04.956526 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
--rw-r--r--   0        0        0     5143 2023-04-18 16:02:04.956591 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
--rw-r--r--   0        0        0      593 2023-04-18 16:02:04.956814 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
--rw-r--r--   0        0        0       60 2023-02-15 16:43:38.797298 lnhub_rest-0.9.8/lnhub_rest/schema/versions.py
--rw-r--r--   0        0        0       13 2023-04-18 16:02:04.956879 lnhub_rest-0.9.8/lnhub_rest/utils/__init__.py
--rw-r--r--   0        0        0      212 2023-04-18 16:02:04.956936 lnhub_rest-0.9.8/lnhub_rest/utils/_access_token.py
--rw-r--r--   0        0        0      352 2023-04-18 16:02:04.956991 lnhub_rest-0.9.8/lnhub_rest/utils/_id.py
--rw-r--r--   0        0        0      109 2023-04-18 16:02:04.957042 lnhub_rest-0.9.8/lnhub_rest/utils/_query.py
--rw-r--r--   0        0        0     3820 2023-04-19 15:57:22.494545 lnhub_rest-0.9.8/lnhub_rest/utils/_test.py
--rw-r--r--   0        0        0     1728 2023-05-28 12:36:10.509265 lnhub_rest-0.9.8/noxfile.py
--rw-r--r--   0        0        0     1152 2023-05-28 13:30:17.362252 lnhub_rest-0.9.8/pyproject.toml
--rwxr-xr-x   0        0        0       29 2023-04-18 16:02:04.957796 lnhub_rest-0.9.8/scripts/run.sh
--rw-r--r--   0        0        0       27 2023-04-18 16:02:04.957868 lnhub_rest-0.9.8/supabase/.gitignore
--rw-r--r--   0        0        0     2548 2023-04-18 16:02:04.957934 lnhub_rest-0.9.8/supabase/config.toml
--rw-r--r--   0        0        0     1212 2023-04-25 15:29:32.858221 lnhub_rest-0.9.8/tests/test_notebooks.py
--rw-r--r--   0        0        0     3353 1970-01-01 00:00:00.000000 lnhub_rest-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1259 2023-06-04 16:55:04.143647 lnhub_rest-0.9.9/.dockerignore
+-rw-r--r--   0        0        0     3245 2023-06-04 16:55:04.143856 lnhub_rest-0.9.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0     5417 2023-06-04 16:55:04.143983 lnhub_rest-0.9.9/.github/workflows/google-cloudrun-docker-prod.yml
+-rw-r--r--   0        0        0     5426 2023-06-04 16:55:04.144061 lnhub_rest-0.9.9/.github/workflows/google-cloudrun-docker-staging.yml
+-rw-r--r--   0        0        0      133 2023-06-04 16:55:04.144133 lnhub_rest-0.9.9/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      613 2023-06-04 16:55:04.144209 lnhub_rest-0.9.9/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1212 2023-06-04 16:55:04.144273 lnhub_rest-0.9.9/.gitignore
+-rw-r--r--   0        0        0       73 2023-06-04 16:55:04.144346 lnhub_rest-0.9.9/.gitmodules
+-rw-r--r--   0        0        0     1772 2023-06-04 16:55:04.144437 lnhub_rest-0.9.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      157 2023-06-04 16:55:04.144527 lnhub_rest-0.9.9/Dockerfile
+-rw-r--r--   0        0        0     2442 2023-06-04 16:55:04.144607 lnhub_rest-0.9.9/README.md
+-rw-r--r--   0        0        0     1680 2023-06-04 16:55:04.144748 lnhub_rest-0.9.9/docs/00-migrate.ipynb
+-rw-r--r--   0        0        0     1189 2023-06-04 16:55:04.144866 lnhub_rest-0.9.9/docs/01-checks/01-check-break-lndb.ipynb
+-rw-r--r--   0        0        0     4487 2023-06-04 16:55:04.145033 lnhub_rest-0.9.9/docs/02-account/02-create-account.ipynb
+-rw-r--r--   0        0        0     5566 2023-06-04 16:55:04.145132 lnhub_rest-0.9.9/docs/02-account/03-update-account.ipynb
+-rw-r--r--   0        0        0     6111 2023-06-04 16:55:04.145223 lnhub_rest-0.9.9/docs/02-account/04-fetch-account.ipynb
+-rw-r--r--   0        0        0     9088 2023-06-04 16:55:04.145378 lnhub_rest-0.9.9/docs/02-account/05-rls.ipynb
+-rw-r--r--   0        0        0    11110 2023-06-04 16:55:04.145524 lnhub_rest-0.9.9/docs/03-instance/01-init-instance.ipynb
+-rw-r--r--   0        0        0     5293 2023-06-04 16:55:04.145623 lnhub_rest-0.9.9/docs/03-instance/02-load-instance.ipynb
+-rw-r--r--   0        0        0     6498 2023-06-04 16:55:04.145734 lnhub_rest-0.9.9/docs/03-instance/03-update-instance.ipynb
+-rw-r--r--   0        0        0     8667 2023-06-04 16:55:04.145825 lnhub_rest-0.9.9/docs/03-instance/04-delete-instance.ipynb
+-rw-r--r--   0        0        0     7001 2023-06-04 16:55:04.145970 lnhub_rest-0.9.9/docs/03-instance/05-fetch-instance.ipynb
+-rw-r--r--   0        0        0    19423 2023-06-04 16:55:04.146050 lnhub_rest-0.9.9/docs/03-instance/06-rls.ipynb
+-rw-r--r--   0        0        0     3990 2023-06-04 16:55:04.146190 lnhub_rest-0.9.9/docs/04-storage/01-add-storage.ipynb
+-rw-r--r--   0        0        0     9837 2023-06-04 16:55:04.146263 lnhub_rest-0.9.9/docs/04-storage/02-rls.ipynb
+-rw-r--r--   0        0        0     3894 2023-06-04 16:55:04.146420 lnhub_rest-0.9.9/docs/05-organization/01-create-organization.ipynb
+-rw-r--r--   0        0        0     4749 2023-06-04 16:55:04.146490 lnhub_rest-0.9.9/docs/05-organization/02-manage-members.ipynb
+-rw-r--r--   0        0        0     5892 2023-06-04 16:55:04.146595 lnhub_rest-0.9.9/docs/05-organization/03-rls.ipynb
+-rw-r--r--   0        0        0     5310 2023-06-04 16:55:04.146724 lnhub_rest-0.9.9/docs/06-integration/01-signup-signin.ipynb
+-rw-r--r--   0        0        0      125 2023-06-04 16:55:04.146794 lnhub_rest-0.9.9/docs/README.md
+-rw-r--r--   0        0        0    25182 2023-06-04 17:58:06.719625 lnhub_rest-0.9.9/docs/changelog.md
+-rw-r--r--   0        0        0      520 2023-06-04 16:55:04.147050 lnhub_rest-0.9.9/docs/migrations.md
+-rw-r--r--   0        0        0      162 2023-06-04 16:55:04.147165 lnhub_rest-0.9.9/docs/notes/index.md
+-rw-r--r--   0        0        0    26418 2023-06-04 16:55:04.147318 lnhub_rest-0.9.9/docs/notes/multiple-sign-ups-same-email.ipynb
+-rw-r--r--   0        0        0      137 2023-06-04 16:55:04.147409 lnhub_rest-0.9.9/lamin-project.yaml
+drwxr-xr-x   0        0        0        0 2023-06-04 16:55:04.147438 lnhub_rest-0.9.9/lndb/
+-rw-r--r--   0        0        0      157 2023-06-04 17:57:59.106082 lnhub_rest-0.9.9/lnhub_rest/__init__.py
+-rw-r--r--   0        0        0     7054 2023-06-04 16:55:04.147701 lnhub_rest-0.9.9/lnhub_rest/__main__.py
+-rw-r--r--   0        0        0       30 2023-06-04 17:57:56.320310 lnhub_rest-0.9.9/lnhub_rest/_assets/__init__.py
+-rw-r--r--   0        0        0     1109 2023-06-04 16:55:04.147957 lnhub_rest-0.9.9/lnhub_rest/_assets/_schemas.py
+-rw-r--r--   0        0        0     1722 2023-06-04 16:55:04.148058 lnhub_rest-0.9.9/lnhub_rest/_check_breaks_lndb.py
+-rw-r--r--   0        0        0     1260 2023-06-04 16:55:04.148133 lnhub_rest-0.9.9/lnhub_rest/_ci.py
+-rw-r--r--   0        0        0     5726 2023-06-04 16:55:04.148215 lnhub_rest-0.9.9/lnhub_rest/_clean_ci.py
+-rw-r--r--   0        0        0     1626 2023-06-04 16:55:04.148301 lnhub_rest-0.9.9/lnhub_rest/config.py
+-rw-r--r--   0        0        0       42 2023-06-04 16:55:04.148404 lnhub_rest-0.9.9/lnhub_rest/core/__init__.py
+-rw-r--r--   0        0        0      285 2023-06-04 16:55:04.148526 lnhub_rest-0.9.9/lnhub_rest/core/account/__init__.py
+-rw-r--r--   0        0        0     2542 2023-06-04 16:55:04.148633 lnhub_rest-0.9.9/lnhub_rest/core/account/_create_account.py
+-rw-r--r--   0        0        0     1062 2023-06-04 16:55:04.148718 lnhub_rest-0.9.9/lnhub_rest/core/account/_crud.py
+-rw-r--r--   0        0        0      739 2023-06-04 16:55:04.148828 lnhub_rest-0.9.9/lnhub_rest/core/account/_delete_account.py
+-rw-r--r--   0        0        0     3325 2023-06-04 16:55:04.148943 lnhub_rest-0.9.9/lnhub_rest/core/account/_signup_signin.py
+-rw-r--r--   0        0        0     1423 2023-06-04 16:55:04.149039 lnhub_rest-0.9.9/lnhub_rest/core/account/_update_account.py
+-rw-r--r--   0        0        0       38 2023-06-04 16:55:04.149148 lnhub_rest-0.9.9/lnhub_rest/core/collaborator/__init__.py
+-rw-r--r--   0        0        0     3056 2023-06-04 16:55:04.149221 lnhub_rest-0.9.9/lnhub_rest/core/collaborator/_crud.py
+-rw-r--r--   0        0        0      243 2023-06-04 16:55:04.149327 lnhub_rest-0.9.9/lnhub_rest/core/instance/__init__.py
+-rw-r--r--   0        0        0     1651 2023-06-04 16:55:04.149404 lnhub_rest-0.9.9/lnhub_rest/core/instance/_crud.py
+-rw-r--r--   0        0        0     1284 2023-06-04 16:55:04.149491 lnhub_rest-0.9.9/lnhub_rest/core/instance/_delete_instance.py
+-rw-r--r--   0        0        0     6096 2023-06-04 16:55:04.149598 lnhub_rest-0.9.9/lnhub_rest/core/instance/_init_instance.py
+-rw-r--r--   0        0        0     1532 2023-06-04 16:55:04.149674 lnhub_rest-0.9.9/lnhub_rest/core/instance/_load_instance.py
+-rw-r--r--   0        0        0     1067 2023-06-04 16:55:04.149758 lnhub_rest-0.9.9/lnhub_rest/core/instance/_update_instance.py
+-rw-r--r--   0        0        0       32 2023-06-04 16:55:04.149860 lnhub_rest-0.9.9/lnhub_rest/core/member/__init__.py
+-rw-r--r--   0        0        0     2078 2023-06-04 16:55:04.149938 lnhub_rest-0.9.9/lnhub_rest/core/member/_crud.py
+-rw-r--r--   0        0        0       80 2023-06-04 16:55:04.150048 lnhub_rest-0.9.9/lnhub_rest/core/storage/__init__.py
+-rw-r--r--   0        0        0     3427 2023-06-04 16:55:04.150173 lnhub_rest-0.9.9/lnhub_rest/core/storage/_add_storage.py
+-rw-r--r--   0        0        0     1167 2023-06-04 16:55:04.150263 lnhub_rest-0.9.9/lnhub_rest/core/storage/_crud.py
+-rw-r--r--   0        0        0      849 2023-06-04 16:55:04.150351 lnhub_rest-0.9.9/lnhub_rest/main.py
+-rw-r--r--   0        0        0       39 2023-06-04 16:55:04.150477 lnhub_rest-0.9.9/lnhub_rest/orm/__init__.py
+-rw-r--r--   0        0        0      199 2023-06-04 16:55:04.150561 lnhub_rest-0.9.9/lnhub_rest/orm/_engine.py
+-rw-r--r--   0        0        0     1968 2023-06-04 16:55:04.150636 lnhub_rest-0.9.9/lnhub_rest/orm/_sbclient.py
+-rw-r--r--   0        0        0      239 2023-06-04 16:55:04.150761 lnhub_rest-0.9.9/lnhub_rest/routers/__init__.py
+-rw-r--r--   0        0        0     4661 2023-06-04 16:55:04.150854 lnhub_rest-0.9.9/lnhub_rest/routers/account.py
+-rw-r--r--   0        0        0      538 2023-06-04 16:55:04.150932 lnhub_rest-0.9.9/lnhub_rest/routers/ci.py
+-rw-r--r--   0        0        0     2313 2023-06-04 16:55:04.151026 lnhub_rest-0.9.9/lnhub_rest/routers/collaborator.py
+-rw-r--r--   0        0        0      408 2023-06-04 16:55:04.151111 lnhub_rest-0.9.9/lnhub_rest/routers/dev.py
+-rw-r--r--   0        0        0     5233 2023-06-04 16:55:04.151198 lnhub_rest-0.9.9/lnhub_rest/routers/instance.py
+-rw-r--r--   0        0        0     2617 2023-06-04 16:55:04.151281 lnhub_rest-0.9.9/lnhub_rest/routers/organization.py
+-rw-r--r--   0        0        0     1074 2023-06-04 16:55:04.151363 lnhub_rest-0.9.9/lnhub_rest/routers/utils.py
+-rw-r--r--   0        0        0      249 2023-06-04 16:55:04.151488 lnhub_rest-0.9.9/lnhub_rest/schema/__init__.py
+-rw-r--r--   0        0        0     4986 2023-06-04 16:55:04.151600 lnhub_rest-0.9.9/lnhub_rest/schema/_core.py
+-rw-r--r--   0        0        0      270 2023-06-04 16:55:04.151675 lnhub_rest-0.9.9/lnhub_rest/schema/_timestamps.py
+-rw-r--r--   0        0        0      262 2023-06-04 16:55:04.151766 lnhub_rest-0.9.9/lnhub_rest/schema/_type.py
+-rw-r--r--   0        0        0      252 2023-06-04 16:55:04.151848 lnhub_rest-0.9.9/lnhub_rest/schema/_users.py
+-rw-r--r--   0        0        0     1079 2023-06-04 16:55:04.151920 lnhub_rest-0.9.9/lnhub_rest/schema/_versions.py
+-rw-r--r--   0        0        0      674 2023-06-04 16:55:04.151996 lnhub_rest-0.9.9/lnhub_rest/schema/alembic.ini
+-rw-r--r--   0        0        0       40 2023-06-04 16:55:04.152112 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/__init__.py
+-rw-r--r--   0        0        0     6020 2023-06-04 16:55:04.152225 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/clone.py
+-rw-r--r--   0        0        0     3033 2023-06-04 16:55:04.152323 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/env.py
+-rw-r--r--   0        0        0     1193 2023-06-04 16:55:04.152428 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0     1319 2023-06-04 16:55:04.152502 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1667 2023-06-04 16:55:04.152577 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0       39 2023-06-04 16:55:04.152652 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/function/__init__.py
+-rw-r--r--   0        0        0     3940 2023-06-04 16:55:04.152781 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0      639 2023-06-04 16:55:04.152849 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
+-rw-r--r--   0        0        0      214 2023-06-04 16:55:04.152949 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
+-rw-r--r--   0        0        0      192 2023-06-04 16:55:04.153018 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
+-rw-r--r--   0        0        0     7619 2023-06-04 16:55:04.153083 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1408 2023-06-04 16:55:04.153166 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0      880 2023-06-04 16:55:04.153256 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
+-rw-r--r--   0        0        0       33 2023-06-04 16:55:04.153322 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/__init__.py
+-rw-r--r--   0        0        0      542 2023-06-04 16:55:04.153405 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/script.py.mako
+-rw-r--r--   0        0        0     5258 2023-06-04 16:55:04.153500 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/testing.py
+-rw-r--r--   0        0        0     9882 2023-06-04 16:55:04.153673 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
+-rw-r--r--   0        0        0      624 2023-06-04 16:55:04.153760 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
+-rw-r--r--   0        0        0      918 2023-06-04 16:55:04.153840 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
+-rw-r--r--   0        0        0      575 2023-06-04 16:55:04.153912 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
+-rw-r--r--   0        0        0      542 2023-06-04 16:55:04.153992 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
+-rw-r--r--   0        0        0     1199 2023-06-04 16:55:04.154081 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
+-rw-r--r--   0        0        0      733 2023-06-04 16:55:04.154149 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
+-rw-r--r--   0        0        0     5143 2023-06-04 16:55:04.154235 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
+-rw-r--r--   0        0        0      593 2023-06-04 16:55:04.154304 lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
+-rw-r--r--   0        0        0       60 2023-06-04 16:55:04.154375 lnhub_rest-0.9.9/lnhub_rest/schema/versions.py
+-rw-r--r--   0        0        0       13 2023-06-04 16:55:04.154487 lnhub_rest-0.9.9/lnhub_rest/utils/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-04 16:55:04.154564 lnhub_rest-0.9.9/lnhub_rest/utils/_access_token.py
+-rw-r--r--   0        0        0      352 2023-06-04 16:55:04.154672 lnhub_rest-0.9.9/lnhub_rest/utils/_id.py
+-rw-r--r--   0        0        0      109 2023-06-04 16:55:04.154735 lnhub_rest-0.9.9/lnhub_rest/utils/_query.py
+-rw-r--r--   0        0        0     3820 2023-06-04 16:55:04.154792 lnhub_rest-0.9.9/lnhub_rest/utils/_test.py
+-rw-r--r--   0        0        0     1728 2023-06-04 16:55:04.154898 lnhub_rest-0.9.9/noxfile.py
+-rw-r--r--   0        0        0     1152 2023-06-04 16:55:04.154978 lnhub_rest-0.9.9/pyproject.toml
+-rwxr-xr-x   0        0        0       29 2023-06-04 16:55:04.155094 lnhub_rest-0.9.9/scripts/run.sh
+-rw-r--r--   0        0        0       27 2023-06-04 16:55:04.155207 lnhub_rest-0.9.9/supabase/.gitignore
+-rw-r--r--   0        0        0     2548 2023-06-04 16:55:04.155292 lnhub_rest-0.9.9/supabase/config.toml
+-rw-r--r--   0        0        0     1211 2023-06-04 17:57:56.320605 lnhub_rest-0.9.9/tests/test_notebooks.py
+-rw-r--r--   0        0        0     3353 1970-01-01 00:00:00.000000 lnhub_rest-0.9.9/PKG-INFO
```

### Comparing `lnhub_rest-0.9.8/.dockerignore` & `lnhub_rest-0.9.9/.dockerignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/.github/workflows/build.yml` & `lnhub_rest-0.9.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/.github/workflows/google-cloudrun-docker-prod.yml` & `lnhub_rest-0.9.9/.github/workflows/google-cloudrun-docker-prod.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/.github/workflows/google-cloudrun-docker-staging.yml` & `lnhub_rest-0.9.9/.github/workflows/google-cloudrun-docker-staging.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/.github/workflows/latest-changes.yml` & `lnhub_rest-0.9.9/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/.gitignore` & `lnhub_rest-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/.pre-commit-config.yaml` & `lnhub_rest-0.9.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/README.md` & `lnhub_rest-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/00-migrate.ipynb` & `lnhub_rest-0.9.9/docs/00-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/01-checks/01-check-break-lndb.ipynb` & `lnhub_rest-0.9.9/docs/01-checks/01-check-break-lndb.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/02-account/02-create-account.ipynb` & `lnhub_rest-0.9.9/docs/02-account/02-create-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/02-account/03-update-account.ipynb` & `lnhub_rest-0.9.9/docs/02-account/03-update-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/02-account/04-fetch-account.ipynb` & `lnhub_rest-0.9.9/docs/02-account/04-fetch-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/02-account/05-rls.ipynb` & `lnhub_rest-0.9.9/docs/02-account/05-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/03-instance/01-init-instance.ipynb` & `lnhub_rest-0.9.9/docs/03-instance/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/03-instance/02-load-instance.ipynb` & `lnhub_rest-0.9.9/docs/03-instance/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/03-instance/03-update-instance.ipynb` & `lnhub_rest-0.9.9/docs/03-instance/03-update-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/03-instance/04-delete-instance.ipynb` & `lnhub_rest-0.9.9/docs/03-instance/04-delete-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/03-instance/05-fetch-instance.ipynb` & `lnhub_rest-0.9.9/docs/03-instance/05-fetch-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/03-instance/06-rls.ipynb` & `lnhub_rest-0.9.9/docs/03-instance/06-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/04-storage/01-add-storage.ipynb` & `lnhub_rest-0.9.9/docs/04-storage/01-add-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/04-storage/02-rls.ipynb` & `lnhub_rest-0.9.9/docs/04-storage/02-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/05-organization/01-create-organization.ipynb` & `lnhub_rest-0.9.9/docs/05-organization/01-create-organization.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/05-organization/02-manage-members.ipynb` & `lnhub_rest-0.9.9/docs/05-organization/02-manage-members.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/05-organization/03-rls.ipynb` & `lnhub_rest-0.9.9/docs/05-organization/03-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/06-integration/01-signup-signin.ipynb` & `lnhub_rest-0.9.9/docs/06-integration/01-signup-signin.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/changelog.md` & `lnhub_rest-0.9.9/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🔥 Remove not-needed assets | [215](https://github.com/laminlabs/lnhub-rest/pull/215) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 | 0.9.9
 ➖ Simplify dependencies | [208](https://github.com/laminlabs/lnhub-rest/pull/208) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.9.8
 ➖ Replace boto3 with botocore | [206](https://github.com/laminlabs/lnhub-rest/pull/206) | [Koncopd](https://github.com/Koncopd) | 2023-05-26 |
 🍱 Update assets | [207](https://github.com/laminlabs/lnhub-rest/pull/207) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 |
 ➖ Streamline dependencies | [205](https://github.com/laminlabs/lnhub-rest/pull/205) | [bpenteado](https://github.com/bpenteado) | 2023-05-10 | 0.9.6
 🔖 Staging version 0.9.5 | [199](https://github.com/laminlabs/lnhub-rest/pull/199) | [bpenteado](https://github.com/bpenteado) | 2023-05-09 | 0.9.5
 👷 Fix deployment in main branch | [201](https://github.com/laminlabs/lnhub-rest/pull/201) | [lawrlee](https://github.com/lawrlee) | 2023-05-09 |
 ✨ Create endpoints to update and delete collaborators | [197](https://github.com/laminlabs/lnhub-rest/pull/197) | [bpenteado](https://github.com/bpenteado) | 2023-05-09 |
```

### Comparing `lnhub_rest-0.9.8/docs/migrations.md` & `lnhub_rest-0.9.9/docs/migrations.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/docs/notes/multiple-sign-ups-same-email.ipynb` & `lnhub_rest-0.9.9/docs/notes/multiple-sign-ups-same-email.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lndb/docs/faq/switch-environment.ipynb` & `lnhub_rest-0.9.9/lnhub_rest/utils/_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,203 +1,239 @@
-00000000: 7b0a 2022 6365 6c6c 7322 3a20 5b0a 2020  {. "cells": [.  
-00000010: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
-00000020: 3a20 226d 6172 6b64 6f77 6e22 2c0a 2020  : "markdown",.  
-00000030: 2022 6964 223a 2022 6234 3364 3039 6435   "id": "b43d09d5
-00000040: 2d32 3664 332d 3434 3064 2d62 3333 342d  -26d3-440d-b334-
-00000050: 3936 3433 6563 3532 3438 6536 222c 0a20  9643ec5248e6",. 
-00000060: 2020 226d 6574 6164 6174 6122 3a20 7b0a    "metadata": {.
-00000070: 2020 2020 2274 6167 7322 3a20 5b5d 0a20      "tags": []. 
-00000080: 2020 7d2c 0a20 2020 2273 6f75 7263 6522    },.   "source"
-00000090: 3a20 5b0a 2020 2020 2223 2054 6573 7420  : [.    "# Test 
-000000a0: 7377 6974 6368 2065 6e76 6972 6f6e 6d65  switch environme
-000000b0: 6e74 220a 2020 205d 0a20 207d 2c0a 2020  nt".   ].  },.  
-000000c0: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
-000000d0: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
-000000e0: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
-000000f0: 6e75 6c6c 2c0a 2020 2022 6964 223a 2022  null,.   "id": "
-00000100: 3333 6332 6262 3736 2d64 3631 662d 3438  33c2bb76-d61f-48
-00000110: 3636 2d38 3765 322d 3738 3065 3631 3630  66-87e2-780e6160
-00000120: 3030 3232 222c 0a20 2020 226d 6574 6164  0022",.   "metad
-00000130: 6174 6122 3a20 7b7d 2c0a 2020 2022 6f75  ata": {},.   "ou
-00000140: 7470 7574 7322 3a20 5b5d 2c0a 2020 2022  tputs": [],.   "
-00000150: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
-00000160: 6672 6f6d 206c 6e64 6220 696d 706f 7274  from lndb import
-00000170: 2073 6574 7469 6e67 732c 2073 6967 6e75   settings, signu
-00000180: 702c 2069 6e69 742c 206c 6f67 696e 5c6e  p, init, login\n
-00000190: 222c 0a20 2020 2022 6672 6f6d 206c 6e64  ",.    "from lnd
-000001a0: 622e 6465 762e 5f73 6574 7469 6e67 735f  b.dev._settings_
-000001b0: 6c6f 6164 2069 6d70 6f72 7420 6c6f 6164  load import load
-000001c0: 5f69 6e73 7461 6e63 655f 7365 7474 696e  _instance_settin
-000001d0: 6773 5c6e 222c 0a20 2020 2022 696d 706f  gs\n",.    "impo
-000001e0: 7274 206f 7322 0a20 2020 5d0a 2020 7d2c  rt os".   ].  },
-000001f0: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
-00000200: 7065 223a 2022 636f 6465 222c 0a20 2020  pe": "code",.   
-00000210: 2265 7865 6375 7469 6f6e 5f63 6f75 6e74  "execution_count
-00000220: 223a 206e 756c 6c2c 0a20 2020 2269 6422  ": null,.   "id"
-00000230: 3a20 2261 3963 6263 3262 3822 2c0a 2020  : "a9cbc2b8",.  
-00000240: 2022 6d65 7461 6461 7461 223a 207b 7d2c   "metadata": {},
-00000250: 0a20 2020 226f 7574 7075 7473 223a 205b  .   "outputs": [
-00000260: 5d2c 0a20 2020 2273 6f75 7263 6522 3a20  ],.   "source": 
-00000270: 5b0a 2020 2020 226c 6f67 696e 285c 2274  [.    "login(\"t
-00000280: 6573 7475 7365 7231 406c 616d 696e 2e61  estuser1@lamin.a
-00000290: 695c 2229 5c6e 222c 0a20 2020 2022 696e  i\")\n",.    "in
-000002a0: 6974 2873 746f 7261 6765 3d5c 226d 7964  it(storage=\"myd
-000002b0: 6174 615f 7072 6f64 5c22 295c 6e22 2c0a  ata_prod\")\n",.
-000002c0: 2020 2020 225c 6e22 2c0a 2020 2020 2275      "\n",.    "u
-000002d0: 7365 725f 6163 6365 7373 5f74 6f6b 656e  ser_access_token
-000002e0: 5f70 726f 6420 3d20 7365 7474 696e 6773  _prod = settings
-000002f0: 2e75 7365 722e 6163 6365 7373 5f74 6f6b  .user.access_tok
-00000300: 656e 220a 2020 205d 0a20 207d 2c0a 2020  en".   ].  },.  
-00000310: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
-00000320: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
-00000330: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
-00000340: 6e75 6c6c 2c0a 2020 2022 6964 223a 2022  null,.   "id": "
-00000350: 6135 6538 6130 6136 222c 0a20 2020 226d  a5e8a0a6",.   "m
-00000360: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
-00000370: 2022 6f75 7470 7574 7322 3a20 5b5d 2c0a   "outputs": [],.
-00000380: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
-00000390: 2020 2022 2320 6f73 2e65 6e76 6972 6f6e     "# os.environ
-000003a0: 5b5c 224c 414d 494e 5f45 4e56 5c22 5d20  [\"LAMIN_ENV\"] 
-000003b0: 3d20 5c22 6465 765c 225c 6e22 2c0a 2020  = \"dev\"\n",.  
-000003c0: 2020 225c 6e22 2c0a 2020 2020 2223 206c    "\n",.    "# l
-000003d0: 6f67 696e 285c 2274 6573 7475 7365 7231  ogin(\"testuser1
-000003e0: 406c 616d 696e 2e61 695c 222c 2070 6173  @lamin.ai\", pas
-000003f0: 7377 6f72 643d 5c22 4243 5252 7650 6a7a  sword=\"BCRRvPjz
-00000400: 6a6e 4557 347a 3053 6734 6563 4234 3734  jnEW4z0Sg4ecB474
-00000410: 4345 644f 6546 4e57 4735 4f67 546e 734f  CEdOeFNWG5OgTnsO
-00000420: 5c22 295c 6e22 2c0a 2020 2020 2223 2069  \")\n",.    "# i
-00000430: 6e69 7428 7374 6f72 6167 653d 5c22 6d79  nit(storage=\"my
-00000440: 6461 7461 5f64 6576 5c22 295c 6e22 2c0a  data_dev\")\n",.
-00000450: 2020 2020 225c 6e22 2c0a 2020 2020 2223      "\n",.    "#
-00000460: 2075 7365 725f 6163 6365 7373 5f74 6f6b   user_access_tok
-00000470: 656e 5f64 6576 203d 2073 6574 7469 6e67  en_dev = setting
-00000480: 732e 7573 6572 2e61 6363 6573 735f 746f  s.user.access_to
-00000490: 6b65 6e22 0a20 2020 5d0a 2020 7d2c 0a20  ken".   ].  },. 
-000004a0: 207b 0a20 2020 2263 656c 6c5f 7479 7065   {.   "cell_type
-000004b0: 223a 2022 636f 6465 222c 0a20 2020 2265  ": "code",.   "e
-000004c0: 7865 6375 7469 6f6e 5f63 6f75 6e74 223a  xecution_count":
-000004d0: 206e 756c 6c2c 0a20 2020 2269 6422 3a20   null,.   "id": 
-000004e0: 2236 6339 3438 3134 3522 2c0a 2020 2022  "6c948145",.   "
-000004f0: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
-00000500: 2020 226f 7574 7075 7473 223a 205b 5d2c    "outputs": [],
-00000510: 0a20 2020 2273 6f75 7263 6522 3a20 5b0a  .   "source": [.
-00000520: 2020 2020 2223 206f 732e 656e 7669 726f      "# os.enviro
-00000530: 6e5b 5c22 4c41 4d49 4e5f 454e 565c 225d  n[\"LAMIN_ENV\"]
-00000540: 203d 205c 2274 6573 745c 225c 6e22 2c0a   = \"test\"\n",.
-00000550: 2020 2020 225c 6e22 2c0a 2020 2020 2223      "\n",.    "#
-00000560: 206c 6f67 696e 285c 2274 6573 7475 7365   login(\"testuse
-00000570: 7231 406c 616d 696e 2e61 695c 222c 2070  r1@lamin.ai\", p
-00000580: 6173 7377 6f72 643d 5c22 3367 5946 7639  assword=\"3gYFv9
-00000590: 3863 744e 7159 7a67 7366 3969 4f72 786d  8ctNqYzgsf9iOrxm
-000005a0: 5655 576b 5432 4c6b 4144 326c 3156 3735  VUWkT2LkAD2l1V75
-000005b0: 6a7a 5c22 295c 6e22 2c0a 2020 2020 2223  jz\")\n",.    "#
-000005c0: 2069 6e69 7428 7374 6f72 6167 653d 5c22   init(storage=\"
-000005d0: 6d79 6461 7461 5f74 6573 745c 2229 5c6e  mydata_test\")\n
-000005e0: 222c 0a20 2020 2022 5c6e 222c 0a20 2020  ",.    "\n",.   
-000005f0: 2022 2320 7573 6572 5f61 6363 6573 735f   "# user_access_
-00000600: 746f 6b65 6e5f 7465 7374 203d 2073 6574  token_test = set
-00000610: 7469 6e67 732e 7573 6572 2e61 6363 6573  tings.user.acces
-00000620: 735f 746f 6b65 6e22 0a20 2020 5d0a 2020  s_token".   ].  
-00000630: 7d2c 0a20 207b 0a20 2020 2263 656c 6c5f  },.  {.   "cell_
-00000640: 7479 7065 223a 2022 636f 6465 222c 0a20  type": "code",. 
-00000650: 2020 2265 7865 6375 7469 6f6e 5f63 6f75    "execution_cou
-00000660: 6e74 223a 206e 756c 6c2c 0a20 2020 2269  nt": null,.   "i
-00000670: 6422 3a20 2266 3633 3636 3964 3822 2c0a  d": "f63669d8",.
-00000680: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-00000690: 7d2c 0a20 2020 226f 7574 7075 7473 223a  },.   "outputs":
-000006a0: 205b 5d2c 0a20 2020 2273 6f75 7263 6522   [],.   "source"
-000006b0: 3a20 5b0a 2020 2020 2223 206f 732e 656e  : [.    "# os.en
-000006c0: 7669 726f 6e5b 5c22 4c41 4d49 4e5f 454e  viron[\"LAMIN_EN
-000006d0: 565c 225d 203d 205c 2270 726f 645c 225c  V\"] = \"prod\"\
-000006e0: 6e22 2c0a 2020 2020 225c 6e22 2c0a 2020  n",.    "\n",.  
-000006f0: 2020 2223 2073 6574 7469 6e67 732e 696e    "# settings.in
-00000700: 7374 616e 6365 2e6e 616d 6520 3d3d 205c  stance.name == \
-00000710: 226d 7964 6174 615f 7072 6f64 5c22 5c6e  "mydata_prod\"\n
-00000720: 222c 0a20 2020 2022 2320 7365 7474 696e  ",.    "# settin
-00000730: 6773 2e75 7365 722e 6163 6365 7373 5f74  gs.user.access_t
-00000740: 6f6b 656e 203d 3d20 7573 6572 5f61 6363  oken == user_acc
-00000750: 6573 735f 746f 6b65 6e5f 7072 6f64 220a  ess_token_prod".
-00000760: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
-00000770: 2022 6365 6c6c 5f74 7970 6522 3a20 2263   "cell_type": "c
-00000780: 6f64 6522 2c0a 2020 2022 6578 6563 7574  ode",.   "execut
-00000790: 696f 6e5f 636f 756e 7422 3a20 6e75 6c6c  ion_count": null
-000007a0: 2c0a 2020 2022 6964 223a 2022 3837 6633  ,.   "id": "87f3
-000007b0: 3730 3035 222c 0a20 2020 226d 6574 6164  7005",.   "metad
-000007c0: 6174 6122 3a20 7b7d 2c0a 2020 2022 6f75  ata": {},.   "ou
-000007d0: 7470 7574 7322 3a20 5b5d 2c0a 2020 2022  tputs": [],.   "
-000007e0: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
-000007f0: 2320 6f73 2e65 6e76 6972 6f6e 5b5c 224c  # os.environ[\"L
-00000800: 414d 494e 5f45 4e56 5c22 5d20 3d20 5c22  AMIN_ENV\"] = \"
-00000810: 6465 765c 225c 6e22 2c0a 2020 2020 225c  dev\"\n",.    "\
-00000820: 6e22 2c0a 2020 2020 2223 2073 6574 7469  n",.    "# setti
-00000830: 6e67 732e 696e 7374 616e 6365 2e6e 616d  ngs.instance.nam
-00000840: 6520 3d3d 205c 226d 7964 6174 615f 6465  e == \"mydata_de
-00000850: 765c 225c 6e22 2c0a 2020 2020 2223 2073  v\"\n",.    "# s
-00000860: 6574 7469 6e67 732e 7573 6572 2e61 6363  ettings.user.acc
-00000870: 6573 735f 746f 6b65 6e20 3d3d 2075 7365  ess_token == use
-00000880: 725f 6163 6365 7373 5f74 6f6b 656e 5f64  r_access_token_d
-00000890: 6576 220a 2020 205d 0a20 207d 2c0a 2020  ev".   ].  },.  
-000008a0: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
-000008b0: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
-000008c0: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
-000008d0: 6e75 6c6c 2c0a 2020 2022 6964 223a 2022  null,.   "id": "
-000008e0: 6462 3935 6265 3865 222c 0a20 2020 226d  db95be8e",.   "m
-000008f0: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
-00000900: 2022 6f75 7470 7574 7322 3a20 5b5d 2c0a   "outputs": [],.
-00000910: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
-00000920: 2020 2022 2320 6f73 2e65 6e76 6972 6f6e     "# os.environ
-00000930: 5b5c 224c 414d 494e 5f45 4e56 5c22 5d20  [\"LAMIN_ENV\"] 
-00000940: 3d20 5c22 7465 7374 5c22 5c6e 222c 0a20  = \"test\"\n",. 
-00000950: 2020 2022 5c6e 222c 0a20 2020 2022 2320     "\n",.    "# 
-00000960: 7365 7474 696e 6773 2e69 6e73 7461 6e63  settings.instanc
-00000970: 652e 6e61 6d65 203d 3d20 5c22 6d79 6461  e.name == \"myda
-00000980: 7461 5f74 6573 745c 225c 6e22 2c0a 2020  ta_test\"\n",.  
-00000990: 2020 2223 2073 6574 7469 6e67 732e 7573    "# settings.us
-000009a0: 6572 2e61 6363 6573 735f 746f 6b65 6e20  er.access_token 
-000009b0: 3d3d 2075 7365 725f 6163 6365 7373 5f74  == user_access_t
-000009c0: 6f6b 656e 5f74 6573 7422 0a20 2020 5d0a  oken_test".   ].
-000009d0: 2020 7d2c 0a20 207b 0a20 2020 2263 656c    },.  {.   "cel
-000009e0: 6c5f 7479 7065 223a 2022 636f 6465 222c  l_type": "code",
-000009f0: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
-00000a00: 6f75 6e74 223a 206e 756c 6c2c 0a20 2020  ount": null,.   
-00000a10: 2269 6422 3a20 2232 3666 6539 3832 6222  "id": "26fe982b"
-00000a20: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
-00000a30: 207b 7d2c 0a20 2020 226f 7574 7075 7473   {},.   "outputs
-00000a40: 223a 205b 5d2c 0a20 2020 2273 6f75 7263  ": [],.   "sourc
-00000a50: 6522 3a20 5b0a 2020 2020 2223 206f 732e  e": [.    "# os.
-00000a60: 656e 7669 726f 6e5b 5c22 4c41 4d49 4e5f  environ[\"LAMIN_
-00000a70: 454e 565c 225d 203d 205c 2270 726f 645c  ENV\"] = \"prod\
-00000a80: 2222 0a20 2020 5d0a 2020 7d0a 205d 2c0a  "".   ].  }. ],.
-00000a90: 2022 6d65 7461 6461 7461 223a 207b 0a20   "metadata": {. 
-00000aa0: 2022 6b65 726e 656c 7370 6563 223a 207b   "kernelspec": {
-00000ab0: 0a20 2020 2264 6973 706c 6179 5f6e 616d  .   "display_nam
-00000ac0: 6522 3a20 2262 6173 6522 2c0a 2020 2022  e": "base",.   "
-00000ad0: 6c61 6e67 7561 6765 223a 2022 7079 7468  language": "pyth
-00000ae0: 6f6e 222c 0a20 2020 226e 616d 6522 3a20  on",.   "name": 
-00000af0: 2270 7974 686f 6e33 220a 2020 7d2c 0a20  "python3".  },. 
-00000b00: 2022 6c61 6e67 7561 6765 5f69 6e66 6f22   "language_info"
-00000b10: 3a20 7b0a 2020 2022 636f 6465 6d69 7272  : {.   "codemirr
-00000b20: 6f72 5f6d 6f64 6522 3a20 7b0a 2020 2020  or_mode": {.    
-00000b30: 226e 616d 6522 3a20 2269 7079 7468 6f6e  "name": "ipython
-00000b40: 222c 0a20 2020 2022 7665 7273 696f 6e22  ",.    "version"
-00000b50: 3a20 330a 2020 207d 2c0a 2020 2022 6669  : 3.   },.   "fi
-00000b60: 6c65 5f65 7874 656e 7369 6f6e 223a 2022  le_extension": "
-00000b70: 2e70 7922 2c0a 2020 2022 6d69 6d65 7479  .py",.   "mimety
-00000b80: 7065 223a 2022 7465 7874 2f78 2d70 7974  pe": "text/x-pyt
-00000b90: 686f 6e22 2c0a 2020 2022 6e61 6d65 223a  hon",.   "name":
-00000ba0: 2022 7079 7468 6f6e 222c 0a20 2020 226e   "python",.   "n
-00000bb0: 6263 6f6e 7665 7274 5f65 7870 6f72 7465  bconvert_exporte
-00000bc0: 7222 3a20 2270 7974 686f 6e22 2c0a 2020  r": "python",.  
-00000bd0: 2022 7079 676d 656e 7473 5f6c 6578 6572   "pygments_lexer
-00000be0: 223a 2022 6970 7974 686f 6e33 222c 0a20  ": "ipython3",. 
-00000bf0: 2020 2276 6572 7369 6f6e 223a 2022 332e    "version": "3.
-00000c00: 392e 3133 220a 2020 7d2c 0a20 2022 7673  9.13".  },.  "vs
-00000c10: 636f 6465 223a 207b 0a20 2020 2269 6e74  code": {.   "int
-00000c20: 6572 7072 6574 6572 223a 207b 0a20 2020  erpreter": {.   
-00000c30: 2022 6861 7368 223a 2022 3430 6433 6130   "hash": "40d3a0
-00000c40: 3930 6635 3463 3635 3639 6162 3136 3332  90f54c6569ab1632
-00000c50: 3333 3262 3634 6232 6330 3363 3339 6463  332b64b2c03c39dc
-00000c60: 6639 3138 6230 3834 3234 6539 3866 3338  f918b08424e98f38
-00000c70: 6235 6165 3061 6638 3866 220a 2020 207d  b5ae0af88f".   }
-00000c80: 0a20 207d 0a20 7d2c 0a20 226e 6266 6f72  .  }. },. "nbfor
-00000c90: 6d61 7422 3a20 342c 0a20 226e 6266 6f72  mat": 4,. "nbfor
-00000ca0: 6d61 745f 6d69 6e6f 7222 3a20 350a 7d0a  mat_minor": 5.}.
+00000000: 696d 706f 7274 206f 730a 696d 706f 7274  import os.import
+00000010: 2075 7569 640a 6672 6f6d 2074 7970 696e   uuid.from typin
+00000020: 6720 696d 706f 7274 2055 6e69 6f6e 0a0a  g import Union..
+00000030: 696d 706f 7274 2072 6571 7565 7374 7320  import requests 
+00000040: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
+00000050: 0a66 726f 6d20 6c6e 6875 625f 7265 7374  .from lnhub_rest
+00000060: 2e63 6f72 652e 6163 636f 756e 742e 5f63  .core.account._c
+00000070: 7275 6420 696d 706f 7274 2073 625f 696e  rud import sb_in
+00000080: 7365 7274 5f61 6363 6f75 6e74 0a66 726f  sert_account.fro
+00000090: 6d20 6c6e 6875 625f 7265 7374 2e63 6f72  m lnhub_rest.cor
+000000a0: 652e 636f 6c6c 6162 6f72 6174 6f72 2e5f  e.collaborator._
+000000b0: 6372 7564 2069 6d70 6f72 7420 7362 5f69  crud import sb_i
+000000c0: 6e73 6572 745f 636f 6c6c 6162 6f72 6174  nsert_collaborat
+000000d0: 6f72 0a66 726f 6d20 6c6e 6875 625f 7265  or.from lnhub_re
+000000e0: 7374 2e63 6f72 652e 696e 7374 616e 6365  st.core.instance
+000000f0: 2e5f 6372 7564 2069 6d70 6f72 7420 7362  ._crud import sb
+00000100: 5f69 6e73 6572 745f 696e 7374 616e 6365  _insert_instance
+00000110: 0a66 726f 6d20 6c6e 6875 625f 7265 7374  .from lnhub_rest
+00000120: 2e63 6f72 652e 7374 6f72 6167 652e 5f63  .core.storage._c
+00000130: 7275 6420 696d 706f 7274 2073 625f 696e  rud import sb_in
+00000140: 7365 7274 5f73 746f 7261 6765 0a66 726f  sert_storage.fro
+00000150: 6d20 6c6e 6875 625f 7265 7374 2e6f 726d  m lnhub_rest.orm
+00000160: 2e5f 7362 636c 6965 6e74 2069 6d70 6f72  ._sbclient impor
+00000170: 7420 280a 2020 2020 636f 6e6e 6563 745f  t (.    connect_
+00000180: 6875 622c 0a20 2020 2063 6f6e 6e65 6374  hub,.    connect
+00000190: 5f68 7562 5f77 6974 685f 6175 7468 2c0a  _hub_with_auth,.
+000001a0: 2020 2020 636f 6e6e 6563 745f 6875 625f      connect_hub_
+000001b0: 7769 7468 5f73 6572 7669 6365 5f72 6f6c  with_service_rol
+000001c0: 652c 0a20 2020 2067 6574 5f6c 616d 696e  e,.    get_lamin
+000001d0: 5f73 6974 655f 6261 7365 5f75 726c 2c0a  _site_base_url,.
+000001e0: 290a 6672 6f6d 206c 6e68 7562 5f72 6573  ).from lnhub_res
+000001f0: 742e 7574 696c 732e 5f61 6363 6573 735f  t.utils._access_
+00000200: 746f 6b65 6e20 696d 706f 7274 2065 7874  token import ext
+00000210: 7261 6374 5f69 640a 6672 6f6d 206c 6e68  ract_id.from lnh
+00000220: 7562 5f72 6573 742e 7574 696c 732e 5f69  ub_rest.utils._i
+00000230: 6420 696d 706f 7274 2062 6173 6536 320a  d import base62.
+00000240: 0a0a 6465 6620 6372 6561 7465 5f74 6573  ..def create_tes
+00000250: 745f 6175 7468 2829 3a0a 2020 2020 6861  t_auth():.    ha
+00000260: 6e64 6c65 203d 2066 226c 616d 696e 2e63  ndle = f"lamin.c
+00000270: 692e 7573 6572 2e7b 6261 7365 3632 2836  i.user.{base62(6
+00000280: 297d 220a 2020 2020 656d 6169 6c20 3d20  )}".    email = 
+00000290: 6622 7b68 616e 646c 657d 4067 6d61 696c  f"{handle}@gmail
+000002a0: 2e63 6f6d 220a 2020 2020 7061 7373 776f  .com".    passwo
+000002b0: 7264 203d 2022 7061 7373 776f 7264 220a  rd = "password".
+000002c0: 0a20 2020 2069 6620 224c 414d 494e 5f45  .    if "LAMIN_E
+000002d0: 4e56 2220 696e 206f 732e 656e 7669 726f  NV" in os.enviro
+000002e0: 6e20 616e 6420 6f73 2e65 6e76 6972 6f6e  n and os.environ
+000002f0: 5b22 4c41 4d49 4e5f 454e 5622 5d20 213d  ["LAMIN_ENV"] !=
+00000300: 2022 6c6f 6361 6c22 3a0a 2020 2020 2020   "local":.      
+00000310: 2020 6875 6220 3d20 636f 6e6e 6563 745f    hub = connect_
+00000320: 6875 625f 7769 7468 5f73 6572 7669 6365  hub_with_service
+00000330: 5f72 6f6c 6528 290a 2020 2020 2020 2020  _role().        
+00000340: 6765 6e65 7261 7465 5f6c 696e 6b5f 7265  generate_link_re
+00000350: 7370 6f6e 7365 203d 2068 7562 2e61 7574  sponse = hub.aut
+00000360: 682e 6164 6d69 6e2e 6765 6e65 7261 7465  h.admin.generate
+00000370: 5f6c 696e 6b28 0a20 2020 2020 2020 2020  _link(.         
+00000380: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00000390: 2020 2020 2022 7479 7065 223a 2022 7369       "type": "si
+000003a0: 676e 7570 222c 0a20 2020 2020 2020 2020  gnup",.         
+000003b0: 2020 2020 2020 2022 656d 6169 6c22 3a20         "email": 
+000003c0: 656d 6169 6c2c 0a20 2020 2020 2020 2020  email,.         
+000003d0: 2020 2020 2020 2022 7061 7373 776f 7264         "password
+000003e0: 223a 2070 6173 7377 6f72 642c 0a20 2020  ": password,.   
+000003f0: 2020 2020 2020 2020 2020 2020 2022 6f70               "op
+00000400: 7469 6f6e 7322 3a20 7b0a 2020 2020 2020  tions": {.      
+00000410: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00000420: 6564 6972 6563 745f 746f 223a 2067 6574  edirect_to": get
+00000430: 5f6c 616d 696e 5f73 6974 655f 6261 7365  _lamin_site_base
+00000440: 5f75 726c 2829 2c0a 2020 2020 2020 2020  _url(),.        
+00000450: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000460: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00000470: 2029 0a20 2020 2020 2020 2061 6374 696f   ).        actio
+00000480: 6e5f 6c69 6e6b 203d 2067 656e 6572 6174  n_link = generat
+00000490: 655f 6c69 6e6b 5f72 6573 706f 6e73 652e  e_link_response.
+000004a0: 7072 6f70 6572 7469 6573 2e61 6374 696f  properties.actio
+000004b0: 6e5f 6c69 6e6b 0a20 2020 2020 2020 2074  n_link.        t
+000004c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+000004d0: 7265 7175 6573 7473 2e67 6574 2861 6374  requests.get(act
+000004e0: 696f 6e5f 6c69 6e6b 290a 2020 2020 2020  ion_link).      
+000004f0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00000500: 6f6e 2061 7320 653a 2020 2320 6e6f 7161  on as e:  # noqa
+00000510: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00000520: 7365 2065 0a20 2020 2020 2020 2061 7574  se e.        aut
+00000530: 685f 7265 7370 6f6e 7365 203d 2068 7562  h_response = hub
+00000540: 2e61 7574 682e 7369 676e 5f69 6e5f 7769  .auth.sign_in_wi
+00000550: 7468 5f70 6173 7377 6f72 6428 0a20 2020  th_password(.   
+00000560: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00000570: 2020 2020 2020 2020 2020 2022 656d 6169             "emai
+00000580: 6c22 3a20 656d 6169 6c2c 0a20 2020 2020  l": email,.     
+00000590: 2020 2020 2020 2020 2020 2022 7061 7373             "pass
+000005a0: 776f 7264 223a 2070 6173 7377 6f72 642c  word": password,
+000005b0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+000005c0: 2020 2020 2020 2029 0a20 2020 2065 6c73         ).    els
+000005d0: 653a 0a20 2020 2020 2020 2068 7562 203d  e:.        hub =
+000005e0: 2063 6f6e 6e65 6374 5f68 7562 2829 0a20   connect_hub(). 
+000005f0: 2020 2020 2020 2061 7574 685f 7265 7370         auth_resp
+00000600: 6f6e 7365 203d 2068 7562 2e61 7574 682e  onse = hub.auth.
+00000610: 7369 676e 5f75 7028 0a20 2020 2020 2020  sign_up(.       
+00000620: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000630: 2020 2020 2020 2022 656d 6169 6c22 3a20         "email": 
+00000640: 656d 6169 6c2c 0a20 2020 2020 2020 2020  email,.         
+00000650: 2020 2020 2020 2022 7061 7373 776f 7264         "password
+00000660: 223a 2070 6173 7377 6f72 642c 0a20 2020  ": password,.   
+00000670: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00000680: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
+00000690: 207b 0a20 2020 2020 2020 2022 6861 6e64   {.        "hand
+000006a0: 6c65 223a 2068 616e 646c 652c 0a20 2020  le": handle,.   
+000006b0: 2020 2020 2022 656d 6169 6c22 3a20 656d       "email": em
+000006c0: 6169 6c2c 0a20 2020 2020 2020 2022 7061  ail,.        "pa
+000006d0: 7373 776f 7264 223a 2070 6173 7377 6f72  ssword": passwor
+000006e0: 642c 0a20 2020 2020 2020 2022 6964 223a  d,.        "id":
+000006f0: 2073 7472 2861 7574 685f 7265 7370 6f6e   str(auth_respon
+00000700: 7365 2e73 6573 7369 6f6e 2e75 7365 722e  se.session.user.
+00000710: 6964 292c 0a20 2020 2020 2020 2022 6163  id),.        "ac
+00000720: 6365 7373 5f74 6f6b 656e 223a 2061 7574  cess_token": aut
+00000730: 685f 7265 7370 6f6e 7365 2e73 6573 7369  h_response.sessi
+00000740: 6f6e 2e61 6363 6573 735f 746f 6b65 6e2c  on.access_token,
+00000750: 0a20 2020 2020 2020 2022 7365 7373 696f  .        "sessio
+00000760: 6e22 3a20 6175 7468 5f72 6573 706f 6e73  n": auth_respons
+00000770: 652e 7365 7373 696f 6e2c 0a20 2020 207d  e.session,.    }
+00000780: 0a0a 0a64 6566 2063 7265 6174 655f 7465  ...def create_te
+00000790: 7374 5f61 6363 6f75 6e74 280a 2020 2020  st_account(.    
+000007a0: 6861 6e64 6c65 3a20 7374 722c 0a20 2020  handle: str,.   
+000007b0: 2061 6363 6573 735f 746f 6b65 6e3a 2073   access_token: s
+000007c0: 7472 2c0a 2020 2020 6f72 6761 6e69 7a61  tr,.    organiza
+000007d0: 7469 6f6e 3a20 556e 696f 6e5b 626f 6f6c  tion: Union[bool
+000007e0: 2c20 4e6f 6e65 5d20 3d20 4661 6c73 652c  , None] = False,
+000007f0: 0a29 3a0a 2020 2020 6875 6220 3d20 636f  .):.    hub = co
+00000800: 6e6e 6563 745f 6875 625f 7769 7468 5f61  nnect_hub_with_a
+00000810: 7574 6828 6163 6365 7373 5f74 6f6b 656e  uth(access_token
+00000820: 3d61 6363 6573 735f 746f 6b65 6e29 0a0a  =access_token)..
+00000830: 2020 2020 6163 636f 756e 745f 6964 203d      account_id =
+00000840: 2065 7874 7261 6374 5f69 6428 6163 6365   extract_id(acce
+00000850: 7373 5f74 6f6b 656e 290a 0a20 2020 2061  ss_token)..    a
+00000860: 6363 6f75 6e74 203d 2073 625f 696e 7365  ccount = sb_inse
+00000870: 7274 5f61 6363 6f75 6e74 280a 2020 2020  rt_account(.    
+00000880: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00000890: 2020 2269 6422 3a20 6163 636f 756e 745f    "id": account_
+000008a0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+000008b0: 226c 6e69 6422 3a20 6261 7365 3632 2838  "lnid": base62(8
+000008c0: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
+000008d0: 6861 6e64 6c65 223a 2068 616e 646c 652c  handle": handle,
+000008e0: 0a20 2020 2020 2020 2020 2020 2022 7573  .            "us
+000008f0: 6572 5f69 6422 3a20 4e6f 6e65 2069 6620  er_id": None if 
+00000900: 6f72 6761 6e69 7a61 7469 6f6e 2065 6c73  organization els
+00000910: 6520 6163 636f 756e 745f 6964 2c0a 2020  e account_id,.  
+00000920: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000930: 2068 7562 2c0a 2020 2020 290a 0a20 2020   hub,.    )..   
+00000940: 2068 7562 2e61 7574 682e 7369 676e 5f6f   hub.auth.sign_o
+00000950: 7574 2829 0a0a 2020 2020 7265 7475 726e  ut()..    return
+00000960: 2061 6363 6f75 6e74 0a0a 0a64 6566 2063   account...def c
+00000970: 7265 6174 655f 7465 7374 5f69 6e73 7461  reate_test_insta
+00000980: 6e63 6528 7374 6f72 6167 655f 6964 3a20  nce(storage_id: 
+00000990: 7374 722c 2061 6363 6573 735f 746f 6b65  str, access_toke
+000009a0: 6e3a 2073 7472 293a 0a20 2020 2068 7562  n: str):.    hub
+000009b0: 203d 2063 6f6e 6e65 6374 5f68 7562 5f77   = connect_hub_w
+000009c0: 6974 685f 6175 7468 2861 6363 6573 735f  ith_auth(access_
+000009d0: 746f 6b65 6e3d 6163 6365 7373 5f74 6f6b  token=access_tok
+000009e0: 656e 290a 0a20 2020 2061 6363 6f75 6e74  en)..    account
+000009f0: 5f69 6420 3d20 6578 7472 6163 745f 6964  _id = extract_id
+00000a00: 2861 6363 6573 735f 746f 6b65 6e29 0a0a  (access_token)..
+00000a10: 2020 2020 6e61 6d65 203d 2066 226c 616d      name = f"lam
+00000a20: 696e 2e63 692e 696e 7374 616e 6365 2e7b  in.ci.instance.{
+00000a30: 6261 7365 3632 2836 297d 220a 0a20 2020  base62(6)}"..   
+00000a40: 2069 6e73 7461 6e63 6520 3d20 7362 5f69   instance = sb_i
+00000a50: 6e73 6572 745f 696e 7374 616e 6365 280a  nsert_instance(.
+00000a60: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00000a70: 2020 2020 2020 2269 6422 3a20 7575 6964        "id": uuid
+00000a80: 2e75 7569 6434 2829 2e68 6578 2c0a 2020  .uuid4().hex,.  
+00000a90: 2020 2020 2020 2020 2020 2261 6363 6f75            "accou
+00000aa0: 6e74 5f69 6422 3a20 6163 636f 756e 745f  nt_id": account_
+00000ab0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00000ac0: 226e 616d 6522 3a20 6e61 6d65 2c0a 2020  "name": name,.  
+00000ad0: 2020 2020 2020 2020 2020 2273 746f 7261            "stora
+00000ae0: 6765 5f69 6422 3a20 7374 6f72 6167 655f  ge_id": storage_
+00000af0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00000b00: 2270 7562 6c69 6322 3a20 5472 7565 2c0a  "public": True,.
+00000b10: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000b20: 2020 2068 7562 2c0a 2020 2020 290a 0a20     hub,.    ).. 
+00000b30: 2020 2068 7562 2e61 7574 682e 7369 676e     hub.auth.sign
+00000b40: 5f6f 7574 2829 0a0a 2020 2020 7265 7475  _out()..    retu
+00000b50: 726e 2069 6e73 7461 6e63 650a 0a0a 6465  rn instance...de
+00000b60: 6620 6372 6561 7465 5f74 6573 745f 7374  f create_test_st
+00000b70: 6f72 6167 6528 6163 6365 7373 5f74 6f6b  orage(access_tok
+00000b80: 656e 3a20 7374 7229 3a0a 2020 2020 6875  en: str):.    hu
+00000b90: 6220 3d20 636f 6e6e 6563 745f 6875 625f  b = connect_hub_
+00000ba0: 7769 7468 5f61 7574 6828 6163 6365 7373  with_auth(access
+00000bb0: 5f74 6f6b 656e 3d61 6363 6573 735f 746f  _token=access_to
+00000bc0: 6b65 6e29 0a0a 2020 2020 726f 6f74 203d  ken)..    root =
+00000bd0: 2066 226c 616d 696e 2e63 692e 7374 6f72   f"lamin.ci.stor
+00000be0: 6167 652e 7b62 6173 6536 3228 3629 7d22  age.{base62(6)}"
+00000bf0: 0a20 2020 2061 6363 6f75 6e74 5f69 6420  .    account_id 
+00000c00: 3d20 6578 7472 6163 745f 6964 2861 6363  = extract_id(acc
+00000c10: 6573 735f 746f 6b65 6e29 0a0a 2020 2020  ess_token)..    
+00000c20: 7374 6f72 6167 6520 3d20 7362 5f69 6e73  storage = sb_ins
+00000c30: 6572 745f 7374 6f72 6167 6528 0a20 2020  ert_storage(.   
+00000c40: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000c50: 2020 2022 6964 223a 2075 7569 642e 7575     "id": uuid.uu
+00000c60: 6964 3428 292e 6865 782c 0a20 2020 2020  id4().hex,.     
+00000c70: 2020 2020 2020 2022 6c6e 6964 223a 2062         "lnid": b
+00000c80: 6173 6536 3228 3829 2c0a 2020 2020 2020  ase62(8),.      
+00000c90: 2020 2020 2020 2263 7265 6174 6564 5f62        "created_b
+00000ca0: 7922 3a20 6163 636f 756e 745f 6964 2c0a  y": account_id,.
+00000cb0: 2020 2020 2020 2020 2020 2020 2272 6f6f              "roo
+00000cc0: 7422 3a20 726f 6f74 2c0a 2020 2020 2020  t": root,.      
+00000cd0: 2020 2020 2020 2272 6567 696f 6e22 3a20        "region": 
+00000ce0: 2275 732d 6561 7374 2d31 222c 0a20 2020  "us-east-1",.   
+00000cf0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00000d00: 2022 7333 222c 0a20 2020 2020 2020 207d   "s3",.        }
+00000d10: 2c0a 2020 2020 2020 2020 6875 622c 0a20  ,.        hub,. 
+00000d20: 2020 2029 0a0a 2020 2020 6875 622e 6175     )..    hub.au
+00000d30: 7468 2e73 6967 6e5f 6f75 7428 290a 0a20  th.sign_out().. 
+00000d40: 2020 2072 6574 7572 6e20 7374 6f72 6167     return storag
+00000d50: 650a 0a0a 6465 6620 6164 645f 7465 7374  e...def add_test
+00000d60: 5f63 6f6c 6c61 626f 7261 746f 7228 0a20  _collaborator(. 
+00000d70: 2020 2069 6e73 7461 6e63 655f 6964 3a20     instance_id: 
+00000d80: 7374 722c 0a20 2020 2061 6363 6f75 6e74  str,.    account
+00000d90: 5f69 643a 2073 7472 2c0a 2020 2020 726f  _id: str,.    ro
+00000da0: 6c65 3a20 7374 722c 0a20 2020 2061 6363  le: str,.    acc
+00000db0: 6573 735f 746f 6b65 6e3a 2073 7472 2c0a  ess_token: str,.
+00000dc0: 293a 0a20 2020 2068 7562 203d 2063 6f6e  ):.    hub = con
+00000dd0: 6e65 6374 5f68 7562 5f77 6974 685f 6175  nect_hub_with_au
+00000de0: 7468 2861 6363 6573 735f 746f 6b65 6e3d  th(access_token=
+00000df0: 6163 6365 7373 5f74 6f6b 656e 290a 0a20  access_token).. 
+00000e00: 2020 2063 6f6c 6c61 626f 7261 746f 7220     collaborator 
+00000e10: 3d20 7362 5f69 6e73 6572 745f 636f 6c6c  = sb_insert_coll
+00000e20: 6162 6f72 6174 6f72 280a 2020 2020 2020  aborator(.      
+00000e30: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00000e40: 2269 6e73 7461 6e63 655f 6964 223a 2069  "instance_id": i
+00000e50: 6e73 7461 6e63 655f 6964 2c0a 2020 2020  nstance_id,.    
+00000e60: 2020 2020 2020 2020 2261 6363 6f75 6e74          "account
+00000e70: 5f69 6422 3a20 6163 636f 756e 745f 6964  _id": account_id
+00000e80: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+00000e90: 6f6c 6522 3a20 726f 6c65 2c0a 2020 2020  ole": role,.    
+00000ea0: 2020 2020 7d2c 0a20 2020 2020 2020 2068      },.        h
+00000eb0: 7562 2c0a 2020 2020 290a 0a20 2020 2068  ub,.    )..    h
+00000ec0: 7562 2e61 7574 682e 7369 676e 5f6f 7574  ub.auth.sign_out
+00000ed0: 2829 0a0a 2020 2020 7265 7475 726e 2063  ()..    return c
+00000ee0: 6f6c 6c61 626f 7261 746f 720a            ollaborator.
```

### Comparing `lnhub_rest-0.9.8/lndb/lndb/_migrate/alembic.ini` & `lnhub_rest-0.9.9/lnhub_rest/schema/alembic.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-[{schema_id}]
-script_location = {package_dir}/migrations
+[cbwk]
+script_location = lnhub_rest/schema/migrations
 file_template = %%(year)d-%%(month).2d-%%(day).2d-%%(rev)s-%%(slug)s
 prepend_sys_path = .
 version_path_separator = os
-sqlalchemy.url = sqlite:///testdb/testdb.lndb
 
 # Logging configuration
 [loggers]
 keys = root,sqlalchemy,alembic
 
 [handlers]
 keys = console
```

### Comparing `lnhub_rest-0.9.8/lndb/pyproject.toml` & `lnhub_rest-0.9.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
-name = "lndb"
+name = "lnhub_rest"
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
-    # PINNED internal LAMIN dependency
-    # !!! lnhub_rest cannot be pinned in LaminDB !!!
-    # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.9.2",
-    # NO other Lamin packages should be pinned or even be a dependency
-    "laminci>=0.3.0",  # disentangle over time
-    "lnschema_core>=0.28.0",
-    "lamin_logger>=0.2.3",
-    # External dependencies
-    "pytest_alembic==0.9.1",  # let's pin this as we use internals
-    "cloudpathlib",  # we can remove this once lnschema-core is released (2023-04-07)
-    "sqlmodel>=0.0.8",
-    "psycopg2-binary",
-    "appdirs",
-    "python-dotenv",
-    "erdiagram",
-    "alembic",
-    "natsort",
-    "pandas",
-    "python-dateutil",
+    # Do NOT add any lamin package as a dependency here!
+    # Neither laminci nor lndb nor lnschema_core etc.
+    # lnhub_rest needs to be upstream
+    "lamin_logger",
+    "supabase==1.0.3",
+    "pyjwt",
 ]
 
 [project.urls]
-Home = "https://github.com/laminlabs/lndb"
+Home = "https://github.com/laminlabs/lnhub-rest"
 
 [project.optional-dependencies]
+server = [
+    "fastapi",
+    "uvicorn",
+    "sqlmodel",
+    "alembic",
+    "pytest_alembic==0.9.1",  # let's pin this as we use internals
+    "psycopg2-binary",
+]
 dev = [
     "pre-commit",
     "nox",
 ]
 test = [
-    "lamindb[bionty,lamin1]>=0.39rc1",
     "pytest>=6.0",
     "pytest-cov",
-    "nbproject-test>=0.4.3",
     "nbproject",
+    "botocore",
 ]
 
 [project.scripts]
-lndb = "lndb.__main__:main"
+lnhub = "lnhub_rest.__main__:main"
 
 [tool.black]
 preview = true
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
+markers = [
+    "integration: marks tests as integration tests (i.e. 'staging' or 'prod' branches)",
+    "local"
+]
 
 [tool.coverage.run]
 omit = [
-    "lndb/*",
+    "lnhub_rest/*",
 ]
```

### Comparing `lnhub_rest-0.9.8/lnhub_rest/__main__.py` & `lnhub_rest-0.9.9/lnhub_rest/__main__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/_assets/_schemas.py` & `lnhub_rest-0.9.9/lnhub_rest/_assets/_schemas.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/_check_breaks_lndb.py` & `lnhub_rest-0.9.9/lnhub_rest/_check_breaks_lndb.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/_ci.py` & `lnhub_rest-0.9.9/lnhub_rest/_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/_clean_ci.py` & `lnhub_rest-0.9.9/lnhub_rest/_clean_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/config.py` & `lnhub_rest-0.9.9/lnhub_rest/config.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/account/_create_account.py` & `lnhub_rest-0.9.9/lnhub_rest/core/account/_create_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/account/_crud.py` & `lnhub_rest-0.9.9/lnhub_rest/core/account/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/account/_delete_account.py` & `lnhub_rest-0.9.9/lnhub_rest/core/account/_delete_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/account/_signup_signin.py` & `lnhub_rest-0.9.9/lnhub_rest/core/account/_signup_signin.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/account/_update_account.py` & `lnhub_rest-0.9.9/lnhub_rest/core/account/_update_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/collaborator/_crud.py` & `lnhub_rest-0.9.9/lnhub_rest/core/collaborator/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/instance/_crud.py` & `lnhub_rest-0.9.9/lnhub_rest/core/instance/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/instance/_delete_instance.py` & `lnhub_rest-0.9.9/lnhub_rest/core/instance/_delete_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/instance/_init_instance.py` & `lnhub_rest-0.9.9/lnhub_rest/core/instance/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/instance/_load_instance.py` & `lnhub_rest-0.9.9/lnhub_rest/core/instance/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/instance/_update_instance.py` & `lnhub_rest-0.9.9/lnhub_rest/core/instance/_update_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/member/_crud.py` & `lnhub_rest-0.9.9/lnhub_rest/core/member/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/storage/_add_storage.py` & `lnhub_rest-0.9.9/lnhub_rest/core/storage/_add_storage.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/core/storage/_crud.py` & `lnhub_rest-0.9.9/lnhub_rest/core/storage/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/main.py` & `lnhub_rest-0.9.9/lnhub_rest/main.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/orm/_sbclient.py` & `lnhub_rest-0.9.9/lnhub_rest/orm/_sbclient.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/routers/account.py` & `lnhub_rest-0.9.9/lnhub_rest/routers/account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/routers/ci.py` & `lnhub_rest-0.9.9/lnhub_rest/routers/ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/routers/collaborator.py` & `lnhub_rest-0.9.9/lnhub_rest/routers/collaborator.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/routers/instance.py` & `lnhub_rest-0.9.9/lnhub_rest/routers/instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/routers/organization.py` & `lnhub_rest-0.9.9/lnhub_rest/routers/organization.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/routers/utils.py` & `lnhub_rest-0.9.9/lnhub_rest/routers/utils.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/_core.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/_core.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/_versions.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/_versions.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/clone.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/env.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/script.py.mako` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/testing.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/testing.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py` & `lnhub_rest-0.9.9/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/noxfile.py` & `lnhub_rest-0.9.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/supabase/config.toml` & `lnhub_rest-0.9.9/supabase/config.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.8/tests/test_notebooks.py` & `lnhub_rest-0.9.9/tests/test_notebooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from pathlib import Path
 
+import nbproject_test as test
 import pytest
 from nbproject._logger import logger
-from nbproject.dev import test
 
 from lnhub_rest._ci import start_local_supabase
 
 # assuming this is in the tests folder
 DOCS_FOLDER = Path(__file__).parents[1] / "docs/"
 LAMIN_ENV = os.environ.get("LAMIN_ENV", "local")
```

### Comparing `lnhub_rest-0.9.8/PKG-INFO` & `lnhub_rest-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnhub_rest
-Version: 0.9.8
+Version: 0.9.9
 Summary: Rest API for the hub.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamin_logger
 Requires-Dist: supabase==1.0.3
 Requires-Dist: pyjwt
 Requires-Dist: pre-commit ; extra == "dev"
```

