# Comparing `tmp/chromadb-client-0.3.30.dev0.tar.gz` & `tmp/chromadb-client-0.4.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-client-0.3.30.dev0.tar", last modified: Wed Jul 12 19:54:58 2023, max compression
+gzip compressed data, was "chromadb-client-0.4.1.dev0.tar", last modified: Mon Jul 17 23:18:33 2023, max compression
```

## Comparing `chromadb-client-0.3.30.dev0.tar` & `chromadb-client-0.4.1.dev0.tar`

### file list

```diff
@@ -1,242 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.410934 chromadb-client-0.3.30.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.422934 chromadb-client-0.3.30.dev0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.422934 chromadb-client-0.3.30.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.github/workflows/chroma-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.github/workflows/chroma-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.422934 chromadb-client-0.3.30.dev0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-12 19:54:51.000000 chromadb-client-0.3.30.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/RELEASE_PROCESS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.422934 chromadb-client-0.3.30.dev0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/backup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/build
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/docker_entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/generate_cloudformation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/integration-test
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/restore.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/setup_linux.sh
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/setup_mac.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.422934 chromadb-client-0.3.30.dev0/bin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/templates/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/test-package.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      297 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/test-remote
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/bin/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.426934 chromadb-client-0.3.30.dev0/chromadb/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.426934 chromadb-client-0.3.30.dev0/chromadb/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10852 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/api/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    19109 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/api/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.426934 chromadb-client-0.3.30.dev0/chromadb/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/api/models/Collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/api/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.426934 chromadb-client-0.3.30.dev0/chromadb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.426934 chromadb-client-0.3.30.dev0/chromadb/db/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/impl/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.426934 chromadb-client-0.3.30.dev0/chromadb/db/index/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/index/hnswlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.426934 chromadb-client-0.3.30.dev0/chromadb/db/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/db/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.426934 chromadb-client-0.3.30.dev0/chromadb/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)   368824 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/experimental/density_relevance.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.426934 chromadb-client-0.3.30.dev0/chromadb/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 19:54:51.000000 chromadb-client-0.3.30.dev0/chromadb/is_thin_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.426934 chromadb-client-0.3.30.dev0/chromadb/segment/
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.414934 chromadb-client-0.3.30.dev0/chromadb/segment/impl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.430934 chromadb-client-0.3.30.dev0/chromadb/segment/impl/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.430934 chromadb-client-0.3.30.dev0/chromadb/segment/impl/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.430934 chromadb-client-0.3.30.dev0/chromadb/segment/impl/vector/
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/segment/impl/vector/local_hnsw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.430934 chromadb-client-0.3.30.dev0/chromadb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.430934 chromadb-client-0.3.30.dev0/chromadb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.430934 chromadb-client-0.3.30.dev0/chromadb/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/telemetry/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.430934 chromadb-client-0.3.30.dev0/chromadb/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.430934 chromadb-client-0.3.30.dev0/chromadb/test/db/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.434934 chromadb-client-0.3.30.dev0/chromadb/test/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/db/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/db/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/db/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.434934 chromadb-client-0.3.30.dev0/chromadb/test/hnswlib/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/hnswlib/test_hnswlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.434934 chromadb-client-0.3.30.dev0/chromadb/test/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.434934 chromadb-client-0.3.30.dev0/chromadb/test/property/
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/property/invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19043 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/property/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/property/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/property/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/property/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.434934 chromadb-client-0.3.30.dev0/chromadb/test/segment/
--rw-r--r--   0 runner    (1001) docker     (123)    15132 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/segment/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    40736 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/test_chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.434934 chromadb-client-0.3.30.dev0/chromadb/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.434934 chromadb-client-0.3.30.dev0/chromadb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/utils/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/chromadb/utils/messageid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.438934 chromadb-client-0.3.30.dev0/chromadb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-12 19:54:58.000000 chromadb-client-0.3.30.dev0/chromadb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-12 19:54:58.000000 chromadb-client-0.3.30.dev0/chromadb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:54:58.000000 chromadb-client-0.3.30.dev0/chromadb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 19:54:58.000000 chromadb-client-0.3.30.dev0/chromadb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 19:54:58.000000 chromadb-client-0.3.30.dev0/chromadb_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.414934 chromadb-client-0.3.30.dev0/clients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.442935 chromadb-client-0.3.30.dev0/clients/js/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/.prettierrc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.414934 chromadb-client-0.3.30.dev0/clients/js/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.442935 chromadb-client-0.3.30.dev0/clients/js/examples/browser/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/examples/browser/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/examples/browser/app.ts
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/examples/browser/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/examples/browser/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.442935 chromadb-client-0.3.30.dev0/clients/js/examples/node/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/examples/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/examples/node/app.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/examples/node/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/genapi.sh
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/jest.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/openapitools.json
--rw-r--r--   0 runner    (1001) docker     (123)   448020 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.442935 chromadb-client-0.3.30.dev0/clients/js/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/ChromaClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/Collection.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.446935 chromadb-client-0.3.30.dev0/clients/js/src/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
--rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.446935 chromadb-client-0.3.30.dev0/clients/js/src/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/generated/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    56700 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/generated/api.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/generated/configuration.ts
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/generated/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/generated/models.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/generated/runtime.ts
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/types.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/src/utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/clients/js/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/add.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/collection.client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/data.ts
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/get.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/initClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/query.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/update.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/tsconfig.module.json
--rw-r--r--   0 runner    (1001) docker     (123)   156893 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/js/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/clients/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/python/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/python/integration-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/python/is_thin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/clients/python/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/config/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/config/backup_disk.xml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/config/chroma_users.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/docker-compose.server.example.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/docker-compose.test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/examples/basic_functionality/
--rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/basic_functionality/alternative_embeddings.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/basic_functionality/local_persistence.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/basic_functionality/where_filtering.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.418934 chromadb-client-0.3.30.dev0/examples/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/examples/deployments/google-cloud-compute/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/deployments/google-cloud-compute/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.418934 chromadb-client-0.3.30.dev0/examples/use_with/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/examples/use_with/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/use_with/cohere/cohere_js.js
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/use_with/cohere/cohere_python.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/examples/use_with/cohere/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/log_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.418934 chromadb-client-0.3.30.dev0/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/migrations/embeddings_queue/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/migrations/metadb/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/migrations/metadb/00001-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:54:58.450935 chromadb-client-0.3.30.dev0/migrations/sysdb/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/migrations/sysdb/00003-collection-dimension.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-12 19:54:51.000000 chromadb-client-0.3.30.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 19:54:38.000000 chromadb-client-0.3.30.dev0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 19:54:58.454935 chromadb-client-0.3.30.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.379676 chromadb-client-0.4.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.303675 chromadb-client-0.4.1.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.311675 chromadb-client-0.4.1.dev0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.311675 chromadb-client-0.4.1.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.github/workflows/chroma-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.github/workflows/chroma-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.311675 chromadb-client-0.4.1.dev0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-17 23:18:33.375676 chromadb-client-0.4.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-17 23:18:27.000000 chromadb-client-0.4.1.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/RELEASE_PROCESS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.315675 chromadb-client-0.4.1.dev0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/bin/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/bin/docker_entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/bin/generate_cloudformation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/bin/integration-test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.315675 chromadb-client-0.4.1.dev0/bin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/bin/test-package.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/bin/test-remote
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/bin/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/bin/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.315675 chromadb-client-0.4.1.dev0/chromadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.315675 chromadb-client-0.4.1.dev0/chromadb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/api/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.315675 chromadb-client-0.4.1.dev0/chromadb/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/api/models/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/api/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.315675 chromadb-client-0.4.1.dev0/chromadb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.315675 chromadb-client-0.4.1.dev0/chromadb/db/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/db/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/db/impl/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/db/impl/sqlite_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/db/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.315675 chromadb-client-0.4.1.dev0/chromadb/db/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/db/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.315675 chromadb-client-0.4.1.dev0/chromadb/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)   368824 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/experimental/density_relevance.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/ingest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:18:27.000000 chromadb-client-0.4.1.dev0/chromadb/is_thin_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/migrations/embeddings_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/migrations/metadb/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/migrations/sysdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.303675 chromadb-client-0.4.1.dev0/chromadb/segment/impl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/segment/impl/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/segment/impl/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/segment/impl/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/segment/impl/vector/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/segment/impl/vector/brute_force_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/segment/impl/vector/hnsw_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/segment/impl/vector/local_hnsw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/segment/impl/vector/local_persistent_hnsw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.327675 chromadb-client-0.4.1.dev0/chromadb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.331675 chromadb-client-0.4.1.dev0/chromadb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.335675 chromadb-client-0.4.1.dev0/chromadb/test/db/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.335675 chromadb-client-0.4.1.dev0/chromadb/test/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/db/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/db/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.339675 chromadb-client-0.4.1.dev0/chromadb/test/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.339675 chromadb-client-0.4.1.dev0/chromadb/test/property/
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/property/invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/property/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/property/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/property/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.343675 chromadb-client-0.4.1.dev0/chromadb/test/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/segment/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41277 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/test_chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/test_multithreaded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.343675 chromadb-client-0.4.1.dev0/chromadb/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.343675 chromadb-client-0.4.1.dev0/chromadb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/utils/distance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/utils/messageid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/chromadb/utils/read_write_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.347675 chromadb-client-0.4.1.dev0/chromadb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-17 23:18:33.000000 chromadb-client-0.4.1.dev0/chromadb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-17 23:18:33.000000 chromadb-client-0.4.1.dev0/chromadb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:18:33.000000 chromadb-client-0.4.1.dev0/chromadb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 23:18:33.000000 chromadb-client-0.4.1.dev0/chromadb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 23:18:33.000000 chromadb-client-0.4.1.dev0/chromadb_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.307675 chromadb-client-0.4.1.dev0/clients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.351675 chromadb-client-0.4.1.dev0/clients/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/.prettierrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.307675 chromadb-client-0.4.1.dev0/clients/js/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.355676 chromadb-client-0.4.1.dev0/clients/js/examples/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/examples/browser/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/examples/browser/app.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/examples/browser/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/examples/browser/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.355676 chromadb-client-0.4.1.dev0/clients/js/examples/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/examples/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/examples/node/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/examples/node/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/genapi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/jest.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/openapitools.json
+-rw-r--r--   0 runner    (1001) docker     (123)   448020 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.359676 chromadb-client-0.4.1.dev0/clients/js/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/Collection.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.363676 chromadb-client-0.4.1.dev0/clients/js/src/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.363676 chromadb-client-0.4.1.dev0/clients/js/src/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/generated/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    54547 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/generated/api.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/generated/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/generated/models.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/types.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/src/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.367676 chromadb-client-0.4.1.dev0/clients/js/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/data.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/initClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/tsconfig.module.json
+-rw-r--r--   0 runner    (1001) docker     (123)   156893 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/js/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.371676 chromadb-client-0.4.1.dev0/clients/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/python/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/python/integration-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/python/is_thin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/clients/python/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/docker-compose.server.example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/docker-compose.test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.371676 chromadb-client-0.4.1.dev0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.371676 chromadb-client-0.4.1.dev0/examples/basic_functionality/
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/basic_functionality/alternative_embeddings.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/basic_functionality/local_persistence.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/basic_functionality/where_filtering.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.307675 chromadb-client-0.4.1.dev0/examples/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.375676 chromadb-client-0.4.1.dev0/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/deployments/google-cloud-compute/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.307675 chromadb-client-0.4.1.dev0/examples/use_with/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:33.375676 chromadb-client-0.4.1.dev0/examples/use_with/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/use_with/cohere/cohere_js.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/use_with/cohere/cohere_python.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/examples/use_with/cohere/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/log_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-17 23:18:27.000000 chromadb-client-0.4.1.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-17 23:18:15.000000 chromadb-client-0.4.1.dev0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:18:33.379676 chromadb-client-0.4.1.dev0/setup.cfg
```

### Comparing `chromadb-client-0.3.30.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `chromadb-client-0.4.1.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `chromadb-client-0.4.1.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `chromadb-client-0.4.1.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/.github/workflows/chroma-client-integration-test.yml` & `chromadb-client-0.4.1.dev0/.github/workflows/chroma-client-integration-test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on:
   push:
     branches:
       - main
   pull_request:
     branches:
       - main
-      - '*'
+      - '**'
 
 jobs:
   test:
     timeout-minutes: 90
     strategy:
       matrix:
         python: ['3.7', '3.8', '3.9', '3.10']
```

### Comparing `chromadb-client-0.3.30.dev0/.github/workflows/chroma-integration-test.yml` & `chromadb-client-0.4.1.dev0/.github/workflows/chroma-integration-test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   push:
     branches:
       - main
       - team/hypothesis-tests
   pull_request:
     branches:
       - main
-      - '*'
+      - '**'
 
 jobs:
   test:
     strategy:
       matrix:
         python: ['3.7']
         platform: [ubuntu-latest]
```

### Comparing `chromadb-client-0.3.30.dev0/.github/workflows/chroma-release-python-client.yml` & `chromadb-client-0.4.1.dev0/.github/workflows/chroma-release-python-client.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/.github/workflows/chroma-release.yml` & `chromadb-client-0.4.1.dev0/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/.github/workflows/chroma-test.yml` & `chromadb-client-0.4.1.dev0/.github/workflows/chroma-test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   push:
     branches:
       - main
       - team/hypothesis-tests
   pull_request:
     branches:
       - main
-      - '*'
+      - '**'
 
 jobs:
   test:
     timeout-minutes: 90
     strategy:
       matrix:
         python: ['3.7', '3.8', '3.9', '3.10']
```

### Comparing `chromadb-client-0.3.30.dev0/.github/workflows/pr-review-checklist.yml` & `chromadb-client-0.4.1.dev0/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/.pre-commit-config.yaml` & `chromadb-client-0.4.1.dev0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/.vscode/settings.json` & `chromadb-client-0.4.1.dev0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/DEVELOP.md` & `chromadb-client-0.4.1.dev0/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/Dockerfile` & `chromadb-client-0.4.1.dev0/Dockerfile`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-FROM python:3.10-slim-bullseye as builder
+FROM python:3.10-slim-bookworm as builder
 
 #RUN apt-get update -qq
 #RUN apt-get install python3.10 python3-pip -y --no-install-recommends && rm -rf /var/lib/apt/lists_/*
 RUN apt-get update --fix-missing && apt-get install -y --fix-missing build-essential
 
 RUN mkdir /install
 WORKDIR /install
 
 COPY ./requirements.txt requirements.txt
 
 RUN pip install --no-cache-dir --upgrade --prefix="/install" -r requirements.txt
 
-FROM python:3.10-slim-bullseye as final
+FROM python:3.10-slim-bookworm as final
 
 RUN mkdir /chroma
 WORKDIR /chroma
 
 COPY --from=builder /install /usr/local
 COPY ./bin/docker_entrypoint.sh /docker_entrypoint.sh
 COPY ./ /chroma
```

### Comparing `chromadb-client-0.3.30.dev0/LICENSE` & `chromadb-client-0.4.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/PKG-INFO` & `chromadb-client-0.4.1.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb-client
-Version: 0.3.30.dev0
+Version: 0.4.1.dev0
 Summary: Chroma Client.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -26,19 +26,16 @@
 pip install chromadb-client # python http-client only library
 ```
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
-from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest",
-                                  chroma_server_host="localhost",
-                                  chroma_server_http_port=8000))
+client = chromadb.HttpClient(host="localhost", port=8000)
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -1,28 +1,26 @@
-Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.30.dev0 Summary:
-Chroma Client. Author-email: Jeff Huber
+Metadata-Version: 2.1 Name: chromadb-client Version: 0.4.1.dev0 Summary: Chroma
+Client. Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
                                  [Chroma_logo]
                  Chroma - the open-source embedding database.
  This package is for the the Python HTTP client-only library for Chroma. This
 client connects to the Chroma Server. If that it not what you are looking for,
                  you might want to check out the full_library.
 ```bash pip install chromadb-client # python http-client only library ``` To
 connect to your server and perform operations using the client only library,
-you can do the following: ```python import chromadb from chromadb.config import
-Settings # Example setup of the client to connect to your chroma server client
-= chromadb.Client(Settings(chroma_api_impl="rest",
-chroma_server_host="localhost", chroma_server_http_port=8000)) collection =
-client.create_collection("all-my-documents") collection.add( documents=["This
-is document1", "This is document2"], metadatas=[{"source": "notion"},
-{"source": "google-docs"}], # filter on these! ids=["doc1", "doc2"], # unique
-for each doc embeddings = [[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results =
-collection.query( query_texts=["This is a query document"], n_results=2, #
-where={"metadata_field": "is_equal_to_this"}, # optional filter #
-where_document={"$contains":"search_string"} # optional filter ) ``` ## License
-[Apache 2.0](./LICENSE)
+you can do the following: ```python import chromadb # Example setup of the
+client to connect to your chroma server client = chromadb.HttpClient
+(host="localhost", port=8000) collection = client.create_collection("all-my-
+documents") collection.add( documents=["This is document1", "This is
+document2"], metadatas=[{"source": "notion"}, {"source": "google-docs"}], #
+filter on these! ids=["doc1", "doc2"], # unique for each doc embeddings = [
+[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results = collection.query( query_texts=
+["This is a query document"], n_results=2, # where={"metadata_field":
+"is_equal_to_this"}, # optional filter # where_document={"$contains":
+"search_string"} # optional filter ) ``` ## License [Apache 2.0](./LICENSE)
```

### Comparing `chromadb-client-0.3.30.dev0/README.md` & `chromadb-client-0.4.1.dev0/chromadb_client.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: chromadb-client
+Version: 0.4.1.dev0
+Summary: Chroma Client.
+Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
+Project-URL: Homepage, https://github.com/chroma-core/chroma
+Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <a href="https://trychroma.com"><img src="https://user-images.githubusercontent.com/891664/227103090-6624bf7d-9524-4e05-9d2c-c28d5d451481.png" alt="Chroma logo"></a>
 </p>
 
 <p align="center">
     <b>Chroma - the open-source embedding database</b>. <br />
     This package is for the the Python HTTP client-only library for Chroma. This client connects to the Chroma Server. If that it not what you are looking for, you might want to check out the <a href="https://github.com/chroma-core/chroma ">full library</a>.
@@ -12,19 +26,16 @@
 pip install chromadb-client # python http-client only library
 ```
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
-from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest",
-                                  chroma_server_host="localhost",
-                                  chroma_server_http_port=8000))
+client = chromadb.HttpClient(host="localhost", port=8000)
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -1,19 +1,26 @@
+Metadata-Version: 2.1 Name: chromadb-client Version: 0.4.1.dev0 Summary: Chroma
+Client. Author-email: Jeff Huber
+trychroma.com>, Anton Troynikov
+trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
+Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE
                                  [Chroma_logo]
                  Chroma - the open-source embedding database.
  This package is for the the Python HTTP client-only library for Chroma. This
 client connects to the Chroma Server. If that it not what you are looking for,
                  you might want to check out the full_library.
 ```bash pip install chromadb-client # python http-client only library ``` To
 connect to your server and perform operations using the client only library,
-you can do the following: ```python import chromadb from chromadb.config import
-Settings # Example setup of the client to connect to your chroma server client
-= chromadb.Client(Settings(chroma_api_impl="rest",
-chroma_server_host="localhost", chroma_server_http_port=8000)) collection =
-client.create_collection("all-my-documents") collection.add( documents=["This
-is document1", "This is document2"], metadatas=[{"source": "notion"},
-{"source": "google-docs"}], # filter on these! ids=["doc1", "doc2"], # unique
-for each doc embeddings = [[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results =
-collection.query( query_texts=["This is a query document"], n_results=2, #
-where={"metadata_field": "is_equal_to_this"}, # optional filter #
-where_document={"$contains":"search_string"} # optional filter ) ``` ## License
-[Apache 2.0](./LICENSE)
+you can do the following: ```python import chromadb # Example setup of the
+client to connect to your chroma server client = chromadb.HttpClient
+(host="localhost", port=8000) collection = client.create_collection("all-my-
+documents") collection.add( documents=["This is document1", "This is
+document2"], metadatas=[{"source": "notion"}, {"source": "google-docs"}], #
+filter on these! ids=["doc1", "doc2"], # unique for each doc embeddings = [
+[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results = collection.query( query_texts=
+["This is a query document"], n_results=2, # where={"metadata_field":
+"is_equal_to_this"}, # optional filter # where_document={"$contains":
+"search_string"} # optional filter ) ``` ## License [Apache 2.0](./LICENSE)
```

### Comparing `chromadb-client-0.3.30.dev0/RELEASE_PROCESS.md` & `chromadb-client-0.4.1.dev0/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/bin/generate_cloudformation.py` & `chromadb-client-0.4.1.dev0/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/api/__init__.py` & `chromadb-client-0.4.1.dev0/chromadb/api/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,211 +12,271 @@
     Include,
     Metadatas,
     Where,
     QueryResult,
     GetResult,
     WhereDocument,
 )
-from chromadb.config import Component
+from chromadb.config import Component, Settings
 import chromadb.utils.embedding_functions as ef
 
 
 class API(Component, ABC):
     @abstractmethod
     def heartbeat(self) -> int:
-        """Returns the current server time in nanoseconds to check if the server is alive
-
-        Args:
-            None
+        """Get the current time in nanoseconds since epoch.
+        Used to check if the server is alive.
 
         Returns:
-            int: The current server time in nanoseconds
+            int: The current time in nanoseconds since epoch
 
         """
         pass
 
+    #
+    # COLLECTION METHODS
+    #
+
     @abstractmethod
     def list_collections(self) -> Sequence[Collection]:
-        """Returns all collections in the database
-
-        Args:
-            None
-
+        """List all collections.
         Returns:
-            dict: A dictionary of collections
+            Sequence[Collection]: A list of collections
 
+        Examples:
+            ```python
+            client.list_collections()
+            # [collection(name="my_collection", metadata={})]
+            ```
         """
         pass
 
     @abstractmethod
     def create_collection(
         self,
         name: str,
         metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
         get_or_create: bool = False,
     ) -> Collection:
-        """Creates a new collection in the database
-
+        """Create a new collection with the given name and metadata.
         Args:
-            name  The name of the collection to create. The name must be unique.
-            metadata: A dictionary of metadata to associate with the collection. Defaults to None.
-            embedding_function: A function that takes documents and returns an embedding. Defaults to None.
-            get_or_create: If True, will return the collection if it already exists,
-                and update the metadata (if applicable). Defaults to False.
+            name: The name of the collection to create.
+            metadata: Optional metadata to associate with the collection.
+            embedding_function: Optional function to use to embed documents.
+                                Uses the default embedding function if not provided.
+            get_or_create: If True, return the existing collection if it exists.
 
         Returns:
-            dict: the created collection
+            Collection: The newly created collection.
 
-        """
-        pass
+        Raises:
+            ValueError: If the collection already exists and get_or_create is False.
+            ValueError: If the collection name is invalid.
 
-    @abstractmethod
-    def delete_collection(
-        self,
-        name: str,
-    ) -> None:
-        """Deletes a collection from the database
+        Examples:
+            ```python
+            client.create_collection("my_collection")
+            # collection(name="my_collection", metadata={})
 
-        Args:
-            name: The name of the collection to delete
+            client.create_collection("my_collection", metadata={"foo": "bar"})
+            # collection(name="my_collection", metadata={"foo": "bar"})
+            ```
         """
+        pass
 
     @abstractmethod
-    def get_or_create_collection(
+    def get_collection(
         self,
         name: str,
-        metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
-        """Calls create_collection with get_or_create=True.
-           If the collection exists, but with different metadata, the metadata will be replaced.
-
+        """Get a collection with the given name.
         Args:
-            name: The name of the collection to create. The name must be unique.
-            metadata: A dictionary of metadata to associate with the collection. Defaults to None.
-            embedding_function: A function that takes documents and returns an embedding. Should be the same as the one used to create the collection. Defaults to None.
+            name: The name of the collection to get
+            embedding_function: Optional function to use to embed documents.
+                                Uses the default embedding function if not provided.
+
         Returns:
-            the created collection
+            Collection: The collection
 
+        Raises:
+            ValueError: If the collection does not exist
+
+        Examples:
+            ```python
+            client.get_collection("my_collection")
+            # collection(name="my_collection", metadata={})
+            ```
         """
         pass
 
     @abstractmethod
-    def get_collection(
+    def get_or_create_collection(
         self,
         name: str,
+        metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
-        """Gets a collection from the database by either name or uuid
-
+        """Get or create a collection with the given name and metadata.
         Args:
-            name: The name of the collection to get. Defaults to None.
-            embedding_function: A function that takes documents and returns an embedding. Should be the same as the one used to create the collection. Defaults to None.
+            name: The name of the collection to get or create
+            metadata: Optional metadata to associate with the collection
+            embedding_function: Optional function to use to embed documents
 
         Returns:
-            dict: the requested collection
+            The collection
 
+        Examples:
+            ```python
+            client.get_or_create_collection("my_collection")
+            # collection(name="my_collection", metadata={})
+            ```
         """
         pass
 
     def _modify(
         self,
         id: UUID,
         new_name: Optional[str] = None,
         new_metadata: Optional[CollectionMetadata] = None,
     ) -> None:
-        """Modify a collection in the database - can update the name and/or metadata
+        """[Internal] Modify a collection by UUID. Can update the name and/or metadata.
 
         Args:
-            current_name: The name of the collection to modify
-            new_name: The new name of the collection. Defaults to None.
-            new_metadata: The new metadata to associate with the collection. Defaults to None.
+            id: The internal UUID of the collection to modify.
+            new_name: The new name of the collection.
+                                If None, the existing name will remain. Defaults to None.
+            new_metadata: The new metadata to associate with the collection.
+                                      Defaults to None.
+        """
+        pass
+
+    @abstractmethod
+    def delete_collection(
+        self,
+        name: str,
+    ) -> None:
+        """Delete a collection with the given name.
+        Args:
+            name: The name of the collection to delete.
+
+        Raises:
+            ValueError: If the collection does not exist.
+
+        Examples:
+            ```python
+            client.delete_collection("my_collection")
+            ```
         """
         pass
 
+    #
+    # ITEM METHODS
+    #
+
     @abstractmethod
     def _add(
         self,
         ids: IDs,
         collection_id: UUID,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
-        """Add embeddings to the data store. This is the most general way to add embeddings to the database.
-        ⚠️ It is recommended to use the more specific methods below when possible.
+        """[Internal] Add embeddings to a collection specified by UUID.
+        If (some) ids already exist, only the new embeddings will be added.
 
         Args:
-            collection_id: The collection to add the embeddings to
-            embedding: The sequence of embeddings to add
+            ids: The ids to associate with the embeddings.
+            collection_id: The UUID of the collection to add the embeddings to.
+            embedding: The sequence of embeddings to add.
             metadata: The metadata to associate with the embeddings. Defaults to None.
             documents: The documents to associate with the embeddings. Defaults to None.
-            ids: The ids to associate with the embeddings. Defaults to None.
+
+        Returns:
+            True if the embeddings were added successfully.
         """
         pass
 
     @abstractmethod
     def _update(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Optional[Embeddings] = None,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
     ) -> bool:
-        """Add embeddings to the data store. This is the most general way to add embeddings to the database.
-        ⚠️ It is recommended to use the more specific methods below when possible.
+        """[Internal] Update entries in a collection specified by UUID.
 
         Args:
-            collection_id: The collection to add the embeddings to
-            embedding: The sequence of embeddings to add
+            collection_id: The UUID of the collection to update the embeddings in.
+            ids: The IDs of the entries to update.
+            embeddings: The sequence of embeddings to update. Defaults to None.
+            metadatas: The metadata to associate with the embeddings. Defaults to None.
+            documents: The documents to associate with the embeddings. Defaults to None.
+
+        Returns:
+            True if the embeddings were updated successfully.
         """
         pass
 
     @abstractmethod
     def _upsert(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
-        """Add or update entries in the embedding store.
-        If an entry with the same id already exists, it will be updated, otherwise it will be added.
+        """[Internal] Add or update entries in the a collection specified by UUID.
+        If an entry with the same id already exists, it will be updated,
+        otherwise it will be added.
 
         Args:
             collection_id: The collection to add the embeddings to
             ids: The ids to associate with the embeddings. Defaults to None.
             embeddings: The sequence of embeddings to add
             metadatas: The metadata to associate with the embeddings. Defaults to None.
             documents: The documents to associate with the embeddings. Defaults to None.
-            increment_index: If True, will incrementally add to the ANN index of the collection. Defaults to True.
+            increment_index: If True, will incrementally add to the ANN index.
+                                          Defaults to True.
         """
         pass
 
     @abstractmethod
     def _count(self, collection_id: UUID) -> int:
-        """Returns the number of embeddings in the database
+        """[Internal] Returns the number of entries in a collection specified by UUID.
 
         Args:
-            collection_id: The collection to count the embeddings in.
-
+            collection_id: The UUID of the collection to count the embeddings in.
 
         Returns:
             int: The number of embeddings in the collection
 
         """
         pass
 
     @abstractmethod
     def _peek(self, collection_id: UUID, n: int = 10) -> GetResult:
+        """[Internal] Returns the first n entries in a collection specified by UUID.
+
+        Args:
+            collection_id: The UUID of the collection to peek into.
+            n: The number of entries to peek. Defaults to 10.
+
+        Returns:
+            GetResult: The first n entries in the collection.
+
+        """
+
         pass
 
     @abstractmethod
     def _get(
         self,
         collection_id: UUID,
         ids: Optional[IDs] = None,
@@ -225,115 +285,126 @@
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         where_document: Optional[WhereDocument] = {},
         include: Include = ["embeddings", "metadatas", "documents"],
     ) -> GetResult:
-        """Gets embeddings from the database. Supports filtering, sorting, and pagination.
-        ⚠️ This method should not be used directly.
+        """[Internal] Returns entries from a collection specified by UUID.
 
         Args:
-            where: A dictionary of key-value pairs to filter the embeddings by. Defaults to {}.
-            sort: The column to sort the embeddings by. Defaults to None.
-            limit: The maximum number of embeddings to return. Defaults to None.
-            offset: The number of embeddings to skip before returning. Defaults to None.
+            ids: The IDs of the entries to get. Defaults to None.
+            where: Conditional filtering on metadata. Defaults to {}.
+            sort: The column to sort the entries by. Defaults to None.
+            limit: The maximum number of entries to return. Defaults to None.
+            offset: The number of entries to skip before returning. Defaults to None.
             page: The page number to return. Defaults to None.
-            page_size: The number of embeddings to return per page. Defaults to None.
-
+            page_size: The number of entries to return per page. Defaults to None.
+            where_document: Conditional filtering on documents. Defaults to {}.
+            include: The fields to include in the response.
+                          Defaults to ["embeddings", "metadatas", "documents"].
         Returns:
-            pd.DataFrame: A pandas dataframe containing the embeddings and metadata
+            GetResult: The entries in the collection that match the query.
 
         """
         pass
 
     @abstractmethod
     def _delete(
         self,
         collection_id: UUID,
         ids: Optional[IDs],
         where: Optional[Where] = {},
         where_document: Optional[WhereDocument] = {},
     ) -> IDs:
-        """Deletes embeddings from the database
-        ⚠️ This method should not be used directly.
+        """[Internal] Deletes entries from a collection specified by UUID.
 
         Args:
-            where: A dictionary of key-value pairs to filter the embeddings by. Defaults to {}.
+            collection_id: The UUID of the collection to delete the entries from.
+            ids: The IDs of the entries to delete. Defaults to None.
+            where: Conditional filtering on metadata. Defaults to {}.
+            where_document: Conditional filtering on documents. Defaults to {}.
 
         Returns:
-            List: The list of internal UUIDs of the deleted embeddings
+            IDs: The list of IDs of the entries that were deleted.
         """
         pass
 
     @abstractmethod
     def _query(
         self,
         collection_id: UUID,
         query_embeddings: Embeddings,
         n_results: int = 10,
         where: Where = {},
         where_document: WhereDocument = {},
         include: Include = ["embeddings", "metadatas", "documents", "distances"],
     ) -> QueryResult:
-        """Gets the nearest neighbors of a single embedding
-        ⚠️ This method should not be used directly.
+        """[Internal] Performs a nearest neighbors query on a collection specified by UUID.
 
         Args:
-            embedding: The embedding to find the nearest neighbors of
-            n_results: The number of nearest neighbors to return. Defaults to 10.
-            where: A dictionary of key-value pairs to filter the embeddings by. Defaults to {}.
+            collection_id: The UUID of the collection to query.
+            query_embeddings: The embeddings to use as the query.
+            n_results: The number of results to return. Defaults to 10.
+            where: Conditional filtering on metadata. Defaults to {}.
+            where_document: Conditional filtering on documents. Defaults to {}.
+            include: The fields to include in the response.
+                          Defaults to ["embeddings", "metadatas", "documents", "distances"].
+
+        Returns:
+            QueryResult: The results of the query.
         """
         pass
 
     @abstractmethod
     def reset(self) -> bool:
-        """Resets the database
-        ⚠️ This is destructive and will delete all data in the database.
-        Args:
-            None
+        """Resets the database. This will delete all collections and entries.
+
         Returns:
-            None
+            bool: True if the database was reset successfully.
         """
         pass
 
     @abstractmethod
     def raw_sql(self, sql: str) -> pd.DataFrame:
         """Runs a raw SQL query against the database
-        ⚠️ This method should not be used directly.
 
         Args:
             sql: The SQL query to run
 
         Returns:
             pd.DataFrame: A pandas dataframe containing the results of the query
         """
         pass
 
     @abstractmethod
     def create_index(self, collection_name: str) -> bool:
         """Creates an index for the given collection
-        ⚠️ This method should not be used directly.
 
         Args:
-            collection_name: The collection to create the index for. Uses the client's collection if None. Defaults to None.
+            collection_name: The collection to create the index for. Defaults to None.
 
         Returns:
             bool: True if the index was created successfully
 
         """
         pass
 
     @abstractmethod
-    def persist(self) -> bool:
-        """Persist the database to disk"""
-        pass
-
-    @abstractmethod
     def get_version(self) -> str:
         """Get the version of Chroma.
 
         Returns:
             str: The version of Chroma
 
         """
         pass
+
+    @abstractmethod
+    def get_settings(self) -> Settings:
+        """Get the settings used to initialize the client.
+
+        Returns:
+            Settings: The settings used to initialize the client.
+
+        """
+        pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/api/fastapi.py` & `chromadb-client-0.4.1.dev0/chromadb/api/fastapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, cast
 from chromadb.api import API
-from chromadb.config import System
+from chromadb.config import Settings, System
 from chromadb.api.types import (
     Documents,
     Embeddings,
     EmbeddingFunction,
     IDs,
     Include,
     Metadatas,
@@ -23,33 +23,50 @@
 import chromadb.errors as errors
 from uuid import UUID
 from chromadb.telemetry import Telemetry
 from overrides import override
 
 
 class FastAPI(API):
+    _settings: Settings
+
     def __init__(self, system: System):
         super().__init__(system)
         url_prefix = "https" if system.settings.chroma_server_ssl_enabled else "http"
         system.settings.require("chroma_server_host")
         system.settings.require("chroma_server_http_port")
-        self._api_url = f"{url_prefix}://{system.settings.chroma_server_host}:{system.settings.chroma_server_http_port}/api/v1"
+
         self._telemetry_client = self.require(Telemetry)
+        self._settings = system.settings
+
+        port_suffix = (
+            f":{system.settings.chroma_server_http_port}"
+            if system.settings.chroma_server_http_port
+            else ""
+        )
+        self._api_url = (
+            f"{url_prefix}://{system.settings.chroma_server_host}{port_suffix}/api/v1"
+        )
+
+        self._header = system.settings.chroma_server_headers
+        self._session = requests.Session()
+        if self._header is not None:
+            self._session.headers.update(self._header)
 
     @override
     def heartbeat(self) -> int:
         """Returns the current server time in nanoseconds to check if the server is alive"""
-        resp = requests.get(self._api_url)
+        resp = self._session.get(self._api_url)
         raise_chroma_error(resp)
         return int(resp.json()["nanosecond heartbeat"])
 
     @override
     def list_collections(self) -> Sequence[Collection]:
         """Returns a list of all collections"""
-        resp = requests.get(self._api_url + "/collections")
+        resp = self._session.get(self._api_url + "/collections")
         raise_chroma_error(resp)
         json_collections = resp.json()
         collections = []
         for json_collection in json_collections:
             collections.append(Collection(self, **json_collection))
 
         return collections
@@ -59,15 +76,15 @@
         self,
         name: str,
         metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
         get_or_create: bool = False,
     ) -> Collection:
         """Creates a collection"""
-        resp = requests.post(
+        resp = self._session.post(
             self._api_url + "/collections",
             data=json.dumps(
                 {"name": name, "metadata": metadata, "get_or_create": get_or_create}
             ),
         )
         raise_chroma_error(resp)
         resp_json = resp.json()
@@ -82,15 +99,15 @@
     @override
     def get_collection(
         self,
         name: str,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
         """Returns a collection"""
-        resp = requests.get(self._api_url + "/collections/" + name)
+        resp = self._session.get(self._api_url + "/collections/" + name)
         raise_chroma_error(resp)
         resp_json = resp.json()
         return Collection(
             client=self,
             name=resp_json["name"],
             id=resp_json["id"],
             embedding_function=embedding_function,
@@ -100,44 +117,42 @@
     @override
     def get_or_create_collection(
         self,
         name: str,
         metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
-        """Get a collection, or return it if it exists"""
-
         return self.create_collection(
             name, metadata, embedding_function, get_or_create=True
         )
 
     @override
     def _modify(
         self,
         id: UUID,
         new_name: Optional[str] = None,
         new_metadata: Optional[CollectionMetadata] = None,
     ) -> None:
         """Updates a collection"""
-        resp = requests.put(
+        resp = self._session.put(
             self._api_url + "/collections/" + str(id),
             data=json.dumps({"new_metadata": new_metadata, "new_name": new_name}),
         )
         raise_chroma_error(resp)
 
     @override
     def delete_collection(self, name: str) -> None:
         """Deletes a collection"""
-        resp = requests.delete(self._api_url + "/collections/" + name)
+        resp = self._session.delete(self._api_url + "/collections/" + name)
         raise_chroma_error(resp)
 
     @override
     def _count(self, collection_id: UUID) -> int:
         """Returns the number of embeddings in the database"""
-        resp = requests.get(
+        resp = self._session.get(
             self._api_url + "/collections/" + str(collection_id) + "/count"
         )
         raise_chroma_error(resp)
         return cast(int, resp.json())
 
     @override
     def _peek(self, collection_id: UUID, n: int = 10) -> GetResult:
@@ -157,20 +172,19 @@
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         where_document: Optional[WhereDocument] = {},
         include: Include = ["metadatas", "documents"],
     ) -> GetResult:
-        """Gets embeddings from the database"""
         if page and page_size:
             offset = (page - 1) * page_size
             limit = page_size
 
-        resp = requests.post(
+        resp = self._session.post(
             self._api_url + "/collections/" + str(collection_id) + "/get",
             data=json.dumps(
                 {
                     "ids": ids,
                     "where": where,
                     "sort": sort,
                     "limit": limit,
@@ -195,16 +209,15 @@
         self,
         collection_id: UUID,
         ids: Optional[IDs] = None,
         where: Optional[Where] = {},
         where_document: Optional[WhereDocument] = {},
     ) -> IDs:
         """Deletes embeddings from the database"""
-
-        resp = requests.post(
+        resp = self._session.post(
             self._api_url + "/collections/" + str(collection_id) + "/delete",
             data=json.dumps(
                 {"where": where, "ids": ids, "where_document": where_document}
             ),
         )
 
         raise_chroma_error(resp)
@@ -220,17 +233,17 @@
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
         """
         Adds a batch of embeddings to the database
         - pass in column oriented data lists
         - by default, the index is progressively built up as you add more data. If for ingestion performance reasons you want to disable this, set increment_index to False
-        -     and then manually create the index yourself with collection.create_index()
+        -   and then manually create the index yourself with collection.create_index()
         """
-        resp = requests.post(
+        resp = self._session.post(
             self._api_url + "/collections/" + str(collection_id) + "/add",
             data=json.dumps(
                 {
                     "ids": ids,
                     "embeddings": embeddings,
                     "metadatas": metadatas,
                     "documents": documents,
@@ -251,16 +264,15 @@
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
     ) -> bool:
         """
         Updates a batch of embeddings in the database
         - pass in column oriented data lists
         """
-
-        resp = requests.post(
+        resp = self._session.post(
             self._api_url + "/collections/" + str(collection_id) + "/update",
             data=json.dumps(
                 {
                     "ids": ids,
                     "embeddings": embeddings,
                     "metadatas": metadatas,
                     "documents": documents,
@@ -278,19 +290,18 @@
         ids: IDs,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
         """
-        Updates a batch of embeddings in the database
+        Upserts a batch of embeddings in the database
         - pass in column oriented data lists
         """
-
-        resp = requests.post(
+        resp = self._session.post(
             self._api_url + "/collections/" + str(collection_id) + "/upsert",
             data=json.dumps(
                 {
                     "ids": ids,
                     "embeddings": embeddings,
                     "metadatas": metadatas,
                     "documents": documents,
@@ -309,16 +320,15 @@
         query_embeddings: Embeddings,
         n_results: int = 10,
         where: Optional[Where] = {},
         where_document: Optional[WhereDocument] = {},
         include: Include = ["metadatas", "documents", "distances"],
     ) -> QueryResult:
         """Gets the nearest neighbors of a single embedding"""
-
-        resp = requests.post(
+        resp = self._session.post(
             self._api_url + "/collections/" + str(collection_id) + "/query",
             data=json.dumps(
                 {
                     "query_embeddings": query_embeddings,
                     "n_results": n_results,
                     "where": where,
                     "where_document": where_document,
@@ -337,50 +347,48 @@
             metadatas=body.get("metadatas", None),
             documents=body.get("documents", None),
         )
 
     @override
     def reset(self) -> bool:
         """Resets the database"""
-        resp = requests.post(self._api_url + "/reset")
-        raise_chroma_error(resp)
-        return cast(bool, resp.json())
-
-    @override
-    def persist(self) -> bool:
-        """Persists the database"""
-        resp = requests.post(self._api_url + "/persist")
+        resp = self._session.post(self._api_url + "/reset")
         raise_chroma_error(resp)
         return cast(bool, resp.json())
 
     @override
     def raw_sql(self, sql: str) -> pd.DataFrame:
         """Runs a raw SQL query against the database"""
-        resp = requests.post(
+        resp = self._session.post(
             self._api_url + "/raw_sql", data=json.dumps({"raw_sql": sql})
         )
         raise_chroma_error(resp)
         return pd.DataFrame.from_dict(resp.json())
 
     @override
     def create_index(self, collection_name: str) -> bool:
-        """Creates an index for the given space key"""
-        resp = requests.post(
+        """Soon deprecated"""
+        resp = self._session.post(
             self._api_url + "/collections/" + collection_name + "/create_index"
         )
         raise_chroma_error(resp)
         return cast(bool, resp.json())
 
     @override
     def get_version(self) -> str:
         """Returns the version of the server"""
-        resp = requests.get(self._api_url + "/version")
+        resp = self._session.get(self._api_url + "/version")
         raise_chroma_error(resp)
         return cast(str, resp.json())
 
+    @override
+    def get_settings(self) -> Settings:
+        """Returns the settings of the client"""
+        return self._settings
+
 
 def raise_chroma_error(resp: requests.Response) -> None:
     """Raises an error if the response is not ok, using a ChromaError if possible"""
     if resp.ok:
         return
 
     chroma_error = None
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/api/local.py` & `chromadb-client-0.4.1.dev0/chromadb/api/segment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-import json
-import time
-from uuid import UUID
-from typing import List, Optional, Sequence, cast
-from chromadb import __version__
 from chromadb.api import API
-from chromadb.db import DB
+from chromadb.config import Settings, System
+from chromadb.db.system import SysDB
+from chromadb.segment import SegmentManager, MetadataReader, VectorReader
+from chromadb.telemetry import Telemetry
+from chromadb.ingest import Producer
+from chromadb.api.models.Collection import Collection
+from chromadb import __version__
+from chromadb.errors import InvalidDimensionException, InvalidCollectionException
+import chromadb.utils.embedding_functions as ef
+
 from chromadb.api.types import (
-    Documents,
+    CollectionMetadata,
     EmbeddingFunction,
-    Embeddings,
-    GetResult,
     IDs,
-    Include,
-    Metadata,
+    Embeddings,
+    Embedding,
     Metadatas,
-    QueryResult,
+    Documents,
     Where,
     WhereDocument,
-    CollectionMetadata,
+    Include,
+    GetResult,
+    QueryResult,
     validate_metadata,
+    validate_update_metadata,
+    validate_where,
+    validate_where_document,
 )
-from chromadb.api.models.Collection import Collection
-from chromadb.config import System
-import chromadb.utils.embedding_functions as ef
-import re
-
-from chromadb.telemetry import Telemetry
 from chromadb.telemetry.events import CollectionAddEvent, CollectionDeleteEvent
+
+import chromadb.types as t
+
+from typing import Optional, Sequence, Generator, List, cast, Set, Dict
 from overrides import override
+from uuid import UUID, uuid4
 import pandas as pd
+import time
 import logging
+import re
 
 logger = logging.getLogger(__name__)
 
 
 # mimics s3 bucket requirements for naming
 def check_index_name(index_name: str) -> None:
     msg = (
@@ -51,323 +59,236 @@
         raise ValueError(msg)
     if ".." in index_name:
         raise ValueError(msg)
     if re.match("^[0-9]{1,3}\\.[0-9]{1,3}\\.[0-9]{1,3}\\.[0-9]{1,3}$", index_name):
         raise ValueError(msg)
 
 
-class LocalAPI(API):
-    _db: DB
+class SegmentAPI(API):
+    """API implementation utilizing the new segment-based internal architecture"""
+
+    _settings: Settings
+    _sysdb: SysDB
+    _manager: SegmentManager
+    _producer: Producer
+    # TODO: fire telemetry events
     _telemetry_client: Telemetry
+    _tenant_id: str
+    _topic_ns: str
+    _collection_cache: Dict[UUID, t.Collection]
 
     def __init__(self, system: System):
         super().__init__(system)
-        self._db = self.require(DB)
+        self._settings = system.settings
+        self._sysdb = self.require(SysDB)
+        self._manager = self.require(SegmentManager)
         self._telemetry_client = self.require(Telemetry)
+        self._producer = self.require(Producer)
+        self._tenant_id = system.settings.tenant_id
+        self._topic_ns = system.settings.topic_namespace
+        self._collection_cache = {}
 
     @override
     def heartbeat(self) -> int:
-        """Ping the database to ensure it is alive
-
-        Returns:
-            The current time in nanoseconds since epoch
-
-        """
         return int(time.time_ns())
 
-    #
-    # COLLECTION METHODS
-    #
+    # TODO: Actually fix CollectionMetadata type to remove type: ignore flags. This is
+    # necessary because changing the value type from `Any` to`` `Union[str, int, float]`
+    # causes the system to somehow convert all values to strings.
     @override
     def create_collection(
         self,
         name: str,
         metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
         get_or_create: bool = False,
     ) -> Collection:
-        """Create a new collection with the given name and metadata.
-        Args:
-            name: The name of the collection to create
-            metadata: Optional metadata to associate with the collection
-            embedding_function: Optional function to use to embed documents
-            get_or_create: If True, return the existing collection if it exists
-
-        Returns:
-            The newly created collection
-
-        Raises:
-            ValueError: If the collection already exists and get_or_create is False
-            ValueError: If the collection name is invalid
-
-        Examples:
-            ```python
-            client.create_collection("my_collection")
-            # collection(name="my_collection", metadata={})
-
-            client.create_collection("my_collection", metadata={"foo": "bar"})
-            # collection(name="my_collection", metadata={"foo": "bar"})
-            ```
-        """
-        check_index_name(name)
+        existing = self._sysdb.get_collections(name=name)
 
         if metadata is not None:
             validate_metadata(metadata)
 
-        res = self._db.create_collection(name, metadata, get_or_create)
+        if existing:
+            if get_or_create:
+                if metadata and existing[0]["metadata"] != metadata:
+                    self._modify(id=existing[0]["id"], new_metadata=metadata)
+                    existing = self._sysdb.get_collections(id=existing[0]["id"])
+                return Collection(
+                    client=self,
+                    id=existing[0]["id"],
+                    name=existing[0]["name"],
+                    metadata=existing[0]["metadata"],  # type: ignore
+                    embedding_function=embedding_function,
+                )
+            else:
+                raise ValueError(f"Collection {name} already exists.")
+
+        # TODO: remove backwards compatibility in naming requirements
+        check_index_name(name)
+
+        id = uuid4()
+        coll = t.Collection(
+            id=id, name=name, metadata=metadata, topic=self._topic(id), dimension=None
+        )
+        self._producer.create_topic(coll["topic"])
+        segments = self._manager.create_segments(coll)
+        self._sysdb.create_collection(coll)
+        for segment in segments:
+            self._sysdb.create_segment(segment)
+
         return Collection(
             client=self,
+            id=id,
             name=name,
+            metadata=metadata,
             embedding_function=embedding_function,
-            id=res[0][0],
-            metadata=res[0][2],
         )
 
     @override
     def get_or_create_collection(
         self,
         name: str,
         metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
-        """Get or create a collection with the given name and metadata.
-        Args:
-            name: The name of the collection to get or create
-            metadata: Optional metadata to associate with the collection
-            embedding_function: Optional function to use to embed documents
-
-        Returns:
-            The collection
-
-        Examples:
-            ```python
-            client.get_or_create_collection("my_collection")
-            # collection(name="my_collection", metadata={})
-            ```
-        """
-
-        if metadata is not None:
-            validate_metadata(metadata)
-
         return self.create_collection(
-            name, metadata, embedding_function, get_or_create=True
+            name=name,
+            metadata=metadata,
+            embedding_function=embedding_function,
+            get_or_create=True,
         )
 
+    # TODO: Actually fix CollectionMetadata type to remove type: ignore flags. This is
+    # necessary because changing the value type from `Any` to`` `Union[str, int, float]`
+    # causes the system to somehow convert all values to strings
     @override
     def get_collection(
         self,
         name: str,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
-        """Get a collection with the given name.
-        Args:
-            name: The name of the collection to get
-            embedding_function: Optional function to use to embed documents
-
-        Returns:
-            The collection
-
-        Raises:
-            ValueError: If the collection does not exist
-
-        Examples:
-            ```python
-            client.get_collection("my_collection")
-            # collection(name="my_collection", metadata={})
-            ```
-        """
-        res = self._db.get_collection(name)
-        if len(res) == 0:
-            raise ValueError(f"Collection {name} does not exist")
-        return Collection(
-            client=self,
-            name=name,
-            id=res[0][0],
-            embedding_function=embedding_function,
-            metadata=res[0][2],
-        )
+        existing = self._sysdb.get_collections(name=name)
+
+        if existing:
+            return Collection(
+                client=self,
+                id=existing[0]["id"],
+                name=existing[0]["name"],
+                metadata=existing[0]["metadata"],  # type: ignore
+                embedding_function=embedding_function,
+            )
+        else:
+            raise ValueError(f"Collection {name} does not exist.")
 
     @override
     def list_collections(self) -> Sequence[Collection]:
-        """List all collections.
-        Returns:
-            A list of collections
-
-        Examples:
-            ```python
-            client.list_collections()
-            # [collection(name="my_collection", metadata={})]
-            ```
-        """
         collections = []
-        db_collections = self._db.list_collections()
+        db_collections = self._sysdb.get_collections()
         for db_collection in db_collections:
             collections.append(
                 Collection(
                     client=self,
-                    id=db_collection[0],
-                    name=db_collection[1],
-                    metadata=db_collection[2],
+                    id=db_collection["id"],
+                    name=db_collection["name"],
+                    metadata=db_collection["metadata"],  # type: ignore
                 )
             )
         return collections
 
     @override
     def _modify(
         self,
         id: UUID,
         new_name: Optional[str] = None,
         new_metadata: Optional[CollectionMetadata] = None,
     ) -> None:
-        if new_name is not None:
+        if new_name:
+            # backwards compatibility in naming requirements (for now)
             check_index_name(new_name)
 
-        self._db.update_collection(id, new_name, new_metadata)
+        if new_metadata:
+            validate_update_metadata(new_metadata)
+
+        # TODO eventually we'll want to use OptionalArgument and Unspecified in the
+        # signature of `_modify` but not changing the API right now.
+        if new_name and new_metadata:
+            self._sysdb.update_collection(id, name=new_name, metadata=new_metadata)
+        elif new_name:
+            self._sysdb.update_collection(id, name=new_name)
+        elif new_metadata:
+            self._sysdb.update_collection(id, metadata=new_metadata)
 
     @override
     def delete_collection(self, name: str) -> None:
-        """Delete a collection with the given name.
-        Args:
-            name: The name of the collection to delete
-
-        Raises:
-            ValueError: If the collection does not exist
-
-        Examples:
-            ```python
-            client.delete_collection("my_collection")
-            ```
-        """
-        self._db.delete_collection(name)
-
-    #
-    # ITEM METHODS
-    #
+        existing = self._sysdb.get_collections(name=name)
+
+        if existing:
+            self._sysdb.delete_collection(existing[0]["id"])
+            for s in self._manager.delete_segments(existing[0]["id"]):
+                self._sysdb.delete_segment(s)
+            self._producer.delete_topic(existing[0]["topic"])
+            if existing and existing[0]["id"] in self._collection_cache:
+                del self._collection_cache[existing[0]["id"]]
+        else:
+            raise ValueError(f"Collection {name} does not exist.")
+
     @override
     def _add(
         self,
         ids: IDs,
         collection_id: UUID,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
-        existing_ids = set(self._get(collection_id, ids=ids, include=[])["ids"])
-        if len(existing_ids) > 0:
-            logger.info(f"Adding {len(existing_ids)} items with ids that already exist")
-            # Partially add the items that don't already exist
-            valid_indices = [i for i, id in enumerate(ids) if id not in existing_ids]
-            if len(valid_indices) == 0:
-                return False
-            filtered_ids: IDs = []
-            filtered_embeddings: Embeddings = []
-            if metadatas is not None:
-                filtered_metadatas: Metadatas = []
-            if documents is not None:
-                filtered_documents: Documents = []
-            for index in valid_indices:
-                filtered_ids.append(ids[index])
-                filtered_embeddings.append(embeddings[index])
-                if metadatas is not None:
-                    filtered_metadatas.append(metadatas[index])
-                if documents is not None:
-                    filtered_documents.append(documents[index])
-            ids = filtered_ids
-            embeddings = filtered_embeddings
-            if metadatas is not None:
-                metadatas = filtered_metadatas
-            if documents is not None:
-                documents = filtered_documents
-
-        added_uuids = self._db.add(
-            collection_id,
-            embeddings=embeddings,
-            metadatas=metadatas,
-            documents=documents,
-            ids=ids,
-        )
+        coll = self._get_collection(collection_id)
+        self._manager.hint_use_collection(collection_id, t.Operation.ADD)
 
-        if increment_index:
-            self._db.add_incremental(collection_id, added_uuids, embeddings)
+        for r in _records(t.Operation.ADD, ids, embeddings, metadatas, documents):
+            self._validate_embedding_record(coll, r)
+            self._producer.submit_embedding(coll["topic"], r)
 
         self._telemetry_client.capture(CollectionAddEvent(str(collection_id), len(ids)))
-        return True  # NIT: should this return the ids of the succesfully added items?
+        return True
 
     @override
     def _update(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Optional[Embeddings] = None,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
     ) -> bool:
-        self._db.update(collection_id, ids, embeddings, metadatas, documents)
+        coll = self._get_collection(collection_id)
+        self._manager.hint_use_collection(collection_id, t.Operation.UPDATE)
+
+        for r in _records(t.Operation.UPDATE, ids, embeddings, metadatas, documents):
+            self._validate_embedding_record(coll, r)
+            self._producer.submit_embedding(coll["topic"], r)
+
         return True
 
     @override
     def _upsert(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
-        # Determine which ids need to be added and which need to be updated based on the ids already in the collection
-        existing_ids = set(self._get(collection_id, ids=ids, include=[])["ids"])
+        coll = self._get_collection(collection_id)
+        self._manager.hint_use_collection(collection_id, t.Operation.UPSERT)
 
-        ids_to_add = []
-        ids_to_update = []
-        embeddings_to_add: Embeddings = []
-        embeddings_to_update: Embeddings = []
-        metadatas_to_add: Optional[Metadatas] = [] if metadatas else None
-        metadatas_to_update: Optional[Metadatas] = [] if metadatas else None
-        documents_to_add: Optional[Documents] = [] if documents else None
-        documents_to_update: Optional[Documents] = [] if documents else None
-
-        for i, id in enumerate(ids):
-            if id in existing_ids:
-                ids_to_update.append(id)
-                if embeddings is not None:
-                    embeddings_to_update.append(embeddings[i])
-                if metadatas is not None:
-                    metadatas_to_update.append(metadatas[i])  # type: ignore
-                if documents is not None:
-                    documents_to_update.append(documents[i])  # type: ignore
-            else:
-                ids_to_add.append(id)
-                if embeddings is not None:
-                    embeddings_to_add.append(embeddings[i])
-                if metadatas is not None:
-                    metadatas_to_add.append(metadatas[i])  # type: ignore
-                if documents is not None:
-                    documents_to_add.append(documents[i])  # type: ignore
-
-        if len(ids_to_add) > 0:
-            self._add(
-                ids_to_add,
-                collection_id,
-                embeddings_to_add,
-                metadatas_to_add,
-                documents_to_add,
-                increment_index=increment_index,
-            )
-
-        if len(ids_to_update) > 0:
-            self._update(
-                collection_id,
-                ids_to_update,
-                embeddings_to_update,
-                metadatas_to_update,
-                documents_to_update,
-            )
-        self._db.update(collection_id, ids, embeddings, metadatas, documents)
+        for r in _records(t.Operation.UPSERT, ids, embeddings, metadatas, documents):
+            self._validate_embedding_record(coll, r)
+            self._producer.submit_embedding(coll["topic"], r)
 
         return True
 
     @override
     def _get(
         self,
         collection_id: UUID,
@@ -377,211 +298,321 @@
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         where_document: Optional[WhereDocument] = {},
         include: Include = ["embeddings", "metadatas", "documents"],
     ) -> GetResult:
-        if where is None:
-            where = {}
+        where = validate_where(where) if where is not None and len(where) > 0 else None
+        where_document = (
+            validate_where_document(where_document)
+            if where_document is not None and len(where_document) > 0
+            else None
+        )
 
-        if where_document is None:
-            where_document = {}
+        metadata_segment = self._manager.get_segment(collection_id, MetadataReader)
+
+        if sort is not None:
+            raise NotImplementedError("Sorting is not yet supported")
 
         if page and page_size:
             offset = (page - 1) * page_size
             limit = page_size
 
-        include_embeddings = "embeddings" in include
-        include_documents = "documents" in include
-        include_metadatas = "metadatas" in include
-
-        # Remove plural from include since db columns are singular
-        db_columns = [column[:-1] for column in include] + ["id"]
-        column_index = {
-            column_name: index for index, column_name in enumerate(db_columns)
-        }
-
-        db_result = self._db.get(
-            collection_uuid=collection_id,
-            ids=ids,
+        records = metadata_segment.get_metadata(
             where=where,
-            sort=sort,
+            where_document=where_document,
+            ids=ids,
             limit=limit,
             offset=offset,
-            where_document=where_document,
-            columns=db_columns,
         )
 
-        get_result = GetResult(
-            ids=[],
-            embeddings=[] if include_embeddings else None,
-            documents=[] if include_documents else None,
-            metadatas=[] if include_metadatas else None,
+        vectors = None
+        if "embeddings" in include:
+            vector_ids = [r["id"] for r in records]
+            vector_segment = self._manager.get_segment(collection_id, VectorReader)
+            vectors = vector_segment.get_vectors(ids=vector_ids)
+
+        # TODO: Fix type so we don't need to ignore
+        # It is possible to have a set of records, some with metadata and some without
+        # Same with documents
+
+        metadatas = [r["metadata"] for r in records]
+
+        if "documents" in include:
+            documents = [_doc(m) for m in metadatas]
+
+        return GetResult(
+            ids=[r["id"] for r in records],
+            embeddings=[r["embedding"] for r in vectors] if vectors else None,
+            metadatas=_clean_metadatas(metadatas) if "metadatas" in include else None,  # type: ignore
+            documents=documents if "documents" in include else None,  # type: ignore
         )
 
-        for entry in db_result:
-            if include_embeddings:
-                cast(List, get_result["embeddings"]).append(  # type: ignore
-                    entry[column_index["embedding"]]
-                )
-            if include_documents:
-                cast(List, get_result["documents"]).append(  # type: ignore
-                    entry[column_index["document"]]
-                )
-            if include_metadatas:
-                cast(List, get_result["metadatas"]).append(  # type: ignore
-                    entry[column_index["metadata"]]
-                )
-            get_result["ids"].append(entry[column_index["id"]])
-        return get_result
-
     @override
     def _delete(
         self,
         collection_id: UUID,
         ids: Optional[IDs] = None,
         where: Optional[Where] = None,
         where_document: Optional[WhereDocument] = None,
     ) -> IDs:
-        if where is None:
-            where = {}
-
-        if where_document is None:
-            where_document = {}
+        where = validate_where(where) if where is not None and len(where) > 0 else None
+        where_document = (
+            validate_where_document(where_document)
+            if where_document is not None and len(where_document) > 0
+            else None
+        )
+
+        coll = self._get_collection(collection_id)
+        self._manager.hint_use_collection(collection_id, t.Operation.DELETE)
+
+        # TODO: Do we want to warn the user that unrestricted _delete() is 99% of the
+        # time a bad idea?
+        if (where or where_document) or not ids:
+            metadata_segment = self._manager.get_segment(collection_id, MetadataReader)
+            records = metadata_segment.get_metadata(
+                where=where, where_document=where_document, ids=ids
+            )
+            ids_to_delete = [r["id"] for r in records]
+        else:
+            ids_to_delete = ids
+
+        for r in _records(t.Operation.DELETE, ids_to_delete):
+            self._validate_embedding_record(coll, r)
+            self._producer.submit_embedding(coll["topic"], r)
 
-        deleted_uuids = self._db.delete(
-            collection_uuid=collection_id,
-            where=where,
-            ids=ids,
-            where_document=where_document,
-        )
         self._telemetry_client.capture(
-            CollectionDeleteEvent(str(collection_id), len(deleted_uuids))
+            CollectionDeleteEvent(str(collection_id), len(ids_to_delete))
         )
-
-        return deleted_uuids
+        return ids_to_delete
 
     @override
     def _count(self, collection_id: UUID) -> int:
-        return self._db.count(collection_id)
-
-    @override
-    def reset(self) -> bool:
-        """Reset the database. This will delete all collections and items.
-
-        Returns:
-            True if the database was reset successfully
-
-        """
-        self._db.reset_state()
-        return True
+        metadata_segment = self._manager.get_segment(collection_id, MetadataReader)
+        return metadata_segment.count()
 
     @override
     def _query(
         self,
         collection_id: UUID,
         query_embeddings: Embeddings,
         n_results: int = 10,
         where: Where = {},
         where_document: WhereDocument = {},
         include: Include = ["documents", "metadatas", "distances"],
     ) -> QueryResult:
-        uuids, distances = self._db.get_nearest_neighbors(
-            collection_uuid=collection_id,
-            where=where,
-            where_document=where_document,
-            embeddings=query_embeddings,
-            n_results=n_results,
+        where = validate_where(where) if where is not None and len(where) > 0 else where
+        where_document = (
+            validate_where_document(where_document)
+            if where_document is not None and len(where_document) > 0
+            else where_document
         )
 
-        include_embeddings = "embeddings" in include
-        include_documents = "documents" in include
-        include_metadatas = "metadatas" in include
-        include_distances = "distances" in include
-
-        query_result = QueryResult(
-            ids=[],
-            embeddings=[] if include_embeddings else None,
-            documents=[] if include_documents else None,
-            metadatas=[] if include_metadatas else None,
-            distances=[] if include_distances else None,
-        )
-        for i in range(len(uuids)):
-            embeddings: Embeddings = []
-            documents: Documents = []
-            ids: IDs = []
-            metadatas: List[Optional[Metadata]] = []
-            # Remove plural from include since db columns are singular
-            db_columns = [
-                column[:-1] for column in include if column != "distances"
-            ] + ["id"]
-            column_index = {
-                column_name: index for index, column_name in enumerate(db_columns)
-            }
-            db_result = self._db.get_by_ids(uuids[i], columns=db_columns)
-
-            for entry in db_result:
-                if include_embeddings:
-                    embeddings.append(entry[column_index["embedding"]])
-                if include_documents:
-                    documents.append(entry[column_index["document"]])
-                if include_metadatas:
-                    metadatas.append(
-                        json.loads(entry[column_index["metadata"]])
-                        if entry[column_index["metadata"]]
-                        else None
-                    )
-                ids.append(entry[column_index["id"]])
-
-            if include_embeddings:
-                cast(List[Embeddings], query_result["embeddings"]).append(embeddings)
-            if include_documents:
-                cast(List[Documents], query_result["documents"]).append(documents)
-            if include_metadatas:
-                cast(List[List[Optional[Metadata]]], query_result["metadatas"]).append(
-                    metadatas
-                )
-            if include_distances:
-                cast(List[float], query_result["distances"]).append(distances[i])
-            query_result["ids"].append(ids)
+        allowed_ids = None
+
+        coll = self._get_collection(collection_id)
+        for embedding in query_embeddings:
+            self._validate_dimension(coll, len(embedding), update=False)
+
+        metadata_reader = self._manager.get_segment(collection_id, MetadataReader)
+
+        if where or where_document:
+            records = metadata_reader.get_metadata(
+                where=where, where_document=where_document
+            )
+            allowed_ids = [r["id"] for r in records]
+
+        query = t.VectorQuery(
+            vectors=query_embeddings,
+            k=n_results,
+            allowed_ids=allowed_ids,
+            include_embeddings="embeddings" in include,
+            options=None,
+        )
+
+        vector_reader = self._manager.get_segment(collection_id, VectorReader)
+        results = vector_reader.query_vectors(query)
+
+        ids: List[List[str]] = []
+        distances: List[List[float]] = []
+        embeddings: List[List[Embedding]] = []
+        documents: List[List[str]] = []
+        metadatas: List[List[t.Metadata]] = []
+
+        for result in results:
+            ids.append([r["id"] for r in result])
+            if "distances" in include:
+                distances.append([r["distance"] for r in result])
+            if "embeddings" in include:
+                embeddings.append([cast(Embedding, r["embedding"]) for r in result])
+
+        if "documents" in include or "metadatas" in include:
+            all_ids: Set[str] = set()
+            for id_list in ids:
+                all_ids.update(id_list)
+            records = metadata_reader.get_metadata(ids=list(all_ids))
+            metadata_by_id = {r["id"]: r["metadata"] for r in records}
+            for id_list in ids:
+                # In the segment based architecture, it is possible for one segment
+                # to have a record that another segment does not have. This results in
+                # data inconsistency. For the case of the local segments and the
+                # local segment manager, there is a case where a thread writes
+                # a record to the vector segment but not the metadata segment.
+                # Then a query'ing thread reads from the vector segment and
+                # queries the metadata segment. The metadata segment does not have
+                # the record. In this case we choose to return potentially
+                # incorrect data in the form of None.
+                metadata_list = [metadata_by_id.get(id, None) for id in id_list]
+                if "metadatas" in include:
+                    metadatas.append(_clean_metadatas(metadata_list))  # type: ignore
+                if "documents" in include:
+                    doc_list = [_doc(m) for m in metadata_list]
+                    documents.append(doc_list)  # type: ignore
 
-        return query_result
+        return QueryResult(
+            ids=ids,
+            distances=distances if distances else None,
+            metadatas=metadatas if metadatas else None,
+            embeddings=embeddings if embeddings else None,
+            documents=documents if documents else None,
+        )
 
     @override
-    def raw_sql(self, sql: str) -> pd.DataFrame:
-        return self._db.raw_sql(sql)  # type: ignore
+    def _peek(self, collection_id: UUID, n: int = 10) -> GetResult:
+        return self._get(collection_id, limit=n)
 
     @override
-    def create_index(self, collection_name: str) -> bool:
-        collection_uuid = self._db.get_collection_uuid_from_name(collection_name)
-        self._db.create_index(collection_uuid=collection_uuid)
-        return True
+    def get_version(self) -> str:
+        return __version__
 
     @override
-    def _peek(self, collection_id: UUID, n: int = 10) -> GetResult:
-        return self._get(
-            collection_id=collection_id,
-            limit=n,
-            include=["embeddings", "documents", "metadatas"],
-        )
+    def reset_state(self) -> None:
+        self._collection_cache = {}
 
     @override
-    def persist(self) -> bool:
-        """Persist the database to disk.
+    def reset(self) -> bool:
+        self._system.reset_state()
+        return True
 
-        Returns:
-            True if the database was persisted successfully
+    @override
+    def raw_sql(self, sql: str) -> pd.DataFrame:
+        raise NotImplementedError()
 
-        """
-        self._db.persist()
+    @override
+    def create_index(self, collection_name: str) -> bool:
+        logger.warning(
+            "Calling create_index is unnecessary, data is now automatically indexed"
+        )
         return True
 
     @override
-    def get_version(self) -> str:
-        """Get the version of Chroma.
+    def get_settings(self) -> Settings:
+        return self._settings
 
-        Returns:
-            The version of Chroma
+    def _topic(self, collection_id: UUID) -> str:
+        return f"persistent://{self._tenant_id}/{self._topic_ns}/{collection_id}"
 
-        """
-        return __version__
+    # TODO: This could potentially cause race conditions in a distributed version of the
+    # system, since the cache is only local.
+    def _validate_embedding_record(
+        self, collection: t.Collection, record: t.SubmitEmbeddingRecord
+    ) -> None:
+        """Validate the dimension of an embedding record before submitting it to the system."""
+        if record["embedding"]:
+            self._validate_dimension(collection, len(record["embedding"]), update=True)
+
+    def _validate_dimension(
+        self, collection: t.Collection, dim: int, update: bool
+    ) -> None:
+        """Validate that a collection supports records of the given dimension. If update
+        is true, update the collection if the collection doesn't already have a
+        dimension."""
+
+        if collection["dimension"] is None:
+            if update:
+                id = collection["id"]
+                self._sysdb.update_collection(id=id, dimension=dim)
+                self._collection_cache[id]["dimension"] = dim
+        elif collection["dimension"] != dim:
+            raise InvalidDimensionException(
+                f"Embedding dimension {dim} does not match collection dimensionality {collection['dimension']}"
+            )
+        else:
+            return  # all is well
+
+    def _get_collection(self, collection_id: UUID) -> t.Collection:
+        """Read-through cache for collection data"""
+        if collection_id not in self._collection_cache:
+            collections = self._sysdb.get_collections(id=collection_id)
+            if not collections:
+                raise InvalidCollectionException(
+                    f"Collection {collection_id} does not exist."
+                )
+            self._collection_cache[collection_id] = collections[0]
+        return self._collection_cache[collection_id]
+
+
+def _records(
+    operation: t.Operation,
+    ids: IDs,
+    embeddings: Optional[Embeddings] = None,
+    metadatas: Optional[Metadatas] = None,
+    documents: Optional[Documents] = None,
+) -> Generator[t.SubmitEmbeddingRecord, None, None]:
+    """Convert parallel lists of embeddings, metadatas and documents to a sequence of
+    SubmitEmbeddingRecords"""
+
+    # Presumes that callers were invoked via  Collection model, which means
+    # that we know that the embeddings, metadatas and documents have already been
+    # normalized and are guaranteed to be consistently named lists.
+
+    # TODO: Fix API types to make it explicit that they've already been normalized
+
+    for i, id in enumerate(ids):
+        metadata = None
+        if metadatas:
+            metadata = metadatas[i]
+
+        if documents:
+            document = documents[i]
+            if metadata:
+                metadata = {**metadata, "chroma:document": document}
+            else:
+                metadata = {"chroma:document": document}
+
+        record = t.SubmitEmbeddingRecord(
+            id=id,
+            embedding=embeddings[i] if embeddings else None,
+            encoding=t.ScalarEncoding.FLOAT32,  # Hardcode for now
+            metadata=metadata,
+            operation=operation,
+        )
+        yield record
+
+
+def _doc(metadata: Optional[t.Metadata]) -> Optional[str]:
+    """Retrieve the document (if any) from a Metadata map"""
+
+    if metadata and "chroma:document" in metadata:
+        return str(metadata["chroma:document"])
+    return None
+
+
+def _clean_metadatas(
+    metadata: List[Optional[t.Metadata]],
+) -> List[Optional[t.Metadata]]:
+    """Remove any chroma-specific metadata keys that the client shouldn't see from a
+    list of metadata maps."""
+    return [_clean_metadata(m) for m in metadata]
+
+
+def _clean_metadata(metadata: Optional[t.Metadata]) -> Optional[t.Metadata]:
+    """Remove any chroma-specific metadata keys that the client shouldn't see from a
+    metadata map."""
+    if not metadata:
+        return None
+    result = {}
+    for k, v in metadata.items():
+        if not k.startswith("chroma:"):
+            result[k] = v
+    return result
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/api/models/Collection.py` & `chromadb-client-0.4.1.dev0/chromadb/api/models/Collection.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/api/types.py` & `chromadb-client-0.4.1.dev0/chromadb/api/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,18 @@
             f"Expected IDs to be unique, found duplicates for: {dups}"
         )
     return ids
 
 
 def validate_metadata(metadata: Metadata) -> Metadata:
     """Validates metadata to ensure it is a dictionary of strings to strings, ints, or floats"""
-    if not isinstance(metadata, dict):
-        raise ValueError(f"Expected metadata to be a dict, got {metadata}")
+    if not isinstance(metadata, dict) and metadata is not None:
+        raise ValueError(f"Expected metadata to be a dict or None, got {metadata}")
+    if metadata is None:
+        return metadata
     if len(metadata) == 0:
         raise ValueError(f"Expected metadata to be a non-empty dict, got {metadata}")
     for key, value in metadata.items():
         if not isinstance(key, str):
             raise ValueError(
                 f"Expected metadata key to be a str, got {key} which is a {type(key)}"
             )
@@ -139,16 +141,18 @@
                 f"Expected metadata value to be a str, int, or float, got {value} which is a {type(value)}"
             )
     return metadata
 
 
 def validate_update_metadata(metadata: UpdateMetadata) -> UpdateMetadata:
     """Validates metadata to ensure it is a dictionary of strings to strings, ints, or floats"""
-    if not isinstance(metadata, dict):
-        raise ValueError(f"Expected metadata to be a dict, got {metadata}")
+    if not isinstance(metadata, dict) and metadata is not None:
+        raise ValueError(f"Expected metadata to be a dict or None, got {metadata}")
+    if metadata is None:
+        return metadata
     if len(metadata) == 0:
         raise ValueError(f"Expected metadata to be a non-empty dict, got {metadata}")
     for key, value in metadata.items():
         if not isinstance(key, str):
             raise ValueError(f"Expected metadata key to be a str, got {key}")
         if not isinstance(value, (str, int, float, type(None))):
             raise ValueError(
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/config.py` & `chromadb-client-0.4.1.dev0/chromadb/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,84 +14,93 @@
     from chromadb.is_thin_client import is_thin_client  # type: ignore
 except ImportError:
     is_thin_client = False
 
 
 logger = logging.getLogger(__name__)
 
+
+LEGACY_ERROR = "You are using a deprecated configuration of Chroma. Please pip install chroma-migrate and run `chroma-migrate` to upgrade your configuration. See https://docs.trychroma.com/migration for more information or join our discord at https://discord.gg/8g5FESbj for help!"
+
+_legacy_config_keys = {
+    "chroma_db_impl",
+}
+
 _legacy_config_values = {
-    "duckdb": "chromadb.db.duckdb.DuckDB",
-    "duckdb+parquet": "chromadb.db.duckdb.PersistentDuckDB",
-    "clickhouse": "chromadb.db.clickhouse.Clickhouse",
-    "rest": "chromadb.api.fastapi.FastAPI",
-    "local": "chromadb.api.local.LocalAPI",
+    "duckdb",
+    "duckdb+parquet",
+    "clickhouse",
+    "local",
+    "rest",
+    "chromadb.db.duckdb.DuckDB",
+    "chromadb.db.duckdb.PersistentDuckDB",
+    "chromadb.db.clickhouse.Clickhouse",
+    "chromadb.api.local.LocalAPI",
 }
 
 # TODO: Don't use concrete types here to avoid circular deps. Strings are fine for right here!
 _abstract_type_keys: Dict[str, str] = {
-    "chromadb.db.DB": "chroma_db_impl",
     "chromadb.api.API": "chroma_api_impl",
     "chromadb.telemetry.Telemetry": "chroma_telemetry_impl",
     "chromadb.ingest.Producer": "chroma_producer_impl",
     "chromadb.ingest.Consumer": "chroma_consumer_impl",
     "chromadb.db.system.SysDB": "chroma_sysdb_impl",
     "chromadb.segment.SegmentManager": "chroma_segment_manager_impl",
 }
 
 
 class Settings(BaseSettings):
     environment: str = ""
 
-    chroma_db_impl: str = "chromadb.db.duckdb.DuckDB"
-    chroma_api_impl: str = "chromadb.api.local.LocalAPI"
+    # Legacy config has to be kept around because pydantic will error on nonexisting keys
+    chroma_db_impl: Optional[str] = None
+
+    chroma_api_impl: str = "chromadb.api.segment.SegmentAPI"  # Can be "chromadb.api.segment.SegmentAPI" or "chromadb.api.fastapi.FastAPI"
     chroma_telemetry_impl: str = "chromadb.telemetry.posthog.Posthog"
 
     # New architecture components
     chroma_sysdb_impl: str = "chromadb.db.impl.sqlite.SqliteDB"
     chroma_producer_impl: str = "chromadb.db.impl.sqlite.SqliteDB"
     chroma_consumer_impl: str = "chromadb.db.impl.sqlite.SqliteDB"
     chroma_segment_manager_impl: str = (
         "chromadb.segment.impl.manager.local.LocalSegmentManager"
     )
 
-    clickhouse_host: Optional[str] = None
-    clickhouse_port: Optional[str] = None
-
     tenant_id: str = "default"
     topic_namespace: str = "default"
 
-    persist_directory: str = ".chroma"
+    is_persistent: bool = False
+    persist_directory: str = "./chroma"
 
     chroma_server_host: Optional[str] = None
+    chroma_server_headers: Optional[Dict[str, str]] = None
     chroma_server_http_port: Optional[str] = None
     chroma_server_ssl_enabled: Optional[bool] = False
     chroma_server_grpc_port: Optional[str] = None
     chroma_server_cors_allow_origins: List[str] = []  # eg ["http://localhost:3000"]
 
     anonymized_telemetry: bool = True
 
     allow_reset: bool = False
 
-    sqlite_database: Optional[str] = ":memory:"
     migrations: Literal["none", "validate", "apply"] = "apply"
 
     def require(self, key: str) -> Any:
         """Return the value of a required config key, or raise an exception if it is not
         set"""
         val = self[key]
         if val is None:
             raise ValueError(f"Missing required config value '{key}'")
         return val
 
     def __getitem__(self, key: str) -> Any:
         val = getattr(self, key)
-        # Backwards compatibility with short names instead of full class names
+        # Error on legacy config values
         if val in _legacy_config_values:
-            newval = _legacy_config_values[val]
-            val = newval
+            raise ValueError(LEGACY_ERROR)
         return val
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
 
 
@@ -138,14 +147,27 @@
 
 class System(Component):
     settings: Settings
 
     _instances: Dict[Type[Component], Component]
 
     def __init__(self, settings: Settings):
+        if is_thin_client:
+            # The thin client is a system with only the API component
+            if settings["chroma_api_impl"] != "chromadb.api.fastapi.FastAPI":
+                raise RuntimeError(
+                    "Chroma is running in http-only client mode, and can only be run with 'chromadb.api.fastapi.FastAPI' as the chroma_api_impl. \
+            see https://docs.trychroma.com/usage-guide?lang=py#using-the-python-http-only-client for more information."
+                )
+
+        # Validate settings don't contain any legacy config values
+        for key in _legacy_config_keys:
+            if settings[key] is not None:
+                raise ValueError(LEGACY_ERROR)
+
         self.settings = settings
         self._instances = {}
         super().__init__(self)
 
     def instance(self, type: Type[T]) -> T:
         """Return an instance of the component type specified. If the system is running,
         the component will be started as well."""
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/db/__init__.py` & `chromadb-client-0.4.1.dev0/chromadb/db/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,11 +125,7 @@
     @abstractmethod
     def raw_sql(self, raw_sql):  # type: ignore
         pass
 
     @abstractmethod
     def create_index(self, collection_uuid: UUID):  # type: ignore
         pass
-
-    @abstractmethod
-    def persist(self) -> None:
-        pass
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/db/base.py` & `chromadb-client-0.4.1.dev0/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/db/clickhouse.py` & `chromadb-client-0.4.1.dev0/chromadb/test/property/strategies.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,656 +1,564 @@
-# type: ignore
-from chromadb.api.types import (
-    Documents,
-    Embeddings,
-    IDs,
-    Metadatas,
-    Where,
-    WhereDocument,
-)
-from chromadb.db import DB
-from chromadb.db.index.hnswlib import Hnswlib, delete_all_indexes
-import uuid
-import json
-from typing import Optional, Sequence, List, Tuple, cast
-import clickhouse_connect
-from clickhouse_connect.driver.client import Client
-from clickhouse_connect import common
-import logging
-from uuid import UUID
-from chromadb.config import System
-from overrides import override
-from chromadb.api.types import Metadata
-
-logger = logging.getLogger(__name__)
-
-COLLECTION_TABLE_SCHEMA = [{"uuid": "UUID"}, {"name": "String"}, {"metadata": "String"}]
-
-EMBEDDING_TABLE_SCHEMA = [
-    {"collection_uuid": "UUID"},
-    {"uuid": "UUID"},
-    {"embedding": "Array(Float64)"},
-    {"document": "Nullable(String)"},
-    {"id": "Nullable(String)"},
-    {"metadata": "Nullable(String)"},
+import hashlib
+import hypothesis
+import hypothesis.strategies as st
+from typing import Any, Optional, List, Dict, Union
+from typing_extensions import TypedDict
+import numpy as np
+import numpy.typing as npt
+import chromadb.api.types as types
+import re
+from hypothesis.strategies._internal.strategies import SearchStrategy
+from hypothesis.errors import InvalidDefinition
+from hypothesis.stateful import RuleBasedStateMachine
+
+from dataclasses import dataclass
+
+from chromadb.api.types import Documents, Embeddings, Metadata
+
+# Set the random seed for reproducibility
+np.random.seed(0)  # unnecessary, hypothesis does this for us
+
+# See Hypothesis documentation for creating strategies at
+# https://hypothesis.readthedocs.io/en/latest/data.html
+
+# NOTE: Because these strategies are used in state machines, we need to
+# work around an issue with state machines, in which strategies that frequently
+# are marked as invalid (i.e. through the use of `assume` or `.filter`) can cause the
+# state machine tests to fail with an hypothesis.errors.Unsatisfiable.
+
+# Ultimately this is because the entire state machine is run as a single Hypothesis
+# example, which ends up drawing from the same strategies an enormous number of times.
+# Whenever a strategy marks itself as invalid, Hypothesis tries to start the entire
+# state machine run over. See https://github.com/HypothesisWorks/hypothesis/issues/3618
+
+# Because strategy generation is all interrelated, seemingly small changes (especially
+# ones called early in a test) can have an outside effect. Generating lists with
+# unique=True, or dictionaries with a min size seems especially bad.
+
+# Please make changes to these strategies incrementally, testing to make sure they don't
+# start generating unsatisfiable examples.
+
+test_hnsw_config = {
+    "hnsw:construction_ef": 128,
+    "hnsw:search_ef": 128,
+    "hnsw:M": 128,
+}
+
+
+class RecordSet(TypedDict):
+    """
+    A generated set of embeddings, ids, metadatas, and documents that
+    represent what a user would pass to the API.
+    """
+
+    ids: Union[types.ID, List[types.ID]]
+    embeddings: Optional[Union[types.Embeddings, types.Embedding]]
+    metadatas: Optional[Union[List[types.Metadata], types.Metadata]]
+    documents: Optional[Union[List[types.Document], types.Document]]
+
+
+class NormalizedRecordSet(TypedDict):
+    """
+    A RecordSet, with all fields normalized to lists.
+    """
+
+    ids: List[types.ID]
+    embeddings: Optional[types.Embeddings]
+    metadatas: Optional[List[types.Metadata]]
+    documents: Optional[List[types.Document]]
+
+
+class StateMachineRecordSet(TypedDict):
+    """
+    Represents the internal state of a state machine in hypothesis tests.
+    """
+
+    ids: List[types.ID]
+    embeddings: types.Embeddings
+    metadatas: List[Optional[types.Metadata]]
+    documents: List[Optional[types.Document]]
+
+
+class Record(TypedDict):
+    """
+    A single generated record.
+    """
+
+    id: types.ID
+    embedding: Optional[types.Embedding]
+    metadata: Optional[types.Metadata]
+    document: Optional[types.Document]
+
+
+# TODO: support arbitrary text everywhere so we don't SQL-inject ourselves.
+# TODO: support empty strings everywhere
+sql_alphabet = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789-_"
+safe_text = st.text(alphabet=sql_alphabet, min_size=1)
+
+# Workaround for FastAPI json encoding peculiarities
+# https://github.com/tiangolo/fastapi/blob/8ac8d70d52bb0dd9eb55ba4e22d3e383943da05c/fastapi/encoders.py#L104
+safe_text = safe_text.filter(lambda s: not s.startswith("_sa"))
+
+safe_integers = st.integers(
+    min_value=-(2**31), max_value=2**31 - 1
+)  # TODO: handle longs
+safe_floats = st.floats(
+    allow_infinity=False,
+    allow_nan=False,
+    allow_subnormal=False,
+    min_value=-1e6,
+    max_value=1e6,
+)  # TODO: handle infinity and NAN
+
+safe_values: List[SearchStrategy[Union[int, float, str]]] = [
+    safe_text,
+    safe_integers,
+    safe_floats,
 ]
 
 
-def db_array_schema_to_clickhouse_schema(table_schema):
-    return_str = ""
-    for element in table_schema:
-        for k, v in element.items():
-            return_str += f"{k} {v}, "
-    return return_str
-
-
-def db_schema_to_keys() -> List[str]:
-    keys = []
-    for element in EMBEDDING_TABLE_SCHEMA:
-        keys.append(list(element.keys())[0])
-    return keys
-
-
-class Clickhouse(DB):
-    #
-    #  INIT METHODS
-    #
-    def __init__(self, system: System):
-        super().__init__(system)
-        self._conn = None
-        self._settings = system.settings
-
-        self._settings.require("clickhouse_host")
-        self._settings.require("clickhouse_port")
-
-    def _init_conn(self):
-        common.set_setting("autogenerate_session_id", False)
-        self._conn = clickhouse_connect.get_client(
-            host=self._settings.clickhouse_host,
-            port=int(self._settings.clickhouse_port),
-        )
-        self._create_table_collections(self._conn)
-        self._create_table_embeddings(self._conn)
-
-    def _get_conn(self) -> Client:
-        if self._conn is None:
-            self._init_conn()
-        return self._conn
-
-    def _create_table_collections(self, conn):
-        conn.command(
-            f"""CREATE TABLE IF NOT EXISTS collections (
-            {db_array_schema_to_clickhouse_schema(COLLECTION_TABLE_SCHEMA)}
-        ) ENGINE = MergeTree() ORDER BY uuid"""
-        )
-
-    def _create_table_embeddings(self, conn):
-        conn.command(
-            f"""CREATE TABLE IF NOT EXISTS embeddings (
-            {db_array_schema_to_clickhouse_schema(EMBEDDING_TABLE_SCHEMA)}
-        ) ENGINE = MergeTree() ORDER BY collection_uuid"""
-        )
-
-    index_cache = {}
-
-    def _index(self, collection_id):
-        """Retrieve an HNSW index instance for the given collection"""
-
-        if collection_id not in self.index_cache:
-            coll = self.get_collection_by_id(collection_id)
-            collection_metadata = coll[2]
-            index = Hnswlib(
-                collection_id,
-                self._settings,
-                collection_metadata,
-                self.count(collection_id),
-            )
-            self.index_cache[collection_id] = index
-
-        return self.index_cache[collection_id]
-
-    def _delete_index(self, collection_id):
-        """Delete an index from the cache"""
-        index = self._index(collection_id)
-        index.delete()
-        del self.index_cache[collection_id]
-
-    #
-    #  UTILITY METHODS
-    #
-    @override
-    def persist(self):
-        raise NotImplementedError(
-            "Clickhouse is a persistent database, this method is not needed"
-        )
-
-    @override
-    def get_collection_uuid_from_name(self, collection_name: str) -> UUID:
-        res = self._get_conn().query(
-            f"""
-            SELECT uuid FROM collections WHERE name = '{collection_name}'
-        """
-        )
-        return res.result_rows[0][0]
+def one_or_both(
+    strategy_a: st.SearchStrategy[Any], strategy_b: st.SearchStrategy[Any]
+) -> st.SearchStrategy[Any]:
+    return st.one_of(
+        st.tuples(strategy_a, strategy_b),
+        st.tuples(strategy_a, st.none()),
+        st.tuples(st.none(), strategy_b),
+    )
 
-    def _create_where_clause(
-        self,
-        collection_uuid: str,
-        ids: Optional[List[str]] = None,
-        where: Where = {},
-        where_document: WhereDocument = {},
-    ):
-        where_clauses: List[str] = []
-        self._format_where(where, where_clauses)
-        if len(where_document) > 0:
-            where_document_clauses = []
-            self._format_where_document(where_document, where_document_clauses)
-            where_clauses.extend(where_document_clauses)
 
-        if ids is not None:
-            where_clauses.append(f" id IN {tuple(ids)}")
+# Temporarily generate only these to avoid SQL formatting issues.
+legal_id_characters = (
+    "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789-_./+"
+)
 
-        where_clauses.append(f"collection_uuid = '{collection_uuid}'")
-        where_str = " AND ".join(where_clauses)
-        where_str = f"WHERE {where_str}"
-        return where_str
-
-    #
-    #  COLLECTION METHODS
-    #
-    @override
-    def create_collection(
-        self,
-        name: str,
-        metadata: Optional[Metadata] = None,
-        get_or_create: bool = False,
-    ) -> Sequence:
-        # poor man's unique constraint
-        dupe_check = self.get_collection(name)
-
-        if len(dupe_check) > 0:
-            if get_or_create:
-                if dupe_check[0][2] != metadata:
-                    self.update_collection(
-                        dupe_check[0][0], new_name=name, new_metadata=metadata
-                    )
-                    dupe_check = self.get_collection(name)
-                logger.info(
-                    f"collection with name {name} already exists, returning existing collection"
-                )
-                return dupe_check
-            else:
-                raise ValueError(f"Collection with name {name} already exists")
+float_types = [np.float16, np.float32, np.float64]
+int_types = [np.int16, np.int32, np.int64]  # TODO: handle int types
 
-        collection_uuid = uuid.uuid4()
-        data_to_insert = [[collection_uuid, name, json.dumps(metadata)]]
 
-        self._get_conn().insert(
-            "collections", data_to_insert, column_names=["uuid", "name", "metadata"]
-        )
-        return [[collection_uuid, name, metadata]]
+@st.composite
+def collection_name(draw: st.DrawFn) -> str:
+    _collection_name_re = re.compile(r"^[a-zA-Z][a-zA-Z0-9-]{1,60}[a-zA-Z0-9]$")
+    _ipv4_address_re = re.compile(r"^([0-9]{1,3}\.){3}[0-9]{1,3}$")
+    _two_periods_re = re.compile(r"\.\.")
 
-    @override
-    def get_collection(self, name: str) -> Sequence:
-        res = (
-            self._get_conn()
-            .query(
-                f"""
-         SELECT * FROM collections WHERE name = '{name}'
-         """
-            )
-            .result_rows
-        )
-        # json.loads the metadata
-        return [[x[0], x[1], json.loads(x[2])] for x in res]
+    name: str = draw(st.from_regex(_collection_name_re))
+    hypothesis.assume(not _ipv4_address_re.match(name))
+    hypothesis.assume(not _two_periods_re.search(name))
 
-    def get_collection_by_id(self, collection_uuid: str):
-        res = (
-            self._get_conn()
-            .query(
-                f"""
-         SELECT * FROM collections WHERE uuid = '{collection_uuid}'
-         """
-            )
-            .result_rows
-        )
-        # json.loads the metadata
-        return [[x[0], x[1], json.loads(x[2])] for x in res][0]
-
-    @override
-    def list_collections(self) -> Sequence:
-        res = self._get_conn().query("SELECT * FROM collections").result_rows
-        return [[x[0], x[1], json.loads(x[2])] for x in res]
-
-    @override
-    def update_collection(
-        self,
-        id: UUID,
-        new_name: Optional[str] = None,
-        new_metadata: Optional[Metadata] = None,
-    ):
-        if new_name is not None:
-            dupe_check = self.get_collection(new_name)
-            if len(dupe_check) > 0 and dupe_check[0][0] != id:
-                raise ValueError(f"Collection with name {new_name} already exists")
-
-            self._get_conn().command(
-                "ALTER TABLE collections UPDATE name = %(new_name)s WHERE uuid = %(uuid)s",
-                parameters={"new_name": new_name, "uuid": id},
-            )
-
-        if new_metadata is not None:
-            self._get_conn().command(
-                "ALTER TABLE collections UPDATE metadata = %(new_metadata)s WHERE uuid = %(uuid)s",
-                parameters={"new_metadata": json.dumps(new_metadata), "uuid": id},
-            )
+    return name
 
-    @override
-    def delete_collection(self, name: str):
-        collection_uuid = self.get_collection_uuid_from_name(name)
-        self._get_conn().command(
-            f"""
-        DELETE FROM embeddings WHERE collection_uuid = '{collection_uuid}'
-        """
-        )
 
-        self._delete_index(collection_uuid)
+collection_metadata = st.one_of(
+    st.none(), st.dictionaries(safe_text, st.one_of(*safe_values))
+)
 
-        self._get_conn().command(
-            f"""
-         DELETE FROM collections WHERE name = '{name}'
-         """
-        )
 
-    #
-    #  ITEM METHODS
-    #
-    @override
-    def add(self, collection_uuid, embeddings, metadatas, documents, ids) -> List[UUID]:
-        data_to_insert = [
-            [
-                collection_uuid,
-                uuid.uuid4(),
-                embedding,
-                json.dumps(metadatas[i]) if metadatas else None,
-                documents[i] if documents else None,
-                ids[i],
-            ]
-            for i, embedding in enumerate(embeddings)
+# TODO: Use a hypothesis strategy while maintaining embedding uniqueness
+#       Or handle duplicate embeddings within a known epsilon
+def create_embeddings(
+    dim: int,
+    count: int,
+    dtype: npt.DTypeLike,
+) -> types.Embeddings:
+    embeddings: types.Embeddings = (
+        np.random.uniform(
+            low=-1.0,
+            high=1.0,
+            size=(count, dim),
+        )
+        .astype(dtype)
+        .tolist()
+    )
+
+    return embeddings
+
+
+class hashing_embedding_function(types.EmbeddingFunction):
+    def __init__(self, dim: int, dtype: npt.DTypeLike) -> None:
+        self.dim = dim
+        self.dtype = dtype
+
+    def __call__(self, texts: types.Documents) -> types.Embeddings:
+        # Hash the texts and convert to hex strings
+        hashed_texts = [
+            list(hashlib.sha256(text.encode("utf-8")).hexdigest()) for text in texts
         ]
-        column_names = [
-            "collection_uuid",
-            "uuid",
-            "embedding",
-            "metadata",
-            "document",
-            "id",
+        # Pad with repetition, or truncate the hex strings to the desired dimension
+        padded_texts = [
+            text * (self.dim // len(text)) + text[: self.dim % len(text)]
+            for text in hashed_texts
         ]
-        self._get_conn().insert("embeddings", data_to_insert, column_names=column_names)
-
-        return [x[1] for x in data_to_insert]  # return uuids
 
-    def _update(
-        self,
-        collection_uuid,
-        ids: IDs,
-        embeddings: Optional[Embeddings],
-        metadatas: Optional[Metadatas],
-        documents: Optional[Documents],
-    ):
-        updates = []
-        parameters = {}
-        for i in range(len(ids)):
-            update_fields = []
-            parameters[f"i{i}"] = ids[i]
-            if embeddings is not None:
-                update_fields.append(f"embedding = %(e{i})s")
-                parameters[f"e{i}"] = embeddings[i]
-            if metadatas is not None:
-                update_fields.append(f"metadata = %(m{i})s")
-                parameters[f"m{i}"] = json.dumps(metadatas[i])
-            if documents is not None:
-                update_fields.append(f"document = %(d{i})s")
-                parameters[f"d{i}"] = documents[i]
-
-            update_statement = f"""
-            UPDATE
-                {",".join(update_fields)}
-            WHERE
-                id = %(i{i})s AND
-                collection_uuid = '{collection_uuid}'{"" if i == len(ids) - 1 else ","}
-            """
-            updates.append(update_statement)
-
-        update_clauses = ("").join(updates)
-        self._get_conn().command(
-            f"ALTER TABLE embeddings {update_clauses}", parameters=parameters
-        )
-
-    @override
-    def update(
-        self,
-        collection_uuid,
-        ids: IDs,
-        embeddings: Optional[Embeddings] = None,
-        metadatas: Optional[Metadatas] = None,
-        documents: Optional[Documents] = None,
-    ) -> bool:
-        # Verify all IDs exist
-        existing_items = self.get(collection_uuid=collection_uuid, ids=ids)
-        if len(existing_items) != len(ids):
-            raise ValueError(
-                f"Could not find {len(ids) - len(existing_items)} items for update"
+        # Convert the hex strings to dtype
+        embeddings: types.Embeddings = np.array(
+            [[int(char, 16) / 15.0 for char in text] for text in padded_texts],
+            dtype=self.dtype,
+        ).tolist()
+
+        return embeddings
+
+
+class not_implemented_embedding_function(types.EmbeddingFunction):
+    def __call__(self, texts: Documents) -> Embeddings:
+        assert False, "This embedding function is not implemented"
+
+
+def embedding_function_strategy(
+    dim: int, dtype: npt.DTypeLike
+) -> st.SearchStrategy[types.EmbeddingFunction]:
+    return st.just(hashing_embedding_function(dim, dtype))
+
+
+@dataclass
+class Collection:
+    name: str
+    metadata: Optional[types.Metadata]
+    dimension: int
+    dtype: npt.DTypeLike
+    known_metadata_keys: types.Metadata
+    known_document_keywords: List[str]
+    has_documents: bool = False
+    has_embeddings: bool = False
+    embedding_function: Optional[types.EmbeddingFunction] = None
+
+
+@st.composite
+def collections(
+    draw: st.DrawFn,
+    add_filterable_data: bool = False,
+    with_hnsw_params: bool = False,
+    has_embeddings: Optional[bool] = None,
+    has_documents: Optional[bool] = None,
+    with_persistent_hnsw_params: bool = False,
+) -> Collection:
+    """Strategy to generate a Collection object. If add_filterable_data is True, then known_metadata_keys and known_document_keywords will be populated with consistent data."""
+
+    assert not ((has_embeddings is False) and (has_documents is False))
+
+    name = draw(collection_name())
+    metadata = draw(collection_metadata)
+    dimension = draw(st.integers(min_value=2, max_value=2048))
+    dtype = draw(st.sampled_from(float_types))
+
+    if with_persistent_hnsw_params and not with_hnsw_params:
+        raise ValueError(
+            "with_hnsw_params requires with_persistent_hnsw_params to be true"
+        )
+
+    if with_hnsw_params:
+        if metadata is None:
+            metadata = {}
+        metadata.update(test_hnsw_config)
+        if with_persistent_hnsw_params:
+            metadata["hnsw:batch_size"] = draw(st.integers(min_value=3, max_value=2000))
+            metadata["hnsw:sync_threshold"] = draw(
+                st.integers(min_value=3, max_value=2000)
             )
-
-        # Update the db
-        self._update(collection_uuid, ids, embeddings, metadatas, documents)
-
-        # Update the index
-        if embeddings is not None:
-            # `get` current returns items in arbitrary order.
-            # TODO if we fix `get`, we can remove this explicit mapping.
-            uuid_mapping = {r[4]: r[1] for r in existing_items}
-            update_uuids = [uuid_mapping[id] for id in ids]
-            index = self._index(collection_uuid)
-            index.add(update_uuids, embeddings, update=True)
-
-    def _get(self, where={}, columns: Optional[List] = None):
-        select_columns = db_schema_to_keys() if columns is None else columns
-        val = (
-            self._get_conn()
-            .query(f"""SELECT {",".join(select_columns)} FROM embeddings {where}""")
-            .result_rows
-        )
-        for i in range(len(val)):
-            # We know val has index abilities, so cast it for typechecker
-            val = cast(list, val)
-            val[i] = list(val[i])
-            # json.load the metadata
-            if "metadata" in select_columns:
-                metadata_column_index = select_columns.index("metadata")
-                db_metadata = val[i][metadata_column_index]
-                val[i][metadata_column_index] = (
-                    json.loads(db_metadata) if db_metadata else None
-                )
-        return val
-
-    def _format_where(self, where, result):
-        for key, value in where.items():
-
-            def has_key_and(clause):
-                return f"(JSONHas(metadata,'{key}') = 1 AND {clause})"
-
-            # Shortcut for $eq
-            if type(value) == str:
-                result.append(
-                    has_key_and(f" JSONExtractString(metadata,'{key}') = '{value}'")
-                )
-            elif type(value) == int:
-                result.append(
-                    has_key_and(f" JSONExtractInt(metadata,'{key}') = {value}")
-                )
-            elif type(value) == float:
-                result.append(
-                    has_key_and(f" JSONExtractFloat(metadata,'{key}') = {value}")
-                )
-            # Operator expression
-            elif type(value) == dict:
-                operator, operand = list(value.items())[0]
-                if operator == "$gt":
-                    return result.append(
-                        has_key_and(f" JSONExtractFloat(metadata,'{key}') > {operand}")
-                    )
-                elif operator == "$lt":
-                    return result.append(
-                        has_key_and(f" JSONExtractFloat(metadata,'{key}') < {operand}")
-                    )
-                elif operator == "$gte":
-                    return result.append(
-                        has_key_and(f" JSONExtractFloat(metadata,'{key}') >= {operand}")
-                    )
-                elif operator == "$lte":
-                    return result.append(
-                        has_key_and(f" JSONExtractFloat(metadata,'{key}') <= {operand}")
-                    )
-                elif operator == "$ne":
-                    if type(operand) == str:
-                        return result.append(
-                            has_key_and(
-                                f" JSONExtractString(metadata,'{key}') != '{operand}'"
-                            )
-                        )
-                    return result.append(
-                        has_key_and(f" JSONExtractFloat(metadata,'{key}') != {operand}")
-                    )
-                elif operator == "$eq":
-                    if type(operand) == str:
-                        return result.append(
-                            has_key_and(
-                                f" JSONExtractString(metadata,'{key}') = '{operand}'"
-                            )
-                        )
-                    return result.append(
-                        has_key_and(f" JSONExtractFloat(metadata,'{key}') = {operand}")
-                    )
-                else:
-                    raise ValueError(
-                        f"Expected one of $gt, $lt, $gte, $lte, $ne, $eq, got {operator}"
-                    )
-            elif type(value) == list:
-                all_subresults = []
-                for subwhere in value:
-                    subresults = []
-                    self._format_where(subwhere, subresults)
-                    all_subresults.append(subresults[0])
-                if key == "$or":
-                    result.append(f"({' OR '.join(all_subresults)})")
-                elif key == "$and":
-                    result.append(f"({' AND '.join(all_subresults)})")
-                else:
-                    raise ValueError(f"Expected one of $or, $and, got {key}")
-
-    def _format_where_document(self, where_document, results):
-        operator = list(where_document.keys())[0]
-        if operator == "$contains":
-            results.append(f"position(document, '{where_document[operator]}') > 0")
-        elif operator == "$and" or operator == "$or":
-            all_subresults = []
-            for subwhere in where_document[operator]:
-                subresults = []
-                self._format_where_document(subwhere, subresults)
-                all_subresults.append(subresults[0])
-            if operator == "$or":
-                results.append(f"({' OR '.join(all_subresults)})")
-            if operator == "$and":
-                results.append(f"({' AND '.join(all_subresults)})")
-        else:
-            raise ValueError(f"Expected one of $contains, $and, $or, got {operator}")
-
-    @override
-    def get(
-        self,
-        where: Where = {},
-        collection_name: Optional[str] = None,
-        collection_uuid: Optional[UUID] = None,
-        ids: Optional[IDs] = None,
-        sort: Optional[str] = None,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        where_document: WhereDocument = {},
-        columns: Optional[List[str]] = None,
-    ) -> Sequence:
-        if collection_name is None and collection_uuid is None:
-            raise TypeError(
-                "Arguments collection_name and collection_uuid cannot both be None"
-            )
-
-        if collection_name is not None:
-            collection_uuid = self.get_collection_uuid_from_name(collection_name)
-
-        where_str = self._create_where_clause(
-            # collection_uuid must be defined at this point, cast it for typechecker
-            cast(str, collection_uuid),
-            ids=ids,
-            where=where,
-            where_document=where_document,
-        )
-
-        if sort is not None:
-            where_str += f" ORDER BY {sort}"
-        else:
-            where_str += " ORDER BY collection_uuid"  # stable ordering
-
-        if limit is not None or isinstance(limit, int):
-            where_str += f" LIMIT {limit}"
-
-        if offset is not None or isinstance(offset, int):
-            where_str += f" OFFSET {offset}"
-
-        val = self._get(where=where_str, columns=columns)
-
-        return val
-
-    @override
-    def count(self, collection_id: UUID) -> int:
-        where_string = f"WHERE collection_uuid = '{collection_id}'"
-        return (
-            self._get_conn()
-            .query(f"SELECT COUNT() FROM embeddings {where_string}")
-            .result_rows[0][0]
-        )
-
-    def _delete(self, where_str: Optional[str] = None) -> List:
-        deleted_uuids = (
-            self._get_conn()
-            .query(f"""SELECT uuid FROM embeddings {where_str}""")
-            .result_rows
-        )
-        self._get_conn().command(
-            f"""
-            DELETE FROM
-                embeddings
-        {where_str}
-        """
-        )
-        return [res[0] for res in deleted_uuids] if len(deleted_uuids) > 0 else []
-
-    @override
-    def delete(
-        self,
-        where: Where = {},
-        collection_uuid: Optional[UUID] = None,
-        ids: Optional[IDs] = None,
-        where_document: WhereDocument = {},
-    ) -> List[str]:
-        where_str = self._create_where_clause(
-            # collection_uuid must be defined at this point, cast it for typechecker
-            cast(str, collection_uuid),
-            ids=ids,
-            where=where,
-            where_document=where_document,
-        )
-
-        deleted_uuids = self._delete(where_str)
-
-        index = self._index(collection_uuid)
-        index.delete_from_index(deleted_uuids)
-
-        return deleted_uuids
-
-    @override
-    def get_by_ids(
-        self, uuids: List[UUID], columns: Optional[List[str]] = None
-    ) -> Sequence:
-        columns = columns + ["uuid"] if columns else ["uuid"]
-        select_columns = db_schema_to_keys() if columns is None else columns
-        response = (
-            self._get_conn()
-            .query(
-                f"""
-        SELECT {",".join(select_columns)} FROM embeddings WHERE uuid IN ({[id.hex for id in uuids]})
-        """
+        # Sometimes, select a space at random
+        if draw(st.booleans()):
+            # TODO: pull the distance functions from a source of truth that lives not
+            # in tests once https://github.com/chroma-core/issues/issues/61 lands
+            metadata["hnsw:space"] = draw(st.sampled_from(["cosine", "l2", "ip"]))
+
+    known_metadata_keys: Dict[str, Union[int, str, float]] = {}
+    if add_filterable_data:
+        while len(known_metadata_keys) < 5:
+            key = draw(safe_text)
+            known_metadata_keys[key] = draw(st.one_of(*safe_values))
+
+    if has_documents is None:
+        has_documents = draw(st.booleans())
+    assert has_documents is not None
+    if has_documents and add_filterable_data:
+        known_document_keywords = draw(st.lists(safe_text, min_size=5, max_size=5))
+    else:
+        known_document_keywords = []
+
+    if not has_documents:
+        has_embeddings = True
+    else:
+        if has_embeddings is None:
+            has_embeddings = draw(st.booleans())
+    assert has_embeddings is not None
+
+    embedding_function = draw(embedding_function_strategy(dimension, dtype))
+
+    return Collection(
+        name=name,
+        metadata=metadata,
+        dimension=dimension,
+        dtype=dtype,
+        known_metadata_keys=known_metadata_keys,
+        has_documents=has_documents,
+        known_document_keywords=known_document_keywords,
+        has_embeddings=has_embeddings,
+        embedding_function=embedding_function,
+    )
+
+
+@st.composite
+def metadata(draw: st.DrawFn, collection: Collection) -> types.Metadata:
+    """Strategy for generating metadata that could be a part of the given collection"""
+    # First draw a random dictionary.
+    metadata: types.Metadata = draw(st.dictionaries(safe_text, st.one_of(*safe_values)))
+    # Then, remove keys that overlap with the known keys for the coll
+    # to avoid type errors when comparing.
+    if collection.known_metadata_keys:
+        for key in collection.known_metadata_keys.keys():
+            if key in metadata:
+                del metadata[key]
+        # Finally, add in some of the known keys for the collection
+        sampling_dict: Dict[str, st.SearchStrategy[Union[str, int, float]]] = {
+            k: st.just(v) for k, v in collection.known_metadata_keys.items()
+        }
+        metadata.update(draw(st.fixed_dictionaries({}, optional=sampling_dict)))
+    return metadata
+
+
+@st.composite
+def document(draw: st.DrawFn, collection: Collection) -> types.Document:
+    """Strategy for generating documents that could be a part of the given collection"""
+
+    # Blacklist certain unicode characters that affect sqlite processing.
+    # For example, the null (/x00) character makes sqlite stop processing a string.
+    blacklist_categories = ("Cc", "Cs")
+    if collection.known_document_keywords:
+        known_words_st = st.sampled_from(collection.known_document_keywords)
+    else:
+        known_words_st = st.text(
+            min_size=1,
+            alphabet=st.characters(blacklist_categories=blacklist_categories),
+        )
+
+    random_words_st = st.text(
+        min_size=1, alphabet=st.characters(blacklist_categories=blacklist_categories)
+    )
+    words = draw(st.lists(st.one_of(known_words_st, random_words_st), min_size=1))
+    return " ".join(words)
+
+
+@st.composite
+def recordsets(
+    draw: st.DrawFn,
+    collection_strategy: SearchStrategy[Collection] = collections(),
+    id_strategy: SearchStrategy[str] = safe_text,
+    min_size: int = 1,
+    max_size: int = 50,
+) -> RecordSet:
+    collection = draw(collection_strategy)
+
+    ids = list(
+        draw(st.lists(id_strategy, min_size=min_size, max_size=max_size, unique=True))
+    )
+
+    embeddings: Optional[Embeddings] = None
+    if collection.has_embeddings:
+        embeddings = create_embeddings(collection.dimension, len(ids), collection.dtype)
+    metadatas = draw(
+        st.lists(metadata(collection), min_size=len(ids), max_size=len(ids))
+    )
+    documents: Optional[Documents] = None
+    if collection.has_documents:
+        documents = draw(
+            st.lists(document(collection), min_size=len(ids), max_size=len(ids))
+        )
+
+    # in the case where we have a single record, sometimes exercise
+    # the code that handles individual values rather than lists.
+    # In this case, any field may be a list or a single value.
+    if len(ids) == 1:
+        single_id: Union[str, List[str]] = ids[0] if draw(st.booleans()) else ids
+        single_embedding = (
+            embeddings[0]
+            if embeddings is not None and draw(st.booleans())
+            else embeddings
+        )
+        single_metadata: Union[Metadata, List[Metadata]] = (
+            metadatas[0] if draw(st.booleans()) else metadatas
+        )
+        single_document = (
+            documents[0] if documents is not None and draw(st.booleans()) else documents
+        )
+        return {
+            "ids": single_id,
+            "embeddings": single_embedding,
+            "metadatas": single_metadata,
+            "documents": single_document,
+        }
+
+    return {
+        "ids": ids,
+        "embeddings": embeddings,
+        "metadatas": metadatas,
+        "documents": documents,
+    }
+
+
+# This class is mostly cloned from from hypothesis.stateful.RuleStrategy,
+# but always runs all the rules, instead of using a FeatureStrategy to
+# enable/disable rules. Disabled rules cause the entire test to be marked invalida and,
+# combined with the complexity of our other strategies, leads to an
+# unacceptably increased incidence of hypothesis.errors.Unsatisfiable.
+class DeterministicRuleStrategy(SearchStrategy):  # type: ignore
+    def __init__(self, machine: RuleBasedStateMachine) -> None:
+        super().__init__()  # type: ignore
+        self.machine = machine
+        self.rules = list(machine.rules())  # type: ignore
+
+        # The order is a bit arbitrary. Primarily we're trying to group rules
+        # that write to the same location together, and to put rules with no
+        # target first as they have less effect on the structure. We order from
+        # fewer to more arguments on grounds that it will plausibly need less
+        # data. This probably won't work especially well and we could be
+        # smarter about it, but it's better than just doing it in definition
+        # order.
+        self.rules.sort(
+            key=lambda rule: (
+                sorted(rule.targets),
+                len(rule.arguments),
+                rule.function.__name__,
             )
-            .result_rows
         )
 
-        # sort db results by the order of the uuids
-        response = sorted(response, key=lambda obj: uuids.index(obj[len(columns) - 1]))
+    def __repr__(self) -> str:
+        return "{}(machine={}({{...}}))".format(
+            self.__class__.__name__,
+            self.machine.__class__.__name__,
+        )
+
+    def do_draw(self, data):  # type: ignore
+        if not any(self.is_valid(rule) for rule in self.rules):
+            msg = f"No progress can be made from state {self.machine!r}"
+            raise InvalidDefinition(msg) from None
+
+        rule = data.draw(st.sampled_from([r for r in self.rules if self.is_valid(r)]))
+        argdata = data.draw(rule.arguments_strategy)
+        return (rule, argdata)
+
+    def is_valid(self, rule) -> bool:  # type: ignore
+        if not all(precond(self.machine) for precond in rule.preconditions):
+            return False
+
+        for b in rule.bundles:
+            bundle = self.machine.bundle(b.name)  # type: ignore
+            if not bundle:
+                return False
+        return True
+
+
+@st.composite
+def where_clause(draw: st.DrawFn, collection: Collection) -> types.Where:
+    """Generate a filter that could be used in a query against the given collection"""
+
+    known_keys = sorted(collection.known_metadata_keys.keys())
+
+    key = draw(st.sampled_from(known_keys))
+    value = collection.known_metadata_keys[key]
+
+    legal_ops: List[Optional[str]] = [None, "$eq", "$ne"]
+    if not isinstance(value, str):
+        legal_ops.extend(["$gt", "$lt", "$lte", "$gte"])
+    if isinstance(value, float):
+        # Add or subtract a small number to avoid floating point rounding errors
+        value = value + draw(st.sampled_from([1e-6, -1e-6]))
+
+    op: types.WhereOperator = draw(st.sampled_from(legal_ops))
+
+    if op is None:
+        return {key: value}
+    else:
+        return {key: {op: value}}
+
+
+@st.composite
+def where_doc_clause(draw: st.DrawFn, collection: Collection) -> types.WhereDocument:
+    """Generate a where_document filter that could be used against the given collection"""
+    if collection.known_document_keywords:
+        word = draw(st.sampled_from(collection.known_document_keywords))
+    else:
+        word = draw(safe_text)
+    return {"$contains": word}
+
+
+def binary_operator_clause(
+    base_st: SearchStrategy[types.Where],
+) -> SearchStrategy[types.Where]:
+    op: SearchStrategy[types.LogicalOperator] = st.sampled_from(["$and", "$or"])
+    return st.dictionaries(
+        keys=op,
+        values=st.lists(base_st, max_size=2, min_size=2),
+        min_size=1,
+        max_size=1,
+    )
+
+
+def binary_document_operator_clause(
+    base_st: SearchStrategy[types.WhereDocument],
+) -> SearchStrategy[types.WhereDocument]:
+    op: SearchStrategy[types.LogicalOperator] = st.sampled_from(["$and", "$or"])
+    return st.dictionaries(
+        keys=op,
+        values=st.lists(base_st, max_size=2, min_size=2),
+        min_size=1,
+        max_size=1,
+    )
+
+
+@st.composite
+def recursive_where_clause(draw: st.DrawFn, collection: Collection) -> types.Where:
+    base_st = where_clause(collection)
+    where: types.Where = draw(st.recursive(base_st, binary_operator_clause))
+    return where
+
+
+@st.composite
+def recursive_where_doc_clause(
+    draw: st.DrawFn, collection: Collection
+) -> types.WhereDocument:
+    base_st = where_doc_clause(collection)
+    where: types.WhereDocument = draw(
+        st.recursive(base_st, binary_document_operator_clause)
+    )
+    return where
+
+
+class Filter(TypedDict):
+    where: Optional[types.Where]
+    ids: Optional[Union[str, List[str]]]
+    where_document: Optional[types.WhereDocument]
+
+
+@st.composite
+def filters(
+    draw: st.DrawFn,
+    collection_st: st.SearchStrategy[Collection],
+    recordset_st: st.SearchStrategy[RecordSet],
+    include_all_ids: bool = False,
+) -> Filter:
+    collection = draw(collection_st)
+    recordset = draw(recordset_st)
+
+    where_clause = draw(st.one_of(st.none(), recursive_where_clause(collection)))
+    where_document_clause = draw(
+        st.one_of(st.none(), recursive_where_doc_clause(collection))
+    )
+
+    ids: Optional[Union[List[types.ID], types.ID]]
+    # Record sets can be a value instead of a list of values if there is only one record
+    if isinstance(recordset["ids"], str):
+        ids = [recordset["ids"]]
+    else:
+        ids = recordset["ids"]
 
-        return response
+    if not include_all_ids:
+        ids = draw(st.one_of(st.none(), st.lists(st.sampled_from(ids))))
+        if ids is not None:
+            # Remove duplicates since hypothesis samples with replacement
+            ids = list(set(ids))
 
-    @override
-    def get_nearest_neighbors(
-        self,
-        collection_uuid: UUID,
-        where: Where = {},
-        embeddings: Optional[Embeddings] = None,
-        n_results: int = 10,
-        where_document: WhereDocument = {},
-    ) -> Tuple[List[List[UUID]], List[List[float]]]:
-        # Either the collection name or the collection uuid must be provided
-        if collection_uuid is None:
-            raise TypeError("Argument collection_uuid cannot be None")
-
-        if len(where) != 0 or len(where_document) != 0:
-            results = self.get(
-                collection_uuid=collection_uuid,
-                where=where,
-                where_document=where_document,
-            )
+    # Test both the single value list and the unwrapped single value case
+    if ids is not None and len(ids) == 1 and draw(st.booleans()):
+        ids = ids[0]
 
-            if len(results) > 0:
-                ids = [x[1] for x in results]
-            else:
-                # No results found, return empty lists
-                return [[] for _ in range(len(embeddings))], [
-                    [] for _ in range(len(embeddings))
-                ]
-        else:
-            ids = None
-
-        index = self._index(collection_uuid)
-        uuids, distances = index.get_nearest_neighbors(embeddings, n_results, ids)
-
-        return uuids, distances
-
-    @override
-    def create_index(self, collection_uuid: UUID):
-        """Create an index for a collection_uuid and optionally scoped to a dataset.
-        Args:
-            collection_uuid (str): The collection_uuid to create an index for
-            dataset (str, optional): The dataset to scope the index to. Defaults to None.
-        Returns:
-            None
-        """
-        get = self.get(collection_uuid=collection_uuid)
-
-        uuids = [x[1] for x in get]
-        embeddings = [x[2] for x in get]
-
-        index = self._index(collection_uuid)
-        index.add(uuids, embeddings)
-
-    @override
-    def add_incremental(
-        self, collection_uuid: UUID, ids: List[UUID], embeddings: Embeddings
-    ) -> None:
-        index = self._index(collection_uuid)
-        index.add(ids, embeddings)
-
-    def reset_indexes(self):
-        delete_all_indexes(self._settings)
-        self.index_cache = {}
-
-    @override
-    def reset_state(self):
-        conn = self._get_conn()
-        conn.command("DROP TABLE collections")
-        conn.command("DROP TABLE embeddings")
-        self._create_table_collections(conn)
-        self._create_table_embeddings(conn)
-
-        self.reset_indexes()
-
-    @override
-    def raw_sql(self, raw_sql):
-        return self._get_conn().query(raw_sql).result_rows
+    return {"where": where_clause, "where_document": where_document_clause, "ids": ids}
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/db/duckdb.py` & `chromadb-client-0.4.1.dev0/chromadb/segment/impl/metadata/sqlite.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,534 +1,534 @@
-# type: ignore
+from typing import Optional, Sequence, Any, Tuple, cast, Generator, Union, Dict
+from chromadb.segment import MetadataReader
+from chromadb.ingest import Consumer
 from chromadb.config import System
-from chromadb.api.types import Documents, Embeddings, IDs, Metadatas
-from chromadb.db.clickhouse import (
-    Clickhouse,
-    db_array_schema_to_clickhouse_schema,
-    EMBEDDING_TABLE_SCHEMA,
-    db_schema_to_keys,
-    COLLECTION_TABLE_SCHEMA,
+from chromadb.types import Segment
+from chromadb.db.impl.sqlite import SqliteDB
+from overrides import override
+from chromadb.db.base import (
+    Cursor,
+    ParameterValue,
+    get_sql,
+)
+from chromadb.types import (
+    Where,
+    WhereDocument,
+    MetadataEmbeddingRecord,
+    EmbeddingRecord,
+    SeqId,
+    Operation,
+    UpdateMetadata,
+    LiteralValue,
+    WhereOperator,
 )
-from typing import List, Optional, Sequence
-import pandas as pd
-import json
-import duckdb
-import uuid
-import os
-import logging
-import atexit
 from uuid import UUID
-from overrides import override
-from chromadb.api.types import Metadata
+from pypika import Table, Tables
+from pypika.queries import QueryBuilder
+import pypika.functions as fn
+from pypika.terms import Criterion, Function
+from itertools import islice, groupby
+from functools import reduce
+import sqlite3
+
+import logging
 
 logger = logging.getLogger(__name__)
 
 
-def clickhouse_to_duckdb_schema(table_schema):
-    for item in table_schema:
-        if "embedding" in item:
-            item["embedding"] = "DOUBLE[]"
-        # capitalize the key
-        item[list(item.keys())[0]] = item[list(item.keys())[0]].upper()
-        if "NULLABLE" in item[list(item.keys())[0]]:
-            item[list(item.keys())[0]] = (
-                item[list(item.keys())[0]].replace("NULLABLE(", "").replace(")", "")
+class SqliteMetadataSegment(MetadataReader):
+    _consumer: Consumer
+    _db: SqliteDB
+    _id: UUID
+    _topic: Optional[str]
+    _subscription: Optional[UUID]
+
+    def __init__(self, system: System, segment: Segment):
+        self._db = system.instance(SqliteDB)
+        self._consumer = system.instance(Consumer)
+        self._id = segment["id"]
+        self._topic = segment["topic"]
+
+    @override
+    def start(self) -> None:
+        if self._topic:
+            seq_id = self.max_seqid()
+            self._subscription = self._consumer.subscribe(
+                self._topic, self._write_metadata, start=seq_id
             )
-        if "UUID" in item[list(item.keys())[0]]:
-            item[list(item.keys())[0]] = "STRING"
-        if "FLOAT64" in item[list(item.keys())[0]]:
-            item[list(item.keys())[0]] = "DOUBLE"
-    return table_schema
-
-
-# TODO: inherits ClickHouse for convenience of copying behavior, not
-# because it's logically a subtype. Factoring out the common behavior
-# to a third superclass they both extend would be preferable.
-class DuckDB(Clickhouse):
-    # duckdb has a different way of connecting to the database
-    def __init__(self, system: System):
-        self._conn = duckdb.connect()
-        self._create_table_collections(self._conn)
-        self._create_table_embeddings(self._conn)
-        self._settings = system.settings
-
-        # Normally this would be handled by super(), but we actually can't invoke
-        # super().__init__ here because we're (incorrectly) inheriting from Clickhouse
-        self._dependencies = set()
-
-        # https://duckdb.org/docs/extensions/overview
-        self._conn.execute("LOAD 'json';")
 
     @override
-    def _create_table_collections(self, conn):
-        conn.execute(
-            f"""CREATE TABLE collections (
-            {db_array_schema_to_clickhouse_schema(clickhouse_to_duckdb_schema(COLLECTION_TABLE_SCHEMA))}
-        ) """
-        )
+    def stop(self) -> None:
+        if self._subscription:
+            self._consumer.unsubscribe(self._subscription)
 
-    # duckdb has different types, so we want to convert the clickhouse schema to duckdb schema
     @override
-    def _create_table_embeddings(self, conn):
-        conn.execute(
-            f"""CREATE TABLE embeddings (
-            {db_array_schema_to_clickhouse_schema(clickhouse_to_duckdb_schema(EMBEDDING_TABLE_SCHEMA))}
-        ) """
+    def max_seqid(self) -> SeqId:
+        t = Table("max_seq_id")
+        q = (
+            self._db.querybuilder()
+            .from_(t)
+            .select(t.seq_id)
+            .where(t.segment_id == ParameterValue(self._db.uuid_to_db(self._id)))
         )
+        sql, params = get_sql(q)
+        with self._db.tx() as cur:
+            result = cur.execute(sql, params).fetchone()
 
-    #
-    #  UTILITY METHODS
-    #
-    @override
-    def get_collection_uuid_from_name(self, collection_name: str) -> UUID:
-        return self._conn.execute(
-            "SELECT uuid FROM collections WHERE name = ?", [collection_name]
-        ).fetchall()[0][0]
-
-    #
-    #  COLLECTION METHODS
-    #
-    @override
-    def create_collection(
-        self,
-        name: str,
-        metadata: Optional[Metadata] = None,
-        get_or_create: bool = False,
-    ) -> Sequence:
-        # poor man's unique constraint
-        dupe_check = self.get_collection(name)
-        if len(dupe_check) > 0:
-            if get_or_create is True:
-                if dupe_check[0][2] != metadata:
-                    self.update_collection(
-                        dupe_check[0][0], new_name=name, new_metadata=metadata
-                    )
-                    dupe_check = self.get_collection(name)
-
-                logger.info(
-                    f"collection with name {name} already exists, returning existing collection"
-                )
-                return dupe_check
+            if result is None:
+                return self._consumer.min_seqid()
             else:
-                raise ValueError(f"Collection with name {name} already exists")
-
-        collection_uuid = uuid.uuid4()
-        self._conn.execute(
-            """INSERT INTO collections (uuid, name, metadata) VALUES (?, ?, ?)""",
-            [str(collection_uuid), name, json.dumps(metadata)],
-        )
-        return [[str(collection_uuid), name, metadata]]
-
-    @override
-    def get_collection(self, name: str) -> Sequence:
-        res = self._conn.execute(
-            """SELECT * FROM collections WHERE name = ?""", [name]
-        ).fetchall()
-        # json.loads the metadata
-        return [[x[0], x[1], json.loads(x[2])] for x in res]
+                return _decode_seq_id(result[0])
 
     @override
-    def get_collection_by_id(self, collection_uuid: str):
-        res = self._conn.execute(
-            """SELECT * FROM collections WHERE uuid = ?""", [collection_uuid]
-        ).fetchone()
-        return [res[0], res[1], json.loads(res[2])]
+    def count(self) -> int:
+        embeddings_t = Table("embeddings")
+        q = (
+            self._db.querybuilder()
+            .from_(embeddings_t)
+            .where(
+                embeddings_t.segment_id == ParameterValue(self._db.uuid_to_db(self._id))
+            )
+            .select(fn.Count(embeddings_t.id))
+        )
+        sql, params = get_sql(q)
+        with self._db.tx() as cur:
+            result = cur.execute(sql, params).fetchone()[0]
+            return cast(int, result)
 
     @override
-    def list_collections(self) -> Sequence:
-        res = self._conn.execute("""SELECT * FROM collections""").fetchall()
-        return [[x[0], x[1], json.loads(x[2])] for x in res]
+    def get_metadata(
+        self,
+        where: Optional[Where] = None,
+        where_document: Optional[WhereDocument] = None,
+        ids: Optional[Sequence[str]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+    ) -> Sequence[MetadataEmbeddingRecord]:
+        """Query for embedding metadata."""
 
-    @override
-    def delete_collection(self, name: str):
-        collection_uuid = self.get_collection_uuid_from_name(name)
-        self._conn.execute(
-            """DELETE FROM embeddings WHERE collection_uuid = ?""", [collection_uuid]
+        embeddings_t, metadata_t, fulltext_t = Tables(
+            "embeddings", "embedding_metadata", "embedding_fulltext"
         )
 
-        self._delete_index(collection_uuid)
-        self._conn.execute("""DELETE FROM collections WHERE name = ?""", [name])
-
-    @override
-    def update_collection(
-        self,
-        id: UUID,
-        new_name: Optional[str] = None,
-        new_metadata: Optional[Metadata] = None,
-    ):
-        if new_name is not None:
-            dupe_check = self.get_collection(new_name)
-            if len(dupe_check) > 0 and dupe_check[0][0] != str(id):
-                raise ValueError(f"Collection with name {new_name} already exists")
-
-            self._conn.execute(
-                """UPDATE collections SET name = ? WHERE uuid = ?""",
-                [new_name, id],
+        q = (
+            (
+                self._db.querybuilder()
+                .from_(embeddings_t)
+                .left_join(metadata_t)
+                .on(embeddings_t.id == metadata_t.id)
             )
-
-        if new_metadata is not None:
-            self._conn.execute(
-                """UPDATE collections SET metadata = ? WHERE uuid = ?""",
-                [json.dumps(new_metadata), id],
+            .select(
+                embeddings_t.id,
+                embeddings_t.embedding_id,
+                embeddings_t.seq_id,
+                metadata_t.key,
+                metadata_t.string_value,
+                metadata_t.int_value,
+                metadata_t.float_value,
             )
-
-    #
-    #  ITEM METHODS
-    #
-    # the execute many syntax is different than clickhouse, the (?,?) syntax is different than clickhouse
-    @override
-    def add(self, collection_uuid, embeddings, metadatas, documents, ids) -> List[UUID]:
-        data_to_insert = [
-            [
-                collection_uuid,
-                str(uuid.uuid4()),
-                embedding,
-                json.dumps(metadatas[i]) if metadatas else None,
-                documents[i] if documents else None,
-                ids[i],
-            ]
-            for i, embedding in enumerate(embeddings)
-        ]
-
-        insert_string = "collection_uuid, uuid, embedding, metadata, document, id"
-
-        self._conn.executemany(
-            f"""
-         INSERT INTO embeddings ({insert_string}) VALUES (?,?,?,?,?,?)""",
-            data_to_insert,
+            .where(
+                embeddings_t.segment_id == ParameterValue(self._db.uuid_to_db(self._id))
+            )
+            .orderby(embeddings_t.id)
         )
 
-        return [uuid.UUID(x[1]) for x in data_to_insert]  # return uuids
-
-    @override
-    def count(self, collection_id: UUID) -> int:
-        where_string = f"WHERE collection_uuid = '{collection_id}'"
-        return self._conn.query(
-            f"SELECT COUNT() FROM embeddings {where_string}"
-        ).fetchall()[0][0]
-
-    @override
-    def _format_where(self, where, result):
-        for key, value in where.items():
-            # Shortcut for $eq
-            if type(value) == str:
-                result.append(f" json_extract_string(metadata,'$.{key}') = '{value}'")
-            if type(value) == int:
-                result.append(
-                    f" CAST(json_extract(metadata,'$.{key}') AS INT) = {value}"
-                )
-            if type(value) == float:
-                result.append(
-                    f" CAST(json_extract(metadata,'$.{key}') AS DOUBLE) = {value}"
-                )
-            # Operator expression
-            elif type(value) == dict:
-                operator, operand = list(value.items())[0]
-                if operator == "$gt":
-                    result.append(
-                        f" CAST(json_extract(metadata,'$.{key}') AS DOUBLE) > {operand}"
-                    )
-                elif operator == "$lt":
-                    result.append(
-                        f" CAST(json_extract(metadata,'$.{key}') AS DOUBLE) < {operand}"
-                    )
-                elif operator == "$gte":
-                    result.append(
-                        f" CAST(json_extract(metadata,'$.{key}') AS DOUBLE) >= {operand}"
-                    )
-                elif operator == "$lte":
-                    result.append(
-                        f" CAST(json_extract(metadata,'$.{key}') AS DOUBLE) <= {operand}"
-                    )
-                elif operator == "$ne":
-                    if type(operand) == str:
-                        return result.append(
-                            f" json_extract_string(metadata,'$.{key}') != '{operand}'"
-                        )
-                    return result.append(
-                        f" CAST(json_extract(metadata,'$.{key}') AS DOUBLE) != {operand}"
-                    )
-                elif operator == "$eq":
-                    if type(operand) == str:
-                        return result.append(
-                            f" json_extract_string(metadata,'$.{key}') = '{operand}'"
-                        )
-                    return result.append(
-                        f" CAST(json_extract(metadata,'$.{key}') AS DOUBLE) = {operand}"
-                    )
-                else:
-                    raise ValueError(f"Operator {operator} not supported")
-            elif type(value) == list:
-                all_subresults = []
-                for subwhere in value:
-                    subresults = []
-                    self._format_where(subwhere, subresults)
-                    all_subresults.append(subresults[0])
-                if key == "$or":
-                    result.append(f"({' OR '.join(all_subresults)})")
-                elif key == "$and":
-                    result.append(f"({' AND '.join(all_subresults)})")
-                else:
-                    raise ValueError(
-                        f"Operator {key} not supported with a list of where clauses"
-                    )
-
-    @override
-    def _format_where_document(self, where_document, results):
-        operator = list(where_document.keys())[0]
-        if operator == "$contains":
-            results.append(f"position('{where_document[operator]}' in document) > 0")
-        elif operator == "$and" or operator == "$or":
-            all_subresults = []
-            for subwhere in where_document[operator]:
-                subresults = []
-                self._format_where_document(subwhere, subresults)
-                all_subresults.append(subresults[0])
-            if operator == "$or":
-                results.append(f"({' OR '.join(all_subresults)})")
-            if operator == "$and":
-                results.append(f"({' AND '.join(all_subresults)})")
-        else:
-            raise ValueError(f"Operator {operator} not supported")
+        if where:
+            q = q.where(self._where_map_criterion(q, where, embeddings_t, metadata_t))
 
-    @override
-    def _get(self, where, columns: Optional[List] = None):
-        select_columns = db_schema_to_keys() if columns is None else columns
-        val = self._conn.execute(
-            f"""SELECT {",".join(select_columns)} FROM embeddings {where}"""
-        ).fetchall()
-        for i in range(len(val)):
-            val[i] = list(val[i])
-            if "collection_uuid" in select_columns:
-                collection_uuid_column_index = select_columns.index("collection_uuid")
-                val[i][collection_uuid_column_index] = uuid.UUID(
-                    val[i][collection_uuid_column_index]
-                )
-            if "uuid" in select_columns:
-                uuid_column_index = select_columns.index("uuid")
-                val[i][uuid_column_index] = uuid.UUID(val[i][uuid_column_index])
-            if "metadata" in select_columns:
-                metadata_column_index = select_columns.index("metadata")
-                val[i][metadata_column_index] = (
-                    json.loads(val[i][metadata_column_index])
-                    if val[i][metadata_column_index]
-                    else None
-                )
-
-        return val
+        if where_document:
+            q = q.where(
+                self._where_doc_criterion(q, where_document, embeddings_t, fulltext_t)
+            )
+            pass
+            # q = self._where_document_query(q, where_document, embeddings_t, fulltext_t)
 
-    @override
-    def _update(
-        self,
-        collection_uuid,
-        ids: IDs,
-        embeddings: Optional[Embeddings],
-        metadatas: Optional[Metadatas],
-        documents: Optional[Documents],
-    ):
-        update_data = []
-        for i in range(len(ids)):
-            data = []
-            update_data.append(data)
-            if embeddings is not None:
-                data.append(embeddings[i])
-            if metadatas is not None:
-                data.append(json.dumps(metadatas[i]))
-            if documents is not None:
-                data.append(documents[i])
-            data.append(ids[i])
-
-        update_fields = []
-        if embeddings is not None:
-            update_fields.append("embedding = ?")
-        if metadatas is not None:
-            update_fields.append("metadata = ?")
-        if documents is not None:
-            update_fields.append("document = ?")
-
-        update_statement = f"""
-        UPDATE
-            embeddings
-        SET
-            {", ".join(update_fields)}
-        WHERE
-            id = ? AND
-            collection_uuid = '{collection_uuid}';
-        """
-        self._conn.executemany(update_statement, update_data)
+        if ids:
+            q = q.where(embeddings_t.embedding_id.isin(ParameterValue(ids)))
 
-    @override
-    def _delete(self, where_str: Optional[str] = None) -> List:
-        uuids_deleted = self._conn.execute(
-            f"""SELECT uuid FROM embeddings {where_str}"""
-        ).fetchall()
-        self._conn.execute(
-            f"""
-            DELETE FROM
-                embeddings
-        {where_str}
-        """
-        ).fetchall()[0]
-        return [uuid.UUID(x[0]) for x in uuids_deleted]
+        limit = limit or 2**63 - 1
+        offset = offset or 0
 
-    @override
-    def get_by_ids(
-        self, uuids: List[UUID], columns: Optional[List[str]] = None
-    ) -> Sequence:
-        # select from duckdb table where ids are in the list
-        if not isinstance(uuids, list):
-            raise TypeError(f"Expected ids to be a list, got {uuids}")
-
-        if not uuids:
-            # create an empty pandas dataframe
-            return pd.DataFrame()
-
-        columns = columns + ["uuid"] if columns else ["uuid"]
-
-        select_columns = db_schema_to_keys() if columns is None else columns
-        response = self._conn.execute(
-            f"""
-            SELECT
-                {",".join(select_columns)}
-            FROM
-                embeddings
-            WHERE
-                uuid IN ({','.join([("'" + str(x) + "'") for x in uuids])})
-        """
-        ).fetchall()
-
-        # sort db results by the order of the uuids
-        response = sorted(
-            response, key=lambda obj: uuids.index(uuid.UUID(obj[len(columns) - 1]))
+        with self._db.tx() as cur:
+            return list(islice(self._records(cur, q), offset, offset + limit))
+
+    def _records(
+        self, cur: Cursor, q: QueryBuilder
+    ) -> Generator[MetadataEmbeddingRecord, None, None]:
+        """Given a cursor and a QueryBuilder, yield a generator of records. Assumes
+        cursor returns rows in ID order."""
+
+        sql, params = get_sql(q)
+        cur.execute(sql, params)
+
+        cur_iterator = iter(cur.fetchone, None)
+        group_iterator = groupby(cur_iterator, lambda r: int(r[0]))
+
+        for _, group in group_iterator:
+            yield self._record(list(group))
+
+    def _record(self, rows: Sequence[Tuple[Any, ...]]) -> MetadataEmbeddingRecord:
+        """Given a list of DB rows with the same ID, construct a
+        MetadataEmbeddingRecord"""
+        _, embedding_id, seq_id = rows[0][:3]
+        metadata = {}
+        for row in rows:
+            key, string_value, int_value, float_value = row[3:]
+            if string_value is not None:
+                metadata[key] = string_value
+            elif int_value is not None:
+                metadata[key] = int_value
+            elif float_value is not None:
+                metadata[key] = float_value
+
+        return MetadataEmbeddingRecord(
+            id=embedding_id,
+            seq_id=_decode_seq_id(seq_id),
+            metadata=metadata or None,
         )
 
-        return response
-
-    @override
-    def raw_sql(self, raw_sql):
-        return self._conn.execute(raw_sql).df()
-
-    # TODO: This method should share logic with clickhouse impl
-    @override
-    def reset_state(self):
-        self._conn.execute("DROP TABLE collections")
-        self._conn.execute("DROP TABLE embeddings")
-        self._create_table_collections(self._conn)
-        self._create_table_embeddings(self._conn)
-
-        self.reset_indexes()
-
-    def __del__(self):
-        logger.info("Exiting: Cleaning up .chroma directory")
-        self.reset_indexes()
-
-    @override
-    def persist(self) -> None:
-        raise NotImplementedError(
-            "Set chroma_db_impl='duckdb+parquet' to get persistence functionality"
+    def _insert_record(
+        self, cur: Cursor, record: EmbeddingRecord, upsert: bool
+    ) -> None:
+        """Add or update a single EmbeddingRecord into the DB"""
+
+        t = Table("embeddings")
+        q = (
+            self._db.querybuilder()
+            .into(t)
+            .columns(t.segment_id, t.embedding_id, t.seq_id)
+            .where(t.segment_id == ParameterValue(self._db.uuid_to_db(self._id)))
+            .where(t.embedding_id == ParameterValue(record["id"]))
+        ).insert(
+            ParameterValue(self._db.uuid_to_db(self._id)),
+            ParameterValue(record["id"]),
+            ParameterValue(_encode_seq_id(record["seq_id"])),
         )
-
-
-class PersistentDuckDB(DuckDB):
-    _save_folder = None
-
-    def __init__(self, system: System):
-        super().__init__(system=system)
-
-        system.settings.require("persist_directory")
-
-        if system.settings.persist_directory == ".chroma":
-            raise ValueError(
-                "You cannot use chroma's cache directory .chroma/, please set a different directory"
+        sql, params = get_sql(q)
+        sql = sql + "RETURNING id"
+        try:
+            id = cur.execute(sql, params).fetchone()[0]
+        except sqlite3.IntegrityError:
+            # Can't use INSERT OR REPLACE here because it changes the primary key.
+            if upsert:
+                return self._update_record(cur, record)
+            else:
+                logger.warning(f"Insert of existing embedding ID: {record['id']}")
+                # We are trying to add for a record that already exists. Fail the call.
+                # We don't throw an exception since this is in principal an async path
+                return
+
+        if record["metadata"]:
+            self._update_metadata(cur, id, record["metadata"])
+
+    def _update_metadata(self, cur: Cursor, id: int, metadata: UpdateMetadata) -> None:
+        """Update the metadata for a single EmbeddingRecord"""
+        t = Table("embedding_metadata")
+        to_delete = [k for k, v in metadata.items() if v is None]
+        if to_delete:
+            q = (
+                self._db.querybuilder()
+                .from_(t)
+                .where(t.id == ParameterValue(id))
+                .where(t.key.isin(ParameterValue(to_delete)))
+                .delete()
             )
+            sql, params = get_sql(q)
+            cur.execute(sql, params)
 
-        self._save_folder = system.settings.persist_directory
-        self.load()
-        # https://docs.python.org/3/library/atexit.html
-        atexit.register(self.persist)
-
-    def set_save_folder(self, path):
-        self._save_folder = path
+        if "chroma:document" in metadata:
+            t = Table("embedding_fulltext")
+            q = (
+                self._db.querybuilder()
+                .from_(t)
+                .where(t.id == ParameterValue(id))
+                .delete()
+            )
+            sql, params = get_sql(q)
+            cur.execute(sql, params)
 
-    def get_save_folder(self):
-        return self._save_folder
+        self._insert_metadata(cur, id, metadata)
 
-    @override
-    def persist(self):
-        """
-        Persist the database to disk
-        """
-        logger.info(
-            f"Persisting DB to disk, putting it in the save folder: {self._save_folder}"
+    def _insert_metadata(self, cur: Cursor, id: int, metadata: UpdateMetadata) -> None:
+        """Insert or update each metadata row for a single embedding record"""
+        t = Table("embedding_metadata")
+        q = (
+            self._db.querybuilder()
+            .into(t)
+            .columns(t.id, t.key, t.string_value, t.int_value, t.float_value)
         )
-        if self._conn is None:
-            return
-
-        if not os.path.exists(self._save_folder):
-            os.makedirs(self._save_folder)
+        for key, value in metadata.items():
+            if isinstance(value, str):
+                q = q.insert(
+                    ParameterValue(id),
+                    ParameterValue(key),
+                    ParameterValue(value),
+                    None,
+                    None,
+                )
+            elif isinstance(value, int):
+                q = q.insert(
+                    ParameterValue(id),
+                    ParameterValue(key),
+                    None,
+                    ParameterValue(value),
+                    None,
+                )
+            elif isinstance(value, float):
+                q = q.insert(
+                    ParameterValue(id),
+                    ParameterValue(key),
+                    None,
+                    None,
+                    ParameterValue(value),
+                )
 
-        # if the db is empty, dont save
-        if self._conn.query("SELECT COUNT() FROM embeddings") == 0:
-            return
-
-        self._conn.execute(
-            f"""
-            COPY
-                (SELECT * FROM embeddings)
-            TO '{self._save_folder}/chroma-embeddings.parquet'
-                (FORMAT PARQUET);
-        """
-        )
+        sql, params = get_sql(q)
+        sql = sql.replace("INSERT", "INSERT OR REPLACE")
+        if sql:
+            cur.execute(sql, params)
+
+        if "chroma:document" in metadata:
+            t = Table("embedding_fulltext")
+            q = (
+                self._db.querybuilder()
+                .into(t)
+                .columns(t.id, t.string_value)
+                .insert(ParameterValue(id), ParameterValue(metadata["chroma:document"]))
+            )
+            sql, params = get_sql(q)
+            cur.execute(sql, params)
 
-        self._conn.execute(
-            f"""
-            COPY
-                (SELECT * FROM collections)
-            TO '{self._save_folder}/chroma-collections.parquet'
-                (FORMAT PARQUET);
-        """
+    def _delete_record(self, cur: Cursor, record: EmbeddingRecord) -> None:
+        """Delete a single EmbeddingRecord from the DB"""
+        t = Table("embeddings")
+        q = (
+            self._db.querybuilder()
+            .from_(t)
+            .where(t.segment_id == ParameterValue(self._db.uuid_to_db(self._id)))
+            .where(t.embedding_id == ParameterValue(record["id"]))
+            .delete()
         )
-
-    def load(self):
-        """
-        Load the database from disk
-        """
-        if not os.path.exists(self._save_folder):
-            os.makedirs(self._save_folder)
-
-        # load in the embeddings
-        if not os.path.exists(f"{self._save_folder}/chroma-embeddings.parquet"):
-            logger.info(f"No existing DB found in {self._save_folder}, skipping load")
+        sql, params = get_sql(q)
+        sql = sql + " RETURNING id"
+        result = cur.execute(sql, params).fetchone()
+        if result is None:
+            logger.warning(f"Delete of nonexisting embedding ID: {record['id']}")
         else:
-            path = self._save_folder + "/chroma-embeddings.parquet"
-            self._conn.execute(
-                f"INSERT INTO embeddings SELECT * FROM read_parquet('{path}');"
-            )
-            logger.info(
-                f"""loaded in {self._conn.query(f"SELECT COUNT() FROM embeddings").fetchall()[0][0]} embeddings"""
+            id = result[0]
+
+            # Manually delete metadata; cannot use cascade because
+            # that triggers on replace
+            metadata_t = Table("embedding_metadata")
+            q = (
+                self._db.querybuilder()
+                .from_(metadata_t)
+                .where(metadata_t.id == ParameterValue(id))
+                .delete()
             )
+            sql, params = get_sql(q)
+            cur.execute(sql, params)
 
-        # load in the collections
-        if not os.path.exists(f"{self._save_folder}/chroma-collections.parquet"):
-            logger.info(f"No existing DB found in {self._save_folder}, skipping load")
+    def _update_record(self, cur: Cursor, record: EmbeddingRecord) -> None:
+        """Update a single EmbeddingRecord in the DB"""
+        t = Table("embeddings")
+        q = (
+            self._db.querybuilder()
+            .update(t)
+            .set(t.seq_id, ParameterValue(_encode_seq_id(record["seq_id"])))
+            .where(t.segment_id == ParameterValue(self._db.uuid_to_db(self._id)))
+            .where(t.embedding_id == ParameterValue(record["id"]))
+        )
+        sql, params = get_sql(q)
+        sql = sql + " RETURNING id"
+        result = cur.execute(sql, params).fetchone()
+        if result is None:
+            logger.warning(f"Update of nonexisting embedding ID: {record['id']}")
         else:
-            path = self._save_folder + "/chroma-collections.parquet"
-            self._conn.execute(
-                f"INSERT INTO collections SELECT * FROM read_parquet('{path}');"
-            )
-            logger.info(
-                f"""loaded in {self._conn.query(f"SELECT COUNT() FROM collections").fetchall()[0][0]} collections"""
-            )
+            id = result[0]
+            if record["metadata"]:
+                self._update_metadata(cur, id, record["metadata"])
+
+    def _write_metadata(self, records: Sequence[EmbeddingRecord]) -> None:
+        """Write embedding metadata to the database. Care should be taken to ensure
+        records are append-only (that is, that seq-ids should increase monotonically)"""
+        with self._db.tx() as cur:
+            for record in records:
+                q = (
+                    self._db.querybuilder()
+                    .into(Table("max_seq_id"))
+                    .columns("segment_id", "seq_id")
+                    .insert(
+                        ParameterValue(self._db.uuid_to_db(self._id)),
+                        ParameterValue(_encode_seq_id(record["seq_id"])),
+                    )
+                )
+                sql, params = get_sql(q)
+                sql = sql.replace("INSERT", "INSERT OR REPLACE")
+                cur.execute(sql, params)
+
+                if record["operation"] == Operation.ADD:
+                    self._insert_record(cur, record, False)
+                elif record["operation"] == Operation.UPSERT:
+                    self._insert_record(cur, record, True)
+                elif record["operation"] == Operation.DELETE:
+                    self._delete_record(cur, record)
+                elif record["operation"] == Operation.UPDATE:
+                    self._update_record(cur, record)
+
+    def _where_map_criterion(
+        self, q: QueryBuilder, where: Where, embeddings_t: Table, metadata_t: Table
+    ) -> Criterion:
+        clause: list[Criterion] = []
+
+        for k, v in where.items():
+            if k == "$and":
+                criteria = [
+                    self._where_map_criterion(q, w, embeddings_t, metadata_t)
+                    for w in cast(Sequence[Where], v)
+                ]
+                clause.append(reduce(lambda x, y: x & y, criteria))
+            elif k == "$or":
+                criteria = [
+                    self._where_map_criterion(q, w, embeddings_t, metadata_t)
+                    for w in cast(Sequence[Where], v)
+                ]
+                clause.append(reduce(lambda x, y: x | y, criteria))
+            else:
+                expr = cast(Union[LiteralValue, Dict[WhereOperator, LiteralValue]], v)
+                sq = (
+                    self._db.querybuilder()
+                    .from_(metadata_t)
+                    .select(metadata_t.id)
+                    .where(metadata_t.key == ParameterValue(k))
+                    .where(_where_clause(expr, metadata_t))
+                )
+                clause.append(embeddings_t.id.isin(sq))
+        return reduce(lambda x, y: x & y, clause)
 
-    def __del__(self):
-        # No-op for duckdb with persistence since the base class will delete the indexes
-        pass
+    class EscapedLike(Function):  # type: ignore
+        def __init__(self, column_name: str, search_term: str, escape_char: str = "\\"):
+            self.column_name = column_name
+            self.search_term = search_term
+            self.escape_char = escape_char
+            super().__init__("LIKE", column_name, search_term)
+
+        def get_function_sql(self, **kwargs: Any) -> str:
+            return f"{self.column_name} LIKE {self.search_term} ESCAPE '{self.escape_char}'"
+
+    def _where_doc_criterion(
+        self,
+        q: QueryBuilder,
+        where: WhereDocument,
+        embeddings_t: Table,
+        fulltext_t: Table,
+    ) -> Criterion:
+        for k, v in where.items():
+            if k == "$and":
+                criteria = [
+                    self._where_doc_criterion(q, w, embeddings_t, fulltext_t)
+                    for w in cast(Sequence[WhereDocument], v)
+                ]
+                return reduce(lambda x, y: x & y, criteria)
+            elif k == "$or":
+                criteria = [
+                    self._where_doc_criterion(q, w, embeddings_t, fulltext_t)
+                    for w in cast(Sequence[WhereDocument], v)
+                ]
+                return reduce(lambda x, y: x | y, criteria)
+            elif k == "$contains":
+                v = cast(str, v)
+                search_term = f"%{_escape_characters(v)}%"
+
+                sq = (
+                    self._db.querybuilder()
+                    .from_(fulltext_t)
+                    .select(fulltext_t.id)
+                    .where(
+                        self.EscapedLike(
+                            fulltext_t.string_value,
+                            ParameterValue(search_term),
+                        )
+                    )
+                )
+                return embeddings_t.id.isin(sq)
+            else:
+                raise ValueError(f"Unknown where_doc operator {k}")
+        raise ValueError("Empty where_doc")
 
-    @override
-    def reset_state(self):
-        super().reset_state()
-        # empty the save folder
-        import shutil
-        import os
 
-        shutil.rmtree(self._save_folder)
-        os.mkdir(self._save_folder)
+def _escape_characters(string: str) -> str:
+    """Escape % and _ characters in a string with a backslash as they are reserved in
+    LIKE clauses"""
+    escaped_string = ""
+    for char in string:
+        if char == "%" or char == "_":
+            escaped_string += "\\"
+        escaped_string += char
+    return escaped_string
+
+
+def _encode_seq_id(seq_id: SeqId) -> bytes:
+    """Encode a SeqID into a byte array"""
+    if seq_id.bit_length() < 64:
+        return int.to_bytes(seq_id, 8, "big")
+    elif seq_id.bit_length() < 192:
+        return int.to_bytes(seq_id, 24, "big")
+    else:
+        raise ValueError(f"Unsupported SeqID: {seq_id}")
+
+
+def _decode_seq_id(seq_id_bytes: bytes) -> SeqId:
+    """Decode a byte array into a SeqID"""
+    if len(seq_id_bytes) == 8:
+        return int.from_bytes(seq_id_bytes, "big")
+    elif len(seq_id_bytes) == 24:
+        return int.from_bytes(seq_id_bytes, "big")
+    else:
+        raise ValueError(f"Unknown SeqID type with length {len(seq_id_bytes)}")
+
+
+def _where_clause(
+    expr: Union[LiteralValue, Dict[WhereOperator, LiteralValue]],
+    table: Table,
+) -> Criterion:
+    """Given a field name, an expression, and a table, construct a Pypika Criterion"""
+
+    # Literal value case
+    if isinstance(expr, (str, int, float)):
+        return _where_clause({"$eq": expr}, table)
+
+    # Operator dict case
+    operator, value = next(iter(expr.items()))
+    return _value_criterion(value, operator, table)
+
+
+def _value_criterion(value: LiteralValue, op: WhereOperator, table: Table) -> Criterion:
+    """Return a criterion to compare a value with the appropriate columns given its type
+    and the operation type."""
+
+    if isinstance(value, str):
+        cols = [table.string_value]
+    elif isinstance(value, int) and op in ("$eq", "$ne"):
+        cols = [table.int_value]
+    elif isinstance(value, float) and op in ("$eq", "$ne"):
+        cols = [table.float_value]
+    else:
+        cols = [table.int_value, table.float_value]
+
+    if op == "$eq":
+        col_exprs = [col == ParameterValue(value) for col in cols]
+    elif op == "$ne":
+        col_exprs = [col != ParameterValue(value) for col in cols]
+    elif op == "$gt":
+        col_exprs = [col > ParameterValue(value) for col in cols]
+    elif op == "$gte":
+        col_exprs = [col >= ParameterValue(value) for col in cols]
+    elif op == "$lt":
+        col_exprs = [col < ParameterValue(value) for col in cols]
+    elif op == "$lte":
+        col_exprs = [col <= ParameterValue(value) for col in cols]
+
+    if op == "$ne":
+        return reduce(lambda x, y: x & y, col_exprs)
+    else:
+        return reduce(lambda x, y: x | y, col_exprs)
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/db/impl/sqlite.py` & `chromadb-client-0.4.1.dev0/chromadb/db/impl/sqlite.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,34 @@
+from chromadb.db.impl.sqlite_pool import Connection, LockPool, PerThreadPool, Pool
 from chromadb.db.migrations import MigratableDB, Migration
 from chromadb.config import System, Settings
 import chromadb.db.base as base
 from chromadb.db.mixins.embeddings_queue import SqlEmbeddingsQueue
 from chromadb.db.mixins.sysdb import SqlSysDB
 import sqlite3
 from overrides import override
 import pypika
 from typing import Sequence, cast, Optional, Type, Any
 from typing_extensions import Literal
 from types import TracebackType
 import os
 from uuid import UUID
 from threading import local
+from importlib_resources import files
+from importlib_resources.abc import Traversable
 
 
 class TxWrapper(base.TxWrapper):
-    def __init__(self, conn: sqlite3.Connection, stack: local) -> None:
+    _conn: Connection
+    _pool: Pool
+
+    def __init__(self, conn_pool: Pool, stack: local):
         self._tx_stack = stack
-        self._conn = conn
+        self._conn = conn_pool.connect()
+        self._pool = conn_pool
 
     @override
     def __enter__(self) -> base.Cursor:
         if len(self._tx_stack.stack) == 0:
             self._conn.execute("BEGIN;")
         self._tx_stack.stack.append(self)
         return self._conn.cursor()  # type: ignore
@@ -35,49 +42,63 @@
     ) -> Literal[False]:
         self._tx_stack.stack.pop()
         if len(self._tx_stack.stack) == 0:
             if exc_type is None:
                 self._conn.commit()
             else:
                 self._conn.rollback()
+        self._pool.return_to_pool(self._conn)
         return False
 
 
 class SqliteDB(MigratableDB, SqlEmbeddingsQueue, SqlSysDB):
-    _conn: sqlite3.Connection
+    _conn_pool: Pool
     _settings: Settings
-    _migration_dirs: Sequence[str]
+    _migration_imports: Sequence[Traversable]
     _db_file: str
     _tx_stack: local
+    _is_persistent: bool
 
     def __init__(self, system: System):
         self._settings = system.settings
-        self._migration_dirs = [
-            "migrations/embeddings_queue",
-            "migrations/sysdb",
-            "migrations/metadb",
+        self._migration_imports = [
+            files("chromadb.migrations.embeddings_queue"),
+            files("chromadb.migrations.sysdb"),
+            files("chromadb.migrations.metadb"),
         ]
-        self._db_file = self._settings.require("sqlite_database")
+        self._is_persistent = self._settings.require("is_persistent")
+        if not self._is_persistent:
+            # In order to allow sqlite to be shared between multiple threads, we need to use a
+            # URI connection string with shared cache.
+            # See https://www.sqlite.org/sharedcache.html
+            # https://stackoverflow.com/questions/3315046/sharing-a-memory-database-between-different-threads-in-python-using-sqlite3-pa
+            self._db_file = "file::memory:?cache=shared"
+            self._conn_pool = LockPool(self._db_file, is_uri=True)
+        else:
+            self._db_file = (
+                self._settings.require("persist_directory") + "/chroma.sqlite3"
+            )
+            if not os.path.exists(self._db_file):
+                os.makedirs(os.path.dirname(self._db_file), exist_ok=True)
+            self._conn_pool = PerThreadPool(self._db_file)
         self._tx_stack = local()
         super().__init__(system)
 
     @override
     def start(self) -> None:
         super().start()
-        self._conn = sqlite3.connect(self._db_file)
-        self._conn.isolation_level = None  # Handle commits explicitly
         with self.tx() as cur:
             cur.execute("PRAGMA foreign_keys = ON")
             cur.execute("PRAGMA case_sensitive_like = ON")
         self.initialize_migrations()
 
     @override
     def stop(self) -> None:
         super().stop()
-        self._conn.close()
+        self._conn_pool.close()
 
     @staticmethod
     @override
     def querybuilder() -> Type[pypika.Query]:
         return pypika.Query  # type: ignore
 
     @staticmethod
@@ -87,33 +108,42 @@
 
     @staticmethod
     @override
     def migration_scope() -> str:
         return "sqlite"
 
     @override
-    def migration_dirs(self) -> Sequence[str]:
-        return self._migration_dirs
+    def migration_dirs(self) -> Sequence[Traversable]:
+        return self._migration_imports
 
     @override
     def tx(self) -> TxWrapper:
         if not hasattr(self._tx_stack, "stack"):
             self._tx_stack.stack = []
-        return TxWrapper(self._conn, stack=self._tx_stack)
+        return TxWrapper(self._conn_pool, stack=self._tx_stack)
 
     @override
     def reset_state(self) -> None:
         if not self._settings.require("allow_reset"):
             raise ValueError(
                 "Resetting the database is not allowed. Set `allow_reset` to true in the config in tests or other non-production environments where reset should be permitted."
             )
-        self._conn.close()
-        db_file = self._settings.require("sqlite_database")
-        if db_file != ":memory:":
-            os.remove(db_file)
+        with self.tx() as cur:
+            # Drop all tables
+            cur.execute(
+                """
+                SELECT name FROM sqlite_master
+                WHERE type='table'
+                """
+            )
+            for row in cur.fetchall():
+                cur.execute(f"DROP TABLE IF EXISTS {row[0]}")
+        self._conn_pool.close()
+        if self._is_persistent:
+            os.remove(self._db_file)
         self.start()
         super().reset_state()
 
     @override
     def setup_migrations(self) -> None:
         with self.tx() as cur:
             cur.execute(
@@ -139,40 +169,40 @@
 
             if cur.fetchone()[0] == 0:
                 return False
             else:
                 return True
 
     @override
-    def db_migrations(self, dir: str) -> Sequence[Migration]:
+    def db_migrations(self, dir: Traversable) -> Sequence[Migration]:
         with self.tx() as cur:
             cur.execute(
                 """
                 SELECT dir, version, filename, sql, hash
                 FROM migrations
                 WHERE dir = ?
                 ORDER BY version ASC
                 """,
-                (dir,),
+                (dir.name,),
             )
 
             migrations = []
             for row in cur.fetchall():
-                dir = cast(str, row[0])
-                version = cast(int, row[1])
-                filename = cast(str, row[2])
-                sql = cast(str, row[3])
-                hash = cast(str, row[4])
+                found_dir = cast(str, row[0])
+                found_version = cast(int, row[1])
+                found_filename = cast(str, row[2])
+                found_sql = cast(str, row[3])
+                found_hash = cast(str, row[4])
                 migrations.append(
                     Migration(
-                        dir=dir,
-                        version=version,
-                        filename=filename,
-                        sql=sql,
-                        hash=hash,
+                        dir=found_dir,
+                        version=found_version,
+                        filename=found_filename,
+                        sql=found_sql,
+                        hash=found_hash,
                         scope=self.migration_scope(),
                     )
                 )
             return migrations
 
     @override
     def apply_migration(self, cur: base.Cursor, migration: Migration) -> None:
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/db/migrations.py` & `chromadb-client-0.4.1.dev0/chromadb/db/migrations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Sequence
-from typing_extensions import TypedDict
-import os
+from typing_extensions import TypedDict, NotRequired
+from importlib_resources.abc import Traversable
 import re
 import hashlib
 from chromadb.db.base import SqlDB, Cursor
 from abc import abstractmethod
 from chromadb.config import System, Settings
 
 
 class MigrationFile(TypedDict):
+    path: NotRequired[Traversable]
     dir: str
     filename: str
     version: int
     scope: str
 
 
 class Migration(MigrationFile):
@@ -55,17 +56,20 @@
 class InvalidMigrationFilename(Exception):
     pass
 
 
 class MigratableDB(SqlDB):
     """Simple base class for databases which support basic migrations.
 
-    Migrations are SQL files stored in a project-relative directory. All migrations in
-    the same directory are assumed to be dependent on previous migrations in the same
-    directory, where "previous" is defined on lexographical ordering of filenames.
+    Migrations are SQL files stored as package resources and accessed via
+    importlib_resources.
+
+    All migrations in the same directory are assumed to be dependent on previous
+    migrations in the same directory, where "previous" is defined on lexographical
+    ordering of filenames.
 
     Migrations have a ascending numeric version number and a hash of the file contents.
     When migrations are applied, the hashes of previous migrations are checked to ensure
     that the database is consistent with the source repository. If they are not, an
     error is thrown and no migrations will be applied.
 
     Migration files must follow the naming convention:
@@ -83,15 +87,15 @@
     @staticmethod
     @abstractmethod
     def migration_scope() -> str:
         """The database implementation to use for migrations (e.g, sqlite, pgsql)"""
         pass
 
     @abstractmethod
-    def migration_dirs(self) -> Sequence[str]:
+    def migration_dirs(self) -> Sequence[Traversable]:
         """Directories containing the migration sequences that should be applied to this
         DB."""
         pass
 
     @abstractmethod
     def setup_migrations(self) -> None:
         """Idempotently creates the migrations table"""
@@ -99,15 +103,15 @@
 
     @abstractmethod
     def migrations_initialized(self) -> bool:
         """Return true if the migrations table exists"""
         pass
 
     @abstractmethod
-    def db_migrations(self, dir: str) -> Sequence[Migration]:
+    def db_migrations(self, dir: Traversable) -> Sequence[Migration]:
         """Return a list of all migrations already applied to this database, from the
         given source directory, in ascending order."""
         pass
 
     @abstractmethod
     def apply_migration(self, cur: Cursor, migration: Migration) -> None:
         """Apply a single migration to the database"""
@@ -132,15 +136,15 @@
             db_migrations = self.db_migrations(dir)
             source_migrations = find_migrations(dir, self.migration_scope())
             unapplied_migrations = verify_migration_sequence(
                 db_migrations, source_migrations
             )
             if len(unapplied_migrations) > 0:
                 version = unapplied_migrations[0]["version"]
-                raise UnappliedMigrationsError(dir=dir, version=version)
+                raise UnappliedMigrationsError(dir=dir.name, version=version)
 
     def apply_migrations(self) -> None:
         """Validate existing migrations, and apply all new ones."""
         self.setup_migrations()
         for dir in self.migration_dirs():
             db_migrations = self.db_migrations(dir)
             source_migrations = find_migrations(dir, self.migration_scope())
@@ -153,21 +157,24 @@
 
 
 # Format is <version>-<name>.<scope>.sql
 # e.g, 00001-users.sqlite.sql
 filename_regex = re.compile(r"(\d+)-(.+)\.(.+)\.sql")
 
 
-def _parse_migration_filename(dir: str, filename: str) -> MigrationFile:
+def _parse_migration_filename(
+    dir: str, filename: str, path: Traversable
+) -> MigrationFile:
     """Parse a migration filename into a MigrationFile object"""
     match = filename_regex.match(filename)
     if match is None:
         raise InvalidMigrationFilename("Invalid migration filename: " + filename)
     version, _, scope = match.groups()
     return {
+        "path": path,
         "dir": dir,
         "filename": filename,
         "version": int(version),
         "scope": scope,
     }
 
 
@@ -199,30 +206,34 @@
                 db_hash=db_migration["hash"],
                 source_hash=source_migration["hash"],
             )
 
     return source_migrations[len(db_migrations) :]
 
 
-def find_migrations(dir: str, scope: str) -> Sequence[Migration]:
+def find_migrations(dir: Traversable, scope: str) -> Sequence[Migration]:
     """Return a list of all migration present in the given directory, in ascending
     order. Filter by scope."""
     files = [
-        _parse_migration_filename(dir, filename)
-        for filename in os.listdir(dir)
-        if filename.endswith(".sql")
+        _parse_migration_filename(dir.name, t.name, t)
+        for t in dir.iterdir()
+        if t.name.endswith(".sql")
     ]
     files = list(filter(lambda f: f["scope"] == scope, files))
     files = sorted(files, key=lambda f: f["version"])
     return [_read_migration_file(f) for f in files]
 
 
 def _read_migration_file(file: MigrationFile) -> Migration:
     """Read a migration file"""
-    sql = open(os.path.join(file["dir"], file["filename"])).read()
+    if "path" not in file or not file["path"].is_file():
+        raise FileNotFoundError(
+            f"No migration file found for dir {file['dir']} with filename {file['filename']} and scope {file['scope']} at version {file['version']}"
+        )
+    sql = file["path"].read_text()
     hash = hashlib.md5(sql.encode("utf-8")).hexdigest()
     return {
         "hash": hash,
         "sql": sql,
         "dir": file["dir"],
         "filename": file["filename"],
         "version": file["version"],
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/db/mixins/embeddings_queue.py` & `chromadb-client-0.4.1.dev0/chromadb/db/mixins/embeddings_queue.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/db/mixins/sysdb.py` & `chromadb-client-0.4.1.dev0/chromadb/db/mixins/sysdb.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/db/system.py` & `chromadb-client-0.4.1.dev0/chromadb/db/system.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/errors.py` & `chromadb-client-0.4.1.dev0/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/experimental/density_relevance.ipynb` & `chromadb-client-0.4.1.dev0/chromadb/experimental/density_relevance.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/ingest/__init__.py` & `chromadb-client-0.4.1.dev0/chromadb/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/segment/__init__.py` & `chromadb-client-0.4.1.dev0/chromadb/segment/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional, Sequence, TypeVar, Type
 from abc import abstractmethod
 from chromadb.types import (
     Collection,
     MetadataEmbeddingRecord,
+    Operation,
     VectorEmbeddingRecord,
     Where,
     WhereDocument,
     VectorQuery,
     VectorQueryResult,
     Segment,
     SeqId,
@@ -101,7 +102,14 @@
     def get_segment(self, collection_id: UUID, type: Type[S]) -> S:
         """Return the segment that should be used for servicing queries to a collection.
         Implementations should cache appropriately; clients are intended to call this
         method repeatedly rather than storing the result (thereby giving this
         implementation full control over which segment impls are in or out of memory at
         a given time.)"""
         pass
+
+    @abstractmethod
+    def hint_use_collection(self, collection_id: UUID, hint_type: Operation) -> None:
+        """Signal to the segment manager that a collection is about to be used, so that
+        it can preload segments as needed. This is only a hint, and implementations are
+        free to ignore it."""
+        pass
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/segment/impl/manager/local.py` & `chromadb-client-0.4.1.dev0/chromadb/segment/impl/manager/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,56 @@
+from threading import Lock
 from chromadb.segment import (
     SegmentImplementation,
     SegmentManager,
     MetadataReader,
     VectorReader,
     S,
 )
 from chromadb.config import System, get_class
 from chromadb.db.system import SysDB
 from overrides import override
 from enum import Enum
-from chromadb.types import Collection, Segment, SegmentScope, Metadata
+from chromadb.types import Collection, Operation, Segment, SegmentScope, Metadata
 from typing import Dict, Type, Sequence, Optional, cast
 from uuid import UUID, uuid4
 from collections import defaultdict
 
 
 class SegmentType(Enum):
     SQLITE = "urn:chroma:segment/metadata/sqlite"
     HNSW_LOCAL_MEMORY = "urn:chroma:segment/vector/hnsw-local-memory"
+    HNSW_LOCAL_PERSISTED = "urn:chroma:segment/vector/hnsw-local-persisted"
 
 
 SEGMENT_TYPE_IMPLS = {
     SegmentType.SQLITE: "chromadb.segment.impl.metadata.sqlite.SqliteMetadataSegment",
     SegmentType.HNSW_LOCAL_MEMORY: "chromadb.segment.impl.vector.local_hnsw.LocalHnswSegment",
+    SegmentType.HNSW_LOCAL_PERSISTED: "chromadb.segment.impl.vector.local_persistent_hnsw.PersistentLocalHnswSegment",
 }
 
 
 class LocalSegmentManager(SegmentManager):
     _sysdb: SysDB
     _system: System
     _instances: Dict[UUID, SegmentImplementation]
     _segment_cache: Dict[UUID, Dict[SegmentScope, Segment]]
+    _vector_segment_type: SegmentType = SegmentType.HNSW_LOCAL_MEMORY
+    _lock: Lock
 
     def __init__(self, system: System):
         super().__init__(system)
         self._sysdb = self.require(SysDB)
         self._system = system
         self._instances = {}
         self._segment_cache = defaultdict(dict)
+        self._lock = Lock()
+
+        if self._system.settings.require("is_persistent"):
+            self._vector_segment_type = SegmentType.HNSW_LOCAL_PERSISTED
 
     @override
     def start(self) -> None:
         for instance in self._instances.values():
             instance.start()
         super().start()
 
@@ -58,15 +67,15 @@
         self._instances = {}
         self._segment_cache = defaultdict(dict)
         super().reset_state()
 
     @override
     def create_segments(self, collection: Collection) -> Sequence[Segment]:
         vector_segment = _segment(
-            SegmentType.HNSW_LOCAL_MEMORY, SegmentScope.VECTOR, collection
+            self._vector_segment_type, SegmentScope.VECTOR, collection
         )
         metadata_segment = _segment(
             SegmentType.SQLITE, SegmentScope.METADATA, collection
         )
         return [vector_segment, metadata_segment]
 
     @override
@@ -93,17 +102,28 @@
         if scope not in self._segment_cache[collection_id]:
             segments = self._sysdb.get_segments(collection=collection_id, scope=scope)
             known_types = set([k.value for k in SEGMENT_TYPE_IMPLS.keys()])
             # Get the first segment of a known type
             segment = next(filter(lambda s: s["type"] in known_types, segments))
             self._segment_cache[collection_id][scope] = segment
 
-        instance = self._instance(self._segment_cache[collection_id][scope])
+        # Instances must be atomically created, so we use a lock to ensure that only one thread
+        # creates the instance.
+        with self._lock:
+            instance = self._instance(self._segment_cache[collection_id][scope])
         return cast(S, instance)
 
+    @override
+    def hint_use_collection(self, collection_id: UUID, hint_type: Operation) -> None:
+        # The local segment manager responds to hints by pre-loading both the metadata and vector
+        # segments for the given collection.
+        for type in [MetadataReader, VectorReader]:
+            # Just use get_segment to load the segment into the cache
+            self.get_segment(collection_id, type)
+
     def _cls(self, segment: Segment) -> Type[SegmentImplementation]:
         classname = SEGMENT_TYPE_IMPLS[SegmentType(segment["type"])]
         cls = get_class(classname, SegmentImplementation)
         return cls
 
     def _instance(self, segment: Segment) -> SegmentImplementation:
         if segment["id"] not in self._instances:
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/server/fastapi/__init__.py` & `chromadb-client-0.4.1.dev0/chromadb/server/fastapi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -88,69 +88,97 @@
 
         self.router = fastapi.APIRouter()
 
         self.router.add_api_route("/api/v1", self.root, methods=["GET"])
         self.router.add_api_route("/api/v1/reset", self.reset, methods=["POST"])
         self.router.add_api_route("/api/v1/version", self.version, methods=["GET"])
         self.router.add_api_route("/api/v1/heartbeat", self.heartbeat, methods=["GET"])
-        self.router.add_api_route("/api/v1/persist", self.persist, methods=["POST"])
-        self.router.add_api_route("/api/v1/raw_sql", self.raw_sql, methods=["POST"])
+        self.router.add_api_route(
+            "/api/v1/raw_sql", self.raw_sql, methods=["POST"], response_model=None
+        )
 
         self.router.add_api_route(
-            "/api/v1/collections", self.list_collections, methods=["GET"]
+            "/api/v1/collections",
+            self.list_collections,
+            methods=["GET"],
+            response_model=None,
         )
         self.router.add_api_route(
-            "/api/v1/collections", self.create_collection, methods=["POST"]
+            "/api/v1/collections",
+            self.create_collection,
+            methods=["POST"],
+            response_model=None,
         )
 
         self.router.add_api_route(
             "/api/v1/collections/{collection_id}/add",
             self.add,
             methods=["POST"],
             status_code=status.HTTP_201_CREATED,
+            response_model=None,
         )
         self.router.add_api_route(
-            "/api/v1/collections/{collection_id}/update", self.update, methods=["POST"]
+            "/api/v1/collections/{collection_id}/update",
+            self.update,
+            methods=["POST"],
+            response_model=None,
         )
         self.router.add_api_route(
-            "/api/v1/collections/{collection_id}/upsert", self.upsert, methods=["POST"]
+            "/api/v1/collections/{collection_id}/upsert",
+            self.upsert,
+            methods=["POST"],
+            response_model=None,
         )
         self.router.add_api_route(
-            "/api/v1/collections/{collection_id}/get", self.get, methods=["POST"]
+            "/api/v1/collections/{collection_id}/get",
+            self.get,
+            methods=["POST"],
+            response_model=None,
         )
         self.router.add_api_route(
-            "/api/v1/collections/{collection_id}/delete", self.delete, methods=["POST"]
+            "/api/v1/collections/{collection_id}/delete",
+            self.delete,
+            methods=["POST"],
+            response_model=None,
         )
         self.router.add_api_route(
-            "/api/v1/collections/{collection_id}/count", self.count, methods=["GET"]
+            "/api/v1/collections/{collection_id}/count",
+            self.count,
+            methods=["GET"],
+            response_model=None,
         )
         self.router.add_api_route(
             "/api/v1/collections/{collection_id}/query",
             self.get_nearest_neighbors,
             methods=["POST"],
+            response_model=None,
         )
         self.router.add_api_route(
             "/api/v1/collections/{collection_name}/create_index",
             self.create_index,
             methods=["POST"],
+            response_model=None,
         )
         self.router.add_api_route(
             "/api/v1/collections/{collection_name}",
             self.get_collection,
             methods=["GET"],
+            response_model=None,
         )
         self.router.add_api_route(
             "/api/v1/collections/{collection_id}",
             self.update_collection,
             methods=["PUT"],
+            response_model=None,
         )
         self.router.add_api_route(
             "/api/v1/collections/{collection_name}",
             self.delete_collection,
             methods=["DELETE"],
+            response_model=None,
         )
 
         self._app.include_router(self.router)
 
         use_route_names_as_operation_ids(self._app)
 
     def app(self) -> fastapi.FastAPI:
@@ -158,17 +186,14 @@
 
     def root(self) -> Dict[str, int]:
         return {"nanosecond heartbeat": self._api.heartbeat()}
 
     def heartbeat(self) -> Dict[str, int]:
         return self.root()
 
-    def persist(self) -> None:
-        self._api.persist()
-
     def version(self) -> str:
         return self._api.get_version()
 
     def list_collections(self) -> Sequence[Collection]:
         return self._api.list_collections()
 
     def create_collection(self, collection: CreateCollection) -> Collection:
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/server/fastapi/types.py` & `chromadb-client-0.4.1.dev0/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/telemetry/__init__.py` & `chromadb-client-0.4.1.dev0/chromadb/telemetry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from threading import Event, Thread
 import chromadb
 from chromadb.config import Component
 from pathlib import Path
 from enum import Enum
 
 TELEMETRY_WHITELISTED_SETTINGS = [
-    "chroma_db_impl",
     "chroma_api_impl",
+    "is_persistent",
     "chroma_server_ssl_enabled",
 ]
 
 
 class ServerContext(Enum):
     NONE = "None"
     FASTAPI = "FastAPI"
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/telemetry/events.py` & `chromadb-client-0.4.1.dev0/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/telemetry/posthog.py` & `chromadb-client-0.4.1.dev0/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/db/test_base.py` & `chromadb-client-0.4.1.dev0/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/db/test_migrations.py` & `chromadb-client-0.4.1.dev0/chromadb/test/db/test_migrations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import pytest
+from importlib_resources import files
 from typing import Generator, List, Callable
 import chromadb.db.migrations as migrations
 from chromadb.db.impl.sqlite import SqliteDB
 from chromadb.config import System, Settings
 from pytest import FixtureRequest
 import copy
 
 
 def sqlite() -> Generator[migrations.MigratableDB, None, None]:
     """Fixture generator for sqlite DB"""
     db = SqliteDB(
         System(
-            Settings(sqlite_database=":memory:", migrations="none", allow_reset=True)
+            Settings(
+                migrations="none",
+                allow_reset=True,
+            )
         )
     )
     db.start()
     yield db
 
 
 def db_fixtures() -> List[Callable[[], Generator[migrations.MigratableDB, None, None]]]:
@@ -43,18 +47,17 @@
         rows = cursor.execute("SELECT * FROM migrations").fetchall()
         assert len(rows) == 0
 
 
 def test_migrations(db: migrations.MigratableDB) -> None:
     db.initialize_migrations()
 
-    db_migrations = db.db_migrations("chromadb/test/db/migrations")
-    source_migrations = migrations.find_migrations(
-        "chromadb/test/db/migrations", db.migration_scope()
-    )
+    dir = files("chromadb.test.db.migrations")
+    db_migrations = db.db_migrations(dir)
+    source_migrations = migrations.find_migrations(dir, db.migration_scope())
 
     unapplied_migrations = migrations.verify_migration_sequence(
         db_migrations, source_migrations
     )
 
     assert unapplied_migrations == source_migrations
 
@@ -62,15 +65,15 @@
         rows = cur.execute("SELECT * FROM migrations").fetchall()
         assert len(rows) == 0
 
     with db.tx() as cur:
         for m in unapplied_migrations[:-1]:
             db.apply_migration(cur, m)
 
-    db_migrations = db.db_migrations("chromadb/test/db/migrations")
+    db_migrations = db.db_migrations(dir)
     unapplied_migrations = migrations.verify_migration_sequence(
         db_migrations, source_migrations
     )
 
     assert len(unapplied_migrations) == 1
     assert unapplied_migrations[0]["version"] == 3
 
@@ -81,15 +84,15 @@
         with pytest.raises(Exception):
             cur.execute("SELECT * FROM table3").fetchall()
 
     with db.tx() as cur:
         for m in unapplied_migrations:
             db.apply_migration(cur, m)
 
-    db_migrations = db.db_migrations("chromadb/test/db/migrations")
+    db_migrations = db.db_migrations(dir)
     unapplied_migrations = migrations.verify_migration_sequence(
         db_migrations, source_migrations
     )
 
     assert len(unapplied_migrations) == 0
 
     with db.tx() as cur:
@@ -98,29 +101,28 @@
 
 
 def test_tampered_migration(db: migrations.MigratableDB) -> None:
     db.reset_state()
 
     db.setup_migrations()
 
-    source_migrations = migrations.find_migrations(
-        "chromadb/test/db/migrations", db.migration_scope()
-    )
+    dir = files("chromadb.test.db.migrations")
+    source_migrations = migrations.find_migrations(dir, db.migration_scope())
 
-    db_migrations = db.db_migrations("chromadb/test/db/migrations")
+    db_migrations = db.db_migrations(dir)
 
     unapplied_migrations = migrations.verify_migration_sequence(
         db_migrations, source_migrations
     )
 
     with db.tx() as cur:
         for m in unapplied_migrations:
             db.apply_migration(cur, m)
 
-    db_migrations = db.db_migrations("chromadb/test/db/migrations")
+    db_migrations = db.db_migrations(dir)
     unapplied_migrations = migrations.verify_migration_sequence(
         db_migrations, source_migrations
     )
     assert len(unapplied_migrations) == 0
 
     inconsistent_version_migrations = copy.deepcopy(source_migrations)
     inconsistent_version_migrations[0]["version"] = 2
@@ -139,15 +141,16 @@
         )
 
 
 def test_initialization(
     monkeypatch: pytest.MonkeyPatch, db: migrations.MigratableDB
 ) -> None:
     db.reset_state()
-    monkeypatch.setattr(db, "migration_dirs", lambda: ["chromadb/test/db/migrations"])
+    dir = files("chromadb.test.db.migrations")
+    monkeypatch.setattr(db, "migration_dirs", lambda: [dir])
 
     assert not db.migrations_initialized()
 
     with pytest.raises(migrations.UninitializedMigrationsError):
         db.validate_migrations()
 
     db.setup_migrations()
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/db/test_system.py` & `chromadb-client-0.4.1.dev0/chromadb/test/db/test_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,46 @@
+import os
+import shutil
+import tempfile
 import pytest
 from typing import Generator, List, Callable, Dict, Union
 from chromadb.types import Collection, Segment, SegmentScope
 from chromadb.db.impl.sqlite import SqliteDB
 from chromadb.config import System, Settings
 from chromadb.db.system import SysDB
 from chromadb.db.base import NotFoundError, UniqueConstraintError
 from pytest import FixtureRequest
 import uuid
 
 
 def sqlite() -> Generator[SysDB, None, None]:
     """Fixture generator for sqlite DB"""
-    db = SqliteDB(System(Settings(sqlite_database=":memory:", allow_reset=True)))
+    db = SqliteDB(System(Settings(allow_reset=True)))
     db.start()
     yield db
     db.stop()
 
 
+def sqlite_persistent() -> Generator[SysDB, None, None]:
+    """Fixture generator for sqlite DB"""
+    save_path = tempfile.mkdtemp()
+    db = SqliteDB(
+        System(
+            Settings(allow_reset=True, is_persistent=True, persist_directory=save_path)
+        )
+    )
+    db.start()
+    yield db
+    db.stop()
+    if os.path.exists(save_path):
+        shutil.rmtree(save_path)
+
+
 def db_fixtures() -> List[Callable[[], Generator[SysDB, None, None]]]:
-    return [sqlite]
+    return [sqlite, sqlite_persistent]
 
 
 @pytest.fixture(scope="module", params=db_fixtures())
 def sysdb(request: FixtureRequest) -> Generator[SysDB, None, None]:
     yield next(request.param())
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/ingest/test_producer_consumer.py` & `chromadb-client-0.4.1.dev0/chromadb/test/ingest/test_producer_consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+import shutil
+import tempfile
 import pytest
 from itertools import count
 from typing import (
     Generator,
     List,
     Callable,
     Optional,
@@ -22,23 +25,37 @@
 from chromadb.config import System, Settings
 from pytest import FixtureRequest, approx
 from asyncio import Event, wait_for, TimeoutError
 
 
 def sqlite() -> Generator[Tuple[Producer, Consumer], None, None]:
     """Fixture generator for sqlite Producer + Consumer"""
-    system = System(Settings(sqlite_database=":memory:", allow_reset=True))
+    system = System(Settings(allow_reset=True))
     db = system.require(SqliteDB)
     system.start()
     yield db, db
     system.stop()
 
 
+def sqlite_persistent() -> Generator[Tuple[Producer, Consumer], None, None]:
+    """Fixture generator for sqlite_persistent Producer + Consumer"""
+    save_path = tempfile.mkdtemp()
+    system = System(
+        Settings(allow_reset=True, is_persistent=True, persist_directory=save_path)
+    )
+    db = system.require(SqliteDB)
+    system.start()
+    yield db, db
+    system.stop()
+    if os.path.exists(save_path):
+        shutil.rmtree(save_path)
+
+
 def fixtures() -> List[Callable[[], Generator[Tuple[Producer, Consumer], None, None]]]:
-    return [sqlite]
+    return [sqlite, sqlite_persistent]
 
 
 @pytest.fixture(scope="module", params=fixtures())
 def producer_consumer(
     request: FixtureRequest,
 ) -> Generator[Tuple[Producer, Consumer], None, None]:
     yield next(request.param())
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/property/invariants.py` & `chromadb-client-0.4.1.dev0/chromadb/test/property/invariants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import math
 from chromadb.test.property.strategies import NormalizedRecordSet, RecordSet
-from typing import Callable, Optional, Tuple, Union, List, TypeVar, cast, Dict
+from typing import Callable, Optional, Tuple, Union, List, TypeVar, cast
 from typing_extensions import Literal
 import numpy as np
 import numpy.typing as npt
 from chromadb.api import types
 from chromadb.api.models.Collection import Collection
 from hypothesis import note
 from hypothesis.errors import InvalidArgument
 
+from chromadb.utils import distance_functions
+
 T = TypeVar("T")
 
 
 def wrap(value: Union[T, List[T]]) -> List[T]:
     """Wrap a value in a list if it is not a list"""
     if value is None:
         raise InvalidArgument("value cannot be None")
@@ -120,31 +122,20 @@
 
 
 def no_duplicates(collection: Collection) -> None:
     ids = collection.get()["ids"]
     assert len(ids) == len(set(ids))
 
 
-# These match what the spec of hnswlib is
-# This epsilon is used to prevent division by zero and the value is the same
-# https://github.com/nmslib/hnswlib/blob/359b2ba87358224963986f709e593d799064ace6/python_bindings/bindings.cpp#L238
-NORM_EPS = 1e-30
-distance_functions: Dict[str, Callable[[npt.ArrayLike, npt.ArrayLike], float]] = {
-    "l2": lambda x, y: np.linalg.norm(x - y) ** 2,  # type: ignore
-    "cosine": lambda x, y: 1 - np.dot(x, y) / ((np.linalg.norm(x) + NORM_EPS) * (np.linalg.norm(y) + NORM_EPS)),  # type: ignore
-    "ip": lambda x, y: 1 - np.dot(x, y),  # type: ignore
-}
-
-
 def _exact_distances(
     query: types.Embeddings,
     targets: types.Embeddings,
-    distance_fn: Callable[[npt.ArrayLike, npt.ArrayLike], float] = distance_functions[
-        "l2"
-    ],
+    distance_fn: Callable[
+        [npt.ArrayLike, npt.ArrayLike], float
+    ] = distance_functions.l2,
 ) -> Tuple[List[List[int]], List[List[float]]]:
     """Return the ordered indices and distances from each query to each target"""
     np_query = np.array(query)
     np_targets = np.array(targets)
 
     # Compute the distance between each query and each target, using the distance function
     distances = np.apply_along_axis(
@@ -164,14 +155,15 @@
 
 def ann_accuracy(
     collection: Collection,
     record_set: RecordSet,
     n_results: int = 1,
     min_recall: float = 0.99,
     embedding_function: Optional[types.EmbeddingFunction] = None,
+    query_indices: Optional[List[int]] = None,
 ) -> None:
     """Validate that the API performs nearest_neighbor searches correctly"""
     normalized_record_set = wrap_all(record_set)
 
     if len(normalized_record_set["ids"]) == 0:
         return  # nothing to test here
 
@@ -181,42 +173,48 @@
         assert embedding_function is not None
         assert normalized_record_set["documents"] is not None
         assert isinstance(normalized_record_set["documents"], list)
         # Compute the embeddings for the documents
         embeddings = embedding_function(normalized_record_set["documents"])
 
     # l2 is the default distance function
-    distance_function = distance_functions["l2"]
+    distance_function = distance_functions.l2
     accuracy_threshold = 1e-6
     assert collection.metadata is not None
     assert embeddings is not None
     if "hnsw:space" in collection.metadata:
         space = collection.metadata["hnsw:space"]
         # TODO: ip and cosine are numerically unstable in HNSW.
         # The higher the dimensionality, the more noise is introduced, since each float element
         # of the vector has noise added, which is then subsequently included in all normalization calculations.
         # This means that higher dimensions will have more noise, and thus more error.
         assert all(isinstance(e, list) for e in embeddings)
         dim = len(embeddings[0])
         accuracy_threshold = accuracy_threshold * math.pow(10, int(math.log10(dim)))
 
         if space == "cosine":
-            distance_function = distance_functions["cosine"]
-
+            distance_function = distance_functions.cosine
         if space == "ip":
-            distance_function = distance_functions["ip"]
+            distance_function = distance_functions.ip
 
     # Perform exact distance computation
+    query_embeddings = (
+        embeddings if query_indices is None else [embeddings[i] for i in query_indices]
+    )
+    query_documents = normalized_record_set["documents"]
+    if query_indices is not None and query_documents is not None:
+        query_documents = [query_documents[i] for i in query_indices]
+
     indices, distances = _exact_distances(
-        embeddings, embeddings, distance_fn=distance_function
+        query_embeddings, embeddings, distance_fn=distance_function
     )
 
     query_results = collection.query(
-        query_embeddings=normalized_record_set["embeddings"],
-        query_texts=normalized_record_set["documents"] if not have_embeddings else None,
+        query_embeddings=query_embeddings if have_embeddings else None,
+        query_texts=query_documents if not have_embeddings else None,
         n_results=n_results,
         include=["embeddings", "documents", "metadatas", "distances"],
     )
 
     assert query_results["distances"] is not None
     assert query_results["documents"] is not None
     assert query_results["metadatas"] is not None
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/property/test_add.py` & `chromadb-client-0.4.1.dev0/chromadb/test/property/test_add.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         metadata=collection.metadata,
         embedding_function=collection.embedding_function,
     )
     normalized_record_set = invariants.wrap_all(record_set)
 
     if not invariants.is_metadata_valid(normalized_record_set):
         with pytest.raises(Exception):
-            collection.add(**normalized_record_set)
+            coll.add(**normalized_record_set)
         return
 
     coll.add(**record_set)
 
     invariants.count(coll, cast(strategies.RecordSet, normalized_record_set))
     n_results = max(1, (len(normalized_record_set["ids"]) // 10))
     invariants.ann_accuracy(
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/property/test_collections.py` & `chromadb-client-0.4.1.dev0/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/property/test_cross_version_persist.py` & `chromadb-client-0.4.1.dev0/chromadb/test/property/test_cross_version_persist.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,17 +74,22 @@
 
 
 def configurations(versions: List[str]) -> List[Tuple[str, Settings]]:
     return [
         (
             version,
             Settings(
-                chroma_api_impl="local",
-                chroma_db_impl="duckdb+parquet",
-                persist_directory=tempfile.gettempdir() + "/tests/" + version + "/",
+                chroma_api_impl="chromadb.api.segment.SegmentAPI",
+                chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
+                chroma_producer_impl="chromadb.db.impl.sqlite.SqliteDB",
+                chroma_consumer_impl="chromadb.db.impl.sqlite.SqliteDB",
+                chroma_segment_manager_impl="chromadb.segment.impl.manager.local.LocalSegmentManager",
+                allow_reset=True,
+                is_persistent=True,
+                persist_directory=tempfile.gettempdir(),
             ),
         )
         for version in versions
     ]
 
 
 test_old_versions = versions()
@@ -195,15 +200,14 @@
         assert coll.count() == len(check_embeddings["embeddings"] or [])
         # Check ids
         result = coll.get()
         actual_ids = result["ids"]
         embedding_id_to_index = {id: i for i, id in enumerate(check_embeddings["ids"])}
         actual_ids = sorted(actual_ids, key=lambda id: embedding_id_to_index[id])
         assert actual_ids == check_embeddings["ids"]
-        api.persist()
     except Exception as e:
         conn.send(e)
         raise e
 
 
 # Since we can't pickle the embedding function, we always generate record sets with embeddings
 collection_st: st.SearchStrategy[strategies.Collection] = st.shared(
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/property/test_embeddings.py` & `chromadb-client-0.4.1.dev0/chromadb/test/property/test_embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import pytest
 import logging
 import hypothesis.strategies as st
-from typing import Set, cast, Union, DefaultDict
+from typing import Dict, Set, cast, Union, DefaultDict
 from dataclasses import dataclass
 from chromadb.api.types import ID, Include, IDs
 import chromadb.errors as errors
 from chromadb.api import API
 from chromadb.api.models.Collection import Collection
-from chromadb.db.impl.sqlite import SqliteDB
 import chromadb.test.property.strategies as strategies
 from hypothesis.stateful import (
     Bundle,
     RuleBasedStateMachine,
     MultipleResults,
     rule,
     initialize,
@@ -233,24 +232,19 @@
                     )[
                         0
                     ]
                 if normalized_record_set["metadatas"] is not None:
                     # Sqlite merges the metadata, as opposed to old
                     # implementations which overwrites it
                     record_set_state = self.record_set_state["metadatas"][target_idx]
-                    if (
-                        hasattr(self.api, "_sysdb")
-                        and type(self.api._sysdb) == SqliteDB
-                        and record_set_state is not None
-                    ):
+                    if record_set_state is not None:
+                        record_set_state = cast(
+                            Dict[str, Union[str, int, float]], record_set_state
+                        )
                         record_set_state.update(normalized_record_set["metadatas"][idx])
-                    else:
-                        self.record_set_state["metadatas"][
-                            target_idx
-                        ] = normalized_record_set["metadatas"][idx]
                 if normalized_record_set["documents"] is not None:
                     self.record_set_state["documents"][
                         target_idx
                     ] = normalized_record_set["documents"][idx]
             else:
                 # Add path
                 self.record_set_state["ids"].append(id)
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/property/test_filtering.py` & `chromadb-client-0.4.1.dev0/chromadb/test/property/test_filtering.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/property/test_persist.py` & `chromadb-client-0.4.1.dev0/chromadb/test/property/test_persist.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,42 +9,60 @@
 from chromadb.api import API
 from chromadb.config import Settings
 import chromadb.test.property.strategies as strategies
 import chromadb.test.property.invariants as invariants
 from chromadb.test.property.test_embeddings import (
     EmbeddingStateMachine,
     EmbeddingStateMachineStates,
+    collection_st as embedding_collection_st,
+    trace,
+)
+from hypothesis.stateful import (
+    run_state_machine_as_test,
+    rule,
+    precondition,
+    initialize,
 )
-from hypothesis.stateful import run_state_machine_as_test, rule, precondition
 import os
 import shutil
 import tempfile
 
 CreatePersistAPI = Callable[[], API]
 
 configurations = [
     Settings(
-        chroma_api_impl="local",
-        chroma_db_impl="duckdb+parquet",
+        chroma_api_impl="chromadb.api.segment.SegmentAPI",
+        chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
+        chroma_producer_impl="chromadb.db.impl.sqlite.SqliteDB",
+        chroma_consumer_impl="chromadb.db.impl.sqlite.SqliteDB",
+        chroma_segment_manager_impl="chromadb.segment.impl.manager.local.LocalSegmentManager",
+        allow_reset=True,
+        is_persistent=True,
         persist_directory=tempfile.gettempdir() + "/tests",
-    )
+    ),
 ]
 
 
 @pytest.fixture(scope="module", params=configurations)
 def settings(request: pytest.FixtureRequest) -> Generator[Settings, None, None]:
     configuration = request.param
-    yield configuration
     save_path = configuration.persist_directory
+    # Create if it doesn't exist
+    if not os.path.exists(save_path):
+        os.makedirs(save_path, exist_ok=True)
+    yield configuration
     # Remove if it exists
     if os.path.exists(save_path):
         shutil.rmtree(save_path)
 
 
-collection_st = st.shared(strategies.collections(with_hnsw_params=True), key="coll")
+collection_st = st.shared(
+    strategies.collections(with_hnsw_params=True, with_persistent_hnsw_params=True),
+    key="coll",
+)
 
 
 @given(
     collection_strategy=collection_st,
     embeddings_strategy=strategies.recordsets(collection_st),
 )
 def test_persist(
@@ -73,15 +91,14 @@
     invariants.ids_match(coll, embeddings_strategy)
     invariants.ann_accuracy(
         coll,
         embeddings_strategy,
         embedding_function=collection_strategy.embedding_function,
     )
 
-    api_1.persist()
     del api_1
 
     api_2 = chromadb.Client(settings)
     coll = api_2.get_collection(
         name=collection_strategy.name,
         embedding_function=collection_strategy.embedding_function,
     )
@@ -126,22 +143,39 @@
     def __init__(self, api: API, settings: Settings):
         self.api = api
         self.settings = settings
         self.last_persist_delay = 10
         self.api.reset()
         super().__init__(self.api)
 
+    @initialize(collection=embedding_collection_st, batch_size=st.integers(min_value=3, max_value=2000), sync_threshold=st.integers(min_value=3, max_value=2000))  # type: ignore
+    def initialize(
+        self, collection: strategies.Collection, batch_size: int, sync_threshold: int
+    ):
+        self.api.reset()
+        self.collection = self.api.create_collection(
+            name=collection.name,
+            metadata=collection.metadata,
+            embedding_function=collection.embedding_function,
+        )
+        self.embedding_function = collection.embedding_function
+        trace("init")
+        self.on_state_change(EmbeddingStateMachineStates.initialize)
+
+        self.record_set_state = strategies.StateMachineRecordSet(
+            ids=[], metadatas=[], documents=[], embeddings=[]
+        )
+
     @precondition(
         lambda self: len(self.record_set_state["ids"]) >= 1
         and self.last_persist_delay <= 0
     )
     @rule()
     def persist(self) -> None:
         self.on_state_change(PersistEmbeddingsStateMachineStates.persist)
-        self.api.persist()
         collection_name = self.collection.name
         # Create a new process and then inside the process run the invariants
         # TODO: Once we switch off of duckdb and onto sqlite we can remove this
         ctx = multiprocessing.get_context("spawn")
         conn1, conn2 = multiprocessing.Pipe()
         p = ctx.Process(
             target=load_and_check,
@@ -156,14 +190,17 @@
 
     def on_state_change(self, new_state: str) -> None:
         if new_state == PersistEmbeddingsStateMachineStates.persist:
             self.last_persist_delay = 10
         else:
             self.last_persist_delay -= 1
 
+    def teardown(self) -> None:
+        self.api.reset()
+
 
 def test_persist_embeddings_state(
     caplog: pytest.LogCaptureFixture, settings: Settings
 ) -> None:
     caplog.set_level(logging.ERROR)
     api = chromadb.Client(settings)
     run_state_machine_as_test(
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/segment/test_metadata.py` & `chromadb-client-0.4.1.dev0/chromadb/test/segment/test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+import shutil
+import tempfile
 import pytest
 from typing import Generator, List, Callable, Iterator, Dict, Optional, Union, Sequence
 from chromadb.config import System, Settings
 from chromadb.types import (
     SubmitEmbeddingRecord,
     MetadataEmbeddingRecord,
     Operation,
@@ -19,23 +22,37 @@
 
 from pytest import FixtureRequest
 from itertools import count
 
 
 def sqlite() -> Generator[System, None, None]:
     """Fixture generator for sqlite DB"""
-    settings = Settings(sqlite_database=":memory:", allow_reset=True)
+    settings = Settings(allow_reset=True, is_persistent=False)
     system = System(settings)
     system.start()
     yield system
     system.stop()
 
 
+def sqlite_persistent() -> Generator[System, None, None]:
+    """Fixture generator for sqlite DB"""
+    save_path = tempfile.mkdtemp()
+    settings = Settings(
+        allow_reset=True, is_persistent=True, persist_directory=save_path
+    )
+    system = System(settings)
+    system.start()
+    yield system
+    system.stop()
+    if os.path.exists(save_path):
+        shutil.rmtree(save_path)
+
+
 def system_fixtures() -> List[Callable[[], Generator[System, None, None]]]:
-    return [sqlite]
+    return [sqlite, sqlite_persistent]
 
 
 @pytest.fixture(scope="module", params=system_fixtures())
 def system(request: FixtureRequest) -> Generator[System, None, None]:
     yield next(request.param())
 
 
@@ -102,16 +119,16 @@
         time.sleep(0.25)
     raise TimeoutError(f"Timed out waiting for seq_id {seq_id}")
 
 
 def test_insert_and_count(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset_state()
     producer = system.instance(Producer)
+    system.reset_state()
 
     topic = str(segment_definition["topic"])
 
     max_id = 0
     for i in range(3):
         max_id = producer.submit_embedding(topic, next(sample_embeddings))
 
@@ -140,17 +157,16 @@
         assert e["id"] == a["id"]
         assert e["metadata"] == a["metadata"]
 
 
 def test_get(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset_state()
-
     producer = system.instance(Producer)
+    system.reset_state()
     topic = str(segment_definition["topic"])
 
     embeddings = [next(sample_embeddings) for i in range(10)]
 
     seq_ids = []
     for e in embeddings:
         seq_ids.append(producer.submit_embedding(topic, e))
@@ -238,17 +254,16 @@
     )
     assert len(result) == 1
 
 
 def test_fulltext(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset_state()
-
     producer = system.instance(Producer)
+    system.reset_state()
     topic = str(segment_definition["topic"])
 
     segment = SqliteMetadataSegment(system, segment_definition)
     segment.start()
 
     max_id = 0
     for i in range(100):
@@ -300,17 +315,16 @@
     result = segment.get_metadata(where_document={"$contains": "zer"})
     assert len(result) == 9
 
 
 def test_delete(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset_state()
-
     producer = system.instance(Producer)
+    system.reset_state()
     topic = str(segment_definition["topic"])
 
     segment = SqliteMetadataSegment(system, segment_definition)
     segment.start()
 
     embeddings = [next(sample_embeddings) for i in range(10)]
 
@@ -363,17 +377,16 @@
     assert segment.count() == 10
     results = segment.get_metadata(ids=["embedding_0"])
 
 
 def test_update(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset_state()
-
     producer = system.instance(Producer)
+    system.reset_state()
     topic = str(segment_definition["topic"])
 
     segment = SqliteMetadataSegment(system, segment_definition)
     segment.start()
 
     _test_update(sample_embeddings, producer, segment, topic, Operation.UPDATE)
 
@@ -391,17 +404,16 @@
     assert len(results) == 0
     assert segment.count() == 3
 
 
 def test_upsert(
     system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
 ) -> None:
-    system.reset_state()
-
     producer = system.instance(Producer)
+    system.reset_state()
     topic = str(segment_definition["topic"])
 
     segment = SqliteMetadataSegment(system, segment_definition)
     segment.start()
 
     _test_update(sample_embeddings, producer, segment, topic, Operation.UPSERT)
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/segment/test_vector.py` & `chromadb-client-0.4.1.dev0/chromadb/test/segment/test_vector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from typing import Generator, List, Callable, Iterator, cast
+from typing import Generator, List, Callable, Iterator, Type, cast
 from chromadb.config import System, Settings
 from chromadb.types import (
     SubmitEmbeddingRecord,
     VectorQuery,
     Operation,
     ScalarEncoding,
     Segment,
@@ -12,31 +12,66 @@
     Vector,
 )
 from chromadb.ingest import Producer
 from chromadb.segment import VectorReader
 import uuid
 import time
 
-from chromadb.segment.impl.vector.local_hnsw import LocalHnswSegment
+from chromadb.segment.impl.vector.local_hnsw import (
+    LocalHnswSegment,
+)
+
+from chromadb.segment.impl.vector.local_persistent_hnsw import (
+    PersistentLocalHnswSegment,
+)
 
 from pytest import FixtureRequest
 from itertools import count
+import tempfile
+import os
+import shutil
 
 
 def sqlite() -> Generator[System, None, None]:
     """Fixture generator for sqlite DB"""
-    settings = Settings(sqlite_database=":memory:", allow_reset=True)
+    save_path = tempfile.mkdtemp()
+    settings = Settings(
+        allow_reset=True,
+        is_persistent=False,
+        persist_directory=save_path,
+    )
+    system = System(settings)
+    system.start()
+    yield system
+    system.stop()
+    if os.path.exists(save_path):
+        shutil.rmtree(save_path)
+
+
+def sqlite_persistent() -> Generator[System, None, None]:
+    """Fixture generator for sqlite DB"""
+    save_path = tempfile.mkdtemp()
+    settings = Settings(
+        allow_reset=True,
+        is_persistent=True,
+        persist_directory=save_path,
+    )
     system = System(settings)
     system.start()
     yield system
     system.stop()
+    if os.path.exists(save_path):
+        shutil.rmtree(save_path)
 
 
+# We will excercise in memory, persistent sqlite with both ephemeral and persistent hnsw.
+# We technically never expose persitent sqlite with memory hnsw to users, but it's a valid
+# configuration, so we test it here.
 def system_fixtures() -> List[Callable[[], Generator[System, None, None]]]:
-    return [sqlite]
+    return [sqlite, sqlite_persistent]
 
 
 @pytest.fixture(scope="module", params=system_fixtures())
 def system(request: FixtureRequest) -> Generator[System, None, None]:
     yield next(request.param())
 
 
@@ -56,47 +91,60 @@
             operation=Operation.ADD,
         )
         return record
 
     return (create_record(i) for i in count())
 
 
-segment_definition = Segment(
-    id=uuid.uuid4(),
-    type="test_type",
-    scope=SegmentScope.VECTOR,
-    topic="persistent://test/test/test_topic_1",
-    collection=None,
-    metadata=None,
-)
+def vector_readers() -> List[Type[VectorReader]]:
+    return [LocalHnswSegment, PersistentLocalHnswSegment]
+
+
+@pytest.fixture(scope="module", params=vector_readers())
+def vector_reader(request: FixtureRequest) -> Generator[Type[VectorReader], None, None]:
+    yield request.param
+
+
+def create_random_segment_definition() -> Segment:
+    return Segment(
+        id=uuid.uuid4(),
+        type="test_type",
+        scope=SegmentScope.VECTOR,
+        topic="persistent://test/test/test_topic_1",
+        collection=None,
+        metadata=None,
+    )
 
 
 def sync(segment: VectorReader, seq_id: SeqId) -> None:
     # Try for up to 5 seconds, then throw a TimeoutError
     start = time.time()
     while time.time() - start < 5:
         if segment.max_seqid() >= seq_id:
             return
         time.sleep(0.25)
     raise TimeoutError(f"Timed out waiting for seq_id {seq_id}")
 
 
 def test_insert_and_count(
-    system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
+    system: System,
+    sample_embeddings: Iterator[SubmitEmbeddingRecord],
+    vector_reader: Type[VectorReader],
 ) -> None:
-    system.reset_state()
     producer = system.instance(Producer)
 
+    system.reset_state()
+    segment_definition = create_random_segment_definition()
     topic = str(segment_definition["topic"])
 
     max_id = 0
     for i in range(3):
         max_id = producer.submit_embedding(topic, next(sample_embeddings))
 
-    segment = LocalHnswSegment(system, segment_definition)
+    segment = vector_reader(system, segment_definition)
     segment.start()
 
     sync(segment, max_id)
 
     assert segment.count() == 3
     for i in range(3):
         max_id = producer.submit_embedding(topic, next(sample_embeddings))
@@ -110,22 +158,24 @@
 
 
 def approx_equal_vector(a: Vector, b: Vector, epsilon: float = 0.0001) -> bool:
     return all(approx_equal(x, y, epsilon) for x, y in zip(a, b))
 
 
 def test_get_vectors(
-    system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
+    system: System,
+    sample_embeddings: Iterator[SubmitEmbeddingRecord],
+    vector_reader: Type[VectorReader],
 ) -> None:
-    system.reset_state()
     producer = system.instance(Producer)
-
+    system.reset_state()
+    segment_definition = create_random_segment_definition()
     topic = str(segment_definition["topic"])
 
-    segment = LocalHnswSegment(system, segment_definition)
+    segment = vector_reader(system, segment_definition)
     segment.start()
 
     embeddings = [next(sample_embeddings) for i in range(10)]
 
     seq_ids: List[SeqId] = []
     for e in embeddings:
         seq_ids.append(producer.submit_embedding(topic, e))
@@ -153,22 +203,24 @@
         assert approx_equal_vector(
             actual["embedding"], cast(Vector, expected["embedding"])
         )
         assert actual["seq_id"] == seq_id
 
 
 def test_ann_query(
-    system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
+    system: System,
+    sample_embeddings: Iterator[SubmitEmbeddingRecord],
+    vector_reader: Type[VectorReader],
 ) -> None:
-    system.reset_state()
     producer = system.instance(Producer)
-
+    system.reset_state()
+    segment_definition = create_random_segment_definition()
     topic = str(segment_definition["topic"])
 
-    segment = LocalHnswSegment(system, segment_definition)
+    segment = vector_reader(system, segment_definition)
     segment.start()
 
     embeddings = [next(sample_embeddings) for i in range(100)]
 
     seq_ids: List[SeqId] = []
     for e in embeddings:
         seq_ids.append(producer.submit_embedding(topic, e))
@@ -216,22 +268,24 @@
         assert len(r) == 3
         assert r[0]["id"] == embeddings[i]["id"]
         assert r[1]["id"] == embeddings[i - 1]["id"]
         assert r[2]["id"] == embeddings[i + 1]["id"]
 
 
 def test_delete(
-    system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
+    system: System,
+    sample_embeddings: Iterator[SubmitEmbeddingRecord],
+    vector_reader: Type[VectorReader],
 ) -> None:
-    system.reset_state()
     producer = system.instance(Producer)
-
+    system.reset_state()
+    segment_definition = create_random_segment_definition()
     topic = str(segment_definition["topic"])
 
-    segment = LocalHnswSegment(system, segment_definition)
+    segment = vector_reader(system, segment_definition)
     segment.start()
 
     embeddings = [next(sample_embeddings) for i in range(5)]
 
     seq_ids: List[SeqId] = []
     for e in embeddings:
         seq_ids.append(producer.submit_embedding(topic, e))
@@ -257,14 +311,16 @@
     # Assert that the record is gone using `count`
     assert segment.count() == 4
 
     # Assert that the record is gone using `get`
     assert segment.get_vectors(ids=[embeddings[0]["id"]]) == []
     results = segment.get_vectors()
     assert len(results) == 4
+    # get_vectors returns results in arbitrary order
+    results = sorted(results, key=lambda v: v["id"])
     for actual, expected in zip(results, embeddings[1:]):
         assert actual["id"] == expected["id"]
         assert approx_equal_vector(
             actual["embedding"], cast(Vector, expected["embedding"])
         )
 
     # Assert that the record is gone from KNN search
@@ -353,22 +409,24 @@
     knn_results = segment.query_vectors(query)[0]
     assert knn_results[0]["id"] == embeddings[0]["id"]
     assert knn_results[1]["id"] == embeddings[2]["id"]
     assert knn_results[2]["id"] == embeddings[1]["id"]
 
 
 def test_update(
-    system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
+    system: System,
+    sample_embeddings: Iterator[SubmitEmbeddingRecord],
+    vector_reader: Type[VectorReader],
 ) -> None:
-    system.reset_state()
     producer = system.instance(Producer)
-
+    system.reset_state()
+    segment_definition = create_random_segment_definition()
     topic = str(segment_definition["topic"])
 
-    segment = LocalHnswSegment(system, segment_definition)
+    segment = vector_reader(system, segment_definition)
     segment.start()
 
     _test_update(producer, topic, segment, sample_embeddings, Operation.UPDATE)
 
     # test updating a nonexistent record
     seq_id = producer.submit_embedding(
         topic,
@@ -384,22 +442,24 @@
     sync(segment, seq_id)
 
     assert segment.count() == 3
     assert segment.get_vectors(ids=["no_such_record"]) == []
 
 
 def test_upsert(
-    system: System, sample_embeddings: Iterator[SubmitEmbeddingRecord]
+    system: System,
+    sample_embeddings: Iterator[SubmitEmbeddingRecord],
+    vector_reader: Type[VectorReader],
 ) -> None:
-    system.reset_state()
     producer = system.instance(Producer)
-
+    system.reset_state()
+    segment_definition = create_random_segment_definition()
     topic = str(segment_definition["topic"])
 
-    segment = LocalHnswSegment(system, segment_definition)
+    segment = vector_reader(system, segment_definition)
     segment.start()
 
     _test_update(producer, topic, segment, sample_embeddings, Operation.UPSERT)
 
     # test updating a nonexistent record
     seq_id = producer.submit_embedding(
         topic,
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/test_api.py` & `chromadb-client-0.4.1.dev0/chromadb/test/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,40 @@
 )
 
 
 @pytest.fixture
 def local_persist_api():
     return chromadb.Client(
         Settings(
-            chroma_api_impl="local",
-            chroma_db_impl="duckdb+parquet",
-            persist_directory=tempfile.gettempdir() + "/test_server",
-        )
+            chroma_api_impl="chromadb.api.segment.SegmentAPI",
+            chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
+            chroma_producer_impl="chromadb.db.impl.sqlite.SqliteDB",
+            chroma_consumer_impl="chromadb.db.impl.sqlite.SqliteDB",
+            chroma_segment_manager_impl="chromadb.segment.impl.manager.local.LocalSegmentManager",
+            allow_reset=True,
+            is_persistent=True,
+            persist_directory=tempfile.gettempdir(),
+        ),
     )
 
 
 # https://docs.pytest.org/en/6.2.x/fixture.html#fixtures-can-be-requested-more-than-once-per-test-return-values-are-cached
 @pytest.fixture
 def local_persist_api_cache_bust():
     return chromadb.Client(
         Settings(
-            chroma_api_impl="local",
-            chroma_db_impl="duckdb+parquet",
-            persist_directory=tempfile.gettempdir() + "/test_server",
-        )
+            chroma_api_impl="chromadb.api.segment.SegmentAPI",
+            chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
+            chroma_producer_impl="chromadb.db.impl.sqlite.SqliteDB",
+            chroma_consumer_impl="chromadb.db.impl.sqlite.SqliteDB",
+            chroma_segment_manager_impl="chromadb.segment.impl.manager.local.LocalSegmentManager",
+            allow_reset=True,
+            is_persistent=True,
+            persist_directory=tempfile.gettempdir(),
+        ),
     )
 
 
 def approx_equal(a, b, tolerance=1e-6) -> bool:
     return abs(a - b) < tolerance
 
 
@@ -48,17 +58,14 @@
 @pytest.mark.parametrize("api_fixture", [local_persist_api])
 def test_persist_index_loading(api_fixture, request):
     api = request.getfixturevalue("local_persist_api")
     api.reset()
     collection = api.create_collection("test")
     collection.add(ids="id1", documents="hello")
 
-    api.persist()
-    del api
-
     api2 = request.getfixturevalue("local_persist_api_cache_bust")
     collection = api2.get_collection("test")
 
     nn = collection.query(
         query_texts="hello",
         n_results=1,
         include=["embeddings", "documents", "metadatas", "distances"],
@@ -71,17 +78,14 @@
 def test_persist_index_loading_embedding_function(api_fixture, request):
     embedding_function = lambda x: [[1, 2, 3] for _ in range(len(x))]  # noqa E731
     api = request.getfixturevalue("local_persist_api")
     api.reset()
     collection = api.create_collection("test", embedding_function=embedding_function)
     collection.add(ids="id1", documents="hello")
 
-    api.persist()
-    del api
-
     api2 = request.getfixturevalue("local_persist_api_cache_bust")
     collection = api2.get_collection("test", embedding_function=embedding_function)
 
     nn = collection.query(
         query_texts="hello",
         n_results=1,
         include=["embeddings", "documents", "metadatas", "distances"],
@@ -96,17 +100,14 @@
     api = request.getfixturevalue("local_persist_api")
     api.reset()
     collection = api.get_or_create_collection(
         "test", embedding_function=embedding_function
     )
     collection.add(ids="id1", documents="hello")
 
-    api.persist()
-    del api
-
     api2 = request.getfixturevalue("local_persist_api_cache_bust")
     collection = api2.get_or_create_collection(
         "test", embedding_function=embedding_function
     )
 
     nn = collection.query(
         query_texts="hello",
@@ -131,24 +132,19 @@
 
     collection = api.create_collection("testspace")
 
     collection.add(**batch_records)
 
     assert collection.count() == 2
 
-    api.persist()
-    del api
-
     api = request.getfixturevalue(api_fixture.__name__)
     collection = api.get_collection("testspace")
     assert collection.count() == 2
 
     api.delete_collection("testspace")
-    api.persist()
-    del api
 
     api = request.getfixturevalue(api_fixture.__name__)
     assert api.list_collections() == []
 
 
 def test_heartbeat(api):
     heartbeat_ns = api.heartbeat()
@@ -1048,14 +1044,15 @@
     # Delete with malformed ids
     with pytest.raises(ValueError) as e:
         collection.delete(ids=["valid", 0])
     assert "ID" in str(e.value)
 
 
 def test_index_params(api):
+    EPS = 1e-12
     # first standard add
     api.reset()
     collection = api.create_collection(name="test_index_params")
     collection.add(**records)
     items = collection.query(
         query_embeddings=[0.6, 1.12, 1.6],
         n_results=1,
@@ -1069,16 +1066,16 @@
         metadata={"hnsw:space": "cosine", "hnsw:construction_ef": 20, "hnsw:M": 5},
     )
     collection.add(**records)
     items = collection.query(
         query_embeddings=[0.6, 1.12, 1.6],
         n_results=1,
     )
-    assert items["distances"][0][0] > 0
-    assert items["distances"][0][0] < 1
+    assert items["distances"][0][0] > 0 - EPS
+    assert items["distances"][0][0] < 1 + EPS
 
     # ip
     api.reset()
     collection = api.create_collection(
         name="test_index_params", metadata={"hnsw:space": "ip"}
     )
     collection.add(**records)
@@ -1104,22 +1101,24 @@
         )
         collection.add(**records)
 
 
 def test_persist_index_loading_params(api, request):
     api = request.getfixturevalue("local_persist_api")
     api.reset()
-    collection = api.create_collection("test", metadata={"hnsw:space": "ip"})
+    collection = api.create_collection(
+        "test",
+        metadata={"hnsw:space": "ip"},
+    )
     collection.add(ids="id1", documents="hello")
 
-    api.persist()
-    del api
-
     api2 = request.getfixturevalue("local_persist_api_cache_bust")
-    collection = api2.get_collection("test")
+    collection = api2.get_collection(
+        "test",
+    )
 
     assert collection.metadata["hnsw:space"] == "ip"
 
     nn = collection.query(
         query_texts="hello",
         n_results=1,
         include=["embeddings", "documents", "metadatas", "distances"],
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/test_chroma.py` & `chromadb-client-0.4.1.dev0/chromadb/test/test_chroma.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,107 @@
 import unittest
 import os
 from unittest.mock import patch, Mock
-
+import pytest
 import chromadb
 import chromadb.config
-from chromadb.db import DB
+from chromadb.db.system import SysDB
+from chromadb.ingest import Consumer, Producer
 
 
 class GetDBTest(unittest.TestCase):
-    @patch("chromadb.db.duckdb.DuckDB", autospec=True)
+    @patch("chromadb.db.impl.sqlite.SqliteDB", autospec=True)
     def test_default_db(self, mock: Mock) -> None:
         system = chromadb.config.System(
             chromadb.config.Settings(persist_directory="./foo")
         )
-        system.instance(DB)
+        system.instance(SysDB)
         assert mock.called
 
-    @patch("chromadb.db.duckdb.PersistentDuckDB", autospec=True)
-    def test_persistent_duckdb(self, mock: Mock) -> None:
+    @patch("chromadb.db.impl.sqlite.SqliteDB", autospec=True)
+    def test_sqlite_sysdb(self, mock: Mock) -> None:
         system = chromadb.config.System(
             chromadb.config.Settings(
-                chroma_db_impl="duckdb+parquet", persist_directory="./foo"
+                chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
+                persist_directory="./foo",
             )
         )
-        system.instance(DB)
+        system.instance(SysDB)
         assert mock.called
 
-    @patch("chromadb.db.clickhouse.Clickhouse", autospec=True)
-    def test_clickhouse(self, mock: Mock) -> None:
+    @patch("chromadb.db.impl.sqlite.SqliteDB", autospec=True)
+    def test_sqlite_queue(self, mock: Mock) -> None:
         system = chromadb.config.System(
             chromadb.config.Settings(
-                chroma_db_impl="clickhouse",
+                chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
+                chroma_producer_impl="chromadb.db.impl.sqlite.SqliteDB",
+                chroma_consumer_impl="chromadb.db.impl.sqlite.SqliteDB",
                 persist_directory="./foo",
-                clickhouse_host="foo",
-                clickhouse_port="666",
             )
         )
-        system.instance(DB)
+        system.instance(Producer)
+        system.instance(Consumer)
         assert mock.called
 
 
 class GetAPITest(unittest.TestCase):
-    @patch("chromadb.api.local.LocalAPI", autospec=True)
+    @patch("chromadb.api.segment.SegmentAPI", autospec=True)
     @patch.dict(os.environ, {}, clear=True)
     def test_local(self, mock_api: Mock) -> None:
         chromadb.Client(chromadb.config.Settings(persist_directory="./foo"))
         assert mock_api.called
 
-    @patch("chromadb.db.duckdb.DuckDB", autospec=True)
+    @patch("chromadb.db.impl.sqlite.SqliteDB", autospec=True)
     @patch.dict(os.environ, {}, clear=True)
     def test_local_db(self, mock_db: Mock) -> None:
         chromadb.Client(chromadb.config.Settings(persist_directory="./foo"))
         assert mock_db.called
 
     @patch("chromadb.api.fastapi.FastAPI", autospec=True)
     @patch.dict(os.environ, {}, clear=True)
     def test_fastapi(self, mock: Mock) -> None:
         chromadb.Client(
             chromadb.config.Settings(
-                chroma_api_impl="rest",
+                chroma_api_impl="chromadb.api.fastapi.FastAPI",
                 persist_directory="./foo",
                 chroma_server_host="foo",
                 chroma_server_http_port="80",
             )
         )
         assert mock.called
+
+    @patch("chromadb.api.fastapi.FastAPI", autospec=True)
+    @patch.dict(os.environ, {}, clear=True)
+    def test_settings_pass_to_fastapi(self, mock: Mock) -> None:
+        settings = chromadb.config.Settings(
+            chroma_api_impl="chromadb.api.fastapi.FastAPI",
+            chroma_server_host="foo",
+            chroma_server_http_port="80",
+            chroma_server_headers={"foo": "bar"},
+        )
+        chromadb.Client(settings)
+
+        # Check that the mock was called
+        assert mock.called
+
+        # Retrieve the arguments with which the mock was called
+        # `call_args` returns a tuple, where the first element is a tuple of positional arguments
+        # and the second element is a dictionary of keyword arguments. We assume here that
+        # the settings object is passed as a positional argument.
+        args, kwargs = mock.call_args
+        passed_settings = args[0] if args else None
+
+        # Check if the settings passed to the mock match the settings we used
+        # raise Exception(passed_settings.settings)
+        assert passed_settings.settings == settings
+
+
+def test_legacy_values() -> None:
+    with pytest.raises(ValueError):
+        chromadb.Client(
+            chromadb.config.Settings(
+                chroma_api_impl="chromadb.api.local.LocalAPI",
+                persist_directory="./foo",
+                chroma_server_host="foo",
+                chroma_server_http_port="80",
+            )
+        )
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/test_config.py` & `chromadb-client-0.4.1.dev0/chromadb/test/test_config.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/test/utils/test_messagid.py` & `chromadb-client-0.4.1.dev0/chromadb/test/utils/test_messagid.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/types.py` & `chromadb-client-0.4.1.dev0/chromadb/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/utils/embedding_functions.py` & `chromadb-client-0.4.1.dev0/chromadb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb/utils/messageid.py` & `chromadb-client-0.4.1.dev0/chromadb/utils/messageid.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/chromadb_client.egg-info/PKG-INFO` & `chromadb-client-0.4.1.dev0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: chromadb-client
-Version: 0.3.30.dev0
-Summary: Chroma Client.
-Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
-Project-URL: Homepage, https://github.com/chroma-core/chroma
-Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <a href="https://trychroma.com"><img src="https://user-images.githubusercontent.com/891664/227103090-6624bf7d-9524-4e05-9d2c-c28d5d451481.png" alt="Chroma logo"></a>
 </p>
 
 <p align="center">
     <b>Chroma - the open-source embedding database</b>. <br />
     This package is for the the Python HTTP client-only library for Chroma. This client connects to the Chroma Server. If that it not what you are looking for, you might want to check out the <a href="https://github.com/chroma-core/chroma ">full library</a>.
@@ -26,19 +12,16 @@
 pip install chromadb-client # python http-client only library
 ```
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
-from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest",
-                                  chroma_server_host="localhost",
-                                  chroma_server_http_port=8000))
+client = chromadb.HttpClient(host="localhost", port=8000)
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -1,28 +1,17 @@
-Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.30.dev0 Summary:
-Chroma Client. Author-email: Jeff Huber
-trychroma.com>, Anton Troynikov
-trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
-Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE
                                  [Chroma_logo]
                  Chroma - the open-source embedding database.
  This package is for the the Python HTTP client-only library for Chroma. This
 client connects to the Chroma Server. If that it not what you are looking for,
                  you might want to check out the full_library.
 ```bash pip install chromadb-client # python http-client only library ``` To
 connect to your server and perform operations using the client only library,
-you can do the following: ```python import chromadb from chromadb.config import
-Settings # Example setup of the client to connect to your chroma server client
-= chromadb.Client(Settings(chroma_api_impl="rest",
-chroma_server_host="localhost", chroma_server_http_port=8000)) collection =
-client.create_collection("all-my-documents") collection.add( documents=["This
-is document1", "This is document2"], metadatas=[{"source": "notion"},
-{"source": "google-docs"}], # filter on these! ids=["doc1", "doc2"], # unique
-for each doc embeddings = [[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results =
-collection.query( query_texts=["This is a query document"], n_results=2, #
-where={"metadata_field": "is_equal_to_this"}, # optional filter #
-where_document={"$contains":"search_string"} # optional filter ) ``` ## License
-[Apache 2.0](./LICENSE)
+you can do the following: ```python import chromadb # Example setup of the
+client to connect to your chroma server client = chromadb.HttpClient
+(host="localhost", port=8000) collection = client.create_collection("all-my-
+documents") collection.add( documents=["This is document1", "This is
+document2"], metadatas=[{"source": "notion"}, {"source": "google-docs"}], #
+filter on these! ids=["doc1", "doc2"], # unique for each doc embeddings = [
+[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results = collection.query( query_texts=
+["This is a query document"], n_results=2, # where={"metadata_field":
+"is_equal_to_this"}, # optional filter # where_document={"$contains":
+"search_string"} # optional filter ) ``` ## License [Apache 2.0](./LICENSE)
```

### Comparing `chromadb-client-0.3.30.dev0/chromadb_client.egg-info/SOURCES.txt` & `chromadb-client-0.4.1.dev0/chromadb_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,92 +20,98 @@
 .github/workflows/chroma-client-integration-test.yml
 .github/workflows/chroma-integration-test.yml
 .github/workflows/chroma-release-python-client.yml
 .github/workflows/chroma-release.yml
 .github/workflows/chroma-test.yml
 .github/workflows/pr-review-checklist.yml
 .vscode/settings.json
-bin/backup.sh
 bin/build
 bin/docker_entrypoint.sh
 bin/generate_cloudformation.py
 bin/integration-test
-bin/restore.sh
-bin/setup_linux.sh
-bin/setup_mac.sh
 bin/test-package.sh
 bin/test-remote
 bin/test.py
 bin/version
 bin/templates/docker-compose.yml
 chromadb/__init__.py
 chromadb/app.py
 chromadb/config.py
 chromadb/errors.py
 chromadb/is_thin_client.py
 chromadb/types.py
 chromadb/api/__init__.py
 chromadb/api/fastapi.py
-chromadb/api/local.py
 chromadb/api/segment.py
 chromadb/api/types.py
 chromadb/api/models/Collection.py
 chromadb/db/__init__.py
 chromadb/db/base.py
-chromadb/db/clickhouse.py
-chromadb/db/duckdb.py
 chromadb/db/migrations.py
 chromadb/db/system.py
 chromadb/db/impl/__init__.py
 chromadb/db/impl/sqlite.py
-chromadb/db/index/__init__.py
-chromadb/db/index/hnswlib.py
+chromadb/db/impl/sqlite_pool.py
 chromadb/db/mixins/embeddings_queue.py
 chromadb/db/mixins/sysdb.py
 chromadb/experimental/density_relevance.ipynb
 chromadb/ingest/__init__.py
+chromadb/migrations/__init__.py
+chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
+chromadb/migrations/sysdb/00001-collections.sqlite.sql
+chromadb/migrations/sysdb/00002-segments.sqlite.sql
+chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
 chromadb/segment/__init__.py
 chromadb/segment/impl/manager/local.py
 chromadb/segment/impl/metadata/sqlite.py
+chromadb/segment/impl/vector/batch.py
+chromadb/segment/impl/vector/brute_force_index.py
+chromadb/segment/impl/vector/hnsw_params.py
 chromadb/segment/impl/vector/local_hnsw.py
+chromadb/segment/impl/vector/local_persistent_hnsw.py
 chromadb/server/__init__.py
 chromadb/server/fastapi/__init__.py
 chromadb/server/fastapi/types.py
 chromadb/telemetry/__init__.py
 chromadb/telemetry/events.py
 chromadb/telemetry/posthog.py
 chromadb/test/conftest.py
 chromadb/test/test_api.py
 chromadb/test/test_chroma.py
+chromadb/test/test_client.py
 chromadb/test/test_config.py
+chromadb/test/test_multithreaded.py
 chromadb/test/db/test_base.py
 chromadb/test/db/test_migrations.py
 chromadb/test/db/test_system.py
 chromadb/test/db/migrations/00001-migration-1.psql.sql
 chromadb/test/db/migrations/00001-migration-1.sqlite.sql
 chromadb/test/db/migrations/00002-migration-2.psql.sql
 chromadb/test/db/migrations/00002-migration-2.sqlite.sql
 chromadb/test/db/migrations/00003-migration-3.psql.sql
 chromadb/test/db/migrations/00003-migration-3.sqlite.sql
-chromadb/test/hnswlib/test_hnswlib.py
+chromadb/test/db/migrations/__init__.py
 chromadb/test/ingest/test_producer_consumer.py
 chromadb/test/property/invariants.py
 chromadb/test/property/strategies.py
 chromadb/test/property/test_add.py
 chromadb/test/property/test_collections.py
 chromadb/test/property/test_cross_version_persist.py
 chromadb/test/property/test_embeddings.py
 chromadb/test/property/test_filtering.py
 chromadb/test/property/test_persist.py
 chromadb/test/segment/test_metadata.py
 chromadb/test/segment/test_vector.py
 chromadb/test/utils/test_messagid.py
 chromadb/utils/__init__.py
+chromadb/utils/distance_functions.py
 chromadb/utils/embedding_functions.py
 chromadb/utils/messageid.py
+chromadb/utils/read_write_lock.py
 chromadb_client.egg-info/PKG-INFO
 chromadb_client.egg-info/SOURCES.txt
 chromadb_client.egg-info/dependency_links.txt
 chromadb_client.egg-info/requires.txt
 chromadb_client.egg-info/top_level.txt
 clients/js/.gitignore
 clients/js/.prettierignore
@@ -160,26 +166,19 @@
 clients/js/test/update.collection.test.ts
 clients/js/test/upsert.collections.test.ts
 clients/python/README.md
 clients/python/build_python_thin_client.sh
 clients/python/integration-test.sh
 clients/python/is_thin_client.py
 clients/python/pyproject.toml
-config/backup_disk.xml
-config/chroma_users.xml
 examples/README.md
 examples/basic_functionality/alternative_embeddings.ipynb
 examples/basic_functionality/local_persistence.ipynb
 examples/basic_functionality/where_filtering.ipynb
 examples/deployments/google-cloud-compute/README.md
 examples/deployments/google-cloud-compute/chroma.tf
 examples/deployments/google-cloud-compute/main.tf
 examples/deployments/google-cloud-compute/startup.sh
 examples/deployments/google-cloud-compute/variables.tf
 examples/use_with/cohere/cohere_js.js
 examples/use_with/cohere/cohere_python.ipynb
-examples/use_with/cohere/package.json
-migrations/embeddings_queue/00001-embeddings.sqlite.sql
-migrations/metadb/00001-embedding-metadata.sqlite.sql
-migrations/sysdb/00001-collections.sqlite.sql
-migrations/sysdb/00002-segments.sqlite.sql
-migrations/sysdb/00003-collection-dimension.sqlite.sql
+examples/use_with/cohere/package.json
```

### Comparing `chromadb-client-0.3.30.dev0/clients/js/DEVELOP.md` & `chromadb-client-0.4.1.dev0/clients/js/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/LICENSE` & `chromadb-client-0.4.1.dev0/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/README.md` & `chromadb-client-0.4.1.dev0/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/examples/browser/app.ts` & `chromadb-client-0.4.1.dev0/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/examples/browser/index.html` & `chromadb-client-0.4.1.dev0/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/examples/browser/yarn.lock` & `chromadb-client-0.4.1.dev0/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/examples/node/app.js` & `chromadb-client-0.4.1.dev0/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/examples/node/yarn.lock` & `chromadb-client-0.4.1.dev0/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/genapi.sh` & `chromadb-client-0.4.1.dev0/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/package-lock.json` & `chromadb-client-0.4.1.dev0/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/package.json` & `chromadb-client-0.4.1.dev0/clients/js/package.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/ChromaClient.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/ChromaClient.ts`

 * *Files 2% similar despite different names*

```diff
@@ -80,21 +80,14 @@
     public async heartbeat(): Promise<number> {
         const response = await this.api.heartbeat(this.api.options);
         let ret = await handleSuccess(response);
         return ret["nanosecond heartbeat"]
     }
 
     /**
-     * @ignore
-     */
-    public async persist(): Promise<never> {
-        throw new Error("Not implemented in JS client");
-    }
-
-    /**
      * Creates a new collection with the specified properties.
      *
      * @param {Object} params - The parameters for creating a new collection.
      * @param {string} params.name - The name of the collection.
      * @param {CollectionMetadata} [params.metadata] - Optional metadata associated with the collection.
      * @param {IEmbeddingFunction} [params.embeddingFunction] - Optional custom embedding function for the collection.
      *
```

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/Collection.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/Collection.ts`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,15 @@
         const response = await this.api.add(this.id,
             {
                 // @ts-ignore
                 ids: idsArray,
                 embeddings: embeddingsArray as number[][], // We know this is defined because of the validate function
                 // @ts-ignore
                 documents: documentsArray,
+                // @ts-ignore
                 metadatas: metadatasArray,
             }, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
 
         return response
     }
@@ -244,14 +245,15 @@
         const response = await this.api.upsert(this.id,
             {
                 //@ts-ignore
                 ids: idsArray,
                 embeddings: embeddingsArray as number[][], // We know this is defined because of the validate function
                 //@ts-ignore
                 documents: documentsArray,
+                //@ts-ignore
                 metadatas: metadatasArray,
             },
             this.api.options
         )
             .then(handleSuccess)
             .catch(handleError);
 
@@ -357,14 +359,15 @@
 
         return await this.api
             .aGet(this.id, {
                 ids: idsArray,
                 where,
                 limit,
                 offset,
+                //@ts-ignore
                 include,
                 where_document: whereDocument,
             }, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
     }
 
@@ -508,14 +511,15 @@
 
         return await this.api
             .getNearestNeighbors(this.id, {
                 query_embeddings: query_embeddingsArray,
                 where,
                 n_results: nResults,
                 where_document: whereDocument,
+                //@ts-ignore
                 include: include,
             }, this.api.options)
             .then(handleSuccess)
             .catch(handleError);
     }
 
     /**
```

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/generated/README.md` & `chromadb-client-0.4.1.dev0/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/generated/api.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/generated/api.ts`

 * *Files 2% similar despite different names*

```diff
@@ -410,40 +410,14 @@
 			}
 			return {
 				url: localVarPath,
 				options: localVarRequestOptions,
 			};
 		},
 		/**
-		 * @summary Persist
-		 * @param {RequestInit} [options] Override http request option.
-		 * @throws {RequiredError}
-		 */
-		persist(options: RequestInit = {}): FetchArgs {
-			let localVarPath = `/api/v1/persist`;
-			const localVarPathQueryStart = localVarPath.indexOf("?");
-			const localVarRequestOptions: RequestInit = Object.assign({ method: 'POST' }, options);
-			const localVarHeaderParameter: Headers = options.headers ? new Headers(options.headers) : new Headers();
-			const localVarQueryParameter = new URLSearchParams(localVarPathQueryStart !== -1 ? localVarPath.substring(localVarPathQueryStart + 1) : "");
-			if (localVarPathQueryStart !== -1) {
-				localVarPath = localVarPath.substring(0, localVarPathQueryStart);
-			}
-
-			localVarRequestOptions.headers = localVarHeaderParameter;
-
-			const localVarQueryParameterString = localVarQueryParameter.toString();
-			if (localVarQueryParameterString) {
-				localVarPath += "?" + localVarQueryParameterString;
-			}
-			return {
-				url: localVarPath,
-				options: localVarRequestOptions,
-			};
-		},
-		/**
 		 * @summary Raw Sql
 		 * @param {Api.RawSql} request
 		 * @param {RequestInit} [options] Override http request option.
 		 * @throws {RequiredError}
 		 */
 		rawSql(request: Api.RawSql, options: RequestInit = {}): FetchArgs {
 			// verify required parameter 'request' is not null or undefined
@@ -998,36 +972,14 @@
 						throw response;
 					}
 					throw response;
 				});
 			};
 		},
 		/**
-		 * @summary Persist
-		 * @param {RequestInit} [options] Override http request option.
-		 * @throws {RequiredError}
-		 */
-		persist(options?: RequestInit): (fetch?: FetchAPI, basePath?: string) => Promise<Api.Persist200Response> {
-			const localVarFetchArgs = ApiApiFetchParamCreator(configuration).persist(options);
-			return (fetch: FetchAPI = defaultFetch, basePath: string = BASE_PATH) => {
-				return fetch(basePath + localVarFetchArgs.url, localVarFetchArgs.options).then((response) => {
-					const contentType = response.headers.get('Content-Type');
-					const mimeType = contentType ? contentType.replace(/;.*/, '') : undefined;
-
-					if (response.status === 200) {
-						if (mimeType === 'application/json') {
-							return response.json() as any;
-						}
-						throw response;
-					}
-					throw response;
-				});
-			};
-		},
-		/**
 		 * @summary Raw Sql
 		 * @param {Api.RawSql} request
 		 * @param {RequestInit} [options] Override http request option.
 		 * @throws {RequiredError}
 		 */
 		rawSql(request: Api.RawSql, options?: RequestInit): (fetch?: FetchAPI, basePath?: string) => Promise<Api.RawSql200Response> {
 			const localVarFetchArgs = ApiApiFetchParamCreator(configuration).rawSql(request, options);
@@ -1335,23 +1287,14 @@
 	 * @throws {RequiredError}
 	 */
 	public listCollections(options?: RequestInit) {
 		return ApiApiFp(this.configuration).listCollections(options)(this.fetch, this.basePath);
 	}
 
 	/**
-	 * @summary Persist
-	 * @param {RequestInit} [options] Override http request option.
-	 * @throws {RequiredError}
-	 */
-	public persist(options?: RequestInit) {
-		return ApiApiFp(this.configuration).persist(options)(this.fetch, this.basePath);
-	}
-
-	/**
 	 * @summary Raw Sql
 	 * @param {Api.RawSql} request
 	 * @param {RequestInit} [options] Override http request option.
 	 * @throws {RequiredError}
 	 */
 	public rawSql(request: Api.RawSql, options?: RequestInit) {
 		return ApiApiFp(this.configuration).rawSql(request, options)(this.fetch, this.basePath);
```

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/generated/configuration.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/generated/models.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/generated/models.ts`

 * *Files 26% similar despite different names*

```diff
@@ -13,66 +13,30 @@
  */
 
 export namespace Api {
 	export interface Add201Response {
 	}
 
 	export interface AddEmbedding {
-		embeddings: Api.AddEmbedding.Embedding[];
-		metadatas?: Api.AddEmbedding.Metadatas.ArrayValue[] | Api.AddEmbedding.Metadatas.ObjectValue;
-		documents?: string | Api.AddEmbedding.Documents.ArrayValue[];
-		ids?: string | Api.AddEmbedding.Ids.ArrayValue[];
+		embeddings?: Api.AddEmbedding.Embedding[];
+		metadatas?: Api.AddEmbedding.Metadata[];
+		documents?: string[];
+		ids: string[];
 		'increment_index'?: boolean;
 	}
 
 	/**
 	 * @export
 	 * @namespace AddEmbedding
 	 */
 	export namespace AddEmbedding {
 		export interface Embedding {
 		}
 
-		export type Metadatas = Api.AddEmbedding.Metadatas.ArrayValue[] | Api.AddEmbedding.Metadatas.ObjectValue;
-
-		/**
-		 * @export
-		 * @namespace Metadatas
-		 */
-		export namespace Metadatas {
-			export interface ArrayValue {
-			}
-
-			export interface ObjectValue {
-			}
-
-		}
-
-		export type Documents = string | Api.AddEmbedding.Documents.ArrayValue[];
-
-		/**
-		 * @export
-		 * @namespace Documents
-		 */
-		export namespace Documents {
-			export interface ArrayValue {
-			}
-
-		}
-
-		export type Ids = string | Api.AddEmbedding.Ids.ArrayValue[];
-
-		/**
-		 * @export
-		 * @namespace Ids
-		 */
-		export namespace Ids {
-			export interface ArrayValue {
-			}
-
+		export interface Metadata {
 		}
 
 	}
 
 	export interface ADelete200Response {
 	}
 
@@ -104,75 +68,87 @@
 	export interface CreateIndex200Response {
 	}
 
 	export interface DeleteCollection200Response {
 	}
 
 	export interface DeleteEmbedding {
-		ids?: Api.DeleteEmbedding.Id[];
+		ids?: string[];
 		where?: Api.DeleteEmbedding.Where;
 		'where_document'?: Api.DeleteEmbedding.WhereDocument;
 	}
 
 	/**
 	 * @export
 	 * @namespace DeleteEmbedding
 	 */
 	export namespace DeleteEmbedding {
-		export interface Id {
-		}
-
 		export interface Where {
 		}
 
 		export interface WhereDocument {
 		}
 
 	}
 
 	export interface GetCollection200Response {
 	}
 
 	export interface GetEmbedding {
-		ids?: Api.GetEmbedding.Id[];
+		ids?: string[];
 		where?: Api.GetEmbedding.Where;
 		'where_document'?: Api.GetEmbedding.WhereDocument;
 		sort?: string;
 		/**
 		 * @type {number}
 		 * @memberof GetEmbedding
 		 */
 		limit?: number;
 		/**
 		 * @type {number}
 		 * @memberof GetEmbedding
 		 */
 		offset?: number;
-		include?: Api.GetEmbedding.IncludeEnum[];
+		include?: (Api.GetEmbedding.Include.EnumValueEnum | Api.GetEmbedding.Include.EnumValueEnum2 | Api.GetEmbedding.Include.EnumValueEnum3 | Api.GetEmbedding.Include.EnumValueEnum4)[];
 	}
 
 	/**
 	 * @export
 	 * @namespace GetEmbedding
 	 */
 	export namespace GetEmbedding {
-		export interface Id {
-		}
-
 		export interface Where {
 		}
 
 		export interface WhereDocument {
 		}
 
-		export enum IncludeEnum {
-			Documents = 'documents',
-			Embeddings = 'embeddings',
-			Metadatas = 'metadatas',
-			Distances = 'distances'
+		export type Include = Api.GetEmbedding.Include.EnumValueEnum | Api.GetEmbedding.Include.EnumValueEnum2 | Api.GetEmbedding.Include.EnumValueEnum3 | Api.GetEmbedding.Include.EnumValueEnum4;
+
+		/**
+		 * @export
+		 * @namespace Include
+		 */
+		export namespace Include {
+			export enum EnumValueEnum {
+				Documents = 'documents'
+			}
+
+			export enum EnumValueEnum2 {
+				Embeddings = 'embeddings'
+			}
+
+			export enum EnumValueEnum3 {
+				Metadatas = 'metadatas'
+			}
+
+			export enum EnumValueEnum4 {
+				Distances = 'distances'
+			}
+
 		}
 
 	}
 
 	export interface GetNearestNeighbors200Response {
 	}
 
@@ -182,27 +158,24 @@
 	export interface HTTPValidationError {
 		detail?: Api.ValidationError[];
 	}
 
 	export interface ListCollections200Response {
 	}
 
-	export interface Persist200Response {
-	}
-
 	export interface QueryEmbedding {
 		where?: Api.QueryEmbedding.Where;
 		'where_document'?: Api.QueryEmbedding.WhereDocument;
 		'query_embeddings': Api.QueryEmbedding.QueryEmbedding2[];
 		/**
 		 * @type {number}
 		 * @memberof QueryEmbedding
 		 */
 		'n_results'?: number;
-		include?: Api.QueryEmbedding.IncludeEnum[];
+		include?: (Api.QueryEmbedding.Include.EnumValueEnum | Api.QueryEmbedding.Include.EnumValueEnum2 | Api.QueryEmbedding.Include.EnumValueEnum3 | Api.QueryEmbedding.Include.EnumValueEnum4)[];
 	}
 
 	/**
 	 * @export
 	 * @namespace QueryEmbedding
 	 */
 	export namespace QueryEmbedding {
@@ -211,25 +184,43 @@
 
 		export interface WhereDocument {
 		}
 
 		export interface QueryEmbedding2 {
 		}
 
-		export enum IncludeEnum {
-			Documents = 'documents',
-			Embeddings = 'embeddings',
-			Metadatas = 'metadatas',
-			Distances = 'distances'
+		export type Include = Api.QueryEmbedding.Include.EnumValueEnum | Api.QueryEmbedding.Include.EnumValueEnum2 | Api.QueryEmbedding.Include.EnumValueEnum3 | Api.QueryEmbedding.Include.EnumValueEnum4;
+
+		/**
+		 * @export
+		 * @namespace Include
+		 */
+		export namespace Include {
+			export enum EnumValueEnum {
+				Documents = 'documents'
+			}
+
+			export enum EnumValueEnum2 {
+				Embeddings = 'embeddings'
+			}
+
+			export enum EnumValueEnum3 {
+				Metadatas = 'metadatas'
+			}
+
+			export enum EnumValueEnum4 {
+				Distances = 'distances'
+			}
+
 		}
 
 	}
 
 	export interface RawSql {
-		'raw_sql'?: string;
+		'raw_sql': string;
 	}
 
 	export interface RawSql200Response {
 	}
 
 	export interface Reset200Response {
 	}
@@ -256,65 +247,29 @@
 	}
 
 	export interface UpdateCollection200Response {
 	}
 
 	export interface UpdateEmbedding {
 		embeddings?: Api.UpdateEmbedding.Embedding[];
-		metadatas?: Api.UpdateEmbedding.Metadatas.ArrayValue[] | Api.UpdateEmbedding.Metadatas.ObjectValue;
-		documents?: string | Api.UpdateEmbedding.Documents.ArrayValue[];
-		ids?: string | Api.UpdateEmbedding.Ids.ArrayValue[];
+		metadatas?: Api.UpdateEmbedding.Metadata[];
+		documents?: string[];
+		ids: string[];
 		'increment_index'?: boolean;
 	}
 
 	/**
 	 * @export
 	 * @namespace UpdateEmbedding
 	 */
 	export namespace UpdateEmbedding {
 		export interface Embedding {
 		}
 
-		export type Metadatas = Api.UpdateEmbedding.Metadatas.ArrayValue[] | Api.UpdateEmbedding.Metadatas.ObjectValue;
-
-		/**
-		 * @export
-		 * @namespace Metadatas
-		 */
-		export namespace Metadatas {
-			export interface ArrayValue {
-			}
-
-			export interface ObjectValue {
-			}
-
-		}
-
-		export type Documents = string | Api.UpdateEmbedding.Documents.ArrayValue[];
-
-		/**
-		 * @export
-		 * @namespace Documents
-		 */
-		export namespace Documents {
-			export interface ArrayValue {
-			}
-
-		}
-
-		export type Ids = string | Api.UpdateEmbedding.Ids.ArrayValue[];
-
-		/**
-		 * @export
-		 * @namespace Ids
-		 */
-		export namespace Ids {
-			export interface ArrayValue {
-			}
-
+		export interface Metadata {
 		}
 
 	}
 
 	export interface Upsert200Response {
 	}
```

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/generated/runtime.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/types.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/types.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/src/utils.ts` & `chromadb-client-0.4.1.dev0/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/test/add.collections.test.ts` & `chromadb-client-0.4.1.dev0/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/test/client.test.ts` & `chromadb-client-0.4.1.dev0/clients/js/test/client.test.ts`

 * *Files 0% similar despite different names*

```diff
@@ -187,9 +187,9 @@
         [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]
     ]
     const metadatas = [{ test: 'test1' }, { test: 'test2' }, { test: 'test3' }]
     await collection.add({ ids, embeddings, metadatas })
     // @ts-ignore - supposed to fail
     const results = await collection.get({ where: { "test": { "$contains": "hello" } } });
     expect(results.error).toBeDefined()
-    expect(results.error).toBe("ValueError('Expected one of $gt, $lt, $gte, $lte, $ne, $eq, got $contains')")
+    expect(results.error).toBe("ValueError('Expected where operator to be one of $gt, $gte, $lt, $lte, $ne, $eq, got $contains')")
 })
```

### Comparing `chromadb-client-0.3.30.dev0/clients/js/test/collection.client.test.ts` & `chromadb-client-0.4.1.dev0/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/test/collection.test.ts` & `chromadb-client-0.4.1.dev0/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/test/delete.collection.test.ts` & `chromadb-client-0.4.1.dev0/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/test/get.collection.test.ts` & `chromadb-client-0.4.1.dev0/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/test/peek.collection.test.ts` & `chromadb-client-0.4.1.dev0/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/test/query.collection.test.ts` & `chromadb-client-0.4.1.dev0/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/test/update.collection.test.ts` & `chromadb-client-0.4.1.dev0/clients/js/test/update.collection.test.ts`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
       IncludeEnum.Metadatas,
       IncludeEnum.Documents,
     ]
   });
   expect(results2).toBeDefined();
   expect(results2).toBeInstanceOf(Object);
   expect(results2.embeddings![0]).toEqual([1, 2, 3, 4, 5, 6, 7, 8, 9, 11]);
-  expect(results2.metadatas[0]).toEqual({ test: "test1new" });
+  expect(results2.metadatas[0]).toEqual({ test: "test1new", float_value: -2 });
   expect(results2.documents[0]).toEqual("doc1new");
 });
 
 // this currently fails
 // test("it should update metadata or documents to array of Nones", async () => {
 //   await chroma.reset();
 //   const collection = await chroma.createCollection({ name: "test" });
```

### Comparing `chromadb-client-0.3.30.dev0/clients/js/test/upsert.collections.test.ts` & `chromadb-client-0.4.1.dev0/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/js/yarn.lock` & `chromadb-client-0.4.1.dev0/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/python/README.md` & `chromadb-client-0.4.1.dev0/clients/python/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,19 +12,16 @@
 pip install chromadb-client # python http-client only library
 ```
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
-from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest",
-                                  chroma_server_host="localhost",
-                                  chroma_server_http_port=8000))
+client = chromadb.HttpClient(host="localhost", port=8000)
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -1,19 +1,17 @@
                                  [Chroma_logo]
                  Chroma - the open-source embedding database.
  This package is for the the Python HTTP client-only library for Chroma. This
 client connects to the Chroma Server. If that it not what you are looking for,
                  you might want to check out the full_library.
 ```bash pip install chromadb-client # python http-client only library ``` To
 connect to your server and perform operations using the client only library,
-you can do the following: ```python import chromadb from chromadb.config import
-Settings # Example setup of the client to connect to your chroma server client
-= chromadb.Client(Settings(chroma_api_impl="rest",
-chroma_server_host="localhost", chroma_server_http_port=8000)) collection =
-client.create_collection("all-my-documents") collection.add( documents=["This
-is document1", "This is document2"], metadatas=[{"source": "notion"},
-{"source": "google-docs"}], # filter on these! ids=["doc1", "doc2"], # unique
-for each doc embeddings = [[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results =
-collection.query( query_texts=["This is a query document"], n_results=2, #
-where={"metadata_field": "is_equal_to_this"}, # optional filter #
-where_document={"$contains":"search_string"} # optional filter ) ``` ## License
-[Apache 2.0](./LICENSE)
+you can do the following: ```python import chromadb # Example setup of the
+client to connect to your chroma server client = chromadb.HttpClient
+(host="localhost", port=8000) collection = client.create_collection("all-my-
+documents") collection.add( documents=["This is document1", "This is
+document2"], metadatas=[{"source": "notion"}, {"source": "google-docs"}], #
+filter on these! ids=["doc1", "doc2"], # unique for each doc embeddings = [
+[1.2, 2.1, ...], [1.2, 2.1, ...]] ) results = collection.query( query_texts=
+["This is a query document"], n_results=2, # where={"metadata_field":
+"is_equal_to_this"}, # optional filter # where_document={"$contains":
+"search_string"} # optional filter ) ``` ## License [Apache 2.0](./LICENSE)
```

### Comparing `chromadb-client-0.3.30.dev0/clients/python/build_python_thin_client.sh` & `chromadb-client-0.4.1.dev0/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/clients/python/integration-test.sh` & `chromadb-client-0.4.1.dev0/clients/python/integration-test.sh`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 }
 
 trap cleanup EXIT
 
 docker compose -f docker-compose.test.yml up --build -d
 
 export CHROMA_INTEGRATION_TEST_ONLY=1
-export CHROMA_API_IMPL=rest
+export CHROMA_API_IMPL=chromadb.api.fastapi.FastAPI
 export CHROMA_SERVER_HOST=localhost
 export CHROMA_SERVER_HTTP_PORT=8000
 
 echo testing: python -m pytest "$@"
 
 # Copy the thin client flag script in place, uvicorn takes a while to startup inside docker
 sleep 5
```

### Comparing `chromadb-client-0.3.30.dev0/clients/python/pyproject.toml` & `chromadb-client-0.4.1.dev0/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/examples/README.md` & `chromadb-client-0.4.1.dev0/examples/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/examples/basic_functionality/alternative_embeddings.ipynb` & `chromadb-client-0.4.1.dev0/examples/basic_functionality/alternative_embeddings.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904729352678572%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'execution_count': 1}, 2: {'execution_count': "*

 * *            "2, 'outputs': []}, 3: {'execution_count': 3}, 4: {'execution_count': 4, 'source': "*

 * *            '{insert: [(2, \'    api_key="OPENAI_KEY", # Replace with your own OpenAI API '*

 * *            "key\\n')], delete: [2]}}, 5: {'execution_count': 5, 'source': {insert: [(1, "*

 * *            '\'openai_collection = client.get_or_create_collection(name="openai_embeddings", '*

 * *            "embedding_function=open […]*

```diff
@@ -1,106 +1,99 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 " # Alternative Embeddings\n",
                 " \n",
                 " This notebook demonstrates how to use alternative embedding functions.\n",
                 " "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import chromadb"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Using embedded DuckDB without persistence: data will be transient\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "client = chromadb.Client()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from chromadb.utils import embedding_functions"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Using OpenAI Embeddings. This assumes you have the openai package installed\n",
                 "openai_ef = embedding_functions.OpenAIEmbeddingFunction(\n",
-                "    api_key=\"OPENAI_API_KEY\", # Replace with your own OpenAI API key\n",
+                "    api_key=\"OPENAI_KEY\", # Replace with your own OpenAI API key\n",
                 "    model_name=\"text-embedding-ada-002\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Create a new chroma collection\n",
-                "openai_collection = client.create_collection(name=\"openai_embeddings\", embedding_function=openai_ef)"
+                "openai_collection = client.get_or_create_collection(name=\"openai_embeddings\", embedding_function=openai_ef)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "openai_collection.add(\n",
                 "    documents=[\"This is a document\", \"This is another document\"],\n",
                 "    metadatas=[{\"source\": \"my_source\"}, {\"source\": \"my_source\"}],\n",
                 "    ids=[\"id1\", \"id2\"]\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'ids': [['id1', 'id2']],\n",
-                            " 'embeddings': None,\n",
-                            " 'documents': [['This is a document', 'This is another document']],\n",
+                            " 'distances': [[0.1385088860988617, 0.2017185091972351]],\n",
                             " 'metadatas': [[{'source': 'my_source'}, {'source': 'my_source'}]],\n",
-                            " 'distances': [[0.13865342736244202, 0.20187020301818848]]}"
+                            " 'embeddings': None,\n",
+                            " 'documents': [['This is a document', 'This is another document']]}"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "results = openai_collection.query(\n",
                 "    query_texts=[\"This is a query document\"],\n",
@@ -320,13 +313,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.10.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `chromadb-client-0.3.30.dev0/examples/basic_functionality/local_persistence.ipynb` & `chromadb-client-0.4.1.dev0/examples/basic_functionality/local_persistence.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9664765211640212%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'This notebook demonstrates how to configure Chroma to "*

 * *            "persist to disk, then load it back in. ')], delete: [1]}}, 1: {'source': ['import "*

 * *            "chromadb']}, 3: {'outputs': [], 'source': ['# Add some data to the collection\\n', "*

 * *            "'collection.add(\\n', '    embeddings=[\\n', '        [1.1, 2.3, 3.2],\\n', '        "*

 * *            "[4.5, 6.9, 4.4],\\n', '        [1.1, 2.3, 3.2],\\n', '        [4.5, 6.9, 4.4],\\n', "*

 * *            "'      […]*

```diff
@@ -2,72 +2,45 @@
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Local Peristence Demo\n",
-                "This notebook demonstrates how to persist the in-memory version of Chroma to disk, then load it back in. "
+                "This notebook demonstrates how to configure Chroma to persist to disk, then load it back in. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import chromadb\n",
-                "from chromadb.config import Settings"
+                "import chromadb"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Running Chroma using direct local API.\n",
-                        "No existing DB found in db, skipping load\n",
-                        "No existing DB found in db, skipping load\n"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/antontroynikov/miniforge3/envs/chroma/lib/python3.9/site-packages/tqdm/auto.py:22: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html\n",
-                        "  from .autonotebook import tqdm as notebook_tqdm\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "# Create a new Chroma client with persistence enabled. \n",
                 "persist_directory = \"db\"\n",
                 "\n",
-                "client = chromadb.Client(\n",
-                "    Settings(\n",
-                "        persist_directory=persist_directory,\n",
-                "        chroma_db_impl=\"duckdb+parquet\",\n",
-                "    )\n",
-                ")\n",
-                "\n",
-                "# Start from scratch\n",
-                "client.reset()\n",
+                "client = chromadb.PersistentClient(path=persist_directory)\n",
                 "\n",
                 "# Create a new chroma collection\n",
                 "collection_name = \"peristed_collection\"\n",
-                "collection = client.create_collection(name=collection_name)"
+                "collection = client.get_or_create_collection(name=collection_name)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Add some data to the collection\n",
                 "collection.add(\n",
                 "    embeddings=[\n",
                 "        [1.1, 2.3, 3.2],\n",
@@ -92,79 +65,35 @@
                 "    documents=[\"doc1\", \"doc2\", \"doc3\", \"doc4\", \"doc5\", \"doc6\", \"doc7\", \"doc8\"],\n",
                 "    ids=[\"id1\", \"id2\", \"id3\", \"id4\", \"id5\", \"id6\", \"id7\", \"id8\"],\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Persisting DB to disk, putting it in the save folder db\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "text/plain": [
-                            "True"
-                        ]
-                    },
-                    "execution_count": 5,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "# Persist the DB. This also happens automatically when the client is garbage collected.\n",
-                "# In a notebook, prefer to call persist explicitly.\n",
-                "client.persist()\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 4,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Running Chroma using direct local API.\n",
-                        "loaded in 8 embeddings\n",
-                        "loaded in 1 collections\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "# Create a new client with the same settings\n",
-                "client = chromadb.Client(\n",
-                "    Settings(\n",
-                "        persist_directory=persist_directory,\n",
-                "        chroma_db_impl=\"duckdb+parquet\",\n",
-                "    )\n",
-                ")\n",
+                "client = chromadb.PersistentClient(path=persist_directory)\n",
                 "\n",
                 "# Load the collection\n",
                 "collection = client.get_collection(collection_name)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "{'embeddings': [[[1.1, 2.3, 3.2]]], 'documents': [['doc5']], 'ids': [['id5']], 'metadatas': [[{'uri': 'img5.png', 'style': 'style1'}]], 'distances': [[0.0]]}\n"
+                        "{'ids': [['id1']], 'distances': [[5.1159076593562386e-15]], 'metadatas': [[{'style': 'style1', 'uri': 'img1.png'}]], 'embeddings': None, 'documents': [['doc1']]}\n"
                     ]
                 }
             ],
             "source": [
                 "# Query the collection\n",
                 "results = collection.query(\n",
                 "    query_embeddings=[[1.1, 2.3, 3.2]],\n",
@@ -172,33 +101,65 @@
                 ")\n",
                 "\n",
                 "print(results)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Persisting DB to disk, putting it in the save folder db\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "{'ids': ['id1', 'id2', 'id3', 'id4', 'id5', 'id6', 'id7', 'id8'],\n",
+                            " 'embeddings': [[1.100000023841858, 2.299999952316284, 3.200000047683716],\n",
+                            "  [4.5, 6.900000095367432, 4.400000095367432],\n",
+                            "  [1.100000023841858, 2.299999952316284, 3.200000047683716],\n",
+                            "  [4.5, 6.900000095367432, 4.400000095367432],\n",
+                            "  [1.100000023841858, 2.299999952316284, 3.200000047683716],\n",
+                            "  [4.5, 6.900000095367432, 4.400000095367432],\n",
+                            "  [1.100000023841858, 2.299999952316284, 3.200000047683716],\n",
+                            "  [4.5, 6.900000095367432, 4.400000095367432]],\n",
+                            " 'metadatas': [{'style': 'style1', 'uri': 'img1.png'},\n",
+                            "  {'style': 'style2', 'uri': 'img2.png'},\n",
+                            "  {'style': 'style1', 'uri': 'img3.png'},\n",
+                            "  {'style': 'style1', 'uri': 'img4.png'},\n",
+                            "  {'style': 'style1', 'uri': 'img5.png'},\n",
+                            "  {'style': 'style1', 'uri': 'img6.png'},\n",
+                            "  {'style': 'style1', 'uri': 'img7.png'},\n",
+                            "  {'style': 'style1', 'uri': 'img8.png'}],\n",
+                            " 'documents': ['doc1', 'doc2', 'doc3', 'doc4', 'doc5', 'doc6', 'doc7', 'doc8']}"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
+                "collection.get(include=[\"embeddings\", \"metadatas\", \"documents\"])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "# Clean up\n",
-                "client.reset()\n",
-                "client.persist()\n",
-                "\n",
-                "# You can also just delete the persist directory\n",
-                "!rm -rf db/"
+                "! rm -rf db"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "chroma",
             "language": "python",
             "name": "python3"
@@ -209,15 +170,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.10.8"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "88f09714c9334832bac29166716f9f6a879ee2a4ed4822c1d4120cb2393b58dd"
             }
         }
```

### Comparing `chromadb-client-0.3.30.dev0/examples/basic_functionality/where_filtering.ipynb` & `chromadb-client-0.4.1.dev0/examples/basic_functionality/where_filtering.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9728932429453263%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1}, 2: {'execution_count': 2, 'outputs': []}, 3: "*

 * *            "{'execution_count': 3, 'outputs': []}, 4: {'execution_count': 4}, 5: "*

 * *            '{\'execution_count\': 5, \'outputs\': {0: {\'data\': {\'text/plain\': {insert: [(2, " '*

 * *            '\'metadatas\': [{\'status\': \'read\'}],\\n"), (3, " \'documents\': [\'A document '*

 * *            'that discusses international affairs\']}")], delete: [3, 2]}}, \'execution_count\': '*

 * *            "5}}}, 6: {'execution_count': 6 […]*

```diff
@@ -7,60 +7,44 @@
             "source": [
                 "# Where Filtering\n",
                 "This notebook demonstrates how to use where filtering to filter the data returned from get or query."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import chromadb"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 2,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Using embedded DuckDB without persistence: data will be transient\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "client = chromadb.Client()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 3,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "No embedding_function provided, using default embedding function: SentenceTransformerEmbeddingFunction\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "# Create a new chroma collection\n",
                 "collection_name = \"filter_example_collection\"\n",
                 "collection = client.create_collection(name=collection_name)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Add some data to the collection\n",
                 "collection.add(\n",
                 "    embeddings=[\n",
                 "        [1.1, 2.3, 3.2],\n",
@@ -85,90 +69,97 @@
                 "    documents=[\"A document that discusses domestic policy\", \"A document that discusses international affairs\", \"A document that discusses kittens\", \"A document that discusses dogs\", \"A document that discusses chocolate\", \"A document that is sixth that discusses government\", \"A document that discusses international affairs\", \"A document that discusses global affairs\"],\n",
                 "    ids=[\"id1\", \"id2\", \"id3\", \"id4\", \"id5\", \"id6\", \"id7\", \"id8\"],\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'ids': ['id7'],\n",
                             " 'embeddings': None,\n",
-                            " 'documents': ['A document that discusses international affairs'],\n",
-                            " 'metadatas': [{'status': 'read'}]}"
+                            " 'metadatas': [{'status': 'read'}],\n",
+                            " 'documents': ['A document that discusses international affairs']}"
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Get documents that are read and about affairs\n",
                 "collection.get(where={\"status\": \"read\"}, where_document={\"$contains\": \"affairs\"})"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'ids': ['id8', 'id1'],\n",
+                            "{'ids': ['id1', 'id8'],\n",
                             " 'embeddings': None,\n",
-                            " 'documents': ['A document that discusses global affairs',\n",
-                            "  'A document that discusses domestic policy'],\n",
-                            " 'metadatas': [{'status': 'unread'}, {'status': 'read'}]}"
+                            " 'metadatas': [{'status': 'read'}, {'status': 'unread'}],\n",
+                            " 'documents': ['A document that discusses domestic policy',\n",
+                            "  'A document that discusses global affairs']}"
                         ]
                     },
-                    "execution_count": 30,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Get documents that are about global affairs or domestic policy\n",
                 "collection.get(where_document={\"$or\": [{\"$contains\": \"global affairs\"}, {\"$contains\": \"domestic policy\"}]})"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'ids': [['id7', 'id2', 'id8']],\n",
-                            " 'embeddings': None,\n",
-                            " 'documents': [['A document that discusses international affairs',\n",
-                            "   'A document that discusses international affairs',\n",
-                            "   'A document that discusses global affairs']],\n",
+                            " 'distances': [[16.740001678466797, 87.22000122070312, 87.22000122070312]],\n",
                             " 'metadatas': [[{'status': 'read'},\n",
                             "   {'status': 'unread'},\n",
                             "   {'status': 'unread'}]],\n",
-                            " 'distances': [[16.740001678466797, 87.22000122070312, 87.22000122070312]]}"
+                            " 'embeddings': None,\n",
+                            " 'documents': [['A document that discusses international affairs',\n",
+                            "   'A document that discusses international affairs',\n",
+                            "   'A document that discusses global affairs']]}"
                         ]
                     },
-                    "execution_count": 31,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Get 5 closest vectors to [0, 0, 0] that are about affairs\n",
                 "# Outputs 3 docs because collection only has 3 docs about affairs\n",
                 "collection.query(query_embeddings=[[0, 0, 0]], where_document={\"$contains\": \"affairs\"}, n_results=5)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `chromadb-client-0.3.30.dev0/examples/deployments/google-cloud-compute/README.md` & `chromadb-client-0.4.1.dev0/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/examples/deployments/google-cloud-compute/chroma.tf` & `chromadb-client-0.4.1.dev0/examples/deployments/google-cloud-compute/chroma.tf`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/examples/deployments/google-cloud-compute/startup.sh` & `chromadb-client-0.4.1.dev0/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/examples/use_with/cohere/cohere_js.js` & `chromadb-client-0.4.1.dev0/examples/use_with/cohere/cohere_js.js`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/examples/use_with/cohere/cohere_python.ipynb` & `chromadb-client-0.4.1.dev0/examples/use_with/cohere/cohere_python.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/migrations/metadb/00001-embedding-metadata.sqlite.sql` & `chromadb-client-0.4.1.dev0/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.30.dev0/pyproject.toml` & `chromadb-client-0.4.1.dev0/pyproject.toml`

 * *Files identical despite different names*

