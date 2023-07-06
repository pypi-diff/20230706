# Comparing `tmp/MindsDB-23.6.5.1.tar.gz` & `tmp/MindsDB-23.7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MindsDB-23.6.5.1.tar", last modified: Tue Jun 27 16:39:45 2023, max compression
+gzip compressed data, was "dist/MindsDB-23.7.1.0.tar", last modified: Thu Jul  6 13:43:00 2023, max compression
```

## Comparing `MindsDB-23.6.5.1.tar` & `MindsDB-23.7.1.0.tar`

### file list

```diff
@@ -1,1415 +1,1419 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/MindsDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25610 2023-06-27 16:39:44.000000 MindsDB-23.6.5.1/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    67789 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:39:44.000000 MindsDB-23.6.5.1/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-06-27 16:39:44.000000 MindsDB-23.6.5.1/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 16:39:44.000000 MindsDB-23.6.5.1/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25610 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/common/check_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/chatbots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/chatbots.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/namespaces/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    57116 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    68016 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/nlp/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/api/postgres/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autokeras_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autokeras_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/binance_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/binance_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/binance_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/binance_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/binance_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cohere_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cohere_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cohere_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cohere_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/cohere_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/eventstoredb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/file_handler/file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/flaml_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/flaml_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/flaml_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/flaml_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/flaml_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/github_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/github_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/github_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/github_handler/github_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/github_handler/github_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/github_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/github_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gitlab_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gitlab_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gitlab_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_fit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_fit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_fit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_fit_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hackernews_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hackernews_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hackernews_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/jira_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/langchain_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/langchain_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/langchain_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21902 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/langchain_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/langchain_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/llama_index_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/llama_index_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/llama_index_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/llama_index_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ludwig_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   164968 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/merlion_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/merlion_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mlflow_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png
--rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monkeylearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/monkeylearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29331 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/openai_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/openai_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/paypal_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/paypal_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/paypal_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/paypal_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/paypal_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/postgres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ray_serve_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/realtime_slack_chat_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/realtime_slack_chat_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/realtime_slack_chat_handler/realtime_slack_chat_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/realtime_slack_chat_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/reddit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/reddit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/reddit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/reddit_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/reddit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rocket_chat_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rockset_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rockset_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/shopify_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/shopify_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/shopify_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/shopify_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/shopify_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/solr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
--rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/error.png
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
--rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
--rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/stripe_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/stripe_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/stripe_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58244 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/stripe_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/stripe_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tpot_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/utilities/query_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/web_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/web_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/web_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39688 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/web_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/web_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/web_handler/web_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/question_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/writer_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_client/db_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_client/ml_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_client/ml_grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/handler_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/ml_exec_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/ml_handler_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/realtime_chat_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/libs/storage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/utilities/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/utilities/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/realtime_chat_handler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/realtime_chatbot_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/realtime_chatbot_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-27 16:39:29.000000 MindsDB-23.6.5.1/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22431 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10557 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/interfaces/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/interfaces/stream/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/stream/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/stream/base/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/interfaces/stream/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/hooks/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/log_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/mindsdb/utilities/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/requirements/requirements-grpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/requirements/requirements-telemetry.txt
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 16:39:45.000000 MindsDB-23.6.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-27 16:39:30.000000 MindsDB-23.6.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 13:42:47.000000 MindsDB-23.7.1.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25610 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    68060 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25610 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-07-06 13:42:47.000000 MindsDB-23.7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/common/check_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/chatbots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/chatbots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/namespaces/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57762 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68207 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/nlp/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/api/postgres/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autokeras_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autokeras_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cohere_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cohere_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cohere_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cohere_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/cohere_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/eventstoredb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/file_handler/file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/flaml_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/flaml_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/flaml_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/flaml_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/flaml_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gitlab_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gitlab_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gitlab_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_fit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_fit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_fit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_fit_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hackernews_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hackernews_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hackernews_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/jira_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21902 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/langchain_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/llama_index_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/llama_index_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/llama_index_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ludwig_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164968 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/merlion_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mlflow_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/create-database.png
+-rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monkeylearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/monkeylearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/openai_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/openai_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/paypal_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/paypal_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/paypal_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/paypal_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/paypal_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/postgres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/realtime_slack_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/reddit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/reddit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/reddit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/reddit_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/reddit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rocket_chat_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rockset_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/shopify_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/shopify_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/shopify_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/shopify_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/shopify_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/solr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
+-rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/stripe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/stripe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/stripe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58244 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/stripe_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/stripe_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tpot_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/utilities/query_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/utilities/query_utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/web_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/web_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/web_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39688 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/web_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/web_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/web_handler/web_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/question_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_client/db_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_client/ml_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_client/ml_grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/handler_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/learn_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/ml_exec_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/ml_handler_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/realtime_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/libs/storage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/utilities/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/realtime_chat_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/realtime_chatbot_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/realtime_chatbot_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23736 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21829 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16623 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/interfaces/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/interfaces/stream/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/stream/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/stream/base/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/interfaces/stream/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/hooks/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/requirements/requirements-grpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/requirements/requirements-telemetry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:43:00.000000 MindsDB-23.7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-06 13:42:48.000000 MindsDB-23.7.1.0/setup.py
```

### Comparing `MindsDB-23.6.5.1/MindsDB.egg-info/PKG-INFO` & `MindsDB-23.7.1.0/MindsDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.6.5.1
+Version: 23.7.1.0
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -200,132 +200,132 @@
         MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: telemetry
 Provides-Extra: grpc
+Provides-Extra: telemetry
 Provides-Extra: all_extras
-Provides-Extra: tdengine
-Provides-Extra: yugabyte
-Provides-Extra: opengauss
-Provides-Extra: merlion
-Provides-Extra: ignite
+Provides-Extra: informix
+Provides-Extra: slack
+Provides-Extra: google_search
+Provides-Extra: ingres
+Provides-Extra: teradata
+Provides-Extra: openai
+Provides-Extra: postgres
+Provides-Extra: databricks
+Provides-Extra: monkeylearn
+Provides-Extra: vitess
 Provides-Extra: lightwood
+Provides-Extra: autosklearn
 Provides-Extra: datastax
-Provides-Extra: informix
-Provides-Extra: huggingface_api
-Provides-Extra: scylla
-Provides-Extra: huggingface
+Provides-Extra: influxdb
+Provides-Extra: s3
+Provides-Extra: mediawiki
+Provides-Extra: nuo_jdbc
 Provides-Extra: access
-Provides-Extra: frappe
-Provides-Extra: teradata
-Provides-Extra: mlflow
-Provides-Extra: cockroach
-Provides-Extra: confluence
-Provides-Extra: elasticsearch
+Provides-Extra: shopify
+Provides-Extra: surrealdb
+Provides-Extra: derby
+Provides-Extra: databend
+Provides-Extra: sheets
+Provides-Extra: empress
+Provides-Extra: yugabyte
+Provides-Extra: huggingface
+Provides-Extra: binance
+Provides-Extra: db2
+Provides-Extra: solr
+Provides-Extra: opengauss
+Provides-Extra: mongodb
+Provides-Extra: ray_serve
+Provides-Extra: scylla
+Provides-Extra: merlion
+Provides-Extra: sendinblue
+Provides-Extra: mendeley
 Provides-Extra: mariadb
 Provides-Extra: cloud_sql
-Provides-Extra: empress
-Provides-Extra: cohere
-Provides-Extra: langchain
-Provides-Extra: mysql
-Provides-Extra: d0lt
-Provides-Extra: sheets
-Provides-Extra: druid
-Provides-Extra: phoenix
-Provides-Extra: planetscale
-Provides-Extra: paypal
-Provides-Extra: web
-Provides-Extra: mediawiki
-Provides-Extra: aurora
-Provides-Extra: realtime_slack_chat
-Provides-Extra: dremio
-Provides-Extra: tidb
-Provides-Extra: jira
+Provides-Extra: google_calendar
+Provides-Extra: firebird
+Provides-Extra: elasticsearch
+Provides-Extra: cassandra
+Provides-Extra: sqreamdb
 Provides-Extra: redshift
-Provides-Extra: rockset
-Provides-Extra: twitter
-Provides-Extra: bigquery
-Provides-Extra: google_content_shopping
+Provides-Extra: supabase
+Provides-Extra: planetscale
+Provides-Extra: strava
+Provides-Extra: sqlany
+Provides-Extra: huggingface_api
 Provides-Extra: neuralforecast
-Provides-Extra: edgelessdb
-Provides-Extra: db2
-Provides-Extra: cloud_spanner
-Provides-Extra: databend
-Provides-Extra: youtube
-Provides-Extra: postgres
-Provides-Extra: sendinblue
-Provides-Extra: ludwig
-Provides-Extra: tpot
-Provides-Extra: airtable
-Provides-Extra: clickhouse
-Provides-Extra: influxdb
-Provides-Extra: dynamodb
-Provides-Extra: nuo_jdbc
-Provides-Extra: pinot
-Provides-Extra: matrixone
-Provides-Extra: trino
-Provides-Extra: monkeylearn
 Provides-Extra: questdb
-Provides-Extra: vitess
-Provides-Extra: llama_index
-Provides-Extra: gmail
-Provides-Extra: openai
-Provides-Extra: cassandra
-Provides-Extra: materialize
-Provides-Extra: quickbooks
+Provides-Extra: mysql
+Provides-Extra: plaid
+Provides-Extra: newsapi
+Provides-Extra: altibase
+Provides-Extra: clickhouse
 Provides-Extra: impala
 Provides-Extra: singlestore
-Provides-Extra: google_search
+Provides-Extra: airtable
+Provides-Extra: oracle
+Provides-Extra: google_content_shopping
 Provides-Extra: duckdb
-Provides-Extra: solr
-Provides-Extra: mssql
-Provides-Extra: flaml
-Provides-Extra: github
-Provides-Extra: supabase
 Provides-Extra: statsforecast
-Provides-Extra: stripe
-Provides-Extra: ingres
-Provides-Extra: autosklearn
-Provides-Extra: hsqldb
-Provides-Extra: slack
-Provides-Extra: mendeley
-Provides-Extra: orioledb
-Provides-Extra: gitlab
-Provides-Extra: mongodb
+Provides-Extra: pinot
+Provides-Extra: google_books
+Provides-Extra: youtube
+Provides-Extra: bigquery
 Provides-Extra: vertica
-Provides-Extra: snowflake
-Provides-Extra: firebird
-Provides-Extra: strava
+Provides-Extra: mssql
 Provides-Extra: crate
-Provides-Extra: couchbase
-Provides-Extra: timescaledb
-Provides-Extra: binance
-Provides-Extra: maxdb
-Provides-Extra: s3
-Provides-Extra: shopify
-Provides-Extra: monetdb
-Provides-Extra: sqreamdb
-Provides-Extra: ckan
-Provides-Extra: writer
-Provides-Extra: ray_serve
-Provides-Extra: sqlany
-Provides-Extra: derby
-Provides-Extra: google_calendar
-Provides-Extra: hana
+Provides-Extra: langchain
+Provides-Extra: ignite
+Provides-Extra: cloud_spanner
+Provides-Extra: rockset
+Provides-Extra: realtime_slack_chat
 Provides-Extra: hive
-Provides-Extra: google_books
-Provides-Extra: surrealdb
+Provides-Extra: dynamodb
+Provides-Extra: timescaledb
+Provides-Extra: ludwig
 Provides-Extra: google_fit
+Provides-Extra: cockroach
+Provides-Extra: github
+Provides-Extra: mlflow
+Provides-Extra: flaml
+Provides-Extra: aurora
+Provides-Extra: quickbooks
+Provides-Extra: gitlab
+Provides-Extra: ckan
+Provides-Extra: d0lt
+Provides-Extra: cohere
+Provides-Extra: dremio
+Provides-Extra: stripe
+Provides-Extra: hsqldb
+Provides-Extra: monetdb
+Provides-Extra: frappe
+Provides-Extra: jira
 Provides-Extra: rocket_chat
-Provides-Extra: newsapi
+Provides-Extra: web
+Provides-Extra: materialize
 Provides-Extra: reddit
-Provides-Extra: plaid
-Provides-Extra: databricks
-Provides-Extra: altibase
-Provides-Extra: starrocks
-Provides-Extra: oracle
 Provides-Extra: oceanbase
+Provides-Extra: trino
+Provides-Extra: maxdb
+Provides-Extra: tdengine
+Provides-Extra: matrixone
+Provides-Extra: starrocks
+Provides-Extra: writer
+Provides-Extra: hana
+Provides-Extra: phoenix
+Provides-Extra: tpot
+Provides-Extra: tidb
+Provides-Extra: edgelessdb
+Provides-Extra: confluence
+Provides-Extra: couchbase
+Provides-Extra: snowflake
+Provides-Extra: orioledb
+Provides-Extra: llama_index
+Provides-Extra: paypal
+Provides-Extra: druid
+Provides-Extra: gmail
+Provides-Extra: twitter
 Provides-Extra: all_handlers_extras
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.6.5.1 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.7.1.0 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -137,49 +137,49 @@
                             mindsdb.com/newsletter/
   ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
   product updates, information about MindsDB events and contests, and useful
   content, like tutorials. ## License MindsDB is licensed under [GNU General
  Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
  Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
- Type: text/markdown Provides-Extra: telemetry Provides-Extra: grpc Provides-
- Extra: all_extras Provides-Extra: tdengine Provides-Extra: yugabyte Provides-
-Extra: opengauss Provides-Extra: merlion Provides-Extra: ignite Provides-Extra:
-  lightwood Provides-Extra: datastax Provides-Extra: informix Provides-Extra:
- huggingface_api Provides-Extra: scylla Provides-Extra: huggingface Provides-
- Extra: access Provides-Extra: frappe Provides-Extra: teradata Provides-Extra:
-  mlflow Provides-Extra: cockroach Provides-Extra: confluence Provides-Extra:
-elasticsearch Provides-Extra: mariadb Provides-Extra: cloud_sql Provides-Extra:
-empress Provides-Extra: cohere Provides-Extra: langchain Provides-Extra: mysql
-  Provides-Extra: d0lt Provides-Extra: sheets Provides-Extra: druid Provides-
-  Extra: phoenix Provides-Extra: planetscale Provides-Extra: paypal Provides-
-  Extra: web Provides-Extra: mediawiki Provides-Extra: aurora Provides-Extra:
-realtime_slack_chat Provides-Extra: dremio Provides-Extra: tidb Provides-Extra:
- jira Provides-Extra: redshift Provides-Extra: rockset Provides-Extra: twitter
-  Provides-Extra: bigquery Provides-Extra: google_content_shopping Provides-
-Extra: neuralforecast Provides-Extra: edgelessdb Provides-Extra: db2 Provides-
-Extra: cloud_spanner Provides-Extra: databend Provides-Extra: youtube Provides-
-  Extra: postgres Provides-Extra: sendinblue Provides-Extra: ludwig Provides-
-Extra: tpot Provides-Extra: airtable Provides-Extra: clickhouse Provides-Extra:
-  influxdb Provides-Extra: dynamodb Provides-Extra: nuo_jdbc Provides-Extra:
-     pinot Provides-Extra: matrixone Provides-Extra: trino Provides-Extra:
-  monkeylearn Provides-Extra: questdb Provides-Extra: vitess Provides-Extra:
-   llama_index Provides-Extra: gmail Provides-Extra: openai Provides-Extra:
-  cassandra Provides-Extra: materialize Provides-Extra: quickbooks Provides-
-    Extra: impala Provides-Extra: singlestore Provides-Extra: google_search
-  Provides-Extra: duckdb Provides-Extra: solr Provides-Extra: mssql Provides-
- Extra: flaml Provides-Extra: github Provides-Extra: supabase Provides-Extra:
-  statsforecast Provides-Extra: stripe Provides-Extra: ingres Provides-Extra:
-   autosklearn Provides-Extra: hsqldb Provides-Extra: slack Provides-Extra:
-   mendeley Provides-Extra: orioledb Provides-Extra: gitlab Provides-Extra:
-   mongodb Provides-Extra: vertica Provides-Extra: snowflake Provides-Extra:
-firebird Provides-Extra: strava Provides-Extra: crate Provides-Extra: couchbase
-   Provides-Extra: timescaledb Provides-Extra: binance Provides-Extra: maxdb
- Provides-Extra: s3 Provides-Extra: shopify Provides-Extra: monetdb Provides-
-  Extra: sqreamdb Provides-Extra: ckan Provides-Extra: writer Provides-Extra:
-    ray_serve Provides-Extra: sqlany Provides-Extra: derby Provides-Extra:
-   google_calendar Provides-Extra: hana Provides-Extra: hive Provides-Extra:
-  google_books Provides-Extra: surrealdb Provides-Extra: google_fit Provides-
-  Extra: rocket_chat Provides-Extra: newsapi Provides-Extra: reddit Provides-
-  Extra: plaid Provides-Extra: databricks Provides-Extra: altibase Provides-
-  Extra: starrocks Provides-Extra: oracle Provides-Extra: oceanbase Provides-
-                          Extra: all_handlers_extras
+ Type: text/markdown Provides-Extra: grpc Provides-Extra: telemetry Provides-
+  Extra: all_extras Provides-Extra: informix Provides-Extra: slack Provides-
+Extra: google_search Provides-Extra: ingres Provides-Extra: teradata Provides-
+  Extra: openai Provides-Extra: postgres Provides-Extra: databricks Provides-
+ Extra: monkeylearn Provides-Extra: vitess Provides-Extra: lightwood Provides-
+Extra: autosklearn Provides-Extra: datastax Provides-Extra: influxdb Provides-
+ Extra: s3 Provides-Extra: mediawiki Provides-Extra: nuo_jdbc Provides-Extra:
+access Provides-Extra: shopify Provides-Extra: surrealdb Provides-Extra: derby
+    Provides-Extra: databend Provides-Extra: sheets Provides-Extra: empress
+ Provides-Extra: yugabyte Provides-Extra: huggingface Provides-Extra: binance
+ Provides-Extra: db2 Provides-Extra: solr Provides-Extra: opengauss Provides-
+Extra: mongodb Provides-Extra: ray_serve Provides-Extra: scylla Provides-Extra:
+  merlion Provides-Extra: sendinblue Provides-Extra: mendeley Provides-Extra:
+  mariadb Provides-Extra: cloud_sql Provides-Extra: google_calendar Provides-
+    Extra: firebird Provides-Extra: elasticsearch Provides-Extra: cassandra
+  Provides-Extra: sqreamdb Provides-Extra: redshift Provides-Extra: supabase
+   Provides-Extra: planetscale Provides-Extra: strava Provides-Extra: sqlany
+Provides-Extra: huggingface_api Provides-Extra: neuralforecast Provides-Extra:
+  questdb Provides-Extra: mysql Provides-Extra: plaid Provides-Extra: newsapi
+  Provides-Extra: altibase Provides-Extra: clickhouse Provides-Extra: impala
+  Provides-Extra: singlestore Provides-Extra: airtable Provides-Extra: oracle
+Provides-Extra: google_content_shopping Provides-Extra: duckdb Provides-Extra:
+  statsforecast Provides-Extra: pinot Provides-Extra: google_books Provides-
+Extra: youtube Provides-Extra: bigquery Provides-Extra: vertica Provides-Extra:
+ mssql Provides-Extra: crate Provides-Extra: langchain Provides-Extra: ignite
+     Provides-Extra: cloud_spanner Provides-Extra: rockset Provides-Extra:
+  realtime_slack_chat Provides-Extra: hive Provides-Extra: dynamodb Provides-
+Extra: timescaledb Provides-Extra: ludwig Provides-Extra: google_fit Provides-
+Extra: cockroach Provides-Extra: github Provides-Extra: mlflow Provides-Extra:
+flaml Provides-Extra: aurora Provides-Extra: quickbooks Provides-Extra: gitlab
+  Provides-Extra: ckan Provides-Extra: d0lt Provides-Extra: cohere Provides-
+  Extra: dremio Provides-Extra: stripe Provides-Extra: hsqldb Provides-Extra:
+monetdb Provides-Extra: frappe Provides-Extra: jira Provides-Extra: rocket_chat
+    Provides-Extra: web Provides-Extra: materialize Provides-Extra: reddit
+Provides-Extra: oceanbase Provides-Extra: trino Provides-Extra: maxdb Provides-
+ Extra: tdengine Provides-Extra: matrixone Provides-Extra: starrocks Provides-
+Extra: writer Provides-Extra: hana Provides-Extra: phoenix Provides-Extra: tpot
+  Provides-Extra: tidb Provides-Extra: edgelessdb Provides-Extra: confluence
+ Provides-Extra: couchbase Provides-Extra: snowflake Provides-Extra: orioledb
+   Provides-Extra: llama_index Provides-Extra: paypal Provides-Extra: druid
+         Provides-Extra: gmail Provides-Extra: twitter Provides-Extra:
+                             all_handlers_extras
```

### Comparing `MindsDB-23.6.5.1/MindsDB.egg-info/SOURCES.txt` & `MindsDB-23.7.1.0/MindsDB.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -968,14 +968,16 @@
 mindsdb/integrations/handlers/twitter_handler/__about__.py
 mindsdb/integrations/handlers/twitter_handler/__init__.py
 mindsdb/integrations/handlers/twitter_handler/icon.svg
 mindsdb/integrations/handlers/twitter_handler/requirements.txt
 mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
 mindsdb/integrations/handlers/utilities/__init__.py
 mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
+mindsdb/integrations/handlers/utilities/query_utilities/exceptions.py
+mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py
 mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
 mindsdb/integrations/handlers/vertica_handler/__about__.py
 mindsdb/integrations/handlers/vertica_handler/__init__.py
 mindsdb/integrations/handlers/vertica_handler/icon.svg
 mindsdb/integrations/handlers/vertica_handler/requirements.txt
 mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
 mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
@@ -1025,14 +1027,15 @@
 mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
 mindsdb/integrations/handlers_wrapper/ml_handler_service.py
 mindsdb/integrations/libs/__init__.py
 mindsdb/integrations/libs/api_handler.py
 mindsdb/integrations/libs/base.py
 mindsdb/integrations/libs/const.py
 mindsdb/integrations/libs/handler_helpers.py
+mindsdb/integrations/libs/learn_process.py
 mindsdb/integrations/libs/ml_exec_base.py
 mindsdb/integrations/libs/ml_handler_proc.py
 mindsdb/integrations/libs/net_helpers.py
 mindsdb/integrations/libs/realtime_chat_handler.py
 mindsdb/integrations/libs/response.py
 mindsdb/integrations/libs/storage_handler.py
 mindsdb/integrations/utilities/__init__.py
@@ -1118,14 +1121,15 @@
 mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
 mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
 mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
 mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
 mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
 mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
 mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
+mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py
 mindsdb/migrations/versions/__init__.py
 mindsdb/utilities/__init__.py
 mindsdb/utilities/auth.py
 mindsdb/utilities/cache.py
 mindsdb/utilities/config.py
 mindsdb/utilities/context.py
 mindsdb/utilities/fs.py
```

### Comparing `MindsDB-23.6.5.1/MindsDB.egg-info/requires.txt` & `MindsDB-23.7.1.0/MindsDB.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,186 +24,186 @@
 checksumdir>=1.2.0
 duckdb==0.6.0
 requests>=2.0.0
 mysql-connector-python
 clickhouse-driver
 clickhouse-sqlalchemy
 charset-normalizer
-dill>=0.3.4
 pyOpenSSL>=22.0.0
 pydateinfer==0.3.0
 pyarrow<10.1.0,>=10.0.1
 dataprep_ml
 python-magic>=0.4.27
 openpyxl>=3.1.1
+dill==0.3.6
 slack_sdk
 
 [access]
 pyodbc
 sqlalchemy-access
 
 [airtable]
 duckdb
 
 [all_extras]
-sentry-sdk
 grpcio-tools
+sentry-sdk
 
 [all_handlers_extras]
-langchain==0.0.186
-stripe
-protobuf==3.20.*
-mindsdb_sql<0.5.0,>=0.4.9
-sentence_transformers
-pyHive
-pyodbc==4.0.34
-tweepy
-google-auth-oauthlib
+praw
+db-dtypes
+snowflake-sqlalchemy>=1.4.3
+neuralforecast<1.5.0,>=1.4.0
+mindsdb>=22.10.2.1
+google-cloud-spanner
+pydantic==1.10.8
+monkeylearn==3.6.0
+rocketchat_API
+pyignite
+mlflow
+tpot<=0.11.7
+cohere==4.5.1
+sqlanydb
+ckanapi
+psycopg[binary]
+duckdb==0.7.1
+scylla-driver
+mindsdb>=23.3.5.0
+IfxPy
+hierarchicalforecast<1.0
+hyperopt
+pytz
 trino~=0.313.0
+transformers==4.21.0
+pyHive
+dask
+sqlalchemy-hana
+pandas<=1.4.3
+ibm-db
+mediawikiapi
+bs4
+ludwig[distributed]>=0.5.2
+html2text
+elasticsearch-dbapi
+sentencepiece==0.1.97
+sqlalchemy-vertica-python
+sqlalchemy-bigquery
+mindsdb>=23.3.2.0
+taospy
+psycopg2
+pandas
+plaid-python
 thrift
-redshift_connector
-crate[sqlalchemy]
-duckdb
-pinotdb
-newsapi-python
-sqlanydb
-requests==2.28.0
-couchbase==4.0.2
+slack_sdk
+sqlalchemy-access
+oracledb==1.0.2
+impyla
+pyodbc==4.0.34
 teradatasql
-pydantic==1.10.8
-chromadb==0.3.25
-sqlalchemy-solr
+auto-sklearn
+tweepy
 pyodbc
-bs4
-sqlalchemy
-hyperopt<1.0
-ckanapi
-pyphoenix
-neuralforecast<1.5.0,>=1.4.0
-ray[serve]
-sasl
-db-dtypes
-snowflake-connector-python>=2.7.12
-sentencepiece==0.1.97
+sentence_transformers
+stravalib
+google-api-python-client
 tensorflow
+pymssql>=2.1.4
+google-auth-httplib2
 certifi
+pyphoenix
+sqlalchemy
+hdbcli
+newsapi-python
+SQLAlchemy
+wikipedia==1.4.0
+statsforecast<2.0,>=1.4.0
+openai<=0.28.0
+clickhouse-sqlalchemy
+flaml<=1.2.3
+google-auth-oauthlib
+pinotdb
+ray[serve]
+mindsdb>=22.6.2.1
+databricks-sql-connector
 tiktoken>=0.3.0
-mindsdb>=22.12.4.3
-openai==0.27.0
-pytz
 pymysql
+tzlocal
+stripe
+elasticsearch
+sqlalchemy-monetdb
+paypalrestsdk
+sasl
+protobuf==3.20.*
+sib_api_v3_sdk
+psycopg
+sqlalchemy-sqlany
+pydruid
+mindsdb>=22.7.5.0
 boto3
-atlassian-python-api
-html2text
-tqdm
-openai>=0.27.0
-plaid-python
-fdb
+pymonetdb
+ShopifyAPI
+pysqream_sqlalchemy>=0.8
 lightwood[all_extras]>=22.8.1.0
-SQLAlchemy
-sib_api_v3_sdk
-mindsdb-evaluator>=0.0.6
-mysql-connector-python
-IfxPy
-flaml<=1.2.3
-transformers==4.21.0
-openai<=0.28.0
-sqlalchemy-informix
+mindsdb>=22.12.4.3
+crate[sqlalchemy]
+binance-connector
+rockset
+requests-kerberos==0.12.0
+ingres_sa_dialect==0.3
+chromadb==0.3.25
+redshift_connector
+pygithub
+sqlalchemy-databricks
+google
+openai==0.27.0
+markupsafe==2.0.1
+mindsdb_sql<0.5.0,>=0.4.4
+sqlalchemy-redshift
+langchain<=0.0.192
 ibm-db-sa
-ShopifyAPI
-impyla
+sqlalchemy_dremio
 phoenixdb
-pandas<=1.4.3
-pymonetdb
-scylla-driver
-tpot<=0.11.7
-elasticsearch-dbapi
+mindsdb_sql<0.5.0,>=0.4.9
+snowflake-connector-python>=2.7.12
+duckdb
+torch
 websocket
+hyperopt<1.0
 mindsdb_sql>=0.4.0
-sqlalchemy-vertica-python
-clickhouse-sqlalchemy
-hyperopt
+pysurrealdb
+openai>=0.27.0
+tqdm
+sqlalchemy-informix
+dill
+couchbase==4.0.2
+mindsdb-evaluator>=0.0.6
+llama-index==0.6.11
+jaydebeapi
+pymongo[srv]>=4.1.1
+mendeley
+qbosdk
+vertica-python
 pysqream>=3.2.5
-ibm-db
-paypalrestsdk
-binance-connector
-wikipedia==1.4.0
-slack_sdk
-requests-kerberos==0.12.0
-databricks-sql-connector
-monkeylearn==3.6.0
-hugging_py_face
 mindsdb_sql<0.5.0,>=0.4.6
-vertica-python
-google-auth-httplib2
-mlflow
-duckdb==0.7.1.dev187
-rockset
-google-cloud-spanner
-jaydebeapi
+teradatasqlalchemy
+sqlalchemy-solr
+ray<=1.13.0
 python-gitlab
+fdb
 sqlalchemy<2.0.0
-auto-sklearn
-mindsdb>=22.7.5.0
-taospy
-sqlalchemy-bigquery
-torch
-google-api-python-client
-sqlalchemy-access
-sqlalchemy_dremio
-psycopg
-hierarchicalforecast<1.0
-ingres_sa_dialect==0.3
-sqlalchemy-sqlany
-google-cloud-bigquery
-elasticsearch
-dill
-duckdb==0.7.1
-mindsdb>=22.10.2.1
-ray<=1.13.0
-pymssql>=2.1.4
-teradatasqlalchemy
-mindsdb>=22.6.2.1
-pygithub
-pysqream_sqlalchemy>=0.8
-markupsafe==2.0.1
-salesforce-merlion<=1.3.1,>=1.2.0
-langchain<=0.0.192
+duckdb==0.7.1.dev187
 pyhive
-google
-stravalib
-rocketchat_API
-mindsdb>=23.3.5.0
-pydruid
-mindsdb>=23.3.2.0
-mindsdb_sql<0.5.0,>=0.4.4
-psycopg2
-snowflake-sqlalchemy>=1.4.3
-praw
-tzlocal
-qbosdk
-llama-index==0.6.11
-pysurrealdb
-sqlalchemy-redshift
-dask
-pyignite
-sqlalchemy-hana
-hdbcli
-sqlalchemy-monetdb
-mediawikiapi
-sqlalchemy-databricks
-statsforecast<2.0,>=1.4.0
-oracledb==1.0.2
-pandas
-psycopg[binary]
-cohere==4.5.1
-pymongo[srv]>=4.1.1
-ludwig[distributed]>=0.5.2
+mysql-connector-python
+salesforce-merlion<=1.3.1,>=1.2.0
+google-cloud-bigquery
+hugging_py_face
+atlassian-python-api
 thrift-sasl
-mendeley
+requests==2.28.0
+langchain==0.0.186
 
 [altibase]
 jaydebeapi
 
 [aurora]
 psycopg[binary]
 mysql-connector-python
@@ -395,14 +395,16 @@
 
 [langchain]
 mindsdb>=23.3.2.0
 mindsdb_sql<0.5.0,>=0.4.9
 openai==0.27.0
 langchain==0.0.186
 wikipedia==1.4.0
+pandas
+tiktoken>=0.3.0
 
 [lightwood]
 lightwood[all_extras]>=22.8.1.0
 mindsdb_sql>=0.4.0
 mindsdb>=22.7.5.0
 
 [llama_index]
```

### Comparing `MindsDB-23.6.5.1/PKG-INFO` & `MindsDB-23.7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.6.5.1
+Version: 23.7.1.0
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -200,132 +200,132 @@
         MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: telemetry
 Provides-Extra: grpc
+Provides-Extra: telemetry
 Provides-Extra: all_extras
-Provides-Extra: tdengine
-Provides-Extra: yugabyte
-Provides-Extra: opengauss
-Provides-Extra: merlion
-Provides-Extra: ignite
+Provides-Extra: informix
+Provides-Extra: slack
+Provides-Extra: google_search
+Provides-Extra: ingres
+Provides-Extra: teradata
+Provides-Extra: openai
+Provides-Extra: postgres
+Provides-Extra: databricks
+Provides-Extra: monkeylearn
+Provides-Extra: vitess
 Provides-Extra: lightwood
+Provides-Extra: autosklearn
 Provides-Extra: datastax
-Provides-Extra: informix
-Provides-Extra: huggingface_api
-Provides-Extra: scylla
-Provides-Extra: huggingface
+Provides-Extra: influxdb
+Provides-Extra: s3
+Provides-Extra: mediawiki
+Provides-Extra: nuo_jdbc
 Provides-Extra: access
-Provides-Extra: frappe
-Provides-Extra: teradata
-Provides-Extra: mlflow
-Provides-Extra: cockroach
-Provides-Extra: confluence
-Provides-Extra: elasticsearch
+Provides-Extra: shopify
+Provides-Extra: surrealdb
+Provides-Extra: derby
+Provides-Extra: databend
+Provides-Extra: sheets
+Provides-Extra: empress
+Provides-Extra: yugabyte
+Provides-Extra: huggingface
+Provides-Extra: binance
+Provides-Extra: db2
+Provides-Extra: solr
+Provides-Extra: opengauss
+Provides-Extra: mongodb
+Provides-Extra: ray_serve
+Provides-Extra: scylla
+Provides-Extra: merlion
+Provides-Extra: sendinblue
+Provides-Extra: mendeley
 Provides-Extra: mariadb
 Provides-Extra: cloud_sql
-Provides-Extra: empress
-Provides-Extra: cohere
-Provides-Extra: langchain
-Provides-Extra: mysql
-Provides-Extra: d0lt
-Provides-Extra: sheets
-Provides-Extra: druid
-Provides-Extra: phoenix
-Provides-Extra: planetscale
-Provides-Extra: paypal
-Provides-Extra: web
-Provides-Extra: mediawiki
-Provides-Extra: aurora
-Provides-Extra: realtime_slack_chat
-Provides-Extra: dremio
-Provides-Extra: tidb
-Provides-Extra: jira
+Provides-Extra: google_calendar
+Provides-Extra: firebird
+Provides-Extra: elasticsearch
+Provides-Extra: cassandra
+Provides-Extra: sqreamdb
 Provides-Extra: redshift
-Provides-Extra: rockset
-Provides-Extra: twitter
-Provides-Extra: bigquery
-Provides-Extra: google_content_shopping
+Provides-Extra: supabase
+Provides-Extra: planetscale
+Provides-Extra: strava
+Provides-Extra: sqlany
+Provides-Extra: huggingface_api
 Provides-Extra: neuralforecast
-Provides-Extra: edgelessdb
-Provides-Extra: db2
-Provides-Extra: cloud_spanner
-Provides-Extra: databend
-Provides-Extra: youtube
-Provides-Extra: postgres
-Provides-Extra: sendinblue
-Provides-Extra: ludwig
-Provides-Extra: tpot
-Provides-Extra: airtable
-Provides-Extra: clickhouse
-Provides-Extra: influxdb
-Provides-Extra: dynamodb
-Provides-Extra: nuo_jdbc
-Provides-Extra: pinot
-Provides-Extra: matrixone
-Provides-Extra: trino
-Provides-Extra: monkeylearn
 Provides-Extra: questdb
-Provides-Extra: vitess
-Provides-Extra: llama_index
-Provides-Extra: gmail
-Provides-Extra: openai
-Provides-Extra: cassandra
-Provides-Extra: materialize
-Provides-Extra: quickbooks
+Provides-Extra: mysql
+Provides-Extra: plaid
+Provides-Extra: newsapi
+Provides-Extra: altibase
+Provides-Extra: clickhouse
 Provides-Extra: impala
 Provides-Extra: singlestore
-Provides-Extra: google_search
+Provides-Extra: airtable
+Provides-Extra: oracle
+Provides-Extra: google_content_shopping
 Provides-Extra: duckdb
-Provides-Extra: solr
-Provides-Extra: mssql
-Provides-Extra: flaml
-Provides-Extra: github
-Provides-Extra: supabase
 Provides-Extra: statsforecast
-Provides-Extra: stripe
-Provides-Extra: ingres
-Provides-Extra: autosklearn
-Provides-Extra: hsqldb
-Provides-Extra: slack
-Provides-Extra: mendeley
-Provides-Extra: orioledb
-Provides-Extra: gitlab
-Provides-Extra: mongodb
+Provides-Extra: pinot
+Provides-Extra: google_books
+Provides-Extra: youtube
+Provides-Extra: bigquery
 Provides-Extra: vertica
-Provides-Extra: snowflake
-Provides-Extra: firebird
-Provides-Extra: strava
+Provides-Extra: mssql
 Provides-Extra: crate
-Provides-Extra: couchbase
-Provides-Extra: timescaledb
-Provides-Extra: binance
-Provides-Extra: maxdb
-Provides-Extra: s3
-Provides-Extra: shopify
-Provides-Extra: monetdb
-Provides-Extra: sqreamdb
-Provides-Extra: ckan
-Provides-Extra: writer
-Provides-Extra: ray_serve
-Provides-Extra: sqlany
-Provides-Extra: derby
-Provides-Extra: google_calendar
-Provides-Extra: hana
+Provides-Extra: langchain
+Provides-Extra: ignite
+Provides-Extra: cloud_spanner
+Provides-Extra: rockset
+Provides-Extra: realtime_slack_chat
 Provides-Extra: hive
-Provides-Extra: google_books
-Provides-Extra: surrealdb
+Provides-Extra: dynamodb
+Provides-Extra: timescaledb
+Provides-Extra: ludwig
 Provides-Extra: google_fit
+Provides-Extra: cockroach
+Provides-Extra: github
+Provides-Extra: mlflow
+Provides-Extra: flaml
+Provides-Extra: aurora
+Provides-Extra: quickbooks
+Provides-Extra: gitlab
+Provides-Extra: ckan
+Provides-Extra: d0lt
+Provides-Extra: cohere
+Provides-Extra: dremio
+Provides-Extra: stripe
+Provides-Extra: hsqldb
+Provides-Extra: monetdb
+Provides-Extra: frappe
+Provides-Extra: jira
 Provides-Extra: rocket_chat
-Provides-Extra: newsapi
+Provides-Extra: web
+Provides-Extra: materialize
 Provides-Extra: reddit
-Provides-Extra: plaid
-Provides-Extra: databricks
-Provides-Extra: altibase
-Provides-Extra: starrocks
-Provides-Extra: oracle
 Provides-Extra: oceanbase
+Provides-Extra: trino
+Provides-Extra: maxdb
+Provides-Extra: tdengine
+Provides-Extra: matrixone
+Provides-Extra: starrocks
+Provides-Extra: writer
+Provides-Extra: hana
+Provides-Extra: phoenix
+Provides-Extra: tpot
+Provides-Extra: tidb
+Provides-Extra: edgelessdb
+Provides-Extra: confluence
+Provides-Extra: couchbase
+Provides-Extra: snowflake
+Provides-Extra: orioledb
+Provides-Extra: llama_index
+Provides-Extra: paypal
+Provides-Extra: druid
+Provides-Extra: gmail
+Provides-Extra: twitter
 Provides-Extra: all_handlers_extras
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.6.5.1 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.7.1.0 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -137,49 +137,49 @@
                             mindsdb.com/newsletter/
   ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
   product updates, information about MindsDB events and contests, and useful
   content, like tutorials. ## License MindsDB is licensed under [GNU General
  Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
  Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
- Type: text/markdown Provides-Extra: telemetry Provides-Extra: grpc Provides-
- Extra: all_extras Provides-Extra: tdengine Provides-Extra: yugabyte Provides-
-Extra: opengauss Provides-Extra: merlion Provides-Extra: ignite Provides-Extra:
-  lightwood Provides-Extra: datastax Provides-Extra: informix Provides-Extra:
- huggingface_api Provides-Extra: scylla Provides-Extra: huggingface Provides-
- Extra: access Provides-Extra: frappe Provides-Extra: teradata Provides-Extra:
-  mlflow Provides-Extra: cockroach Provides-Extra: confluence Provides-Extra:
-elasticsearch Provides-Extra: mariadb Provides-Extra: cloud_sql Provides-Extra:
-empress Provides-Extra: cohere Provides-Extra: langchain Provides-Extra: mysql
-  Provides-Extra: d0lt Provides-Extra: sheets Provides-Extra: druid Provides-
-  Extra: phoenix Provides-Extra: planetscale Provides-Extra: paypal Provides-
-  Extra: web Provides-Extra: mediawiki Provides-Extra: aurora Provides-Extra:
-realtime_slack_chat Provides-Extra: dremio Provides-Extra: tidb Provides-Extra:
- jira Provides-Extra: redshift Provides-Extra: rockset Provides-Extra: twitter
-  Provides-Extra: bigquery Provides-Extra: google_content_shopping Provides-
-Extra: neuralforecast Provides-Extra: edgelessdb Provides-Extra: db2 Provides-
-Extra: cloud_spanner Provides-Extra: databend Provides-Extra: youtube Provides-
-  Extra: postgres Provides-Extra: sendinblue Provides-Extra: ludwig Provides-
-Extra: tpot Provides-Extra: airtable Provides-Extra: clickhouse Provides-Extra:
-  influxdb Provides-Extra: dynamodb Provides-Extra: nuo_jdbc Provides-Extra:
-     pinot Provides-Extra: matrixone Provides-Extra: trino Provides-Extra:
-  monkeylearn Provides-Extra: questdb Provides-Extra: vitess Provides-Extra:
-   llama_index Provides-Extra: gmail Provides-Extra: openai Provides-Extra:
-  cassandra Provides-Extra: materialize Provides-Extra: quickbooks Provides-
-    Extra: impala Provides-Extra: singlestore Provides-Extra: google_search
-  Provides-Extra: duckdb Provides-Extra: solr Provides-Extra: mssql Provides-
- Extra: flaml Provides-Extra: github Provides-Extra: supabase Provides-Extra:
-  statsforecast Provides-Extra: stripe Provides-Extra: ingres Provides-Extra:
-   autosklearn Provides-Extra: hsqldb Provides-Extra: slack Provides-Extra:
-   mendeley Provides-Extra: orioledb Provides-Extra: gitlab Provides-Extra:
-   mongodb Provides-Extra: vertica Provides-Extra: snowflake Provides-Extra:
-firebird Provides-Extra: strava Provides-Extra: crate Provides-Extra: couchbase
-   Provides-Extra: timescaledb Provides-Extra: binance Provides-Extra: maxdb
- Provides-Extra: s3 Provides-Extra: shopify Provides-Extra: monetdb Provides-
-  Extra: sqreamdb Provides-Extra: ckan Provides-Extra: writer Provides-Extra:
-    ray_serve Provides-Extra: sqlany Provides-Extra: derby Provides-Extra:
-   google_calendar Provides-Extra: hana Provides-Extra: hive Provides-Extra:
-  google_books Provides-Extra: surrealdb Provides-Extra: google_fit Provides-
-  Extra: rocket_chat Provides-Extra: newsapi Provides-Extra: reddit Provides-
-  Extra: plaid Provides-Extra: databricks Provides-Extra: altibase Provides-
-  Extra: starrocks Provides-Extra: oracle Provides-Extra: oceanbase Provides-
-                          Extra: all_handlers_extras
+ Type: text/markdown Provides-Extra: grpc Provides-Extra: telemetry Provides-
+  Extra: all_extras Provides-Extra: informix Provides-Extra: slack Provides-
+Extra: google_search Provides-Extra: ingres Provides-Extra: teradata Provides-
+  Extra: openai Provides-Extra: postgres Provides-Extra: databricks Provides-
+ Extra: monkeylearn Provides-Extra: vitess Provides-Extra: lightwood Provides-
+Extra: autosklearn Provides-Extra: datastax Provides-Extra: influxdb Provides-
+ Extra: s3 Provides-Extra: mediawiki Provides-Extra: nuo_jdbc Provides-Extra:
+access Provides-Extra: shopify Provides-Extra: surrealdb Provides-Extra: derby
+    Provides-Extra: databend Provides-Extra: sheets Provides-Extra: empress
+ Provides-Extra: yugabyte Provides-Extra: huggingface Provides-Extra: binance
+ Provides-Extra: db2 Provides-Extra: solr Provides-Extra: opengauss Provides-
+Extra: mongodb Provides-Extra: ray_serve Provides-Extra: scylla Provides-Extra:
+  merlion Provides-Extra: sendinblue Provides-Extra: mendeley Provides-Extra:
+  mariadb Provides-Extra: cloud_sql Provides-Extra: google_calendar Provides-
+    Extra: firebird Provides-Extra: elasticsearch Provides-Extra: cassandra
+  Provides-Extra: sqreamdb Provides-Extra: redshift Provides-Extra: supabase
+   Provides-Extra: planetscale Provides-Extra: strava Provides-Extra: sqlany
+Provides-Extra: huggingface_api Provides-Extra: neuralforecast Provides-Extra:
+  questdb Provides-Extra: mysql Provides-Extra: plaid Provides-Extra: newsapi
+  Provides-Extra: altibase Provides-Extra: clickhouse Provides-Extra: impala
+  Provides-Extra: singlestore Provides-Extra: airtable Provides-Extra: oracle
+Provides-Extra: google_content_shopping Provides-Extra: duckdb Provides-Extra:
+  statsforecast Provides-Extra: pinot Provides-Extra: google_books Provides-
+Extra: youtube Provides-Extra: bigquery Provides-Extra: vertica Provides-Extra:
+ mssql Provides-Extra: crate Provides-Extra: langchain Provides-Extra: ignite
+     Provides-Extra: cloud_spanner Provides-Extra: rockset Provides-Extra:
+  realtime_slack_chat Provides-Extra: hive Provides-Extra: dynamodb Provides-
+Extra: timescaledb Provides-Extra: ludwig Provides-Extra: google_fit Provides-
+Extra: cockroach Provides-Extra: github Provides-Extra: mlflow Provides-Extra:
+flaml Provides-Extra: aurora Provides-Extra: quickbooks Provides-Extra: gitlab
+  Provides-Extra: ckan Provides-Extra: d0lt Provides-Extra: cohere Provides-
+  Extra: dremio Provides-Extra: stripe Provides-Extra: hsqldb Provides-Extra:
+monetdb Provides-Extra: frappe Provides-Extra: jira Provides-Extra: rocket_chat
+    Provides-Extra: web Provides-Extra: materialize Provides-Extra: reddit
+Provides-Extra: oceanbase Provides-Extra: trino Provides-Extra: maxdb Provides-
+ Extra: tdengine Provides-Extra: matrixone Provides-Extra: starrocks Provides-
+Extra: writer Provides-Extra: hana Provides-Extra: phoenix Provides-Extra: tpot
+  Provides-Extra: tidb Provides-Extra: edgelessdb Provides-Extra: confluence
+ Provides-Extra: couchbase Provides-Extra: snowflake Provides-Extra: orioledb
+   Provides-Extra: llama_index Provides-Extra: paypal Provides-Extra: druid
+         Provides-Extra: gmail Provides-Extra: twitter Provides-Extra:
+                             all_handlers_extras
```

### Comparing `MindsDB-23.6.5.1/README.md` & `MindsDB-23.7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/__main__.py` & `MindsDB-23.7.1.0/mindsdb/__main__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/common/check_auth.py` & `MindsDB-23.7.1.0/mindsdb/api/common/check_auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/gui.py` & `MindsDB-23.7.1.0/mindsdb/api/http/gui.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-23.7.1.0/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/initialize.py` & `MindsDB-23.7.1.0/mindsdb/api/http/initialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,14 +251,19 @@
                 'Authorization is required to complete the request'
             )
         # endregion
 
         company_id = request.headers.get('company-id')
         user_class = request.headers.get('user-class')
 
+        try:
+            email_confirmed = int(request.headers.get('email-confirmed', 1))
+        except ValueError:
+            email_confirmed = 1
+
         if company_id is not None:
             try:
                 company_id = int(company_id)
             except Exception as e:
                 log.get_log('http').error(f'Cloud not parse company id: {company_id} | exception: {e}')
                 company_id = None
 
@@ -269,14 +274,15 @@
                 log.get_log('http').error(f'Cloud not parse user_class: {user_class} | exception: {e}')
                 user_class = 0
         else:
             user_class = 0
 
         ctx.company_id = company_id
         ctx.user_class = user_class
+        ctx.email_confirmed = email_confirmed
 
     # Wait for static initialization.
     if not no_studio and init_static_thread is not None:
         init_static_thread.join()
 
     return app
```

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/auth.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/chatbots.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/chatbots.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             except PredictorRecordNotFound:
                 return http_error(
                     HTTPStatus.NOT_FOUND,
                     'Model not found',
                     f'Model with name {model_name} not found')
 
         # Chatbot must not exist with new name.
-        if name is not None:
+        if name is not None and name != chatbot_name:
             chatbot_with_new_name = chatbot_controller.get_chatbot(name, project_name=project_name)
             if chatbot_with_new_name is not None:
                 return http_error(
                     HTTPStatus.CONFLICT,
                     'Chatbot already exists',
                     f'Chatbot with name {name} already exists. Please choose a different one.'
                 )
```

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/config.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/databases.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/default.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/default.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/file.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/file.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/models.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/models.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/projects.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/sql.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/tab.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/tree.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/util.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import psutil
 import tempfile
 from pathlib import Path
 
 from flask import request
 from flask_restx import Resource
 from flask import current_app as ca
 
@@ -11,14 +10,15 @@
 from mindsdb.utilities.telemetry import (
     enable_telemetry,
     disable_telemetry,
     telemetry_file_exists,
     inject_telemetry_to_static
 )
 from mindsdb.api.http.gui import update_static
+from mindsdb.utilities.fs import clean_unlinked_process_marks
 
 
 @ns_conf.route('/ping')
 class Ping(Resource):
     @ns_conf.doc('get_ping')
     def get(self):
         '''Checks server avaliable'''
@@ -41,23 +41,18 @@
         if os.name != 'posix':
             return response
 
         for process_type in response:
             processes_dir = Path(tempfile.gettempdir()).joinpath(f'mindsdb/processes/{process_type}/')
             if not processes_dir.is_dir():
                 continue
+            clean_unlinked_process_marks()
             process_marks = [x.name for x in processes_dir.iterdir()]
-            for p_mark in process_marks:
-                pid = int(p_mark.split('-')[0])
-                try:
-                    psutil.Process(pid)
-                except Exception:
-                    processes_dir.joinpath(p_mark).unlink()
-                else:
-                    response[process_type] = True
+            if len(process_marks) > 0:
+                response[process_type] = True
 
         return response
 
 
 @ns_conf.route('/telemetry')
 class Telemetry(Resource):
     @ns_conf.doc('get_telemetry_status')
```

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/namespaces/views.py` & `MindsDB-23.7.1.0/mindsdb/api/http/namespaces/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/start.py` & `MindsDB-23.7.1.0/mindsdb/api/http/start.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,30 +5,37 @@
 from waitress import serve
 
 from mindsdb.api.http.initialize import initialize_app
 from mindsdb.interfaces.storage import db
 from mindsdb.utilities import log
 from mindsdb.utilities.config import Config
 from mindsdb.utilities.functions import init_lexer_parsers
+from mindsdb.integrations.libs.ml_exec_base import process_cache
+from mindsdb.interfaces.database.integrations import integration_controller
 
 
 def start(verbose, no_studio, with_nlp):
     config = Config()
+    is_cloud = config.get('cloud', False)
 
     server = os.environ.get('MINDSDB_DEFAULT_SERVER', 'waitress')
     db.init()
     log.initialize_log(config, 'http', wrap_print=True if server.lower() != 'gunicorn' else False)
 
     init_lexer_parsers()
 
     app = initialize_app(config, no_studio, with_nlp)
 
     port = config['api']['http']['port']
     host = config['api']['http']['host']
 
+    process_cache.init({
+        integration_controller.handler_modules['lightwood'].Handler: 4 if is_cloud else 1
+    })
+
     if server.lower() == 'waitress':
         serve(
             app,
             host='*' if host in ('', '0.0.0.0') else host,
             port=port,
             threads=16,
             max_request_body_size=1073741824 * 10,
```

### Comparing `MindsDB-23.6.5.1/mindsdb/api/http/utils.py` & `MindsDB-23.7.1.0/mindsdb/api/http/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/classes/responder.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/classes/scram.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/classes/session.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/company_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 class Responce(Responder):
     def when(self, query):
         return 'company_id' in query
 
     def result(self, query, request_env, mindsdb_env, session):
         company_id = query.get('company_id')
         user_class = query.get('user_class', 0)
+        email_confirmed = query.get('email_confirmed', 1)
         need_response = query.get('need_response', False)
 
         ctx.company_id = company_id
         ctx.user_class = user_class
+        ctx.email_confirmed = email_confirmed
 
         if need_response:
             return {'ok': 1}
 
         return None
```

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/delete.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/find.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/insert.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/insert.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/server.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-23.7.1.0/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     ErNotSupportedYet,
     SqlApiUnknownError,
     ErLogicError,
     ErSqlWrongArguments
 )
 from mindsdb.utilities.cache import get_cache, json_checksum
 import mindsdb.utilities.profiler as profiler
+from mindsdb.utilities.fs import create_process_mark, delete_process_mark
 
 
 superset_subquery = re.compile(r'from[\s\n]*(\(.*\))[\s\n]*as[\s\n]*virtual_table', flags=re.IGNORECASE | re.MULTILINE | re.S)
 
 
 def get_preditor_alias(step, mindsdb_database):
     predictor_name = '.'.join(step.predictor.parts)
@@ -663,24 +664,33 @@
 
     def execute_query(self, params=None):
         if self.fetched_data is not None:
             # no need to execute
             return
 
         steps_data = []
+        process_mark = None
         try:
-            for step in self.planner.execute_steps(params):
+            steps = list(self.planner.execute_steps(params))
+            steps_classes = (x.__class__ for x in steps)
+            predict_steps = (ApplyPredictorRowStep, ApplyPredictorStep, ApplyTimeseriesPredictorStep)
+            if any(s in predict_steps for s in steps_classes):
+                process_mark = create_process_mark('predict')
+            for step in steps:
                 with profiler.Context(f'step: {step.__class__.__name__}'):
                     data = self.execute_step(step, steps_data)
                 step.set_result(data)
                 steps_data.append(data)
         except PlanningException as e:
             raise ErLogicError(e)
         except Exception as e:
             raise e
+        finally:
+            if process_mark is not None:
+                delete_process_mark('predict', process_mark)
 
         # save updated query
         self.query = self.planner.query
 
         # there was no executing
         if len(steps_data) == 0:
             return
@@ -981,30 +991,27 @@
                         data = predictions.to_dict(orient='records')
                         columns_dtypes = dict(predictions.dtypes)
 
                         if data is not None and isinstance(data, list) and self.session.predictor_cache is not False:
                             predictor_cache.set(key, data)
                     else:
                         columns_dtypes = {}
-
                     if len(data) > 0:
                         cols = list(data[0].keys())
                         for col in cols:
                             result.add_column(Column(
                                 name=col,
                                 table_name=table_name[1],
                                 table_alias=table_name[2],
                                 database=table_name[0],
                                 type=columns_dtypes.get(col)
                             ))
-
                     # apply filter
                     if is_timeseries:
                         data = self.apply_ts_filter(data, where_data, step, predictor_metadata)
-
                     result.add_records(data)
 
                 data = result
 
             except Exception as e:
                 raise SqlApiUnknownError(f'error in apply predictor step: {e}') from e
         elif type(step) == JoinStep:
@@ -1423,14 +1430,15 @@
             return predictor_data
 
         def get_date_format(samples):
             # dateinfer reads sql date 2020-04-01 as yyyy-dd-mm. workaround for in
             for date_format, pattern in (
                 ('%Y-%m-%d', r'[\d]{4}-[\d]{2}-[\d]{2}'),
                 ('%Y-%m-%d %H:%M:%S', r'[\d]{4}-[\d]{2}-[\d]{2} [\d]{2}:[\d]{2}:[\d]{2}'),
+                # ('%Y-%m-%d %H:%M:%S%z', r'[\d]{4}-[\d]{2}-[\d]{2} [\d]{2}:[\d]{2}:[\d]{2}\+[\d]{2}:[\d]{2}'),
                 # ('%Y', '[\d]{4}')
             ):
                 if re.match(pattern, samples[0]):
                     # suggested format
                     for sample in samples:
                         try:
                             dt.datetime.strptime(sample, date_format)
```

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,19 +46,21 @@
         tables = self.project.get_tables()
         return table_name in tables
 
     def get_table_columns(self, table_name):
         return self.project.get_columns(table_name)
 
     def predict(self, model_name: str, data, version=None, params=None):
-        project_tables = self.project.get_tables()
-        predictor_table_meta = project_tables[model_name]
-        if predictor_table_meta['update_status'] == 'available':
+        model_metadata = self.project.get_model(model_name)
+        if model_metadata is None:
+            raise Exception(f"Can't find model '{model_name}'")
+        model_metadata = model_metadata['metadata']
+        if model_metadata['update_status'] == 'available':
             raise Exception(f"model '{model_name}' is obsolete and needs to be updated. Run 'RETRAIN {model_name};'")
-        handler = self.integration_controller.get_handler(predictor_table_meta['engine_name'])
+        handler = self.integration_controller.get_handler(model_metadata['engine_name'])
         return handler.predict(model_name, data, project_name=self.project.name, version=version, params=params)
 
     def query(self, query=None, native_query=None, session=None):
         if query is None and native_query is not None:
             query = parse_sql(native_query, dialect='mindsdb')
 
         # region is it query to 'models' or 'models_versions'?
```

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 from mindsdb.interfaces.database.projects import ProjectController
 from mindsdb.interfaces.jobs.jobs_controller import JobsController
 from mindsdb.interfaces.chatbot.chatbot_controller import ChatBotController
 from mindsdb.interfaces.storage.model_fs import HandlerStorage
 from mindsdb.utilities.context import context as ctx
 from mindsdb.utilities.functions import resolve_model_identifier
 import mindsdb.utilities.profiler as profiler
+from mindsdb.utilities.functions import mark_process
 
 
 def _get_show_where(
         statement: ASTNode,
         from_name: Optional[str] = None,
         like_name: Optional[str] = None,
         initial: Optional[ASTNode] = None,
@@ -729,15 +730,16 @@
             else:
                 return
 
         model_record = get_model_record(
             name=model_name,
             project_name=database_name,
             except_absent=except_absent,
-            version=model_version
+            version=model_version,
+            active=True if model_version is None else None
         )
         if not model_record:
             return None
         return {
             'model_record': model_record,
             'project_name': database_name
         }
@@ -806,14 +808,16 @@
         columns = [
             Column(col)
             for col in resp_dict['columns']
         ]
 
         return ExecuteAnswer(answer_type=ANSWER_TYPE.TABLE, columns=columns, data=resp_dict['data'])
 
+    @profiler.profile()
+    @mark_process('learn')
     def answer_finetune_predictor(self, statement):
         model_record = self._get_model_info(statement.name)['model_record']
 
         if statement.using is not None:
             # repack using with lower names
             statement.using = {k.lower(): v for k, v in statement.using.items()}
 
@@ -1093,14 +1097,15 @@
             else:
                 db_name = self.session.database
             project = self.session.database_controller.get_project(db_name)
             project.drop_table(view_name)
 
         return ExecuteAnswer(answer_type=ANSWER_TYPE.OK)
 
+    @mark_process('learn')
     def answer_create_predictor(self, statement):
         integration_name = self.session.database
         if len(statement.name.parts) > 1:
             integration_name = statement.name.parts[0]
         else:
             statement.name.parts = [integration_name, statement.name.parts[-1]]
         integration_name = integration_name.lower()
```

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,28 +411,33 @@
             client_capabilities = struct.unpack('L', client_capabilities)[0]
 
             company_id = self.request.recv(4)
             company_id = struct.unpack('I', company_id)[0]
 
             user_class = self.request.recv(1)
             user_class = struct.unpack('B', user_class)[0]
+            email_confirmed = 1
+            if user_class > 1:
+                email_confirmed = (user_class >> 2) & 1
+            user_class = user_class & 3
 
             database_name_len = self.request.recv(2)
             database_name_len = struct.unpack('H', database_name_len)[0]
 
             database_name = ''
             if database_name_len > 0:
                 database_name = self.request.recv(database_name_len).decode()
 
             return {
                 'is_cloud': True,
                 'client_capabilities': client_capabilities,
                 'company_id': company_id,
                 'user_class': user_class,
-                'database': database_name
+                'database': database_name,
+                'email_confirmed': email_confirmed,
             }
 
         return {
             'is_cloud': False
         }
 
     def to_mysql_columns(self, columns_list):
@@ -628,14 +633,15 @@
 
         self.init_session()
         if cloud_connection['is_cloud'] is False:
             if self.handshake() is False:
                 return
         else:
             ctx.user_class = cloud_connection['user_class']
+            ctx.email_confirmed = cloud_connection['email_confirmed']
             self.client_capabilities = ClentCapabilities(cloud_connection['client_capabilities'])
             self.session.database = cloud_connection['database']
             self.session.username = 'cloud'
             self.session.auth = True
 
         while True:
             logger.debug('Got a new packet')
```

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py` & `MindsDB-23.7.1.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/nlp/nlp.py` & `MindsDB-23.7.1.0/mindsdb/api/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py` & `MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py` & `MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py` & `MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py` & `MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py` & `MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py` & `MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py` & `MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py` & `MindsDB-23.7.1.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/autokeras_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/autokeras_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/config.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/binance_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/binance_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/logo.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/logo.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/cohere_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/cohere_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/confluence_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/confluence_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/logo.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/flaml_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/flaml_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/frappe_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/frappe_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/github_handler/github_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/github_handler/github_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/github_handler/github_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/github_handler/github_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/github_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/github_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_fit_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_fit_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_api_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/huggingface_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/huggingface_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/jira_handler/jira_table.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/jira_handler/jira_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/langchain_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/langchain_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from mindsdb.integrations.utilities.utils import format_exception_error
 from mindsdb.interfaces.model.functions import (
     get_model_records
 )
 from mindsdb.interfaces.storage import db
 from mindsdb.interfaces.storage.fs import FileStorage, RESOURCE_GROUP
 from mindsdb.interfaces.storage.json import get_json_storage
+import mindsdb.utilities.profiler as profiler
 
 from .utils import rep_recur, brack_to_mod, unpack_jsonai_old_args
 
 
 def create_learn_mark():
     if os.name == 'posix':
         p = Path(tempfile.gettempdir()).joinpath('mindsdb/learn_processes/')
@@ -38,14 +39,15 @@
     if os.name == 'posix':
         p = Path(tempfile.gettempdir()).joinpath('mindsdb/learn_processes/').joinpath(f'{os.getpid()}')
         if p.exists():
             p.unlink()
 
 
 @mark_process(name='learn')
+@profiler.profile()
 def run_generate(df: DataFrame, predictor_id: int, model_storage, args: dict = None):
 
     model_storage.training_state_set(current_state_num=1, total_states=5, state_name='Generating problem definition')
     json_ai_override = args.pop('using', {})
 
     if 'dtype_dict' in json_ai_override:
         args['dtype_dict'] = json_ai_override.pop('dtype_dict')
@@ -79,14 +81,15 @@
     json_storage = get_json_storage(
         resource_id=predictor_id
     )
     json_storage.set('json_ai', json_ai.to_dict())
 
 
 @mark_process(name='learn')
+@profiler.profile()
 def run_fit(predictor_id: int, df: pd.DataFrame, model_storage) -> None:
     try:
         predictor_record = db.Predictor.query.with_for_update().get(predictor_id)
         assert predictor_record is not None
 
         predictor_record.data = {'training_log': 'training'}
         predictor_record.status = PREDICTOR_STATUS.TRAINING
@@ -163,21 +166,20 @@
     db.session.commit()
 
 
 @mark_process(name='finetune')
 def run_finetune(df: DataFrame, args: dict, model_storage):
     try:
         base_predictor_id = args['base_model_id']
-        base_predictor_record = db.Predictor.query.filter_by(
-            id=base_predictor_id,
-            status=PREDICTOR_STATUS.COMPLETE
-        ).first()
+        base_predictor_record = db.Predictor.query.get(base_predictor_id)
+        if base_predictor_record.status != PREDICTOR_STATUS.COMPLETE:
+            raise Exception("Base model must be in status 'complete'")
 
         predictor_id = model_storage.predictor_id
-        predictor_record = db.Predictor.query.filter_by(id=predictor_id).first()
+        predictor_record = db.Predictor.query.get(predictor_id)
 
         # TODO move this to ModelStorage (don't work with database directly)
         predictor_record.data = {'training_log': 'training'}
         predictor_record.training_start_at = datetime.now()
         predictor_record.status = PREDICTOR_STATUS.FINETUNING  # TODO: parallel execution block
         db.session.commit()
 
@@ -201,25 +203,14 @@
         predictor_record.data = predictor.model_analysis.to_dict()  # todo: update accuracy in LW as post-finetune hook
         predictor_record.code = base_predictor_record.code
         predictor_record.update_status = 'up_to_date'
         predictor_record.status = PREDICTOR_STATUS.COMPLETE
         predictor_record.training_stop_at = datetime.now()
         db.session.commit()
 
-        predictor_records = get_model_records(
-            active=None,
-            name=predictor_record.name,
-        )
-        predictor_records = [
-            x for x in predictor_records
-            if x.training_stop_at is not None
-        ]
-        predictor_records.sort(key=lambda x: x.training_stop_at)
-        db.session.commit()
-
     except Exception as e:
         log.logger.error(e)
         predictor_id = model_storage.predictor_id
         predictor_record = db.Predictor.query.with_for_update().get(predictor_id)
         print(traceback.format_exc())
         error_message = format_exception_error(e)
         predictor_record.data = {"error": error_message}
```

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,279 +98,280 @@
             predictor = LightwoodHandler.get_predictor(predictor_path, predictor_code)
 
         dtype_dict = predictor.dtype_dict
 
         with profiler.Context('predict'):
             predictions = predictor.predict(df, args=pred_args)
 
-        predictions = predictions.to_dict(orient='records')
+        with profiler.Context('predict-postprocessing'):
+            predictions = predictions.to_dict(orient='records')
 
-        # TODO!!!
-        # after_predict_hook(
-        #     company_id=self.company_id,
-        #     predictor_id=predictor_record.id,
-        #     rows_in_count=df.shape[0],
-        #     columns_in_count=df.shape[1],
-        #     rows_out_count=len(predictions)
-        # )
-
-        # region format result
-        target = args['target']
-        explain_arr = []
-        pred_dicts = []
-        for i, row in enumerate(predictions):
-            values = {
-                'predicted_value': row['prediction'],
-                'confidence': row.get('confidence', None),
-                'anomaly': row.get('anomaly', None),
-                'truth': row.get('truth', None)
-            }
-
-            if predictor.supports_proba:
-                for cls in predictor.statistical_analysis.train_observed_classes:
-                    if row.get(f'__mdb_proba_{cls}', False):
-                        values[f'probability_class_{cls}'] = round(row[f'__mdb_proba_{cls}'], 4)
-
-            for block in predictor.analysis_blocks:
-                if type(block).__name__ == 'ShapleyValues':
-                    cols = block.columns
-                    values['shap_base_response'] = round(row['shap_base_response'], 4)
-                    values['shap_final_response'] = round(row['shap_final_response'], 4)
-                    for col in cols:
-                        values[f'shap_contribution_{col}'] = round(row[f'shap_contribution_{col}'], 4)
-
-            if 'lower' in row:
-                values['confidence_lower_bound'] = row.get('lower', None)
-                values['confidence_upper_bound'] = row.get('upper', None)
-
-            obj = {target: values}
-            explain_arr.append(obj)
-
-            td = {'predicted_value': row['prediction']}
-            for col in df.columns:
-                if col in row:
-                    td[col] = row[col]
-                elif f'order_{col}' in row:
-                    td[col] = row[f'order_{col}']
-                elif f'group_{col}' in row:
-                    td[col] = row[f'group_{col}']
-                else:
-                    orginal_index = row.get('original_index')
-                    if orginal_index is None:
-                        orginal_index = i
-                    td[col] = df.iloc[orginal_index][col]
-            pred_dicts.append({target: td})
-
-        new_pred_dicts = []
-        for row in pred_dicts:
-            new_row = {}
-            for key in row:
-                new_row.update(row[key])
-                new_row[key] = new_row['predicted_value']
-            del new_row['predicted_value']
-            new_pred_dicts.append(new_row)
-        pred_dicts = new_pred_dicts
-
-        columns = list(dtype_dict.keys())
-        predicted_columns = target
-        if not isinstance(predicted_columns, list):
-            predicted_columns = [predicted_columns]
-        # endregion
-
-        original_target_values = {}
-        for col in predicted_columns:
-            df = df.reset_index()
-            original_target_values[col + '_original'] = []
-            for _index, row in df.iterrows():
-                original_target_values[col + '_original'].append(row.get(col))
-
-        # region transform ts predictions
-        timeseries_settings = learn_args.get('timeseries_settings', {'is_timeseries': False})
-
-        if timeseries_settings['is_timeseries'] is True:
-            # offset forecast if have __mdb_forecast_offset > 0
-            forecast_offset = any([
-                row.get('__mdb_forecast_offset') is not None and row['__mdb_forecast_offset'] > 0
-                for row in pred_dicts
-            ])
-
-            group_by = timeseries_settings.get('group_by', [])
-            order_by_column = timeseries_settings['order_by']
-            if isinstance(order_by_column, list):
-                order_by_column = order_by_column[0]
-            horizon = timeseries_settings['horizon']
-
-            # region convert values to lists in case of horizon==1.
-            # That needs to make processing below unified for any case.
-            if horizon == 1:
-                for row in pred_dicts:
-                    if isinstance(row[order_by_column], list) is False:
-                        row[order_by_column] = [row[order_by_column]]
-                    if isinstance(row[target], list) is False:
-                        row[target] = [row[target]]
-                for row in explain_arr:
-                    for col in ('predicted_value', 'confidence', 'confidence_lower_bound', 'confidence_upper_bound'):
-                        if isinstance(row[target][col], list) is False:
-                            row[target][col] = [row[target][col]]
+            # TODO!!!
+            # after_predict_hook(
+            #     company_id=self.company_id,
+            #     predictor_id=predictor_record.id,
+            #     rows_in_count=df.shape[0],
+            #     columns_in_count=df.shape[1],
+            #     rows_out_count=len(predictions)
+            # )
+
+            # region format result
+            target = args['target']
+            explain_arr = []
+            pred_dicts = []
+            for i, row in enumerate(predictions):
+                values = {
+                    'predicted_value': row['prediction'],
+                    'confidence': row.get('confidence', None),
+                    'anomaly': row.get('anomaly', None),
+                    'truth': row.get('truth', None)
+                }
+
+                if predictor.supports_proba:
+                    for cls in predictor.statistical_analysis.train_observed_classes:
+                        if row.get(f'__mdb_proba_{cls}', False):
+                            values[f'probability_class_{cls}'] = round(row[f'__mdb_proba_{cls}'], 4)
+
+                for block in predictor.analysis_blocks:
+                    if type(block).__name__ == 'ShapleyValues':
+                        cols = block.columns
+                        values['shap_base_response'] = round(row['shap_base_response'], 4)
+                        values['shap_final_response'] = round(row['shap_final_response'], 4)
+                        for col in cols:
+                            values[f'shap_contribution_{col}'] = round(row[f'shap_contribution_{col}'], 4)
+
+                if 'lower' in row:
+                    values['confidence_lower_bound'] = row.get('lower', None)
+                    values['confidence_upper_bound'] = row.get('upper', None)
+
+                obj = {target: values}
+                explain_arr.append(obj)
+
+                td = {'predicted_value': row['prediction']}
+                for col in df.columns:
+                    if col in row:
+                        td[col] = row[col]
+                    elif f'order_{col}' in row:
+                        td[col] = row[f'order_{col}']
+                    elif f'group_{col}' in row:
+                        td[col] = row[f'group_{col}']
+                    else:
+                        orginal_index = row.get('original_index')
+                        if orginal_index is None:
+                            orginal_index = i
+                        td[col] = df.iloc[orginal_index][col]
+                pred_dicts.append({target: td})
+
+            new_pred_dicts = []
+            for row in pred_dicts:
+                new_row = {}
+                for key in row:
+                    new_row.update(row[key])
+                    new_row[key] = new_row['predicted_value']
+                del new_row['predicted_value']
+                new_pred_dicts.append(new_row)
+            pred_dicts = new_pred_dicts
+
+            columns = list(dtype_dict.keys())
+            predicted_columns = target
+            if not isinstance(predicted_columns, list):
+                predicted_columns = [predicted_columns]
             # endregion
 
-            if len(group_by) == 0:
-                rows_by_groups = {
-                    (): {
-                        'rows': pred_dicts,
-                        'explanations': explain_arr
-                    }
-                }
-            else:
-                groups = set()
-                for row in pred_dicts:
-                    groups.add(
-                        tuple([row[x] for x in group_by])
-                    )
-
-                # split rows by groups
-                rows_by_groups = {}
-                for group in groups:
-                    rows_by_groups[group] = {
-                        'rows': [],
-                        'explanations': []
+            original_target_values = {}
+            for col in predicted_columns:
+                df = df.reset_index()
+                original_target_values[col + '_original'] = []
+                for _index, row in df.iterrows():
+                    original_target_values[col + '_original'].append(row.get(col))
+
+            # region transform ts predictions
+            timeseries_settings = learn_args.get('timeseries_settings', {'is_timeseries': False})
+
+            if timeseries_settings['is_timeseries'] is True:
+                # offset forecast if have __mdb_forecast_offset > 0
+                forecast_offset = any([
+                    row.get('__mdb_forecast_offset') is not None and row['__mdb_forecast_offset'] > 0
+                    for row in pred_dicts
+                ])
+
+                group_by = timeseries_settings.get('group_by', [])
+                order_by_column = timeseries_settings['order_by']
+                if isinstance(order_by_column, list):
+                    order_by_column = order_by_column[0]
+                horizon = timeseries_settings['horizon']
+
+                # region convert values to lists in case of horizon==1.
+                # That needs to make processing below unified for any case.
+                if horizon == 1:
+                    for row in pred_dicts:
+                        if isinstance(row[order_by_column], list) is False:
+                            row[order_by_column] = [row[order_by_column]]
+                        if isinstance(row[target], list) is False:
+                            row[target] = [row[target]]
+                    for row in explain_arr:
+                        for col in ('predicted_value', 'confidence', 'confidence_lower_bound', 'confidence_upper_bound'):
+                            if isinstance(row[target][col], list) is False:
+                                row[target][col] = [row[target][col]]
+                # endregion
+
+                if len(group_by) == 0:
+                    rows_by_groups = {
+                        (): {
+                            'rows': pred_dicts,
+                            'explanations': explain_arr
+                        }
                     }
-                    for row_index, row in enumerate(pred_dicts):
-                        is_wrong_group = False
-                        for i, group_by_key in enumerate(group_by):
-                            if row[group_by_key] != group[i]:
-                                is_wrong_group = True
-                                break
-                        if not is_wrong_group:
-                            rows_by_groups[group]['rows'].append(row)
-                            rows_by_groups[group]['explanations'].append(explain_arr[row_index])
-
-            for group, data in rows_by_groups.items():
-                rows = data['rows']
-                explanations = data['explanations']
-
-                if len(rows) == 0:
-                    break
-
-                for row in rows:
-                    predictions = row[target]
-                    if isinstance(predictions, list) is False:
-                        predictions = [predictions]
-
-                    date_values = row[order_by_column]
-                    if isinstance(date_values, list) is False:
-                        date_values = [date_values]
-
-                if pred_args.get('force_ts_infer') is True:
-                    # last row contains one additional prediction (used for cases like date > '2020-10-10').
-                    # Extract that prediction from there and join to previous row
-                    rows[-2][order_by_column] = rows[-2][order_by_column].copy()
-                    rows[-2][target] = rows[-2][target].copy()
-
-                    rows[-2][order_by_column].append(rows[-1][order_by_column][-1])
-                    rows[-2][target].append(rows[-1][target][-1])
-                    for col in ('predicted_value', 'confidence', 'confidence_lower_bound', 'confidence_upper_bound'):
-                        explanations[-2][target][col].append(explanations[-1][target][col][-1])
-                    rows.pop()
-                    explanations.pop()
-                    # horizon = horizon + 1
-
-                for i in range(len(rows) - 1):
-                    row_horizon = len(rows[i][target])
-                    if row_horizon > 1:
-                        rows[i][target] = rows[i][target][0]
-                        if isinstance(rows[i][order_by_column], list):
-                            rows[i][order_by_column] = rows[i][order_by_column][0]
-                    for col in ('predicted_value', 'confidence', 'confidence_lower_bound', 'confidence_upper_bound'):
-                        if row_horizon > 1 and col in explanations[i][target]:
-                            explanations[i][target][col] = explanations[i][target][col][0]
-
-                last_row = rows.pop()
-                last_explanation = explanations.pop()
-                for i in range(len(last_row[target])):
-                    new_row = copy.deepcopy(last_row)
-                    new_row[target] = new_row[target][i]
-                    if isinstance(new_row[order_by_column], list):
-                        new_row[order_by_column] = new_row[order_by_column][i]
-                    if '__mindsdb_row_id' in new_row and (i > 0 or forecast_offset):
-                        new_row['__mindsdb_row_id'] = None
-
-                    new_explanation = copy.deepcopy(last_explanation)
-                    for col in ('predicted_value', 'confidence', 'confidence_lower_bound', 'confidence_upper_bound'):
-                        if col in new_explanation[target]:
-                            new_explanation[target][col] = new_explanation[target][col][i]
-                    if i != 0:
-                        new_explanation[target]['anomaly'] = None
-                        new_explanation[target]['truth'] = None
+                else:
+                    groups = set()
+                    for row in pred_dicts:
+                        groups.add(
+                            tuple([row[x] for x in group_by])
+                        )
+
+                    # split rows by groups
+                    rows_by_groups = {}
+                    for group in groups:
+                        rows_by_groups[group] = {
+                            'rows': [],
+                            'explanations': []
+                        }
+                        for row_index, row in enumerate(pred_dicts):
+                            is_wrong_group = False
+                            for i, group_by_key in enumerate(group_by):
+                                if row[group_by_key] != group[i]:
+                                    is_wrong_group = True
+                                    break
+                            if not is_wrong_group:
+                                rows_by_groups[group]['rows'].append(row)
+                                rows_by_groups[group]['explanations'].append(explain_arr[row_index])
+
+                for group, data in rows_by_groups.items():
+                    rows = data['rows']
+                    explanations = data['explanations']
+
+                    if len(rows) == 0:
+                        break
+
+                    for row in rows:
+                        predictions = row[target]
+                        if isinstance(predictions, list) is False:
+                            predictions = [predictions]
+
+                        date_values = row[order_by_column]
+                        if isinstance(date_values, list) is False:
+                            date_values = [date_values]
+
+                    if pred_args.get('force_ts_infer') is True:
+                        # last row contains one additional prediction (used for cases like date > '2020-10-10').
+                        # Extract that prediction from there and join to previous row
+                        rows[-2][order_by_column] = rows[-2][order_by_column].copy()
+                        rows[-2][target] = rows[-2][target].copy()
+
+                        rows[-2][order_by_column].append(rows[-1][order_by_column][-1])
+                        rows[-2][target].append(rows[-1][target][-1])
+                        for col in ('predicted_value', 'confidence', 'confidence_lower_bound', 'confidence_upper_bound'):
+                            explanations[-2][target][col].append(explanations[-1][target][col][-1])
+                        rows.pop()
+                        explanations.pop()
+                        # horizon = horizon + 1
+
+                    for i in range(len(rows) - 1):
+                        row_horizon = len(rows[i][target])
+                        if row_horizon > 1:
+                            rows[i][target] = rows[i][target][0]
+                            if isinstance(rows[i][order_by_column], list):
+                                rows[i][order_by_column] = rows[i][order_by_column][0]
+                        for col in ('predicted_value', 'confidence', 'confidence_lower_bound', 'confidence_upper_bound'):
+                            if row_horizon > 1 and col in explanations[i][target]:
+                                explanations[i][target][col] = explanations[i][target][col][0]
+
+                    last_row = rows.pop()
+                    last_explanation = explanations.pop()
+                    for i in range(len(last_row[target])):
+                        new_row = copy.deepcopy(last_row)
+                        new_row[target] = new_row[target][i]
+                        if isinstance(new_row[order_by_column], list):
+                            new_row[order_by_column] = new_row[order_by_column][i]
+                        if '__mindsdb_row_id' in new_row and (i > 0 or forecast_offset):
+                            new_row['__mindsdb_row_id'] = None
+
+                        new_explanation = copy.deepcopy(last_explanation)
+                        for col in ('predicted_value', 'confidence', 'confidence_lower_bound', 'confidence_upper_bound'):
+                            if col in new_explanation[target]:
+                                new_explanation[target][col] = new_explanation[target][col][i]
+                        if i != 0:
+                            new_explanation[target]['anomaly'] = None
+                            new_explanation[target]['truth'] = None
+
+                        rows.append(new_row)
+                        explanations.append(new_explanation)
+
+                pred_dicts = []
+                explanations = []
+                for group, data in rows_by_groups.items():
+                    pred_dicts.extend(data['rows'])
+                    explanations.extend(data['explanations'])
+
+                original_target_values[f'{target}_original'] = []
+                for i in range(len(pred_dicts)):
+                    original_target_values[f'{target}_original'].append(explanations[i][target].get('truth', None))
+
+                if dtype_dict[order_by_column] == dtype.date:
+                    for row in pred_dicts:
+                        if isinstance(row[order_by_column], (int, float)):
+                            row[order_by_column] = datetime.fromtimestamp(row[order_by_column]).date()
+                elif dtype_dict[order_by_column] == dtype.datetime:
+                    for row in pred_dicts:
+                        if isinstance(row[order_by_column], (int, float)):
+                            row[order_by_column] = datetime.fromtimestamp(row[order_by_column])
 
-                    rows.append(new_row)
-                    explanations.append(new_explanation)
+                explain_arr = explanations
+            # endregion
 
-            pred_dicts = []
-            explanations = []
-            for group, data in rows_by_groups.items():
-                pred_dicts.extend(data['rows'])
-                explanations.extend(data['explanations'])
-
-            original_target_values[f'{target}_original'] = []
-            for i in range(len(pred_dicts)):
-                original_target_values[f'{target}_original'].append(explanations[i][target].get('truth', None))
-
-            if dtype_dict[order_by_column] == dtype.date:
-                for row in pred_dicts:
-                    if isinstance(row[order_by_column], (int, float)):
-                        row[order_by_column] = datetime.fromtimestamp(row[order_by_column]).date()
-            elif dtype_dict[order_by_column] == dtype.datetime:
-                for row in pred_dicts:
-                    if isinstance(row[order_by_column], (int, float)):
-                        row[order_by_column] = datetime.fromtimestamp(row[order_by_column])
-
-            explain_arr = explanations
-        # endregion
-
-        if pred_format == 'explain':
-            return explain_arr
-
-        keys = [x for x in pred_dicts[0] if x in columns]
-        min_max_keys = []
-        for col in predicted_columns:
-            if dtype_dict[col] in (dtype.integer, dtype.float, dtype.num_tsarray):
-                min_max_keys.append(col)
-
-        data = []
-        explains = []
-        keys_to_save = [*keys, '__mindsdb_row_id', 'select_data_query', 'when_data']
-        for i, el in enumerate(pred_dicts):
-            data.append({key: el.get(key) for key in keys_to_save})
-            explains.append(explain_arr[i])
-
-        for i, row in enumerate(data):
-            cast_row_types(row, dtype_dict)
-
-            for k in original_target_values:
-                try:
-                    row[k] = original_target_values[k][i]
-                except Exception:
-                    row[k] = None
-
-            for column_name in columns:
-                if column_name not in row:
-                    row[column_name] = None
-
-            explanation = explains[i]
-            for key in predicted_columns:
-                row[key + '_confidence'] = explanation[key]['confidence']
-                row[key + '_explain'] = json.dumps(explanation[key], cls=NumpyJSONEncoder, ensure_ascii=False)
-                if 'anomaly' in explanation[key]:
-                    row[key + '_anomaly'] = explanation[key]['anomaly']
-            for key in min_max_keys:
-                if 'confidence_lower_bound' in explanation[key]:
-                    row[key + '_min'] = explanation[key]['confidence_lower_bound']
-                if 'confidence_upper_bound' in explanation[key]:
-                    row[key + '_max'] = explanation[key]['confidence_upper_bound']
+            if pred_format == 'explain':
+                return explain_arr
+
+            keys = [x for x in pred_dicts[0] if x in columns]
+            min_max_keys = []
+            for col in predicted_columns:
+                if dtype_dict[col] in (dtype.integer, dtype.float, dtype.num_tsarray):
+                    min_max_keys.append(col)
+
+            data = []
+            explains = []
+            keys_to_save = [*keys, '__mindsdb_row_id', 'select_data_query', 'when_data']
+            for i, el in enumerate(pred_dicts):
+                data.append({key: el.get(key) for key in keys_to_save})
+                explains.append(explain_arr[i])
+
+            for i, row in enumerate(data):
+                cast_row_types(row, dtype_dict)
+
+                for k in original_target_values:
+                    try:
+                        row[k] = original_target_values[k][i]
+                    except Exception:
+                        row[k] = None
+
+                for column_name in columns:
+                    if column_name not in row:
+                        row[column_name] = None
+
+                explanation = explains[i]
+                for key in predicted_columns:
+                    row[key + '_confidence'] = explanation[key]['confidence']
+                    row[key + '_explain'] = json.dumps(explanation[key], cls=NumpyJSONEncoder, ensure_ascii=False)
+                    if 'anomaly' in explanation[key]:
+                        row[key + '_anomaly'] = explanation[key]['anomaly']
+                for key in min_max_keys:
+                    if 'confidence_lower_bound' in explanation[key]:
+                        row[key + '_min'] = explanation[key]['confidence_lower_bound']
+                    if 'confidence_upper_bound' in explanation[key]:
+                        row[key + '_max'] = explanation[key]['confidence_upper_bound']
 
         return pd.DataFrame(data)
 
     def edit_json_ai(self, name: str, json_ai: dict):
         predictor_record = get_model_record(name=name, ml_handler_name='lightwood')
         assert predictor_record is not None
```

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/llama_index_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/llama_index_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/llama_index_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ludwig_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ludwig_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/merlion_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/merlion_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mlflow_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mlflow_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/create-database.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/monkeylearn_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/monkeylearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import concurrent.futures
 from typing import Optional, Dict
 
 import openai
 import numpy as np
 import pandas as pd
 
+from mindsdb.utilities.hooks import before_openai_query, after_openai_query
 from mindsdb.utilities import log
 from mindsdb.utilities.config import Config
 from mindsdb.integrations.libs.base import BaseMLEngine
 from mindsdb.integrations.handlers.openai_handler.helpers import retry_with_exponential_backoff, \
     truncate_msgs_for_token_limit
 
 CHAT_MODELS = ('gpt-3.5-turbo', 'gpt-3.5-turbo-0301', 'gpt-4', 'gpt-4-0314', 'gpt-4-32k', 'gpt-4-32k-0314')
@@ -285,14 +286,16 @@
                 return _submit_image_completion(kwargs, prompts, api_args)
             elif model_name in self.chat_completion_models:
                 return _submit_chat_completion(kwargs, prompts, api_args, df, mode=args.get('mode', 'conversational'))
             else:
                 return _submit_normal_completion(kwargs, prompts, api_args)
 
         def _log_api_call(params, response):
+            after_openai_query(params, response)
+
             params2 = params.copy()
             params2.pop('api_key', None)
             params2.pop('user', None)
             log.logger.debug(f'>>>openai call: {params2}:\n{response}')
 
         def _submit_normal_completion(kwargs, prompts, api_args):
             def _tidy(comp):
@@ -301,14 +304,15 @@
                     if 'text' in c:
                         tidy_comps.append(c['text'].strip('\n').strip(''))
                 return tidy_comps
 
             kwargs['prompt'] = prompts
             kwargs = {**kwargs, **api_args}
 
+            before_openai_query(kwargs)
             resp = _tidy(openai.Completion.create(**kwargs))
             _log_api_call(kwargs, resp)
             return resp
 
         def _submit_chat_completion(kwargs, prompts, api_args, df, mode='conversational'):
             def _tidy(comp):
                 tidy_comps = []
@@ -339,22 +343,25 @@
                         kwargs['messages'].append({'role': 'assistant', 'content': answer})
 
                 if mode == 'conversational-full' or (mode == 'conversational' and pidx == len(prompts) - 1):
                     kwargs['messages'] = truncate_msgs_for_token_limit(kwargs['messages'],
                                                                        kwargs['model'],
                                                                        api_args['max_tokens'])
                     pkwargs = {**kwargs, **api_args}
+
+                    before_openai_query(kwargs)
                     resp = _tidy(openai.ChatCompletion.create(**pkwargs))
                     _log_api_call(pkwargs, resp)
 
                     completions.extend(resp)
                 elif mode == 'default':
                     kwargs['messages'] = [initial_prompt] + [kwargs['messages'][-1]]
                     pkwargs = {**kwargs, **api_args}
 
+                    before_openai_query(kwargs)
                     resp = _tidy(openai.ChatCompletion.create(**pkwargs))
                     _log_api_call(pkwargs, resp)
 
                     completions.extend(resp)
                 else:
                     # in "normal" conversational mode, we request completions only for the last row
                     last_completion_content = None
```

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/openai_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/openai_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/paypal_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/paypal_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/drop-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/planetscale_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/postgres_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/postgres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/realtime_slack_chat_handler/realtime_slack_chat_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/realtime_slack_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/reddit_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/reddit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/rockset_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/rockset_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/logo.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/shopify_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/shopify_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,159 +1,157 @@
-import shopify
 import pandas as pd
 from typing import Text, List, Dict
 
 from mindsdb_sql.parser import ast
 from mindsdb.integrations.libs.api_handler import APITable
 
-from mindsdb.integrations.handlers.utilities.query_utilities import SELECTQueryParser, SELECTQueryExecutor
+from mindsdb.integrations.handlers.utilities.query_utilities.select_query_utilities import SELECTQueryParser, SELECTQueryExecutor
 
 
-class ProductsTable(APITable):
-    """The Shopify Products Table implementation"""
+class CustomersTable(APITable):
+    """The Stripe Customers Table implementation"""
 
     def select(self, query: ast.Select) -> pd.DataFrame:
-        """Pulls data from the Shopify "GET /products" API endpoint.
+        """
+        Pulls Stripe Customer data.
 
         Parameters
         ----------
         query : ast.Select
            Given SQL SELECT query
 
         Returns
         -------
         pd.DataFrame
-            Shopify Products matching the query
+            Stripe Customers matching the query
 
         Raises
         ------
         ValueError
             If the query contains an unsupported condition
         """
 
         select_statement_parser = SELECTQueryParser(
             query,
-            'products',
+            'customers',
             self.get_columns()
         )
         selected_columns, where_conditions, order_by_conditions, result_limit = select_statement_parser.parse_query()
 
-        products_df = pd.json_normalize(self.get_products(limit=result_limit))
-
+        customers_df = pd.json_normalize(self.get_customers(limit=result_limit))
         select_statement_executor = SELECTQueryExecutor(
-            products_df,
+            customers_df,
             selected_columns,
             where_conditions,
             order_by_conditions
         )
-        products_df = select_statement_executor.execute_query()
+        customers_df = select_statement_executor.execute_query()
 
-        return products_df
+        return customers_df
 
     def get_columns(self) -> List[Text]:
-        return pd.json_normalize(self.get_products(limit=1)).columns.tolist()
+        return pd.json_normalize(self.get_customers(limit=1)).columns.tolist()
 
-    def get_products(self, **kwargs) -> List[Dict]:
-        api_session = self.handler.connect()
-        shopify.ShopifyResource.activate_session(api_session)
-        products = shopify.Product.find(**kwargs)
-        return [product.to_dict() for product in products]
+    def get_customers(self, **kwargs) -> List[Dict]:
+        stripe = self.handler.connect()
+        customers = stripe.Customer.list(**kwargs)
+        return [customer.to_dict() for customer in customers]
 
 
-class CustomersTable(APITable):
-    """The Shopify Customers Table implementation"""
+class ProductsTable(APITable):
+    """The Stripe Products Table implementation"""
 
     def select(self, query: ast.Select) -> pd.DataFrame:
-        """Pulls data from the Shopify "GET /customers" API endpoint.
+        """
+        Pulls Stripe Product data.
 
         Parameters
         ----------
         query : ast.Select
            Given SQL SELECT query
 
         Returns
         -------
         pd.DataFrame
-            Shopify Customers matching the query
+            Stripe Products matching the query
 
         Raises
         ------
         ValueError
             If the query contains an unsupported condition
         """
+
         select_statement_parser = SELECTQueryParser(
             query,
-            'customers',
+            'products',
             self.get_columns()
         )
         selected_columns, where_conditions, order_by_conditions, result_limit = select_statement_parser.parse_query()
 
-        customers_df = pd.json_normalize(self.get_customers(limit=result_limit))
-
+        products_df = pd.json_normalize(self.get_products(limit=result_limit))
         select_statement_executor = SELECTQueryExecutor(
-            customers_df,
+            products_df,
             selected_columns,
             where_conditions,
             order_by_conditions
         )
-        customers_df = select_statement_executor.execute_query()
+        products_df = select_statement_executor.execute_query()
 
-        return customers_df
+        return products_df
 
     def get_columns(self) -> List[Text]:
-        return pd.json_normalize(self.get_customers(limit=1)).columns.tolist()
+        return pd.json_normalize(self.get_products(limit=1)).columns.tolist()
 
-    def get_customers(self, **kwargs) -> List[Dict]:
-        api_session = self.handler.connect()
-        shopify.ShopifyResource.activate_session(api_session)
-        customers = shopify.Customer.find(**kwargs)
-        return [customer.to_dict() for customer in customers]
+    def get_products(self, **kwargs) -> List[Dict]:
+        stripe = self.handler.connect()
+        products = stripe.Product.list(**kwargs)
+        return [product.to_dict() for product in products]
 
 
-class OrdersTable(APITable):
-    """The Shopify Orders Table implementation"""
+class PaymentIntentsTable(APITable):
+    """The Stripe Payment Intents Table implementation"""
 
     def select(self, query: ast.Select) -> pd.DataFrame:
-        """Pulls data from the Shopify "GET /orders" API endpoint.
+        """
+        Pulls Stripe Payment Intents data.
 
         Parameters
         ----------
         query : ast.Select
            Given SQL SELECT query
 
         Returns
         -------
         pd.DataFrame
-            Shopify Orders matching the query
+            Stripe Payment Intents matching the query
 
         Raises
         ------
         ValueError
             If the query contains an unsupported condition
         """
+
         select_statement_parser = SELECTQueryParser(
             query,
-            'orders',
+            'payment_intents',
             self.get_columns()
         )
         selected_columns, where_conditions, order_by_conditions, result_limit = select_statement_parser.parse_query()
 
-        orders_df = pd.json_normalize(self.get_orders(limit=result_limit))
-
+        payment_intents_df = pd.json_normalize(self.get_payment_intents(limit=result_limit))
         select_statement_executor = SELECTQueryExecutor(
-            orders_df,
+            payment_intents_df,
             selected_columns,
             where_conditions,
             order_by_conditions
         )
-        orders_df = select_statement_executor.execute_query()
+        payment_intents_df = select_statement_executor.execute_query()
 
-        return orders_df
+        return payment_intents_df
 
     def get_columns(self) -> List[Text]:
-        return pd.json_normalize(self.get_orders(limit=1)).columns.tolist()
+        return pd.json_normalize(self.get_payment_intents(limit=1)).columns.tolist()
 
-    def get_orders(self, **kwargs) -> List[Dict]:
-        api_session = self.handler.connect()
-        shopify.ShopifyResource.activate_session(api_session)
-        orders = shopify.Order.find(**kwargs)
-        return [order.to_dict() for order in orders]
+    def get_payment_intents(self, **kwargs) -> List[Dict]:
+        stripe = self.handler.connect()
+        payment_intents = stripe.PaymentIntent.list(**kwargs)
+        return [payment_intent.to_dict() for payment_intent in payment_intents]
```

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/solr.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/solr.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/error.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/error.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/stripe_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/stripe_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/teradata_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/teradata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/tpot_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/tpot_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/twitter_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/twitter_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/web_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/web_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/web_handler/web_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/web_handler/web_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/ingest.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/ingest.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
         # Create and store locally vectorstore
         db = Chroma.from_documents(
             texts,
             embedding=embeddings_model,
             persist_directory=self.persist_directory,
             client_settings=self.chroma_settings,
+            collection_name=self.args.get("collection_name", "langchain"),
         )
         db.persist()
         db = None
         end_time = time.time()
         elapsed_time = end_time - start_time
 
         logger.info(
```

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/question_answer.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/question_answer.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         )
         self.persist_directory = args["chromadb_storage_path"]
 
         llm = Writer(**model_parameters.dict())
         retriever = get_retriever(
             embeddings_model_name=self.embeddings_model_name,
             persist_directory=self.persist_directory,
-            collection_name=args.get('collection_name', '_default_collection')
+            collection_name=args.get("collection_name", "langchain"),
         )
 
         self.qa = RetrievalQA.from_chain_type(
             llm=llm,
             chain_type="stuff",
             retriever=retriever,
             return_source_documents=True,
```

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/settings.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import os
 from functools import lru_cache
 from typing import List, Union
 
 import pandas as pd
 import torch
 from chromadb import Settings
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.docstore.document import Document
 from langchain.document_loaders import DataFrameLoader
 from langchain.embeddings import HuggingFaceEmbeddings
 from langchain.vectorstores import Chroma
 from pydantic import BaseModel
 
-check_path_exists = lambda path: os.makedirs(path, exist_ok=True)
-
 DEFAULT_EMBEDDINGS_MODEL = "sentence-transformers/all-mpnet-base-v2"
 USER_DEFINED_MODEL_PARAMS = (
     "model_name",
     "max_tokens",
     "temperature",
     "top_p",
     "stop",
@@ -104,15 +101,17 @@
     except ValueError:
         raise ValueError(
             f"The {embeddings_model_name}  is not supported, please select a valid option from Hugging Face Hub!"
         )
     return embedding_model
 
 
-def load_chroma(embeddings_model_name, persist_directory, collection_name, chroma_settings):
+def load_chroma(
+    embeddings_model_name, persist_directory, collection_name, chroma_settings
+):
     return Chroma(
         collection_name=collection_name,
         persist_directory=persist_directory,
         embedding_function=load_embeddings_model(embeddings_model_name),
         client_settings=chroma_settings,
     )
 
@@ -123,10 +122,12 @@
         persist_directory=persist_directory,
         anonymized_telemetry=False,
     )
 
 
 def get_retriever(embeddings_model_name, persist_directory, collection_name):
     chroma_settings = get_chroma_settings(persist_directory)
-    db = load_chroma(embeddings_model_name, persist_directory, collection_name, chroma_settings)
+    db = load_chroma(
+        embeddings_model_name, persist_directory, collection_name, chroma_settings
+    )
     retriever = db.as_retriever()
     return retriever
```

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/setup.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/writer_handler/writer_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from .ingest import Ingestor
 from .question_answer import QuestionAnswerer
 from .settings import (
     DEFAULT_EMBEDDINGS_MODEL,
     USER_DEFINED_MODEL_PARAMS,
     ModelParameters,
-    check_path_exists,
 )
 
 # these require no additional arguments
 
 logger = get_log(logger_name=__name__)
 
 
@@ -64,25 +63,23 @@
 
             if "embeddings_model_name" not in args:
                 logger.info(
                     f"No embeddings model provided in query, using default model: {DEFAULT_EMBEDDINGS_MODEL}"
                 )
 
             chromadb_folder_name = args["chromadb_folder_name"]
+            # create folder for chromadb to persist embeddings
             args["chromadb_storage_path"] = self.engine_storage.folder_get(
                 chromadb_folder_name
             )
-            # check path exists and make
-            check_path_exists(args["chromadb_storage_path"])
             ingestor = Ingestor(df=df, args=args)
             ingestor.embeddings_to_vectordb()
 
-            # Persist changes to chromadb do disk
-            # not sure if this is required?
-            # self.engine_storage.folder_sync(args["chromadb_storage_path"])
+            # for mindsdb cloud, store data in shared file system for cloud version of mindsdb to make it be usable by all mindsdb nodes
+            self.engine_storage.folder_sync(chromadb_folder_name)
 
         else:
             logger.info("Skipping embeddings and ingestion into Chroma VectorDB")
 
         self.model_storage.json_set("args", args)
 
     def predict(self, df: pd.DataFrame = None, args: dict = None):
```

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/__init__.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/icon.png` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers_client/db_client_factory.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers_client/db_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers_client/ml_client_factory.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers_client/ml_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers_client/ml_grpc_client.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers_client/ml_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-23.7.1.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/libs/api_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/libs/api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/libs/base.py` & `MindsDB-23.7.1.0/mindsdb/integrations/libs/base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-23.7.1.0/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-23.7.1.0/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,165 +12,244 @@
     - `learn_process` method: handles async dispatch of the `learn` method in an engine, as well as registering all
       models inside of the internal MindsDB registry.
 
     - `predict_process` method: handles async dispatch of the `predict` method in an engine.
 
 """  # noqa
 
+import time
+import threading
 import datetime as dt
-import traceback
-import importlib
-from typing import Optional
+from typing import Optional, Callable
+from concurrent.futures import ProcessPoolExecutor, Future
 
 import pandas as pd
+from sqlalchemy import func, null
+from sqlalchemy.sql.functions import coalesce
 
 from mindsdb_sql import parse_sql
 from mindsdb_sql.parser.ast.base import ASTNode
-from mindsdb_sql.parser.ast import Identifier, Select, Star, NativeQuery
 
-from mindsdb.integrations.utilities.sql_utils import make_sql_session
 from mindsdb.utilities.config import Config
 import mindsdb.interfaces.storage.db as db
 from mindsdb.integrations.libs.response import (
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
 from mindsdb.__about__ import __version__ as mindsdb_version
 from mindsdb.utilities.hooks import after_predict as after_predict_hook
 from mindsdb.interfaces.model.model_controller import ModelController
 from mindsdb.interfaces.model.functions import (
     get_model_record
 )
-from mindsdb.api.mysql.mysql_proxy.classes.sql_query import SQLQuery
 from mindsdb.integrations.libs.const import PREDICTOR_STATUS
-from mindsdb.integrations.utilities.processes import HandlerProcess
-from mindsdb.utilities.functions import mark_process
-from mindsdb.integrations.utilities.utils import format_exception_error
 from mindsdb.interfaces.database.database import DatabaseController
 from mindsdb.interfaces.storage.model_fs import ModelStorage, HandlerStorage
 from mindsdb.utilities.context import context as ctx
 from mindsdb.interfaces.model.functions import get_model_records
-
 from mindsdb.integrations.handlers_client.ml_client_factory import MLClientFactory
+from mindsdb.integrations.libs.learn_process import learn_process
+from mindsdb.utilities.functions import mark_process
+import mindsdb.utilities.profiler as profiler
 
 from .ml_handler_proc import MLHandlerWrapper, MLHandlerPersistWrapper
 
 import torch.multiprocessing as mp
-mp.get_context('spawn')
+mp_ctx = mp.get_context('spawn')
 
 
 class MLEngineException(Exception):
     pass
 
 
-@mark_process(name='learn')
-def learn_process(class_path, engine, context_dump, integration_id,
-                  predictor_id, problem_definition, set_active,
-                  base_predictor_id=None, training_data_df=None,
-                  data_integration_ref=None, fetch_data_query=None, project_name=None):
-    ctx.load(context_dump)
-    db.init()
+def init_ml_handler(module_path):
+    import importlib  # noqa
 
-    predictor_record = db.Predictor.query.with_for_update().get(predictor_id)
+    from mindsdb.integrations.libs.learn_process import learn_process  # noqa
 
-    try:
-        target = problem_definition['target']
+    importlib.import_module(module_path)
+
+
+def dummy_task():
+    return None
+
+
+class WarmProcess:
+    """ Class-wrapper for a process that persist for a long time. The process
+        may be initialized with any handler requirements. Current implimentation
+        is based on ProcessPoolExecutor just because of multiprocessing.pool
+        produce daemon processes, which can not be used for learning. That
+        bahaviour may be changed only using inheritance.
+    """
+    def __init__(self, initializer: Optional[Callable] = None, initargs: tuple = ()):
+        """ create and init new process
+
+            Args:
+                initializer (Callable): the same as ProcessPoolExecutor initializer
+                initargs (tuple): the same as ProcessPoolExecutor initargs
+        """
+        self.pool = ProcessPoolExecutor(1, initializer=initializer, initargs=initargs)
+        # region bacause of ProcessPoolExecutor does not start new process
+        # untill it get a task, we need manually run dummy task to force init.
+        self.task = self.pool.submit(dummy_task)
+        self._init_done = False
+        self.task.add_done_callback(self._init_done_callback)
+        # endregion
+
+    def __del__(self):
+        self.pool.shutdown(wait=False)
+
+    def _init_done_callback(self, _task):
+        """ callback for initial task
+        """
+        self._init_done = True
 
-        training_data_df = None
+    def ready(self) -> bool:
+        """ check is process ready to get a task or not
 
-        database_controller = DatabaseController()
+            Returns:
+                bool
+        """
+        if self._init_done is False:
+            self.task.result()
+            self._init_done = True
+        if self.task is None or self.task.done():
+            return True
+        return False
+
+    def apply_async(self, func: Callable, *args: tuple, **kwargs: dict) -> Future:
+        """ Run new task
+
+            Args:
+                func (Callable): function to run
+                args (tuple): args to be passed to function
+                kwargs (dict): kwargs to be passed to function
 
-        sql_session = make_sql_session()
-        if data_integration_ref is not None:
-            if data_integration_ref['type'] == 'integration':
-                integration_name = database_controller.get_integration(data_integration_ref['id'])['name']
-                query = Select(
-                    targets=[Star()],
-                    from_table=NativeQuery(
-                        integration=Identifier(integration_name),
-                        query=fetch_data_query
-                    )
-                )
-                sqlquery = SQLQuery(query, session=sql_session)
-            elif data_integration_ref['type'] == 'view':
-                project = database_controller.get_project(project_name)
-                query_ast = parse_sql(fetch_data_query, dialect='mindsdb')
-                view_query_ast = project.query_view(query_ast)
-                sqlquery = SQLQuery(view_query_ast, session=sql_session)
-
-            result = sqlquery.fetch(view='dataframe')
-            training_data_df = result['result']
-
-        training_data_columns_count, training_data_rows_count = 0, 0
-        if training_data_df is not None:
-            training_data_columns_count = len(training_data_df.columns)
-            training_data_rows_count = len(training_data_df)
-
-        predictor_record.training_data_columns_count = training_data_columns_count
-        predictor_record.training_data_rows_count = training_data_rows_count
-        db.session.commit()
-
-        module_name, class_name = class_path
-        module = importlib.import_module(module_name)
-        HandlerClass = getattr(module, class_name)
-        HandlerClass = MLClientFactory(handler_class=HandlerClass, engine=engine)
-
-        handlerStorage = HandlerStorage(integration_id)
-        modelStorage = ModelStorage(predictor_id)
-
-        kwargs = {}
-        if base_predictor_id is not None:
-            kwargs['base_model_storage'] = ModelStorage(base_predictor_id)
-
-        ml_handler = HandlerClass(
-            engine_storage=handlerStorage,
-            model_storage=modelStorage,
-            **kwargs
+            Returns:
+                Future
+        """
+        if not self.ready():
+            raise Exception('Process task is not ready')
+        self.task = self.pool.submit(
+            func, *args, **kwargs
         )
+        return self.task
 
-        if not ml_handler.generative:
-            if training_data_df is not None and target not in training_data_df.columns:
-                raise Exception(
-                    f'Prediction target "{target}" not found in training dataframe: {list(training_data_df.columns)}')
-
-        # create new model
-        if base_predictor_id is None:
-            ml_handler.create(target, df=training_data_df, args=problem_definition)
 
-        # fine-tune (partially train) existing model
-        else:
-            # load model from previous version, use it as starting point
-            problem_definition['base_model_id'] = base_predictor_id
-            ml_handler.finetune(df=training_data_df, args=problem_definition)
-
-        predictor_record.status = PREDICTOR_STATUS.COMPLETE
-        predictor_record.active = set_active
-        db.session.commit()
-        # if retrain and set_active after success creation
-        if set_active is True:
-            models = get_model_records(
-                name=predictor_record.name,
-                project_id=predictor_record.project_id,
-                active=None
-            )
-            for model in models:
-                model.active = False
-            models = [x for x in models if x.status == PREDICTOR_STATUS.COMPLETE]
-            models.sort(key=lambda x: x.created_at)
-            models[-1].active = True
-    except Exception as e:
-        print(traceback.format_exc())
-        error_message = format_exception_error(e)
-
-        predictor_record.data = {"error": error_message}
-        predictor_record.status = PREDICTOR_STATUS.ERROR
-        db.session.commit()
+class ProcessCache:
+    """ simple cache for WarmProcess-es
+    """
+    def __init__(self, ttl: int = 120):
+        """ Args:
+            ttl (int) time to live for unused process
+        """
+        self.cache = {}
+        self._init = False
+        self._lock = threading.Lock()
+        self._ttl = ttl
+        self._keep_alive = {}
+        self._stop_event = threading.Event()
+        self.cleaner_thread = None
+        self._start_clean()
+
+    def __del__(self):
+        self._stop_clean()
 
-    predictor_record.training_stop_at = dt.datetime.now()
-    db.session.commit()
+    def _start_clean(self) -> None:
+        """ start worker that close connections after ttl expired
+        """
+        if (
+            isinstance(self.cleaner_thread, threading.Thread)
+            and self.cleaner_thread.is_alive()
+        ):
+            return
+        self._stop_event.clear()
+        self.cleaner_thread = threading.Thread(target=self._clean)
+        self.cleaner_thread.daemon = True
+        self.cleaner_thread.start()
+
+    def _stop_clean(self) -> None:
+        """ stop clean worker
+        """
+        self._stop_event.set()
+
+    def init(self, preload_handlers: dict):
+        """ run processes for specified handlers
+
+            Args:
+                preload_handlers (dict): {handler_class: count_of_processes}
+        """
+        with self._lock:
+            if self._init is False:
+                self._init = True
+                for handler in preload_handlers:
+                    self._keep_alive[handler.__name__] = preload_handlers[handler]
+                    self.cache[handler.__name__] = {
+                        'last_usage_at': time.time(),
+                        'processes': [
+                            WarmProcess(init_ml_handler, (handler.__module__,))
+                            for _x in range(preload_handlers[handler])
+                        ]
+                    }
+
+    def apply_async(self, handler: object, func: Callable, *args, **kwargs) -> Future:
+        """ run new task. If possible - do it in existing process, if not - start new one.
+
+            Args:
+                handler (object): handler class
+                func (Callable): function to run
+                args (tuple): args to be passed to function
+                kwargs (dict): kwargs to be passed to function
+
+            Returns:
+                Future
+        """
+        with self._lock:
+            handler_name = handler.__name__
+            if handler_name not in self.cache:
+                warm_process = WarmProcess(init_ml_handler, (handler.__module__,))
+                self.cache[handler_name] = {
+                    'last_usage_at': None,
+                    'processes': [warm_process]
+                }
+            else:
+                for warm_process in self.cache[handler_name]['processes']:
+                    if warm_process.ready():
+                        break
+                else:
+                    warm_process = WarmProcess(init_ml_handler, (handler.__module__,))
+                    self.cache[handler_name]['processes'].append(warm_process)
+            task = warm_process.apply_async(func, *args, **kwargs)
+            self.cache[handler_name]['last_usage_at'] = time.time()
+        return task
+
+    def _clean(self) -> None:
+        """ worker that stop unused processes
+        """
+        while self._stop_event.wait(timeout=10) is False:
+            with self._lock:
+                for handler_name in self.cache.keys():
+                    last_usage_at = self.cache[handler_name]['last_usage_at']
+                    processes = self.cache[handler_name]['processes']
+                    if (
+                        (
+                            handler_name not in self._keep_alive
+                            or self._keep_alive[handler_name] < len(processes)
+                        )
+                        and last_usage_at is not None
+                        and (time.time() - last_usage_at) > self._ttl
+                    ):
+                        for i, process in enumerate(processes):
+                            if process.ready():
+                                processes.pop(i)
+                                del process
+                                break
+
+
+process_cache = ProcessCache()
 
 
 class BaseMLEngineExec:
 
     def __init__(self, name, **kwargs):
         """
         ML handler interface converter
@@ -268,22 +347,22 @@
         """ Intakes a raw SQL query and returns the answer given by the ML engine. """
         query_ast = self.parser(query, dialect=self.dialect)
         return self.query(query_ast)
 
     def query_(self, query: ASTNode) -> Response:
         raise Exception('Should not be used')
 
+    @profiler.profile()
     def learn(
         self, model_name, project_name,
         data_integration_ref=None,
         fetch_data_query=None,
         problem_definition=None,
         join_learn_process=False,
         label=None,
-        version=1,
         is_retrain=False,
         set_active=True,
     ):
         # TODO move to model_controller
         """ Trains a model given some data-gathering SQL statement. """
 
         target = problem_definition['target']
@@ -309,44 +388,54 @@
             data={'name': model_name},
             project_id=project.id,
             training_data_columns_count=None,
             training_data_rows_count=None,
             training_start_at=dt.datetime.now(),
             status=PREDICTOR_STATUS.GENERATING,
             label=label,
-            version=version,
+            version=(
+                db.session.query(
+                    coalesce(func.max(db.Predictor.version), 1) + (1 if is_retrain else 0)
+                ).filter_by(
+                    company_id=ctx.company_id,
+                    name=model_name,
+                    project_id=project.id,
+                    deleted_at=null()
+                ).scalar_subquery()),
             active=(not is_retrain),  # if create then active
         )
 
-        db.session.add(predictor_record)
-        db.session.commit()
+        db.serializable_insert(predictor_record)
 
         class_path = [self.handler_class.__module__, self.handler_class.__name__]
 
-        p = HandlerProcess(
+        task = process_cache.apply_async(
+            self.handler_class,
             learn_process,
             class_path,
             self.engine,
             ctx.dump(),
             self.integration_id,
             predictor_record.id,
             problem_definition,
             set_active,
             data_integration_ref=data_integration_ref,
             fetch_data_query=fetch_data_query,
             project_name=project_name
         )
-        p.start()
+
         if join_learn_process is True:
-            p.join()
+            task.result()
             predictor_record = db.Predictor.query.get(predictor_record.id)
             db.session.refresh(predictor_record)
 
         return predictor_record
 
+    @profiler.profile()
+    @mark_process(name='predict')
     def predict(self, model_name: str, data: list, pred_format: str = 'dict',
                 project_name: str = None, version=None, params: dict = None):
         """ Generates predictions with some model and input data. """
         if isinstance(data, dict):
             data = [data]
         df = pd.DataFrame(data)
         kwargs = {
@@ -412,16 +501,17 @@
             predictor_id=predictor_record.id,
             rows_in_count=df.shape[0],
             columns_in_count=df.shape[1],
             rows_out_count=len(predictions)
         )
         return predictions
 
+    @profiler.profile()
     def update(
-            self, model_name, project_name, version,
+            self, model_name, project_name,
             base_model_version: int,
             data_integration_ref=None,
             fetch_data_query=None,
             join_learn_process=False,
             label=None,
             set_active=True,
             args: Optional[dict] = None
@@ -432,15 +522,20 @@
         search_args = {
             'active': None,
             'name': model_name,
             'status': PREDICTOR_STATUS.COMPLETE
         }
         if base_model_version is not None:
             search_args['version'] = base_model_version
+        else:
+            search_args['active'] = True
         predictor_records = get_model_records(**search_args)
+        if len(predictor_records) == 0:
+            raise Exception("Can't find suitable base model")
+
         predictor_records.sort(key=lambda x: x.training_stop_at, reverse=True)
         predictor_records = [x for x in predictor_records if x.training_stop_at is not None]
         base_predictor_record = predictor_records[0]
 
         learn_args = base_predictor_record.learn_args
         learn_args['using'] = args if not learn_args.get('using', False) else {**learn_args['using'], **args}
 
@@ -456,37 +551,47 @@
             data={'name': model_name},
             project_id=project.id,
             training_data_columns_count=None,
             training_data_rows_count=None,
             training_start_at=dt.datetime.now(),
             status=PREDICTOR_STATUS.GENERATING,
             label=label,
-            version=version,
+            version=(
+                db.session.query(
+                    coalesce(func.max(db.Predictor.version), 1) + 1
+                ).filter_by(
+                    company_id=ctx.company_id,
+                    name=model_name,
+                    project_id=project.id,
+                    deleted_at=null()
+                ).scalar_subquery()
+            ),
             active=False
         )
-
-        db.session.add(predictor_record)
-        db.session.commit()
+        with profiler.Context('finetune-update-record-insert'):
+            db.serializable_insert(predictor_record)
 
         class_path = [self.handler_class.__module__, self.handler_class.__name__]
 
-        p = HandlerProcess(
-            learn_process,
-            class_path,
-            self.engine,
-            ctx.dump(),
-            self.integration_id,
-            predictor_record.id,
-            predictor_record.learn_args,
-            set_active,
-            base_predictor_record.id,
-            data_integration_ref=data_integration_ref,
-            fetch_data_query=fetch_data_query,
-            project_name=project_name
-        )
-        p.start()
-        if join_learn_process is True:
-            p.join()
-            predictor_record = db.Predictor.query.get(predictor_record.id)
-            db.session.refresh(predictor_record)
+        with profiler.Context('finetune-update'):
+            task = process_cache.apply_async(
+                self.handler_class,
+                learn_process,
+                class_path,
+                self.engine,
+                ctx.dump(),
+                self.integration_id,
+                predictor_record.id,
+                predictor_record.learn_args,
+                set_active,
+                base_predictor_record.id,
+                data_integration_ref=data_integration_ref,
+                fetch_data_query=fetch_data_query,
+                project_name=project_name
+            )
+
+            if join_learn_process is True:
+                task.result()
+                predictor_record = db.Predictor.query.get(predictor_record.id)
+                db.session.refresh(predictor_record)
 
         return predictor_record
```

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/libs/ml_handler_proc.py` & `MindsDB-23.7.1.0/mindsdb/integrations/libs/ml_handler_proc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-23.7.1.0/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/libs/realtime_chat_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/libs/realtime_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/libs/response.py` & `MindsDB-23.7.1.0/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-23.7.1.0/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/utilities/date_utils.py` & `MindsDB-23.7.1.0/mindsdb/integrations/utilities/date_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/utilities/install.py` & `MindsDB-23.7.1.0/mindsdb/integrations/utilities/install.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/utilities/sql_utils.py` & `MindsDB-23.7.1.0/mindsdb/integrations/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-23.7.1.0/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/integrations/utilities/time_series_utils.py` & `MindsDB-23.7.1.0/mindsdb/integrations/utilities/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_controller.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_message.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_monitor.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_monitor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_task.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/chatbot_thread.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/chatbot_thread.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/realtime_chat_handler_factory.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/realtime_chat_handler_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/realtime_chatbot_task.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/realtime_chatbot_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         # Get model info.
         model = self._session.model_controller.get_model(self._model_name, project_name=project_name)
         model_record = db.Predictor.query.get(model['id'])
 
         # Configure columns to use for responding.
         self._user_col = RealtimeChatBotTask._PROMPT_USER_COLUMN
         if 'using' in model_record.learn_args and 'user_column' in model_record.learn_args['using']:
-            self._user_col = model_record.learn_args['using']['user_column'],
+            self._user_col = model_record.learn_args['using']['user_column']
         self._output_col = model_record.to_predict[0]
 
     def _set_context(self):
         ctx.set_default()
         ctx.company_id = self._bot_record.company_id
         if self._bot_record.user_class is not None:
             ctx.user_class = self._bot_record.user_class
```

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/chatbot/realtime_chatbot_thread.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/chatbot/realtime_chatbot_thread.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/database/database.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/database/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Optional
 from collections import OrderedDict
 
-from mindsdb.interfaces.database.integrations import integration_controller
 from mindsdb.interfaces.database.projects import ProjectController
+import mindsdb.utilities.profiler as profiler
 
 
 class DatabaseController:
     def __init__(self):
+        from mindsdb.interfaces.database.integrations import integration_controller
         self.integration_controller = integration_controller
         self.project_controller = ProjectController()
 
     def delete(self, name: str):
         databases = self.get_dict()
         if name not in databases:
             raise Exception(f"Database '{name}' does not exists")
@@ -21,14 +22,15 @@
             return
         elif db_type == 'data':
             self.integration_controller.delete(name)
             return
         else:
             raise Exception(f"Database with type '{db_type}' cannot be deleted")
 
+    @profiler.profile()
     def get_list(self, filter_type: Optional[str] = None):
         projects = self.project_controller.get_list()
         integrations = self.integration_controller.get_all()
         result = [{
             'name': 'information_schema',
             'type': 'system',
             'id': None,
```

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/database/integrations.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/database/integrations.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 from mindsdb.integrations.libs.base import BaseMLEngine
 from mindsdb.integrations.libs.api_handler import APIHandler
 from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE, HANDLER_TYPE
 from mindsdb.integrations.handlers_client.db_client_factory import DBClient
 from mindsdb.interfaces.model.functions import get_model_records
 from mindsdb.utilities.context import context as ctx
 from mindsdb.utilities.log import get_log
-
+from mindsdb.integrations.libs.ml_exec_base import BaseMLEngineExec
+import mindsdb.utilities.profiler as profiler
 
 logger = get_log()
 
 
 class HandlersCache:
     """ Cache for data handlers that keep connections opened during ttl time from handler last use
     """
@@ -396,14 +397,15 @@
             fs_store=fs_store,
             connection_data=connection_data
         )
 
         logger.debug("%s.create_tmp_handler: create a client to db of %s type", self.__class__.__name__, handler_type)
         return DBClient(handler_type, self.handler_modules[handler_type].Handler, **handler_ars)
 
+    @profiler.profile()
     def get_handler(self, name, case_sensitive=False):
         handler = self.handlers_cache.get(name)
         if handler is not None:
             return handler
 
         if case_sensitive:
             integration_record = db.session.query(db.Integration).filter_by(company_id=ctx.company_id, name=name).first()
@@ -456,16 +458,14 @@
 
         handler_type = self.handler_modules[integration_engine].type
         if handler_type == 'ml':
             handler_ars['storage_factory'] = FileStorageFactory(
                 resource_group=RESOURCE_GROUP.PREDICTOR,
                 sync=True
             )
-        from mindsdb.integrations.libs.base import BaseMLEngine
-        from mindsdb.integrations.libs.ml_exec_base import BaseMLEngineExec
 
         HandlerClass = self.handler_modules[integration_engine].Handler
 
         if isinstance(HandlerClass, type) and issubclass(HandlerClass, BaseMLEngine):
             handler_ars['handler_class'] = HandlerClass
             handler_ars['execution_method'] = getattr(self.handler_modules[integration_engine], 'execution_method', None)
             handler_ars['integration_engine'] = integration_engine
```

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/database/projects.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/database/projects.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from mindsdb_sql import parse_sql
 
 from mindsdb.interfaces.storage import db
 from mindsdb.utilities.config import Config
 from mindsdb.interfaces.model.model_controller import ModelController
 from mindsdb.interfaces.database.views import ViewController
 from mindsdb.utilities.context import context as ctx
+import mindsdb.utilities.profiler as profiler
 
 
 class Project:
     @staticmethod
     def from_record(db_record: db.Project):
         p = Project()
         p.record = db_record
@@ -111,14 +112,77 @@
         view_meta = ViewController().get(
             name=view_name,
             project_name=self.name
         )
         subquery_ast = parse_sql(view_meta['query'], dialect='mindsdb')
         return subquery_ast
 
+    @staticmethod
+    def _get_model_data(predictor_record, integraion_record):
+        predictor_data = predictor_record.data or {}
+        training_time = None
+        if (
+            predictor_record.training_start_at is not None
+            and predictor_record.training_stop_at is None
+            and predictor_record.status != 'error'
+        ):
+            training_time = round((datetime.datetime.now() - predictor_record.training_start_at).total_seconds(), 3)
+        elif (
+            predictor_record.training_start_at is not None
+            and predictor_record.training_stop_at is not None
+        ):
+            training_time = round((predictor_record.training_stop_at - predictor_record.training_start_at).total_seconds(), 3)
+        predictor_meta = {
+            'type': 'model',
+            'id': predictor_record.id,
+            'engine': integraion_record.engine,
+            'engine_name': integraion_record.name,
+            'active': predictor_record.active,
+            'version': predictor_record.version,
+            'status': predictor_record.status,
+            'accuracy': None,
+            'predict': predictor_record.to_predict[0],
+            'update_status': predictor_record.update_status,
+            'mindsdb_version': predictor_record.mindsdb_version,
+            'error': predictor_data.get('error'),
+            'select_data_query': predictor_record.fetch_data_query,
+            'training_options': predictor_record.learn_args,
+            'deletable': True,
+            'label': predictor_record.label,
+            'current_training_phase': predictor_record.training_phase_current,
+            'total_training_phases': predictor_record.training_phase_total,
+            'training_phase_name': predictor_record.training_phase_name,
+            'training_time': training_time
+        }
+        if predictor_data.get('accuracies', None) is not None:
+            if len(predictor_data['accuracies']) > 0:
+                predictor_meta['accuracy'] = float(np.mean(list(predictor_data['accuracies'].values())))
+        return {
+            'name': predictor_record.name,
+            'metadata': predictor_meta,
+            'created_at': predictor_record.created_at
+        }
+
+    def get_model(self, name: str):
+        record = (
+            db.session.query(db.Predictor, db.Integration).filter_by(
+                project_id=self.id,
+                active=True,
+                name=name,
+                deleted_at=sa.null(),
+                company_id=ctx.company_id
+            )
+            .join(db.Integration, db.Integration.id == db.Predictor.integration_id)
+            .order_by(db.Predictor.name, db.Predictor.id)
+            .first()
+        )
+        if record is None:
+            return None
+        return self._get_model_data(record[0], record[1])
+
     def get_models(self, model_id=None):
         query = (
             db.session.query(db.Predictor, db.Integration).filter_by(
                 project_id=self.id,
                 deleted_at=sa.null(),
                 company_id=ctx.company_id
             )
@@ -127,57 +191,15 @@
         )
         if model_id is not None:
             query = query.filter(db.Predictor.id == model_id)
 
         data = []
 
         for predictor_record, integraion_record in query.all():
-            predictor_data = predictor_record.data or {}
-            training_time = None
-            if (
-                predictor_record.training_start_at is not None
-                and predictor_record.training_stop_at is None
-                and predictor_record.status != 'error'
-            ):
-                training_time = int((datetime.datetime.now() - predictor_record.training_start_at).total_seconds())
-            elif (
-                predictor_record.training_start_at is not None
-                and predictor_record.training_stop_at is not None
-            ):
-                training_time = int((predictor_record.training_stop_at - predictor_record.training_start_at).total_seconds())
-            predictor_meta = {
-                'type': 'model',
-                'id': predictor_record.id,
-                'engine': integraion_record.engine,
-                'engine_name': integraion_record.name,
-                'active': predictor_record.active,
-                'version': predictor_record.version,
-                'status': predictor_record.status,
-                'accuracy': None,
-                'predict': predictor_record.to_predict[0],
-                'update_status': predictor_record.update_status,
-                'mindsdb_version': predictor_record.mindsdb_version,
-                'error': predictor_data.get('error'),
-                'select_data_query': predictor_record.fetch_data_query,
-                'training_options': predictor_record.learn_args,
-                'deletable': True,
-                'label': predictor_record.label,
-                'current_training_phase': predictor_record.training_phase_current,
-                'total_training_phases': predictor_record.training_phase_total,
-                'training_phase_name': predictor_record.training_phase_name,
-                'training_time': training_time
-            }
-            if predictor_data.get('accuracies', None) is not None:
-                if len(predictor_data['accuracies']) > 0:
-                    predictor_meta['accuracy'] = float(np.mean(list(predictor_data['accuracies'].values())))
-            data.append({
-                'name': predictor_record.name,
-                'metadata': predictor_meta,
-                'created_at': predictor_record.created_at
-            })
+            data.append(self._get_model_data(predictor_record, integraion_record))
 
         return data
 
     def get_views(self):
         records = (
             db.session.query(db.View).filter_by(
                 project_id=self.id,
@@ -212,14 +234,15 @@
             'metadata': {
                 'type': 'view',
                 'id': view_record.id,
                 'deletable': True
             }
         }
 
+    @profiler.profile()
     def get_tables(self):
         data = OrderedDict()
         data['models'] = {'type': 'table', 'deletable': False}
         data['models_versions'] = {'type': 'table', 'deletable': False}
         data['jobs'] = {'type': 'table', 'deletable': False}
         data['jobs_history'] = {'type': 'table', 'deletable': False}
```

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/database/views.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/file/file_controller.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/model/functions.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/model/functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
 from sqlalchemy import null, func
 
 import mindsdb.interfaces.storage.db as db
 from mindsdb.utilities.context import context as ctx
+import mindsdb.utilities.profiler as profiler
 
 
 class PredictorRecordNotFound(Exception):
     def __init__(self, **kwargs):
         name = kwargs.get('name') or '-'
         predictor_id = kwargs.get('id') or '-'
         super().__init__(
@@ -20,27 +21,29 @@
         name = kwargs.get('name') or '-'
         predictor_id = kwargs.get('id') or '-'
         super().__init__(
             f"Found multiple predictor with: name='{name}' id='{predictor_id}'"
         )
 
 
+@profiler.profile()
 def get_integration_record(name: str) -> db.Integration:
     company_id = ctx.company_id
     if company_id is None:
         company_id = null()
 
     record = (
         db.session.query(db.Integration)
         .filter_by(company_id=company_id, name=name)
         .first()
     )
     return record
 
 
+@profiler.profile()
 def get_project_record(name: str) -> db.Project:
     company_id = ctx.company_id
     if company_id is None:
         company_id = null()
 
     project_record = (
         db.session.query(db.Project)
@@ -49,30 +52,33 @@
             & (db.Project.company_id == company_id)
             & (db.Project.deleted_at == null())
         ).first()
     )
     return project_record
 
 
+@profiler.profile()
 def get_predictor_integration(record: db.Predictor) -> db.Integration:
     integration_record = (
         db.session.query(db.Integration)
         .filter_by(id=record.integration_id).first()
     )
     return integration_record
 
 
+@profiler.profile()
 def get_predictor_project(record: db.Predictor) -> db.Project:
     project_record = (
         db.session.query(db.Project)
         .filter_by(id=record.project_id).first()
     )
     return project_record
 
 
+@profiler.profile()
 def get_model_records(integration_id=None, active=True, deleted_at=null(),
                       project_name: Optional[str] = None, ml_handler_name: Optional[str] = None, **kwargs):
     kwargs['company_id'] = ctx.company_id
     if kwargs['company_id'] is None:
         kwargs['company_id'] = null()
 
     if deleted_at is not None:
@@ -101,14 +107,15 @@
     return (
         db.session.query(db.Predictor)
         .filter_by(**kwargs)
         .all()
     )
 
 
+@profiler.profile()
 def get_model_record(except_absent=False, ml_handler_name: Optional[str] = None,
                      project_name: Optional[str] = None, active: bool = True,
                      deleted_at=null(), version: Optional[int] = None, **kwargs):
     kwargs['company_id'] = ctx.company_id
     if kwargs['company_id'] is None:
         kwargs['company_id'] = null()
```

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/model/model_controller.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/model/model_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     get_model_record,
     get_model_records
 )
 from mindsdb.interfaces.storage.json import get_json_storage
 from mindsdb.interfaces.storage.model_fs import ModelStorage
 from mindsdb.utilities.context import context as ctx
 from mindsdb.utilities.functions import resolve_model_identifier
+import mindsdb.utilities.profiler as profiler
 
 IS_PY36 = sys.version_info[1] <= 6
 
 
 class ModelController():
     config: Config
     fs_store: FsStore
@@ -373,16 +374,14 @@
             active=True
         )
 
         model_name = params['model_name']
         if base_predictor_record is None:
             raise Exception(f"Error: model '{model_name}' does not exist")
 
-        params['version'] = self._get_retrain_finetune_version(params['project_name'], base_predictor_record)
-
         if params['data_integration_ref'] is None:
             params['data_integration_ref'] = base_predictor_record.data_integration_ref
         if params['fetch_data_query'] is None:
             params['fetch_data_query'] = base_predictor_record.fetch_data_query
 
         problem_definition = base_predictor_record.learn_args.copy()
         problem_definition.update(params['problem_definition'])
@@ -390,28 +389,14 @@
 
         params['is_retrain'] = True
         params['set_active'] = set_active
         predictor_record = ml_handler.learn(**params)
 
         return self.get_model_info(predictor_record)
 
-    @staticmethod
-    def _get_retrain_finetune_version(project_name, base_predictor_record):
-        if base_predictor_record is None:
-            raise Exception(f"Error: model '{base_predictor_record.name}' does not exist")
-
-        models = get_model_records(
-            name=base_predictor_record.name,
-            project_name=project_name,
-            active=None
-        )
-        last_version = max([x.version or 1 for x in models])
-
-        return last_version + 1
-
     def prepare_finetune_statement(self, statement, database_controller):
         project_name, model_name, model_version = resolve_model_identifier(statement.name)
         data_integration_ref, fetch_data_query = self._get_data_integration_ref(statement, database_controller)
 
         set_active = True
         if statement.using is not None:
             set_active = statement.using.pop('active', True)
@@ -426,36 +411,35 @@
 
         join_learn_process = args.pop('join_learn_process', False)
 
         base_predictor_record = get_model_record(
             name=model_name,
             project_name=project_name,
             version=model_version,
-            active=None
+            active=True if model_version is None else None
         )
-        version = self._get_retrain_finetune_version(project_name, base_predictor_record)
 
         if data_integration_ref is None:
             data_integration_ref = base_predictor_record.data_integration_ref
         if fetch_data_query is None:
             fetch_data_query = base_predictor_record.fetch_data_query
 
         return dict(
             model_name=model_name,
             project_name=project_name,
             data_integration_ref=data_integration_ref,
             fetch_data_query=fetch_data_query,
             base_model_version=model_version,
-            version=version,
             args=args,
             join_learn_process=join_learn_process,
             label=label,
             set_active=set_active
         )
 
+    @profiler.profile()
     def finetune_model(self, statement, ml_handler):
         params = self.prepare_finetune_statement(statement, ml_handler.database_controller)
         predictor_record = ml_handler.update(**params)
         return self.get_model_info(predictor_record)
 
     def get_model_info(self, predictor_record):
         from mindsdb.interfaces.database.projects import ProjectController
```

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/storage/db.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/storage/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import datetime
 from typing import Dict
 
 import numpy as np
 from sqlalchemy import create_engine, types, UniqueConstraint
 from sqlalchemy.orm import scoped_session, sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy import Column, Integer, String, DateTime, Boolean, Index
+from sqlalchemy import Column, Integer, String, DateTime, Boolean, Index, text
 from sqlalchemy.sql.schema import ForeignKey
 from sqlalchemy import JSON
+from sqlalchemy.exc import OperationalError
 
 Base = declarative_base()
 session, engine = None, None
 
 
 def init(connection_str: str = None):
     global Base, session, engine
@@ -23,14 +24,41 @@
         engine = create_engine(connection_str, echo=False)
     else:
         engine = create_engine(connection_str, convert_unicode=True, pool_size=30, max_overflow=200, echo=False)
     session = scoped_session(sessionmaker(bind=engine, autoflush=True))
     Base.query = session.query_property()
 
 
+def serializable_insert(record: Base, try_count: int = 100):
+    """ Do serializeble insert. If fail - repeat it {try_count} times.
+
+        Args:
+            record (Base): sqlalchey record to insert
+            try_count (int): count of tryes to insert record
+    """
+    commited = False
+    while not commited:
+        session.connection(
+            execution_options={'isolation_level': 'SERIALIZABLE'}
+        )
+        if engine.name == 'postgresql':
+            session.execute(text('LOCK TABLE PREDICTOR IN EXCLUSIVE MODE'))
+        session.add(record)
+        try:
+            session.commit()
+        except OperationalError:
+            # catch 'SerializationFailure' (it should be in str(e), but it may depend on engine)
+            session.rollback()
+            try_count += -1
+            if try_count == 0:
+                raise
+        else:
+            commited = True
+
+
 # Source: https://stackoverflow.com/questions/26646362/numpy-array-is-not-json-serializable
 class NumpyEncoder(json.JSONEncoder):
     """ Special json encoder for numpy types """
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         elif isinstance(obj, np.floating):
```

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/storage/json.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/stream/base/integration.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/stream/base/integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/interfaces/stream/stream.py` & `MindsDB-23.7.1.0/mindsdb/interfaces/stream/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-23.7.1.0/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-23.7.1.0/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-23.7.1.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-23.7.1.0/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-23.7.1.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-23.7.1.0/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-23.7.1.0/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-23.7.1.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/alembic.ini` & `MindsDB-23.7.1.0/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/env.py` & `MindsDB-23.7.1.0/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/migrate.py` & `MindsDB-23.7.1.0/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py` & `MindsDB-23.7.1.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/auth.py` & `MindsDB-23.7.1.0/mindsdb/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/cache.py` & `MindsDB-23.7.1.0/mindsdb/utilities/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 import typing as t
 
 import pandas as pd
 import walrus
 
 from mindsdb.utilities.config import Config
 from mindsdb.utilities.json_encoder import CustomJSONEncoder
+from mindsdb.interfaces.storage.fs import FileLock
+from mindsdb.utilities.context import context as ctx
 
 
 def dataframe_checksum(df: pd.DataFrame):
     checksum = str_checksum(df.to_json())
     return checksum
 
 
@@ -113,36 +115,37 @@
 class FileCache(BaseCache):
     def __init__(self, category, path=None, **kwargs):
         super().__init__(**kwargs)
 
         if path is None:
             path = self.config['paths']['cache']
 
-        # include category
         cache_path = Path(path) / category
-        if not os.path.exists(cache_path):
-            os.makedirs(cache_path)
+
+        company_id = ctx.company_id
+        if company_id is not None:
+            cache_path = cache_path / str(company_id)
+        cache_path.mkdir(parents=True, exist_ok=True)
 
         self.path = cache_path
 
     def clear_old_cache(self):
-        # buffer to delete, to not run delete on every adding
-        buffer_size = 5
-
-        if self.max_size is None:
-            return
-
-        cur_count = len(os.listdir(self.path))
-
-        # remove oldest
-        if cur_count > self.max_size + buffer_size:
-
-            files = sorted(Path(self.path).iterdir(), key=os.path.getmtime)
-            for file in files[:cur_count - self.max_size]:
-                self.delete_file(file)
+        with FileLock(self.path):
+            # buffer to delete, to not run delete on every adding
+            buffer_size = 5
+
+            if self.max_size is None:
+                return
+
+            cur_count = len(os.listdir(self.path))
+
+            if cur_count > self.max_size + buffer_size:
+                files = sorted(Path(self.path).iterdir(), key=os.path.getmtime)
+                for file in files[:cur_count - self.max_size]:
+                    self.delete_file(file)
 
     def file_path(self, name):
         return self.path / name
 
     def set_df(self, name, df):
         path = self.file_path(name)
         df.to_pickle(path)
@@ -154,26 +157,28 @@
 
         with open(path, 'wb') as fd:
             fd.write(value)
         self.clear_old_cache()
 
     def get_df(self, name):
         path = self.file_path(name)
-
-        if not os.path.exists(path):
-            return None
-        return pd.read_pickle(path)
+        with FileLock(self.path):
+            if not os.path.exists(path):
+                return None
+            value = pd.read_pickle(path)
+        return value
 
     def get(self, name):
         path = self.file_path(name)
 
-        if not os.path.exists(path):
-            return None
-        with open(path, 'rb') as fd:
-            value = fd.read()
+        with FileLock(self.path):
+            if not os.path.exists(path):
+                return None
+            with open(path, 'rb') as fd:
+                value = fd.read()
         value = self.deserialize(value)
         return value
 
     def delete(self, name):
         path = self.file_path(name)
         self.delete_file(path)
```

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/config.py` & `MindsDB-23.7.1.0/mindsdb/utilities/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/context.py` & `MindsDB-23.7.1.0/mindsdb/utilities/context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/fs.py` & `MindsDB-23.7.1.0/mindsdb/utilities/fs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,137 +1,144 @@
 import os
-import time
 import tempfile
 import threading
+import time
 from pathlib import Path
 from typing import Optional
 
 import psutil
 from appdirs import user_data_dir
 
 
 def create_directory(path):
     path = Path(path)
     path.mkdir(mode=0o777, exist_ok=True, parents=True)
 
 
 def get_root_path():
-    mindsdb_path = user_data_dir('mindsdb', 'mindsdb')
-    return os.path.join(mindsdb_path, 'var/')
+    mindsdb_path = user_data_dir("mindsdb", "mindsdb")
+    return os.path.join(mindsdb_path, "var/")
 
 
 def get_or_create_data_dir():
-    data_dir = user_data_dir('mindsdb', 'mindsdb')
-    mindsdb_data_dir = os.path.join(data_dir, 'var/')
+    data_dir = user_data_dir("mindsdb", "mindsdb")
+    mindsdb_data_dir = os.path.join(data_dir, "var/")
 
     if os.path.exists(mindsdb_data_dir) is False:
         create_directory(mindsdb_data_dir)
 
     try:
         assert os.path.exists(mindsdb_data_dir)
         assert os.access(mindsdb_data_dir, os.W_OK) is True
     except Exception:
-        raise Exception('MindsDB storage directory does not exist and could not be created')
+        raise Exception(
+            "MindsDB storage directory does not exist and could not be created"
+        )
 
     return mindsdb_data_dir
 
 
 def create_dirs_recursive(path):
     if isinstance(path, dict):
         for p in path.values():
             create_dirs_recursive(p)
     elif isinstance(path, str):
         create_directory(path)
     else:
-        raise ValueError(f'Wrong path: {path}')
+        raise ValueError(f"Wrong path: {path}")
 
 
 def _get_process_mark_id(unified: bool = False) -> str:
-    ''' Creates a text that can be used to identify process+thread
-        Args:
-            unified: bool, if True then result will be same for same process+thread
-        Returns:
-            mark of process+thread
-    '''
-    mark = f'{os.getpid()}-{threading.get_native_id()}'
+    """Creates a text that can be used to identify process+thread
+    Args:
+        unified: bool, if True then result will be same for same process+thread
+    Returns:
+        mark of process+thread
+    """
+    mark = f"{os.getpid()}-{threading.get_native_id()}"
     if unified is True:
         return mark
     return f"{mark}-{str(time.time()).replace('.', '')}"
 
 
-def create_process_mark(folder='learn'):
+def create_process_mark(folder="learn"):
     mark = None
-    if os.name == 'posix':
-        p = Path(tempfile.gettempdir()).joinpath(f'mindsdb/processes/{folder}/')
+    if os.name == "posix":
+        p = Path(tempfile.gettempdir()).joinpath(f"mindsdb/processes/{folder}/")
         p.mkdir(parents=True, exist_ok=True)
         mark = _get_process_mark_id()
         p.joinpath(mark).touch()
     return mark
 
 
-def delete_process_mark(folder: str = 'learn', mark: Optional[str] = None):
+def delete_process_mark(folder: str = "learn", mark: Optional[str] = None):
     if mark is None:
         mark = _get_process_mark_id()
-    if os.name == 'posix':
+    if os.name == "posix":
         p = (
             Path(tempfile.gettempdir())
-            .joinpath(f'mindsdb/processes/{folder}/')
+            .joinpath(f"mindsdb/processes/{folder}/")
             .joinpath(mark)
         )
         if p.exists():
             p.unlink()
 
 
 def clean_process_marks():
-    """ delete all existing processes marks
-    """
-    if os.name != 'posix':
+    """delete all existing processes marks"""
+    if os.name != "posix":
         return
 
-    p = Path(tempfile.gettempdir()).joinpath('mindsdb/processes/')
+    p = Path(tempfile.gettempdir()).joinpath("mindsdb/processes/")
     if p.exists() is False:
         return
     for path in p.iterdir():
         if path.is_dir() is False:
             return
         for file in path.iterdir():
             file.unlink()
 
 
 def clean_unlinked_process_marks():
-    """ delete marks that does not have corresponded processes/threads
-    """
-    if os.name != 'posix':
+    """delete marks that does not have corresponded processes/threads"""
+    if os.name != "posix":
         return
 
-    p = Path(tempfile.gettempdir()).joinpath('mindsdb/processes/')
+    p = Path(tempfile.gettempdir()).joinpath("mindsdb/processes/")
     if p.exists() is False:
         return
     for path in p.iterdir():
         if path.is_dir() is False:
             return
         for file in path.iterdir():
-            parts = file.name.split('-')
+            parts = file.name.split("-")
             process_id = int(parts[0])
             thread_id = int(parts[1])
 
             try:
                 process = psutil.Process(process_id)
                 if process.status() in (psutil.STATUS_ZOMBIE, psutil.STATUS_DEAD):
                     raise psutil.NoSuchProcess(process_id)
 
                 threads = process.threads()
                 try:
                     next(t for t in threads if t.id == thread_id)
                 except StopIteration:
                     from mindsdb.utilities.log import get_log
-                    get_log('main').warning(
-                        f'We have mark for process/thread {process_id}/{thread_id} but it does not exists'
+
+                    get_log("main").warning(
+                        f"We have mark for process/thread {process_id}/{thread_id} but it does not exists"
                     )
                     file.unlink()
 
+            except psutil.AccessDenied:
+                get_log("main").warning(f"access to {process_id} denied")
+
+                continue
+
             except psutil.NoSuchProcess:
                 from mindsdb.utilities.log import get_log
-                get_log('main').warning(
-                    f'We have mark for process/thread {process_id}/{thread_id} but it does not exists'
+
+                get_log("main").warning(
+                    f"We have mark for process/thread {process_id}/{thread_id} but it does not exists"
                 )
                 file.unlink()
```

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/functions.py` & `MindsDB-23.7.1.0/mindsdb/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/hooks/profiling.py` & `MindsDB-23.7.1.0/mindsdb/utilities/hooks/profiling.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 MINDSDB_PROFILING_DB_PASSWORD = os.environ.get("MINDSDB_PROFILING_DB_PASSWORD")
 
 
 def set_level(node, level, internal_id):
     internal_id["id"] += 1
     node["level"] = level
     node["value"] = node["stop_at"] - node["start_at"]
+    node["value_thread"] = node["stop_at_thread"] - node["start_at_thread"]
+    node["value_process"] = node["stop_at_process"] - node["start_at_process"]
     node["internal_id"] = internal_id["id"]
 
     accum = 0
     for child_node in node["children"]:
         set_level(child_node, level + 1, internal_id)
         accum += child_node["value"]
     node["self"] = node["value"] - accum
@@ -29,22 +31,26 @@
 
     profiling = profiling_data
     set_level(profiling["tree"], 0, {"id": 0})
 
     time_start_at = profiling["tree"]["time_start_at"]
     del profiling["tree"]["time_start_at"]
 
-    connection = psycopg.connect(
-        host=MINDSDB_PROFILING_DB_HOST,
-        port=5432,
-        user=MINDSDB_PROFILING_DB_USER,
-        password=MINDSDB_PROFILING_DB_PASSWORD,
-        dbname="postgres",
-        connect_timeout=5
-    )
+    try:
+        connection = psycopg.connect(
+            host=MINDSDB_PROFILING_DB_HOST,
+            port=5432,
+            user=MINDSDB_PROFILING_DB_USER,
+            password=MINDSDB_PROFILING_DB_PASSWORD,
+            dbname="postgres",
+            connect_timeout=5
+        )
+    except Exception:
+        print('cant get acceess to profiling database')
+        return
     cur = connection.cursor()
     cur.execute("""
         insert into profiling
             (data, query, time, hostname, environment, api, total_time, company_id, instance_id)
         values
             (%s, %s, %s, %s, %s, %s, %s, %s, %s)
     """, (
```

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/json_encoder.py` & `MindsDB-23.7.1.0/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/log.py` & `MindsDB-23.7.1.0/mindsdb/utilities/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/log_controller.py` & `MindsDB-23.7.1.0/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/profiler/profiler.py` & `MindsDB-23.7.1.0/mindsdb/utilities/profiler/profiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
         Args:
             tag (str): name of new node
     """
     profiling = ctx.profiling
     new_node = {
         'start_at': time.perf_counter(),
+        'start_at_thread': time.thread_time(),
+        'start_at_process': time.process_time(),
         'stop_at': None,
         'name': tag,
         'children': []
     }
     if profiling['pointer'] is None:
         if profiling['level'] != 1:
             # profiling was activated not in the root of nodes tree
@@ -53,14 +55,16 @@
     """
     profiling = ctx.profiling
     if profiling['pointer'] is None:
         # profiling was activated not in the root of nodes tree
         return
     current_node = _get_current_node(profiling)
     current_node['stop_at'] = time.perf_counter()
+    current_node['stop_at_thread'] = time.thread_time()
+    current_node['stop_at_process'] = time.process_time()
     if len(profiling['pointer']) > 0:
         profiling['pointer'] = profiling['pointer'][:-1]
     else:
         if ctx.profiling['enabled'] is True:
             _send_profiling_results()
         profiling['pointer'] = None
```

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/ps.py` & `MindsDB-23.7.1.0/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/telemetry.py` & `MindsDB-23.7.1.0/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/mindsdb/utilities/wizards.py` & `MindsDB-23.7.1.0/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.5.1/requirements/requirements.txt` & `MindsDB-23.7.1.0/requirements/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 checksumdir >= 1.2.0
 duckdb == 0.6.0
 requests >= 2.0.0
 mysql-connector-python
 clickhouse-driver
 clickhouse-sqlalchemy
 charset-normalizer
-dill >= 0.3.4
 pyOpenSSL >= 22.0.0
 pydateinfer==0.3.0
 pyarrow >= 10.0.1, < 10.1.0
 dataprep_ml
 python-magic >= 0.4.27
 openpyxl >= 3.1.1
+dill == 0.3.6
 slack_sdk
```

### Comparing `MindsDB-23.6.5.1/setup.py` & `MindsDB-23.7.1.0/setup.py`

 * *Files identical despite different names*

