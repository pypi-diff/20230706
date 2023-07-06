# Comparing `tmp/smart_chromadb-0.1.dev733.tar.gz` & `tmp/smart_chromadb-0.1.dev734.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/johnyan/Documents/project/chroma/dist/.tmp-4l85f_2n/smart_chromadb-0.1.dev733.tar", last modified: Wed Jul  5 01:00:13 2023, max compression
+gzip compressed data, was "/Users/johnyan/Documents/project/chroma/dist/.tmp-1muq0w34/smart_chromadb-0.1.dev734.tar", last modified: Thu Jul  6 08:26:27 2023, max compression
```

## Comparing `smart_chromadb-0.1.dev733.tar` & `smart_chromadb-0.1.dev734.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.065730 smart_chromadb-0.1.dev733/
--rw-r--r--   0 johnyan    (501) staff       (20)       84 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.dockerignore
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.814016 smart_chromadb-0.1.dev733/.github/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.845879 smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 johnyan    (501) staff       (20)     1512 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     1520 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     1384 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.850908 smart_chromadb-0.1.dev733/.github/workflows/
--rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1338 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     4169 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/chroma-release.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/chroma-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1734 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 johnyan    (501) staff       (20)      228 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.gitignore
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.pre-commit-config.yaml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.851862 smart_chromadb-0.1.dev733/.vscode/
--rw-r--r--   0 johnyan    (501) staff       (20)     1020 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.vscode/settings.json
--rw-r--r--   0 johnyan    (501) staff       (20)     3323 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/DEVELOP.md
--rw-r--r--   0 johnyan    (501) staff       (20)      647 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/Dockerfile
--rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/LICENSE
--rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-07-05 01:00:13.065086 smart_chromadb-0.1.dev733/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)     5679 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      619 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/RELEASE_PROCESS.md
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.869128 smart_chromadb-0.1.dev733/bin/
--rw-r--r--   0 johnyan    (501) staff       (20)     1610 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/backup.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/build
--rwxr-xr-x   0 johnyan    (501) staff       (20)      234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/docker_entrypoint.sh
--rw-r--r--   0 johnyan    (501) staff       (20)     6462 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/generate_cloudformation.py
--rwxr-xr-x   0 johnyan    (501) staff       (20)      463 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/integration-test
--rw-r--r--   0 johnyan    (501) staff       (20)     1688 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/restore.sh
--rw-r--r--   0 johnyan    (501) staff       (20)     1105 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/setup_linux.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/setup_mac.sh
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.871204 smart_chromadb-0.1.dev733/bin/templates/
--rw-r--r--   0 johnyan    (501) staff       (20)      985 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/templates/docker-compose.yml
--rwxr-xr-x   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/test-package.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      297 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/test-remote
--rw-r--r--   0 johnyan    (501) staff       (20)      205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/test.py
--rwxr-xr-x   0 johnyan    (501) staff       (20)      151 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/version
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.875763 smart_chromadb-0.1.dev733/chromadb/
--rw-r--r--   0 johnyan    (501) staff       (20)      894 2023-07-04 08:34:52.000000 smart_chromadb-0.1.dev733/chromadb/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.883748 smart_chromadb-0.1.dev733/chromadb/api/
--rw-r--r--   0 johnyan    (501) staff       (20)    10898 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/api/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12480 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/api/fastapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)    17852 2023-07-03 08:25:25.000000 smart_chromadb-0.1.dev733/chromadb/api/local.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.884529 smart_chromadb-0.1.dev733/chromadb/api/models/
--rw-r--r--   0 johnyan    (501) staff       (20)    15103 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/api/models/Collection.py
--rw-r--r--   0 johnyan    (501) staff       (20)      819 2023-07-03 07:56:58.000000 smart_chromadb-0.1.dev733/chromadb/api/smartapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11283 2023-07-03 09:25:09.000000 smart_chromadb-0.1.dev733/chromadb/api/types.py
--rw-r--r--   0 johnyan    (501) staff       (20)      168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7231 2023-07-03 08:16:05.000000 smart_chromadb-0.1.dev733/chromadb/config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.895630 smart_chromadb-0.1.dev733/chromadb/db/
--rw-r--r--   0 johnyan    (501) staff       (20)     3390 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6004 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)    22307 2023-07-03 08:25:52.000000 smart_chromadb-0.1.dev733/chromadb/db/clickhouse.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18795 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/duckdb.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.897485 smart_chromadb-0.1.dev733/chromadb/db/impl/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/impl/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/impl/sqlite.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.899510 smart_chromadb-0.1.dev733/chromadb/db/index/
--rw-r--r--   0 johnyan    (501) staff       (20)      447 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/index/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11060 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/index/hnswlib.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8096 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/migrations.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.903241 smart_chromadb-0.1.dev733/chromadb/db/mixins/
--rw-r--r--   0 johnyan    (501) staff       (20)     9193 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15557 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16627 2023-07-05 00:49:42.000000 smart_chromadb-0.1.dev733/chromadb/db/smartdb.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2656 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/system.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1293 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/errors.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.905239 smart_chromadb-0.1.dev733/chromadb/ingest/
--rw-r--r--   0 johnyan    (501) staff       (20)     3643 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/ingest/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.907332 smart_chromadb-0.1.dev733/chromadb/segment/
--rw-r--r--   0 johnyan    (501) staff       (20)     3059 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/segment/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.816756 smart_chromadb-0.1.dev733/chromadb/segment/impl/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.909423 smart_chromadb-0.1.dev733/chromadb/segment/impl/manager/
--rw-r--r--   0 johnyan    (501) staff       (20)     4358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.911260 smart_chromadb-0.1.dev733/chromadb/segment/impl/metadata/
--rw-r--r--   0 johnyan    (501) staff       (20)    17879 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.913905 smart_chromadb-0.1.dev733/chromadb/segment/impl/vector/
--rw-r--r--   0 johnyan    (501) staff       (20)    11965 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/segment/impl/vector/local_hnsw.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.914955 smart_chromadb-0.1.dev733/chromadb/server/
--rw-r--r--   0 johnyan    (501) staff       (20)      172 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/server/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.918217 smart_chromadb-0.1.dev733/chromadb/server/fastapi/
--rw-r--r--   0 johnyan    (501) staff       (20)     9064 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2134 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.922855 smart_chromadb-0.1.dev733/chromadb/telemetry/
--rw-r--r--   0 johnyan    (501) staff       (20)     3214 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/telemetry/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)      591 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/telemetry/events.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.928389 smart_chromadb-0.1.dev733/chromadb/test/
--rw-r--r--   0 johnyan    (501) staff       (20)     3993 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/conftest.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.934819 smart_chromadb-0.1.dev733/chromadb/test/db/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.942083 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/test_base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/test_migrations.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9773 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/test_system.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.943456 smart_chromadb-0.1.dev733/chromadb/test/hnswlib/
--rw-r--r--   0 johnyan    (501) staff       (20)     2337 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/hnswlib/test_hnswlib.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.945671 smart_chromadb-0.1.dev733/chromadb/test/ingest/
--rw-r--r--   0 johnyan    (501) staff       (20)     8117 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.956335 smart_chromadb-0.1.dev733/chromadb/test/property/
--rw-r--r--   0 johnyan    (501) staff       (20)    11294 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/invariants.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18662 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/strategies.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2213 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_add.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6211 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_collections.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9123 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11073 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9062 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_filtering.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5146 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.959593 smart_chromadb-0.1.dev733/chromadb/test/segment/
--rw-r--r--   0 johnyan    (501) staff       (20)    15026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12132 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/segment/test_vector.py
--rw-r--r--   0 johnyan    (501) staff       (20)    40340 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/test_api.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/test_chroma.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4127 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/test_config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.960838 smart_chromadb-0.1.dev733/chromadb/test/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)     3544 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3702 2023-06-30 03:21:44.000000 smart_chromadb-0.1.dev733/chromadb/types.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.963212 smart_chromadb-0.1.dev733/chromadb/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/utils/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16311 2023-06-30 06:12:24.000000 smart_chromadb-0.1.dev733/chromadb/utils/embedding_functions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2301 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/utils/messageid.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.821744 smart_chromadb-0.1.dev733/clients/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.980560 smart_chromadb-0.1.dev733/clients/js/
--rw-r--r--   0 johnyan    (501) staff       (20)       66 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/.gitignore
--rw-r--r--   0 johnyan    (501) staff       (20)       32 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/.prettierignore
--rw-r--r--   0 johnyan    (501) staff       (20)        3 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/.prettierrc.json
--rw-r--r--   0 johnyan    (501) staff       (20)     1256 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/DEVELOP.md
--rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/LICENSE
--rw-r--r--   0 johnyan    (501) staff       (20)     1266 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      324 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/config.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.820147 smart_chromadb-0.1.dev733/clients/js/examples/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.988642 smart_chromadb-0.1.dev733/clients/js/examples/browser/
--rw-r--r--   0 johnyan    (501) staff       (20)      358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/browser/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1787 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/browser/app.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      834 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/browser/index.html
--rw-r--r--   0 johnyan    (501) staff       (20)      409 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/browser/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    71072 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.995260 smart_chromadb-0.1.dev733/clients/js/examples/node/
--rw-r--r--   0 johnyan    (501) staff       (20)       57 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/node/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1191 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/node/app.js
--rw-r--r--   0 johnyan    (501) staff       (20)    46542 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/node/package-lock.json
--rw-r--r--   0 johnyan    (501) staff       (20)      503 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/node/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    17116 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 johnyan    (501) staff       (20)     1075 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/genapi.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      469 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/jest.config.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      153 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/openapitools.json
--rw-r--r--   0 johnyan    (501) staff       (20)   450648 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/package-lock.json
--rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/package.json
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.002684 smart_chromadb-0.1.dev733/clients/js/src/
--rw-r--r--   0 johnyan    (501) staff       (20)     8171 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/ChromaClient.ts
--rw-r--r--   0 johnyan    (501) staff       (20)    19403 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/Collection.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.009777 smart_chromadb-0.1.dev733/clients/js/src/embeddings/
--rw-r--r--   0 johnyan    (501) staff       (20)      938 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)       92 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1563 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
--rwxr-xr-x   0 johnyan    (501) staff       (20)     3402 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.018984 smart_chromadb-0.1.dev733/clients/js/src/generated/
--rw-r--r--   0 johnyan    (501) staff       (20)      921 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)    56700 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/api.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1478 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/configuration.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      429 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/index.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     5862 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/models.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1307 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/runtime.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      490 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/index.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1715 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/types.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2002 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/utils.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.033037 smart_chromadb-0.1.dev733/clients/js/test/
--rw-r--r--   0 johnyan    (501) staff       (20)     2625 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/add.collections.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     7586 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/client.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     3284 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/collection.client.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2551 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/data.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2599 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/get.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      206 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/initClient.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      577 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1990 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/query.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2160 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/update.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      802 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      367 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/tsconfig.json
--rw-r--r--   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/tsconfig.module.json
--rw-r--r--   0 johnyan    (501) staff       (20)   157735 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/yarn.lock
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.040822 smart_chromadb-0.1.dev733/clients/python/
--rw-r--r--   0 johnyan    (501) staff       (20)     1627 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/python/README.md
--rwxr-xr-x   0 johnyan    (501) staff       (20)     1257 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      826 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/python/integration-test.sh
--rw-r--r--   0 johnyan    (501) staff       (20)       22 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/python/is_thin_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1166 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/python/pyproject.toml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.043344 smart_chromadb-0.1.dev733/config/
--rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/config/backup_disk.xml
--rw-r--r--   0 johnyan    (501) staff       (20)      233 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/config/chroma_users.xml
--rw-r--r--   0 johnyan    (501) staff       (20)     1080 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/docker-compose.server.example.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/docker-compose.test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1226 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/docker-compose.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.046211 smart_chromadb-0.1.dev733/examples/
--rw-r--r--   0 johnyan    (501) staff       (20)    10346 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/alternative_embeddings.ipynb
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.822587 smart_chromadb-0.1.dev733/examples/deployments/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.052843 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/
--rw-r--r--   0 johnyan    (501) staff       (20)      611 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      752 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 johnyan    (501) staff       (20)      125 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 johnyan    (501) staff       (20)     2271 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      181 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/variables.tf
--rw-r--r--   0 johnyan    (501) staff       (20)     5830 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/local_persistence.ipynb
--rw-r--r--   0 johnyan    (501) staff       (20)     5493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/where_filtering.ipynb
--rw-r--r--   0 johnyan    (501) staff       (20)      495 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/log_config.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.824657 smart_chromadb-0.1.dev733/migrations/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.054250 smart_chromadb-0.1.dev733/migrations/embeddings_queue/
--rw-r--r--   0 johnyan    (501) staff       (20)      261 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.055369 smart_chromadb-0.1.dev733/migrations/metadb/
--rw-r--r--   0 johnyan    (501) staff       (20)      620 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/migrations/metadb/00001-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.058329 smart_chromadb-0.1.dev733/migrations/sysdb/
--rw-r--r--   0 johnyan    (501) staff       (20)      336 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)      372 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/pull_request_template.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-26 07:09:55.000000 smart_chromadb-0.1.dev733/pyproject.toml
--rw-r--r--   0 johnyan    (501) staff       (20)      352 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/requirements.txt
--rw-r--r--   0 johnyan    (501) staff       (20)      161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/requirements_dev.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       38 2023-07-05 01:00:13.066034 smart_chromadb-0.1.dev733/setup.cfg
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.063993 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/
--rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-07-05 01:00:12.000000 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)     5825 2023-07-05 01:00:12.000000 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/SOURCES.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-07-05 01:00:12.000000 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/dependency_links.txt
--rw-r--r--   0 johnyan    (501) staff       (20)      340 2023-07-05 01:00:12.000000 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/requires.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        9 2023-07-05 01:00:12.000000 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/top_level.txt
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.251569 smart_chromadb-0.1.dev734/
+-rw-r--r--   0 johnyan    (501) staff       (20)       84 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.dockerignore
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:26.980359 smart_chromadb-0.1.dev734/.github/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.015400 smart_chromadb-0.1.dev734/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1512 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1520 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1384 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.020902 smart_chromadb-0.1.dev734/.github/workflows/
+-rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1338 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     4169 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.github/workflows/chroma-release.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.github/workflows/chroma-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1734 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)      228 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.gitignore
+-rw-r--r--   0 johnyan    (501) staff       (20)     1167 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.pre-commit-config.yaml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.021925 smart_chromadb-0.1.dev734/.vscode/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1020 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/.vscode/settings.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     3323 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/DEVELOP.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      647 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/Dockerfile
+-rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/LICENSE
+-rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-07-06 08:26:27.250231 smart_chromadb-0.1.dev734/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)     5679 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      619 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/RELEASE_PROCESS.md
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.036116 smart_chromadb-0.1.dev734/bin/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1610 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/backup.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/build
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/docker_entrypoint.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)     6462 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/generate_cloudformation.py
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      463 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/integration-test
+-rw-r--r--   0 johnyan    (501) staff       (20)     1688 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/restore.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)     1105 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/setup_linux.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/setup_mac.sh
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.038662 smart_chromadb-0.1.dev734/bin/templates/
+-rw-r--r--   0 johnyan    (501) staff       (20)      985 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/test-package.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      297 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/test-remote
+-rw-r--r--   0 johnyan    (501) staff       (20)      205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/test.py
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      151 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/bin/version
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.046431 smart_chromadb-0.1.dev734/chromadb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      894 2023-07-04 08:34:52.000000 smart_chromadb-0.1.dev734/chromadb/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.051313 smart_chromadb-0.1.dev734/chromadb/api/
+-rw-r--r--   0 johnyan    (501) staff       (20)    10943 2023-07-06 08:22:49.000000 smart_chromadb-0.1.dev734/chromadb/api/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12480 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/api/fastapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    17917 2023-07-06 08:23:48.000000 smart_chromadb-0.1.dev734/chromadb/api/local.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.052617 smart_chromadb-0.1.dev734/chromadb/api/models/
+-rw-r--r--   0 johnyan    (501) staff       (20)    15101 2023-07-06 06:54:49.000000 smart_chromadb-0.1.dev734/chromadb/api/models/Collection.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1306 2023-07-06 08:24:24.000000 smart_chromadb-0.1.dev734/chromadb/api/smartapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11283 2023-07-03 09:25:09.000000 smart_chromadb-0.1.dev734/chromadb/api/types.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/app.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7231 2023-07-03 08:16:05.000000 smart_chromadb-0.1.dev734/chromadb/config.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.062858 smart_chromadb-0.1.dev734/chromadb/db/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3405 2023-07-06 07:09:27.000000 smart_chromadb-0.1.dev734/chromadb/db/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6004 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/db/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    22374 2023-07-06 00:55:55.000000 smart_chromadb-0.1.dev734/chromadb/db/clickhouse.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18862 2023-07-06 00:55:55.000000 smart_chromadb-0.1.dev734/chromadb/db/duckdb.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.064100 smart_chromadb-0.1.dev734/chromadb/db/impl/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/db/impl/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/db/impl/sqlite.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.065585 smart_chromadb-0.1.dev734/chromadb/db/index/
+-rw-r--r--   0 johnyan    (501) staff       (20)      447 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/db/index/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11053 2023-07-06 07:28:41.000000 smart_chromadb-0.1.dev734/chromadb/db/index/hnswlib.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8096 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/db/migrations.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.066598 smart_chromadb-0.1.dev734/chromadb/db/mixins/
+-rw-r--r--   0 johnyan    (501) staff       (20)     9193 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15557 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    17753 2023-07-06 06:46:45.000000 smart_chromadb-0.1.dev734/chromadb/db/smartdb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2656 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/db/system.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1293 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/errors.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.067247 smart_chromadb-0.1.dev734/chromadb/ingest/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3643 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/ingest/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.068229 smart_chromadb-0.1.dev734/chromadb/segment/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3059 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/segment/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:26.983298 smart_chromadb-0.1.dev734/chromadb/segment/impl/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.068846 smart_chromadb-0.1.dev734/chromadb/segment/impl/manager/
+-rw-r--r--   0 johnyan    (501) staff       (20)     4358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.069686 smart_chromadb-0.1.dev734/chromadb/segment/impl/metadata/
+-rw-r--r--   0 johnyan    (501) staff       (20)    17879 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.071093 smart_chromadb-0.1.dev734/chromadb/segment/impl/vector/
+-rw-r--r--   0 johnyan    (501) staff       (20)    11965 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/segment/impl/vector/local_hnsw.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.072120 smart_chromadb-0.1.dev734/chromadb/server/
+-rw-r--r--   0 johnyan    (501) staff       (20)      172 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/server/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.074020 smart_chromadb-0.1.dev734/chromadb/server/fastapi/
+-rw-r--r--   0 johnyan    (501) staff       (20)     9064 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2134 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.077280 smart_chromadb-0.1.dev734/chromadb/telemetry/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3214 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/telemetry/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      591 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/telemetry/events.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.091978 smart_chromadb-0.1.dev734/chromadb/test/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3993 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/conftest.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.103398 smart_chromadb-0.1.dev734/chromadb/test/db/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.121081 smart_chromadb-0.1.dev734/chromadb/test/db/migrations/
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)     1168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/db/test_base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9773 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/db/test_system.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.122178 smart_chromadb-0.1.dev734/chromadb/test/hnswlib/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2337 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/hnswlib/test_hnswlib.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.125671 smart_chromadb-0.1.dev734/chromadb/test/ingest/
+-rw-r--r--   0 johnyan    (501) staff       (20)     8117 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.145287 smart_chromadb-0.1.dev734/chromadb/test/property/
+-rw-r--r--   0 johnyan    (501) staff       (20)    11294 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/property/invariants.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18662 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/property/strategies.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2213 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/property/test_add.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6211 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/property/test_collections.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9123 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11073 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9062 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5146 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.148288 smart_chromadb-0.1.dev734/chromadb/test/segment/
+-rw-r--r--   0 johnyan    (501) staff       (20)    15026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12132 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/segment/test_vector.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    40340 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/test_api.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/test_chroma.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4127 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/test_config.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.150221 smart_chromadb-0.1.dev734/chromadb/test/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3544 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3702 2023-06-30 03:21:44.000000 smart_chromadb-0.1.dev734/chromadb/types.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.155197 smart_chromadb-0.1.dev734/chromadb/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/utils/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    16311 2023-06-30 06:12:24.000000 smart_chromadb-0.1.dev734/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2301 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/chromadb/utils/messageid.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:26.988387 smart_chromadb-0.1.dev734/clients/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.175699 smart_chromadb-0.1.dev734/clients/js/
+-rw-r--r--   0 johnyan    (501) staff       (20)       66 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/.gitignore
+-rw-r--r--   0 johnyan    (501) staff       (20)       32 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/.prettierignore
+-rw-r--r--   0 johnyan    (501) staff       (20)        3 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/.prettierrc.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     1256 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/DEVELOP.md
+-rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/LICENSE
+-rw-r--r--   0 johnyan    (501) staff       (20)     1266 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      324 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/config.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:26.986698 smart_chromadb-0.1.dev734/clients/js/examples/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.183740 smart_chromadb-0.1.dev734/clients/js/examples/browser/
+-rw-r--r--   0 johnyan    (501) staff       (20)      358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/examples/browser/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1787 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/examples/browser/app.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      834 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/examples/browser/index.html
+-rw-r--r--   0 johnyan    (501) staff       (20)      409 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/examples/browser/package.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    71072 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.189769 smart_chromadb-0.1.dev734/clients/js/examples/node/
+-rw-r--r--   0 johnyan    (501) staff       (20)       57 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/examples/node/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1191 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/examples/node/app.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    46542 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/examples/node/package-lock.json
+-rw-r--r--   0 johnyan    (501) staff       (20)      503 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/examples/node/package.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    17116 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     1075 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/genapi.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      469 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/jest.config.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      153 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/openapitools.json
+-rw-r--r--   0 johnyan    (501) staff       (20)   450648 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/package-lock.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/package.json
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.199801 smart_chromadb-0.1.dev734/clients/js/src/
+-rw-r--r--   0 johnyan    (501) staff       (20)     8171 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)    19403 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/Collection.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.205356 smart_chromadb-0.1.dev734/clients/js/src/embeddings/
+-rw-r--r--   0 johnyan    (501) staff       (20)      938 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)       92 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1563 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     3402 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.210589 smart_chromadb-0.1.dev734/clients/js/src/generated/
+-rw-r--r--   0 johnyan    (501) staff       (20)      921 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/generated/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)    56700 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/generated/api.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1478 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      429 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/generated/index.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     5862 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/generated/models.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1307 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      490 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/index.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1715 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/types.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2002 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/src/utils.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.222593 smart_chromadb-0.1.dev734/clients/js/test/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2625 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     7586 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/client.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     3284 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2551 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/data.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2599 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      206 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/initClient.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      577 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1990 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2160 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      802 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      367 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/tsconfig.json
+-rw-r--r--   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/tsconfig.module.json
+-rw-r--r--   0 johnyan    (501) staff       (20)   157735 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/js/yarn.lock
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.228715 smart_chromadb-0.1.dev734/clients/python/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1627 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/python/README.md
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     1257 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      826 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/python/integration-test.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)       22 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/python/is_thin_client.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1166 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/clients/python/pyproject.toml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.230682 smart_chromadb-0.1.dev734/config/
+-rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/config/backup_disk.xml
+-rw-r--r--   0 johnyan    (501) staff       (20)      233 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/config/chroma_users.xml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1080 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/docker-compose.server.example.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/docker-compose.test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1226 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/docker-compose.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.233496 smart_chromadb-0.1.dev734/examples/
+-rw-r--r--   0 johnyan    (501) staff       (20)    10346 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/examples/alternative_embeddings.ipynb
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:26.989672 smart_chromadb-0.1.dev734/examples/deployments/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.241591 smart_chromadb-0.1.dev734/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 johnyan    (501) staff       (20)      611 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      752 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)      125 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)     2271 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      181 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/examples/deployments/google-cloud-compute/variables.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)     5830 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/examples/local_persistence.ipynb
+-rw-r--r--   0 johnyan    (501) staff       (20)     5493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/examples/where_filtering.ipynb
+-rw-r--r--   0 johnyan    (501) staff       (20)      495 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/log_config.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:26.992177 smart_chromadb-0.1.dev734/migrations/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.242599 smart_chromadb-0.1.dev734/migrations/embeddings_queue/
+-rw-r--r--   0 johnyan    (501) staff       (20)      261 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.243425 smart_chromadb-0.1.dev734/migrations/metadb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      620 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/migrations/metadb/00001-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.245161 smart_chromadb-0.1.dev734/migrations/sysdb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      336 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)      372 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/pull_request_template.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-26 07:09:55.000000 smart_chromadb-0.1.dev734/pyproject.toml
+-rw-r--r--   0 johnyan    (501) staff       (20)      352 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/requirements.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)      161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev734/requirements_dev.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       38 2023-07-06 08:26:27.251769 smart_chromadb-0.1.dev734/setup.cfg
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-06 08:26:27.248905 smart_chromadb-0.1.dev734/smart_chromadb.egg-info/
+-rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-07-06 08:26:26.000000 smart_chromadb-0.1.dev734/smart_chromadb.egg-info/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)     5825 2023-07-06 08:26:26.000000 smart_chromadb-0.1.dev734/smart_chromadb.egg-info/SOURCES.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-07-06 08:26:26.000000 smart_chromadb-0.1.dev734/smart_chromadb.egg-info/dependency_links.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)      340 2023-07-06 08:26:26.000000 smart_chromadb-0.1.dev734/smart_chromadb.egg-info/requires.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        9 2023-07-06 08:26:26.000000 smart_chromadb-0.1.dev734/smart_chromadb.egg-info/top_level.txt
```

### Comparing `smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/bug_report.yaml` & `smart_chromadb-0.1.dev734/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/feature_request.yaml` & `smart_chromadb-0.1.dev734/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `smart_chromadb-0.1.dev734/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/.github/workflows/chroma-client-integration-test.yml` & `smart_chromadb-0.1.dev734/.github/workflows/chroma-client-integration-test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/.github/workflows/chroma-integration-test.yml` & `smart_chromadb-0.1.dev734/.github/workflows/chroma-integration-test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/.github/workflows/chroma-release-python-client.yml` & `smart_chromadb-0.1.dev734/.github/workflows/chroma-release-python-client.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/.github/workflows/chroma-release.yml` & `smart_chromadb-0.1.dev734/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/.github/workflows/chroma-test.yml` & `smart_chromadb-0.1.dev734/.github/workflows/chroma-test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/.github/workflows/pr-review-checklist.yml` & `smart_chromadb-0.1.dev734/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/.pre-commit-config.yaml` & `smart_chromadb-0.1.dev734/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/.vscode/settings.json` & `smart_chromadb-0.1.dev734/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/DEVELOP.md` & `smart_chromadb-0.1.dev734/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/Dockerfile` & `smart_chromadb-0.1.dev734/Dockerfile`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/LICENSE` & `smart_chromadb-0.1.dev734/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/PKG-INFO` & `smart_chromadb-0.1.dev734/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_chromadb
-Version: 0.1.dev733
+Version: 0.1.dev734
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smart_chromadb Version: 0.1.dev733 Summary: Chroma.
+Metadata-Version: 2.1 Name: smart_chromadb Version: 0.1.dev734 Summary: Chroma.
 Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `smart_chromadb-0.1.dev733/README.md` & `smart_chromadb-0.1.dev734/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/RELEASE_PROCESS.md` & `smart_chromadb-0.1.dev734/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/bin/backup.sh` & `smart_chromadb-0.1.dev734/bin/backup.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/bin/generate_cloudformation.py` & `smart_chromadb-0.1.dev734/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/bin/restore.sh` & `smart_chromadb-0.1.dev734/bin/restore.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/bin/setup_linux.sh` & `smart_chromadb-0.1.dev734/bin/setup_linux.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/bin/templates/docker-compose.yml` & `smart_chromadb-0.1.dev734/bin/templates/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/__init__.py` & `smart_chromadb-0.1.dev734/chromadb/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/api/__init__.py` & `smart_chromadb-0.1.dev734/chromadb/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,31 +102,33 @@
         """
         pass
 
     @abstractmethod
     def get_collection(
         self,
         name: str,
+        id: str = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
         """Gets a collection from the database by either name or uuid
 
         Args:
             name: The name of the collection to get. Defaults to None.
+            id: collection id
             embedding_function: A function that takes documents and returns an embedding. Should be the same as the one used to create the collection. Defaults to None.
 
         Returns:
             dict: the requested collection
 
         """
         pass
 
     def _modify(
         self,
-        id: UUID,
+        id: str,
         new_name: Optional[str] = None,
         new_metadata: Optional[CollectionMetadata] = None,
     ) -> None:
         """Modify a collection in the database - can update the name and/or metadata
 
         Args:
             current_name: The name of the collection to modify
@@ -135,15 +137,15 @@
         """
         pass
 
     @abstractmethod
     def _add(
         self,
         ids: IDs,
-        collection_id: UUID,
+        collection_id: str,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
         """Add embeddings to the data store. This is the most general way to add embeddings to the database.
         ⚠️ It is recommended to use the more specific methods below when possible.
@@ -156,15 +158,15 @@
             ids: The ids to associate with the embeddings. Defaults to None.
         """
         pass
 
     @abstractmethod
     def _update(
         self,
-        collection_id: UUID,
+        collection_id: str,
         ids: IDs,
         embeddings: Optional[Embeddings] = None,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
     ) -> bool:
         """Add embeddings to the data store. This is the most general way to add embeddings to the database.
         ⚠️ It is recommended to use the more specific methods below when possible.
@@ -174,15 +176,15 @@
             embedding: The sequence of embeddings to add
         """
         pass
 
     @abstractmethod
     def _upsert(
         self,
-        collection_id: UUID,
+        collection_id: str,
         ids: IDs,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
         """Add or update entries in the embedding store.
@@ -195,35 +197,35 @@
             metadatas: The metadata to associate with the embeddings. Defaults to None.
             documents: The documents to associate with the embeddings. Defaults to None.
             increment_index: If True, will incrementally add to the ANN index of the collection. Defaults to True.
         """
         pass
 
     @abstractmethod
-    def _count(self, collection_id: UUID) -> int:
+    def _count(self, collection_id: str) -> int:
         """Returns the number of embeddings in the database
 
         Args:
             collection_id: The collection to count the embeddings in.
 
 
         Returns:
             int: The number of embeddings in the collection
 
         """
         pass
 
     @abstractmethod
-    def _peek(self, collection_id: UUID, n: int = 10) -> GetResult:
+    def _peek(self, collection_id: str, n: int = 10) -> GetResult:
         pass
 
     @abstractmethod
     def _get(
         self,
-        collection_id: UUID,
+        collection_id: str,
         ids: Optional[IDs] = None,
         where: Optional[Where] = {},
         sort: Optional[str] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
@@ -246,15 +248,15 @@
 
         """
         pass
 
     @abstractmethod
     def _delete(
         self,
-        collection_id: UUID,
+        collection_id: str,
         ids: Optional[IDs],
         where: Optional[Where] = {},
         where_document: Optional[WhereDocument] = {},
     ) -> IDs:
         """Deletes embeddings from the database
         ⚠️ This method should not be used directly.
 
@@ -265,15 +267,15 @@
             List: The list of internal UUIDs of the deleted embeddings
         """
         pass
 
     @abstractmethod
     def _query(
         self,
-        collection_id: UUID,
+        collection_id: str,
         query_embeddings: Embeddings,
         n_results: int = 10,
         where: Where = {},
         where_document: WhereDocument = {},
         include: Include = ["embeddings", "metadatas", "documents", "distances"],
     ) -> QueryResult:
         """Gets the nearest neighbors of a single embedding
```

### Comparing `smart_chromadb-0.1.dev733/chromadb/api/fastapi.py` & `smart_chromadb-0.1.dev734/chromadb/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/api/local.py` & `smart_chromadb-0.1.dev734/chromadb/api/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,34 +142,36 @@
             name, metadata, embedding_function, get_or_create=True
         )
 
     @override
     def get_collection(
         self,
         name: str,
+        id: str = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
         """Get a collection with the given name.
         Args:
             name: The name of the collection to get
+            id: the name of the collection
             embedding_function: Optional function to use to embed documents
 
         Returns:
             The collection
 
         Raises:
             ValueError: If the collection does not exist
 
         Examples:
             ```python
             client.get_collection("my_collection")
             # collection(name="my_collection", metadata={})
             ```
         """
-        res = self._db.get_collection(name)
+        res = self._db.get_collection(name, id=id)
         if len(res) == 0:
             raise ValueError(f"Collection {name} does not exist")
         return Collection(
             client=self,
             name=name,
             id=res[0][0],
             embedding_function=embedding_function,
@@ -200,15 +202,15 @@
                 )
             )
         return collections
 
     @override
     def _modify(
         self,
-        id: UUID,
+        id: str,
         new_name: Optional[str] = None,
         new_metadata: Optional[CollectionMetadata] = None,
     ) -> None:
         if new_name is not None:
             check_index_name(new_name)
 
         self._db.update_collection(id, new_name, new_metadata)
@@ -232,15 +234,15 @@
     #
     # ITEM METHODS
     #
     @override
     def _add(
         self,
         ids: IDs,
-        collection_id: UUID,
+        collection_id: str,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
         existing_ids = self._get(collection_id, ids=ids, include=[])["ids"]
         if len(existing_ids) > 0:
@@ -261,27 +263,27 @@
 
         self._telemetry_client.capture(CollectionAddEvent(str(collection_id), len(ids)))
         return True  # NIT: should this return the ids of the succesfully added items?
 
     @override
     def _update(
         self,
-        collection_id: UUID,
+        collection_id: str,
         ids: IDs,
         embeddings: Optional[Embeddings] = None,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
     ) -> bool:
         self._db.update(collection_id, ids, embeddings, metadatas, documents)
         return True
 
     @override
     def _upsert(
         self,
-        collection_id: UUID,
+        collection_id: str,
         ids: IDs,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
         # Determine which ids need to be added and which need to be updated based on the ids already in the collection
@@ -335,15 +337,15 @@
         self._db.update(collection_id, ids, embeddings, metadatas, documents)
 
         return True
 
     @override
     def _get(
         self,
-        collection_id: UUID,
+        collection_id: str,
         ids: Optional[IDs] = None,
         where: Optional[Where] = {},
         sort: Optional[str] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
@@ -403,15 +405,15 @@
                 )
             get_result["ids"].append(entry[column_index["id"]])
         return get_result
 
     @override
     def _delete(
         self,
-        collection_id: UUID,
+        collection_id: str,
         ids: Optional[IDs] = None,
         where: Optional[Where] = None,
         where_document: Optional[WhereDocument] = None,
     ) -> IDs:
         if where is None:
             where = {}
 
@@ -427,15 +429,15 @@
         self._telemetry_client.capture(
             CollectionDeleteEvent(str(collection_id), len(deleted_uuids))
         )
 
         return deleted_uuids
 
     @override
-    def _count(self, collection_id: UUID) -> int:
+    def _count(self, collection_id: str) -> int:
         return self._db.count(collection_id)
 
     @override
     def reset(self) -> None:
         """Reset the database. This will delete all collections and items.
 
         Returns:
@@ -443,15 +445,15 @@
 
         """
         self._db.reset()
 
     @override
     def _query(
         self,
-        collection_id: UUID,
+        collection_id: str,
         query_embeddings: Embeddings,
         n_results: int = 10,
         where: Where = {},
         where_document: WhereDocument = {},
         include: Include = ["documents", "metadatas", "distances"],
     ) -> QueryResult:
         uuids, distances = self._db.get_nearest_neighbors(
@@ -522,15 +524,15 @@
     @override
     def create_index(self, collection_name: str) -> bool:
         collection_uuid = self._db.get_collection_uuid_from_name(collection_name)
         self._db.create_index(collection_uuid=collection_uuid)
         return True
 
     @override
-    def _peek(self, collection_id: UUID, n: int = 10) -> GetResult:
+    def _peek(self, collection_id: str, n: int = 10) -> GetResult:
         return self._get(
             collection_id=collection_id,
             limit=n,
             include=["embeddings", "documents", "metadatas"],
         )
 
     @override
```

### Comparing `smart_chromadb-0.1.dev733/chromadb/api/models/Collection.py` & `smart_chromadb-0.1.dev734/chromadb/api/models/Collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,24 +32,24 @@
 
 if TYPE_CHECKING:
     from chromadb.api import API
 
 
 class Collection(BaseModel):
     name: str
-    id: UUID
+    id: str
     metadata: Optional[CollectionMetadata] = None
     _client: "API" = PrivateAttr()
     _embedding_function: Optional[EmbeddingFunction] = PrivateAttr()
 
     def __init__(
         self,
         client: "API",
         name: str,
-        id: UUID,
+        id: str,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
         metadata: Optional[CollectionMetadata] = None,
     ):
         self._client = client
         self._embedding_function = embedding_function
         super().__init__(name=name, metadata=metadata, id=id)
```

### Comparing `smart_chromadb-0.1.dev733/chromadb/api/smartapi.py` & `smart_chromadb-0.1.dev734/chromadb/api/smartapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,24 +10,43 @@
 from chromadb.api.local import LocalAPI
 
 
 class SmartAPI(LocalAPI):
 
     @override
     def _query(
-        self,
-        collection_id: UUID,
-        query_embeddings: Embeddings,
-        n_results: int = 10,
-        where: Where = {},
-        where_document: WhereDocument = {},
-        include: Include = ["documents", "metadatas", "distances"],
+            self,
+            collection_id: str,
+            query_embeddings: Embeddings,
+            n_results: int = 10,
+            where: Where = {},
+            where_document: WhereDocument = {},
+            include: Include = ["documents", "metadatas", "distances"],
     ) -> QueryResult:
         query_result = self._db.get_nearest_neighbors_smart(
             collection_uuid=collection_id,
             where=where,
             where_document=where_document,
             embeddings=query_embeddings,
             n_results=n_results,
         )
 
         return query_result
+
+    @override
+    def _add(
+            self,
+            ids,
+            collection_id: str,
+            embeddings: Embeddings,
+            metadatas=None,
+            documents=None,
+            increment_index: bool = True,
+    ) -> bool:
+        added_uuids = self._db.add(
+            collection_id,
+            embeddings=embeddings,
+            metadatas=metadatas,
+            documents=documents,
+            ids=ids,
+        )
+        return True
```

### Comparing `smart_chromadb-0.1.dev733/chromadb/api/types.py` & `smart_chromadb-0.1.dev734/chromadb/api/types.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/config.py` & `smart_chromadb-0.1.dev734/chromadb/config.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/__init__.py` & `smart_chromadb-0.1.dev734/chromadb/db/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         name: str,
         metadata: Optional[Metadata] = None,
         get_or_create: bool = False,
     ) -> Sequence:  # type: ignore
         pass
 
     @abstractmethod
-    def get_collection(self, name: str) -> Sequence:  # type: ignore
+    def get_collection(self, name: str, id: str = None) -> Sequence:  # type: ignore
         pass
 
     @abstractmethod
     def list_collections(self) -> Sequence:  # type: ignore
         pass
 
     @abstractmethod
@@ -49,15 +49,15 @@
     @abstractmethod
     def get_collection_uuid_from_name(self, collection_name: str) -> UUID:
         pass
 
     @abstractmethod
     def add(
         self,
-        collection_uuid: UUID,
+        collection_uuid: str,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas],
         documents: Optional[Documents],
         ids: List[str],
     ) -> List[UUID]:
         pass
```

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/base.py` & `smart_chromadb-0.1.dev734/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/clickhouse.py` & `smart_chromadb-0.1.dev734/chromadb/db/clickhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,17 @@
 
         self._get_conn().insert(
             "collections", data_to_insert, column_names=["uuid", "name", "metadata"]
         )
         return [[collection_uuid, name, metadata]]
 
     @override
-    def get_collection(self, name: str) -> Sequence:
+    def get_collection(self, name: str, id: str = None) -> Sequence:
+        if id:
+            return [[id, name, {}]]
         res = (
             self._get_conn()
             .query(
                 f"""
          SELECT * FROM collections WHERE name = '{name}'
          """
             )
```

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/duckdb.py` & `smart_chromadb-0.1.dev734/chromadb/db/duckdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,17 @@
         self._conn.execute(
             """INSERT INTO collections (uuid, name, metadata) VALUES (?, ?, ?)""",
             [str(collection_uuid), name, json.dumps(metadata)],
         )
         return [[str(collection_uuid), name, metadata]]
 
     @override
-    def get_collection(self, name: str) -> Sequence:
+    def get_collection(self, name: str, id: str = None) -> Sequence:
+        if id:
+            return [[id, name, {}]]
         res = self._conn.execute(
             """SELECT * FROM collections WHERE name = ?""", [name]
         ).fetchall()
         # json.loads the metadata
         return [[x[0], x[1], json.loads(x[2])] for x in res]
 
     @override
```

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/impl/sqlite.py` & `smart_chromadb-0.1.dev734/chromadb/db/impl/sqlite.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/index/hnswlib.py` & `smart_chromadb-0.1.dev734/chromadb/db/index/hnswlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,32 +59,32 @@
         self.M = int(metadata.get("hnsw:M", 16))
         self.num_threads = int(
             metadata.get("hnsw:num_threads", multiprocessing.cpu_count())
         )
         self.resize_factor = float(metadata.get("hnsw:resize_factor", 1.2))
 
 
-def hexid(id: Union[str, UUID]) -> str:
+def hexid(id: Union[str, str]) -> str:
     """Backwards compatibility for old indexes which called uuid.hex on UUID ids"""
-    return id.hex if isinstance(id, UUID) else id
+    return id.hex if isinstance(id, str) else id
 
 
 def delete_all_indexes(settings: Settings) -> None:
     if os.path.exists(f"{settings.persist_directory}/index"):
         for file in os.listdir(f"{settings.persist_directory}/index"):
             os.remove(f"{settings.persist_directory}/index/{file}")
 
 
 class Hnswlib(Index):
     _id: str
     _index: hnswlib.Index
     _index_metadata: IndexMetadata
     _params: HnswParams
     _id_to_label: Dict[str, int]
-    _label_to_id: Dict[int, UUID]
+    _label_to_id: Dict[int, str]
 
     def __init__(
         self,
         id: str,
         settings: Settings,
         metadata: Dict[str, str],
         number_elements: int,
@@ -128,15 +128,15 @@
         idx_dim = self._index.dim
         if dim != idx_dim:
             raise InvalidDimensionException(
                 f"Dimensionality of ({dim}) does not match index dimensionality ({idx_dim})"
             )
 
     def add(
-        self, ids: List[UUID], embeddings: Embeddings, update: bool = False
+        self, ids: List[str], embeddings: Embeddings, update: bool = False
     ) -> None:
         """Add or update embeddings to the index"""
 
         dim = len(embeddings[0])
 
         if self._index is None:
             self._init_index(dim)
@@ -188,15 +188,15 @@
             pass
 
         self._index = None
         self._collection_uuid = None
         self._id_to_label = {}
         self._label_to_id = {}
 
-    def delete_from_index(self, ids: List[UUID]) -> None:
+    def delete_from_index(self, ids: List[str]) -> None:
         if self._index is not None:
             for id in ids:
                 label = self._id_to_label[hexid(id)]
                 self._index.mark_deleted(label)
                 del self._label_to_id[label]
                 del self._id_to_label[hexid(id)]
                 self._index_metadata["curr_elements"] -= 1
@@ -255,16 +255,16 @@
                 max(curr_elements * self._params.resize_factor, DEFAULT_CAPACITY)
             ),
         )
         self._index.set_ef(self._params.search_ef)
         self._index.set_num_threads(self._params.num_threads)
 
     def get_nearest_neighbors(
-        self, query: Embeddings, k: int, ids: Optional[List[UUID]] = None
-    ) -> Tuple[List[List[UUID]], List[List[float]]]:
+        self, query: Embeddings, k: int, ids: Optional[List[str]] = None
+    ) -> Tuple[List[List[str]], List[List[float]]]:
         # The only case where the index is none is if no elements have been added
         # We don't save the index until at least one element has been added
         # And so there is also nothing at load time for persisted indexes
         # In the case where no elements have been added, we return empty
         if self._index is None:
             return [[] for _ in range(len(query))], [[] for _ in range(len(query))]
```

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/migrations.py` & `smart_chromadb-0.1.dev734/chromadb/db/migrations.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/mixins/embeddings_queue.py` & `smart_chromadb-0.1.dev734/chromadb/db/mixins/embeddings_queue.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/mixins/sysdb.py` & `smart_chromadb-0.1.dev734/chromadb/db/mixins/sysdb.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/smartdb.py` & `smart_chromadb-0.1.dev734/chromadb/db/smartdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import json
 import uuid
 import logging
 from uuid import UUID
 from overrides import override
 from chromadb.api.types import Metadata
 from smart_chart.common.connect_db import DB_conn
+import requests
 
 logger = logging.getLogger(__name__)
 
 
 class StarRocksDB(Clickhouse):
     _conn: object
 
@@ -39,17 +40,37 @@
 
 
     def _execute_sql(self, sql):
         return self._conn.execute_sql_list([sql], self._connect_dict)
 
     def _execute_load(self, contents, table):
         if self._load_dict:
-            table = f"{self._connect_dict['db']}.{table}"
             contents[0][0] = '__' + contents[0][0]
-            self._conn.insert_contents(contents, table, 100, self._load_dict)
+            if self._load_dict['host'].startswith('http'):
+                url = self._load_dict['host'] + '/etl/api/upload_file_api/'
+                data = {"type": table,
+                        "filename": table,
+                        "token": self._load_dict['password'],
+                        "visitor": self._load_dict['user'],
+                        "contents": json.dumps(contents)
+                        }
+                # 上传,https可能需要参数 verify=False
+                response = requests.post(url, data=data)
+                if response.status_code == 200:
+                    response = response.json()
+                elif response.status_code == 504:
+                    response = {"result": "timeout", "data": "Pls wait for mail"}
+                else:
+                    response = {"result": "error", "data": "some thing wrong"}
+
+                if response['result'] == 'error':
+                    raise Exception(response['data'])
+            else:
+                table = f"{self._connect_dict['db']}.{table}"
+                self._conn.insert_contents(contents, table, 100, self._load_dict)
         else:
             table = f"{table}({','.join(contents[0])})"
             contents = contents[1:]
             self._conn.insert_contents_mysql(contents, table, 100, self._connect_dict)
 
     @override
     def _create_table_collections(self, conn):
@@ -100,15 +121,17 @@
 
         collection_uuid = uuid.uuid4()
         sql = f"""INSERT INTO collections (uuid, name, metadata) VALUES ('{collection_uuid}','{name}','{json.dumps(metadata)}')"""
         self._execute_sql(sql)
         return [[str(collection_uuid), name, metadata]]
 
     @override
-    def get_collection(self, name: str) -> Sequence:
+    def get_collection(self, name: str, id: str = None) -> Sequence:
+        if id:
+            return [[id, name, {}]]
         sql = f"""SELECT * FROM collections WHERE name = '{name}'"""
         res = self._execute_sql(sql)[1:]
         # json.loads the metadata
         return [[x[0], x[1], json.loads(x[2])] for x in res]
 
     @override
     def get_collection_by_id(self, collection_uuid: str):
@@ -156,17 +179,17 @@
     @override
     def add(self, collection_uuid, embeddings, metadatas, documents, ids) -> List[UUID]:
         data_to_insert = [
             [
                 str(collection_uuid),
                 str(uuid.uuid4()),
                 str(embedding),
-                json.dumps(metadatas[i]) if metadatas else '',
-                documents[i] if documents else '',
-                ids[i],
+                json.dumps(metadatas[i]).replace('\t', ' ') if metadatas else '',
+                documents[i].replace('\t', ' ') if documents else '',
+                str(ids[i]),
             ]
             for i, embedding in enumerate(embeddings)
         ]
 
         insert_string = "collection_uuid, uuid, embedding, metadata, document, id"
         data_to_insert = [insert_string.split(',')] + data_to_insert
         self._execute_load(data_to_insert, 'embeddings')
```

### Comparing `smart_chromadb-0.1.dev733/chromadb/db/system.py` & `smart_chromadb-0.1.dev734/chromadb/db/system.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/errors.py` & `smart_chromadb-0.1.dev734/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/ingest/__init__.py` & `smart_chromadb-0.1.dev734/chromadb/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/segment/__init__.py` & `smart_chromadb-0.1.dev734/chromadb/segment/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/segment/impl/manager/local.py` & `smart_chromadb-0.1.dev734/chromadb/segment/impl/manager/local.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/segment/impl/metadata/sqlite.py` & `smart_chromadb-0.1.dev734/chromadb/segment/impl/metadata/sqlite.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/segment/impl/vector/local_hnsw.py` & `smart_chromadb-0.1.dev734/chromadb/segment/impl/vector/local_hnsw.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/server/fastapi/__init__.py` & `smart_chromadb-0.1.dev734/chromadb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/server/fastapi/types.py` & `smart_chromadb-0.1.dev734/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/telemetry/__init__.py` & `smart_chromadb-0.1.dev734/chromadb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/telemetry/events.py` & `smart_chromadb-0.1.dev734/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/telemetry/posthog.py` & `smart_chromadb-0.1.dev734/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/conftest.py` & `smart_chromadb-0.1.dev734/chromadb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/db/test_base.py` & `smart_chromadb-0.1.dev734/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/db/test_migrations.py` & `smart_chromadb-0.1.dev734/chromadb/test/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/db/test_system.py` & `smart_chromadb-0.1.dev734/chromadb/test/db/test_system.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/hnswlib/test_hnswlib.py` & `smart_chromadb-0.1.dev734/chromadb/test/hnswlib/test_hnswlib.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/ingest/test_producer_consumer.py` & `smart_chromadb-0.1.dev734/chromadb/test/ingest/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/property/invariants.py` & `smart_chromadb-0.1.dev734/chromadb/test/property/invariants.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/property/strategies.py` & `smart_chromadb-0.1.dev734/chromadb/test/property/strategies.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/property/test_add.py` & `smart_chromadb-0.1.dev734/chromadb/test/property/test_add.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/property/test_collections.py` & `smart_chromadb-0.1.dev734/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/property/test_cross_version_persist.py` & `smart_chromadb-0.1.dev734/chromadb/test/property/test_cross_version_persist.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/property/test_embeddings.py` & `smart_chromadb-0.1.dev734/chromadb/test/property/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/property/test_filtering.py` & `smart_chromadb-0.1.dev734/chromadb/test/property/test_filtering.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/property/test_persist.py` & `smart_chromadb-0.1.dev734/chromadb/test/property/test_persist.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/segment/test_metadata.py` & `smart_chromadb-0.1.dev734/chromadb/test/segment/test_metadata.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/segment/test_vector.py` & `smart_chromadb-0.1.dev734/chromadb/test/segment/test_vector.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/test_api.py` & `smart_chromadb-0.1.dev734/chromadb/test/test_api.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/test_chroma.py` & `smart_chromadb-0.1.dev734/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/test_config.py` & `smart_chromadb-0.1.dev734/chromadb/test/test_config.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/test/utils/test_messagid.py` & `smart_chromadb-0.1.dev734/chromadb/test/utils/test_messagid.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/types.py` & `smart_chromadb-0.1.dev734/chromadb/types.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/utils/embedding_functions.py` & `smart_chromadb-0.1.dev734/chromadb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/chromadb/utils/messageid.py` & `smart_chromadb-0.1.dev734/chromadb/utils/messageid.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/DEVELOP.md` & `smart_chromadb-0.1.dev734/clients/js/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/LICENSE` & `smart_chromadb-0.1.dev734/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/README.md` & `smart_chromadb-0.1.dev734/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/examples/browser/app.ts` & `smart_chromadb-0.1.dev734/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/examples/browser/index.html` & `smart_chromadb-0.1.dev734/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/examples/browser/yarn.lock` & `smart_chromadb-0.1.dev734/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/examples/node/app.js` & `smart_chromadb-0.1.dev734/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/examples/node/package-lock.json` & `smart_chromadb-0.1.dev734/clients/js/examples/node/package-lock.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/examples/node/yarn.lock` & `smart_chromadb-0.1.dev734/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/genapi.sh` & `smart_chromadb-0.1.dev734/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/package-lock.json` & `smart_chromadb-0.1.dev734/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/package.json` & `smart_chromadb-0.1.dev734/clients/js/package.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/ChromaClient.ts` & `smart_chromadb-0.1.dev734/clients/js/src/ChromaClient.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/Collection.ts` & `smart_chromadb-0.1.dev734/clients/js/src/Collection.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `smart_chromadb-0.1.dev734/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `smart_chromadb-0.1.dev734/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/embeddings/TransformersEmbeddingFunction.ts` & `smart_chromadb-0.1.dev734/clients/js/src/embeddings/TransformersEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/embeddings/WebAIEmbeddingFunction.ts` & `smart_chromadb-0.1.dev734/clients/js/src/embeddings/WebAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/generated/README.md` & `smart_chromadb-0.1.dev734/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/generated/api.ts` & `smart_chromadb-0.1.dev734/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/generated/configuration.ts` & `smart_chromadb-0.1.dev734/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/generated/models.ts` & `smart_chromadb-0.1.dev734/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/generated/runtime.ts` & `smart_chromadb-0.1.dev734/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/types.ts` & `smart_chromadb-0.1.dev734/clients/js/src/types.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/src/utils.ts` & `smart_chromadb-0.1.dev734/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/test/add.collections.test.ts` & `smart_chromadb-0.1.dev734/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/test/client.test.ts` & `smart_chromadb-0.1.dev734/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/test/collection.client.test.ts` & `smart_chromadb-0.1.dev734/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/test/collection.test.ts` & `smart_chromadb-0.1.dev734/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/test/delete.collection.test.ts` & `smart_chromadb-0.1.dev734/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/test/get.collection.test.ts` & `smart_chromadb-0.1.dev734/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/test/peek.collection.test.ts` & `smart_chromadb-0.1.dev734/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/test/query.collection.test.ts` & `smart_chromadb-0.1.dev734/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/test/update.collection.test.ts` & `smart_chromadb-0.1.dev734/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/test/upsert.collections.test.ts` & `smart_chromadb-0.1.dev734/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/js/yarn.lock` & `smart_chromadb-0.1.dev734/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/python/README.md` & `smart_chromadb-0.1.dev734/clients/python/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/python/build_python_thin_client.sh` & `smart_chromadb-0.1.dev734/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/python/integration-test.sh` & `smart_chromadb-0.1.dev734/clients/python/integration-test.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/clients/python/pyproject.toml` & `smart_chromadb-0.1.dev734/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/docker-compose.server.example.yml` & `smart_chromadb-0.1.dev734/docker-compose.server.example.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/docker-compose.test.yml` & `smart_chromadb-0.1.dev734/docker-compose.test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/docker-compose.yml` & `smart_chromadb-0.1.dev734/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/examples/alternative_embeddings.ipynb` & `smart_chromadb-0.1.dev734/examples/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/README.md` & `smart_chromadb-0.1.dev734/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/chroma.tf` & `smart_chromadb-0.1.dev734/examples/deployments/google-cloud-compute/chroma.tf`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/startup.sh` & `smart_chromadb-0.1.dev734/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/examples/local_persistence.ipynb` & `smart_chromadb-0.1.dev734/examples/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/examples/where_filtering.ipynb` & `smart_chromadb-0.1.dev734/examples/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/migrations/metadb/00001-embedding-metadata.sqlite.sql` & `smart_chromadb-0.1.dev734/migrations/metadb/00001-embedding-metadata.sqlite.sql`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/pyproject.toml` & `smart_chromadb-0.1.dev734/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev733/smart_chromadb.egg-info/PKG-INFO` & `smart_chromadb-0.1.dev734/smart_chromadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-chromadb
-Version: 0.1.dev733
+Version: 0.1.dev734
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smart-chromadb Version: 0.1.dev733 Summary: Chroma.
+Metadata-Version: 2.1 Name: smart-chromadb Version: 0.1.dev734 Summary: Chroma.
 Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `smart_chromadb-0.1.dev733/smart_chromadb.egg-info/SOURCES.txt` & `smart_chromadb-0.1.dev734/smart_chromadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

