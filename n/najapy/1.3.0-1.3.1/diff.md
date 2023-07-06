# Comparing `tmp/najapy-1.3.0.tar.gz` & `tmp/najapy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "najapy-1.3.0.tar", last modified: Wed May 24 09:28:16 2023, max compression
+gzip compressed data, was "najapy-1.3.1.tar", last modified: Thu Jul  6 11:08:23 2023, max compression
```

## Comparing `najapy-1.3.0.tar` & `najapy-1.3.1.tar`

### file list

```diff
@@ -1,120 +1,135 @@
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.238783 najapy-1.3.0/
--rw-r--r--   0 lanqiao    (501) staff       (20)    11357 2022-07-06 03:22:18.000000 najapy-1.3.0/LICENSE
--rw-r--r--   0 lanqiao    (501) staff       (20)     2700 2023-05-24 09:28:16.237525 najapy-1.3.0/PKG-INFO
--rw-r--r--   0 lanqiao    (501) staff       (20)     2236 2022-07-06 03:22:18.000000 najapy-1.3.0/README.md
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.146727 najapy-1.3.0/najapy/
--rw-r--r--   0 lanqiao    (501) staff       (20)       48 2023-05-24 07:51:05.000000 najapy-1.3.0/najapy/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.151073 najapy-1.3.0/najapy/asyncio/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/asyncio/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3731 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/asyncio/future.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.153917 najapy-1.3.0/najapy/cache/
--rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/cache/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     4209 2023-05-24 08:53:21.000000 najapy-1.3.0/najapy/cache/base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    10506 2023-05-24 07:59:26.000000 najapy-1.3.0/najapy/cache/redis.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.164336 najapy-1.3.0/najapy/common/
--rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     8923 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/async_base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    21982 2023-03-17 06:07:48.000000 najapy-1.3.0/najapy/common/base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2827 2023-03-02 04:19:59.000000 najapy-1.3.0/najapy/common/buffer.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      564 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/error.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     6647 2022-10-14 09:29:48.000000 najapy-1.3.0/najapy/common/excel.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/interface.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/metaclass.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1681 2023-03-17 09:08:13.000000 najapy-1.3.0/najapy/common/process.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     8528 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/struct.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2607 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/task.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.167287 najapy-1.3.0/najapy/database/
--rw-r--r--   0 lanqiao    (501) staff       (20)       49 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/database/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3750 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/database/mongo.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    15285 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/database/mysql.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.168930 najapy-1.3.0/najapy/enum/
--rw-r--r--   0 lanqiao    (501) staff       (20)       19 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/enum/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3141 2023-02-07 09:30:47.000000 najapy-1.3.0/najapy/enum/base_enum.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.175118 najapy-1.3.0/najapy/event/
--rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/event/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3443 2023-03-20 10:41:03.000000 najapy-1.3.0/najapy/event/async_event.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1210 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/event/event.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.177235 najapy-1.3.0/najapy/frame/
--rwxr-xr-x   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.180622 najapy-1.3.0/najapy/frame/fastapi/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/fastapi/__init__.py
--rwxr-xr-x   0 lanqiao    (501) staff       (20)     3263 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/fastapi/base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3067 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/fastapi/form.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1042 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/fastapi/response.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1723 2023-03-02 04:30:39.000000 najapy-1.3.0/najapy/frame/fastapi/ws.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3334 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/logging.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.182276 najapy-1.3.0/najapy/net/
--rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/net/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     8066 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/net/http.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.183038 najapy-1.3.0/najapy/scaffold/
--rw-r--r--   0 lanqiao    (501) staff       (20)       16 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.184519 najapy-1.3.0/najapy/scaffold/fastapi_example_project/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.191698 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.192923 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.194246 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)       75 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/base_model.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.196572 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/
--rw-r--r--   0 lanqiao    (501) staff       (20)        1 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3629 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.198805 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      842 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      315 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/activate.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.200446 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.204074 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/external_view.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/internal_view.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/model.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/schemas.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/service.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.213139 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/
--rw-r--r--   0 lanqiao    (501) staff       (20)     3486 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.dev.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.rel.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      107 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/gunicorn.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.dev.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.rel.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      983 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1276 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/main.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      582 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/router.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.213545 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/services/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/services/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.214605 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/utils/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/utils/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1655 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      161 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/manage.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.216414 najapy-1.3.0/najapy/static/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/static/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)   208075 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/static/cacert.pem
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.150036 najapy-1.3.0/najapy.egg-info/
--rw-r--r--   0 lanqiao    (501) staff       (20)     2700 2023-05-24 09:28:15.000000 najapy-1.3.0/najapy.egg-info/PKG-INFO
--rw-r--r--   0 lanqiao    (501) staff       (20)     3949 2023-05-24 09:28:16.000000 najapy-1.3.0/najapy.egg-info/SOURCES.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)        1 2023-05-24 09:28:15.000000 najapy-1.3.0/najapy.egg-info/dependency_links.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)      499 2023-05-24 09:28:15.000000 najapy-1.3.0/najapy.egg-info/requires.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)       13 2023-05-24 09:28:15.000000 najapy-1.3.0/najapy.egg-info/top_level.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)       38 2023-05-24 09:28:16.239210 najapy-1.3.0/setup.cfg
--rw-r--r--   0 lanqiao    (501) staff       (20)     1898 2023-03-29 01:56:02.000000 najapy-1.3.0/setup.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.225534 najapy-1.3.0/tests/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-10-14 09:29:48.000000 najapy-1.3.0/tests/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      166 2022-10-14 09:29:48.000000 najapy-1.3.0/tests/main.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      863 2023-03-02 04:30:39.000000 najapy-1.3.0/tests/test_buffer.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3059 2023-01-12 02:07:34.000000 najapy-1.3.0/tests/test_func_cache.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.235584 najapy-1.3.0/tests/test_redis/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-03-15 01:19:41.000000 najapy-1.3.0/tests/test_redis/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     6863 2023-03-20 02:43:59.000000 najapy-1.3.0/tests/test_redis/conftest.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1337 2023-03-16 04:32:18.000000 najapy-1.3.0/tests/test_redis/mocks.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    26721 2023-03-29 02:50:21.000000 najapy-1.3.0/tests/test_redis/test_commands.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    10554 2023-03-20 02:45:47.000000 najapy-1.3.0/tests/test_redis/test_connection_pool.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2889 2023-03-27 06:50:02.000000 najapy-1.3.0/tests/test_redis/test_distributed_event.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2079 2023-03-24 10:25:17.000000 najapy-1.3.0/tests/test_redis/test_lock.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2587 2023-03-27 06:38:07.000000 najapy-1.3.0/tests/test_redis/test_pub_sub.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      923 2023-03-30 08:02:33.000000 najapy-1.3.0/tests/test_redis/test_share_cache.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1319 2022-11-21 08:43:49.000000 najapy-1.3.0/tests/test_utils.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.802632 najapy-1.3.1/
+-rw-r--r--   0 lanqiao    (501) staff       (20)    11357 2022-07-06 03:22:18.000000 najapy-1.3.1/LICENSE
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2836 2023-07-06 11:08:23.801777 najapy-1.3.1/PKG-INFO
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2372 2023-06-29 07:51:40.000000 najapy-1.3.1/README.md
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.747203 najapy-1.3.1/najapy/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       48 2023-06-29 07:33:14.000000 najapy-1.3.1/najapy/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.750529 najapy-1.3.1/najapy/asyncio/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/asyncio/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3731 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/asyncio/future.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.752102 najapy-1.3.1/najapy/cache/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/cache/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     4209 2023-05-24 08:53:21.000000 najapy-1.3.1/najapy/cache/base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    10506 2023-05-24 07:59:26.000000 najapy-1.3.1/najapy/cache/redis.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.758527 najapy-1.3.1/najapy/common/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     8923 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/async_base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    23020 2023-06-30 05:47:17.000000 najapy-1.3.1/najapy/common/base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2827 2023-03-02 04:19:59.000000 najapy-1.3.1/najapy/common/buffer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      564 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/error.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     6647 2022-10-14 09:29:48.000000 najapy-1.3.1/najapy/common/excel.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/interface.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/metaclass.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1691 2023-07-05 08:49:30.000000 najapy-1.3.1/najapy/common/pool.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1681 2023-03-17 09:08:13.000000 najapy-1.3.1/najapy/common/process.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     8528 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/struct.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2607 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/task.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.760176 najapy-1.3.1/najapy/database/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       49 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/database/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3750 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/database/mongo.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    15285 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/database/mysql.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.761336 najapy-1.3.1/najapy/enum/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       19 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/enum/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3141 2023-02-07 09:30:47.000000 najapy-1.3.1/najapy/enum/base_enum.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.763184 najapy-1.3.1/najapy/event/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/event/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3443 2023-07-03 12:07:52.000000 najapy-1.3.1/najapy/event/async_event.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1210 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/event/event.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.764351 najapy-1.3.1/najapy/frame/
+-rwxr-xr-x   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.767504 najapy-1.3.1/najapy/frame/fastapi/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/fastapi/__init__.py
+-rwxr-xr-x   0 lanqiao    (501) staff       (20)     3263 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/fastapi/base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3067 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/fastapi/form.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1042 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/fastapi/response.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1723 2023-03-02 04:30:39.000000 najapy-1.3.1/najapy/frame/fastapi/ws.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3334 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/logging.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.768273 najapy-1.3.1/najapy/middleware/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-06-29 07:36:25.000000 najapy-1.3.1/najapy/middleware/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.770605 najapy-1.3.1/najapy/middleware/rabbitmq/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-06-29 07:36:39.000000 najapy-1.3.1/najapy/middleware/rabbitmq/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     5629 2023-07-06 06:07:51.000000 najapy-1.3.1/najapy/middleware/rabbitmq/consumer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     7046 2023-07-05 08:41:39.000000 najapy-1.3.1/najapy/middleware/rabbitmq/producer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2649 2023-07-05 08:58:21.000000 najapy-1.3.1/najapy/middleware/rabbitmq/producer_pool.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.771861 najapy-1.3.1/najapy/net/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/net/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     8066 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/net/http.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.772416 najapy-1.3.1/najapy/scaffold/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       16 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.773312 najapy-1.3.1/najapy/scaffold/fastapi_example_project/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.775737 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.776284 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.777103 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)       75 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/base_model.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.778122 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        1 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3629 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.779253 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      842 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      315 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/activate.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.779907 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.782422 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/external_view.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/internal_view.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/model.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/schemas.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/service.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.786963 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3486 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.dev.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.rel.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      107 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/gunicorn.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.dev.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.rel.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      983 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1276 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/main.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      582 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/router.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.787361 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/services/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/services/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.788215 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/utils/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/utils/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1655 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      161 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/manage.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.789340 najapy-1.3.1/najapy/static/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/static/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)   208075 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/static/cacert.pem
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.749703 najapy-1.3.1/najapy.egg-info/
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2836 2023-07-06 11:08:23.000000 najapy-1.3.1/najapy.egg-info/PKG-INFO
+-rw-r--r--   0 lanqiao    (501) staff       (20)     4359 2023-07-06 11:08:23.000000 najapy-1.3.1/najapy.egg-info/SOURCES.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)        1 2023-07-06 11:08:23.000000 najapy-1.3.1/najapy.egg-info/dependency_links.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)      524 2023-07-06 11:08:23.000000 najapy-1.3.1/najapy.egg-info/requires.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)       13 2023-07-06 11:08:23.000000 najapy-1.3.1/najapy.egg-info/top_level.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)       38 2023-07-06 11:08:23.802809 najapy-1.3.1/setup.cfg
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1951 2023-06-30 07:24:25.000000 najapy-1.3.1/setup.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.793568 najapy-1.3.1/tests/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-10-14 09:29:48.000000 najapy-1.3.1/tests/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      166 2022-10-14 09:29:48.000000 najapy-1.3.1/tests/main.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      863 2023-03-02 04:30:39.000000 najapy-1.3.1/tests/test_buffer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3059 2023-01-12 02:07:34.000000 najapy-1.3.1/tests/test_func_cache.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1596 2023-07-04 09:54:43.000000 najapy-1.3.1/tests/test_obj_pool.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.795458 najapy-1.3.1/tests/test_rabbitmq/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       51 2023-07-05 02:21:37.000000 najapy-1.3.1/tests/test_rabbitmq/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1690 2023-07-06 10:37:21.000000 najapy-1.3.1/tests/test_rabbitmq/test_counsumer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3804 2023-07-06 10:59:25.000000 najapy-1.3.1/tests/test_rabbitmq/test_procuder_pool.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     4296 2023-07-05 09:02:09.000000 najapy-1.3.1/tests/test_rabbitmq/test_producer.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.800843 najapy-1.3.1/tests/test_redis/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-03-15 01:19:41.000000 najapy-1.3.1/tests/test_redis/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     6863 2023-03-20 02:43:59.000000 najapy-1.3.1/tests/test_redis/conftest.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1337 2023-03-16 04:32:18.000000 najapy-1.3.1/tests/test_redis/mocks.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    26721 2023-03-29 02:50:21.000000 najapy-1.3.1/tests/test_redis/test_commands.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    10554 2023-03-20 02:45:47.000000 najapy-1.3.1/tests/test_redis/test_connection_pool.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2889 2023-03-27 06:50:02.000000 najapy-1.3.1/tests/test_redis/test_distributed_event.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2079 2023-03-24 10:25:17.000000 najapy-1.3.1/tests/test_redis/test_lock.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2587 2023-03-27 06:38:07.000000 najapy-1.3.1/tests/test_redis/test_pub_sub.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      923 2023-03-30 08:02:33.000000 najapy-1.3.1/tests/test_redis/test_share_cache.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1319 2023-06-30 05:56:22.000000 najapy-1.3.1/tests/test_sync_utils.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1319 2023-06-30 03:14:48.000000 najapy-1.3.1/tests/test_utils.py
```

### Comparing `najapy-1.3.0/LICENSE` & `najapy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/PKG-INFO` & `najapy-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: najapy
-Version: 1.3.0
+Version: 1.3.1
 Summary: Async Suite For Python
 Home-page: https://github.com/lanqiao-dev/najapy.git
 Author: lanqiao
 Author-email: 
 License: Apache License Version 2.0
 Platform: all
 Classifier: Programming Language :: Python :: 3.8
@@ -48,11 +48,13 @@
 │    │    ├── async_event                       异步事件工具集
 │    │    └── event                          	同步事件工具集
 │    ├── frame                                  框架层
 │    │    ├── fastapi                          	fastapi工具集
 │    │    │    ├── base                         基础工具集
 │    │    │    └── response                     响应工具集
 │    │    └── logging                           日志工具类
+│    ├── middleware                             中间件层
+│    │    └── rabbitmq                          RabbitMQ
 │    ├── net                                    网络层
 │    │    ├── cacert                            根证书
 └────└──  └── http                          	http工具集
 ```
```

### Comparing `najapy-1.3.0/README.md` & `najapy-1.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,11 +32,13 @@
 │    │    ├── async_event                       异步事件工具集
 │    │    └── event                          	同步事件工具集
 │    ├── frame                                  框架层
 │    │    ├── fastapi                          	fastapi工具集
 │    │    │    ├── base                         基础工具集
 │    │    │    └── response                     响应工具集
 │    │    └── logging                           日志工具类
+│    ├── middleware                             中间件层
+│    │    └── rabbitmq                          RabbitMQ
 │    ├── net                                    网络层
 │    │    ├── cacert                            根证书
 └────└──  └── http                          	http工具集
 ```
```

### Comparing `najapy-1.3.0/najapy/asyncio/future.py` & `najapy-1.3.1/najapy/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/cache/base.py` & `najapy-1.3.1/najapy/cache/base.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/cache/redis.py` & `najapy-1.3.1/najapy/cache/redis.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/common/async_base.py` & `najapy-1.3.1/najapy/common/async_base.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/common/base.py` & `najapy-1.3.1/najapy/common/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import psutil
 import xmltodict
 import xml.dom.minidom
 import jwt
 import pytz
 import loguru
 import ujson
+from art import tprint
 from cachetools import TTLCache, cached
 import msgpack
 
 from najapy.common.metaclass import Singleton
 
 
 class _Utils(Singleton):
@@ -572,15 +573,15 @@
     def rsa_decryption(cls, pri_key_file_name: str, msg: str, split_length=128):
         msg = cls.b64_decode(msg, standard=True, for_bytes=True)
         private_key = cls.read_rsa_key(pri_key_file_name)
         cipher = PKCS1_cipher.new(private_key)
 
         res = []
         for i in range(0, len(msg), split_length):
-            res.append(cipher.decrypt(msg[i: i+split_length], 0))
+            res.append(cipher.decrypt(msg[i: i + split_length], 0))
 
         back_text = b"".join(res)
         return back_text.decode()
 
     @classmethod
     def ordered_dict(cls, val=None):
 
@@ -806,14 +807,49 @@
     def msgpack_encode(cls, val, **kwargs):
         return msgpack.dumps(val, **kwargs)
 
     @classmethod
     def msgpack_decode(cls, val, **kwargs):
         return msgpack.loads(val, **kwargs)
 
+    @staticmethod
+    def output_art(text="LQ-NAJAPY"):
+        fonts = ["varsity", "swampland", "sub-zero", "stforek", "soft", "chiseled", "standard", "block"]
+        font = random.choice(fonts)
+        tprint(text, font=font)
+
+    @staticmethod
+    def mask_id_number(id_number):
+        """
+        将身份证号进行脱敏处理，返回脱敏后的身份证号。
+        """
+        if len(id_number) == 15:
+            return id_number[:6] + '*' * 6 + id_number[-3:]
+        elif len(id_number) == 18:
+            return id_number[:6] + '*' * 8 + id_number[-4:]
+        else:
+            return id_number
+
+    @staticmethod
+    def validate_phone_simple_format(phone, no_area_code=False):
+        result = None
+
+        if not phone:
+            return result
+
+        match_res = re.match(r'^(\+86|86)?(1)\d{10}$', phone)
+        if not match_res:
+            return result
+
+        if no_area_code:
+            phone = re.sub(r'(\+86)|(86)', '', phone)
+
+        result = phone
+        return result
+
 
 @contextmanager
 def catch_error():
     """异常捕获，打印error级日志
 
     通过with语句捕获异常，代码更清晰，还可以使用Ignore异常安全的跳出with代码块
```

### Comparing `najapy-1.3.0/najapy/common/buffer.py` & `najapy-1.3.1/najapy/common/buffer.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/common/error.py` & `najapy-1.3.1/najapy/common/error.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/common/excel.py` & `najapy-1.3.1/najapy/common/excel.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/common/interface.py` & `najapy-1.3.1/najapy/common/interface.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/common/metaclass.py` & `najapy-1.3.1/najapy/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/common/process.py` & `najapy-1.3.1/najapy/common/process.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/common/struct.py` & `najapy-1.3.1/najapy/common/struct.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/common/task.py` & `najapy-1.3.1/najapy/common/task.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/database/mongo.py` & `najapy-1.3.1/najapy/database/mongo.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/database/mysql.py` & `najapy-1.3.1/najapy/database/mysql.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/enum/base_enum.py` & `najapy-1.3.1/najapy/enum/base_enum.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/event/async_event.py` & `najapy-1.3.1/najapy/event/async_event.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/event/event.py` & `najapy-1.3.1/najapy/event/event.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/frame/fastapi/base.py` & `najapy-1.3.1/najapy/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/frame/fastapi/form.py` & `najapy-1.3.1/najapy/frame/fastapi/form.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/frame/fastapi/response.py` & `najapy-1.3.1/najapy/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/frame/fastapi/ws.py` & `najapy-1.3.1/najapy/frame/fastapi/ws.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/frame/logging.py` & `najapy-1.3.1/najapy/frame/logging.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/net/http.py` & `najapy-1.3.1/najapy/net/http.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py` & `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py` & `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py` & `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py` & `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/main.py` & `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/main.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/router.py` & `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/router.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py` & `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy/static/cacert.pem` & `najapy-1.3.1/najapy/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/najapy.egg-info/PKG-INFO` & `najapy-1.3.1/najapy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: najapy
-Version: 1.3.0
+Version: 1.3.1
 Summary: Async Suite For Python
 Home-page: https://github.com/lanqiao-dev/najapy.git
 Author: lanqiao
 Author-email: 
 License: Apache License Version 2.0
 Platform: all
 Classifier: Programming Language :: Python :: 3.8
@@ -48,11 +48,13 @@
 │    │    ├── async_event                       异步事件工具集
 │    │    └── event                          	同步事件工具集
 │    ├── frame                                  框架层
 │    │    ├── fastapi                          	fastapi工具集
 │    │    │    ├── base                         基础工具集
 │    │    │    └── response                     响应工具集
 │    │    └── logging                           日志工具类
+│    ├── middleware                             中间件层
+│    │    └── rabbitmq                          RabbitMQ
 │    ├── net                                    网络层
 │    │    ├── cacert                            根证书
 └────└──  └── http                          	http工具集
 ```
```

### Comparing `najapy-1.3.0/setup.py` & `najapy-1.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,14 +46,16 @@
           r'xlrd==1.2.0',
           r'xmltodict==0.12.0',
           r'websockets==10.3',
           r'pyzmq==22.3.0',
           r'pytest-asyncio==0.18.3',
           r'pycryptodome==3.11.0',
           r'msgpack==1.0.3',
+          r'aio-pika==9.1.3',
+          r'art==6.0',
       ],
       classifiers=[
           r'Programming Language :: Python :: 3.8',
           r'License :: OSI Approved :: Apache Software License',
           r'Operating System :: POSIX :: Linux',
       ],
       )
```

### Comparing `najapy-1.3.0/tests/test_buffer.py` & `najapy-1.3.1/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/tests/test_func_cache.py` & `najapy-1.3.1/tests/test_func_cache.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/tests/test_redis/conftest.py` & `najapy-1.3.1/tests/test_redis/conftest.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/tests/test_redis/mocks.py` & `najapy-1.3.1/tests/test_redis/mocks.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/tests/test_redis/test_commands.py` & `najapy-1.3.1/tests/test_redis/test_commands.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/tests/test_redis/test_connection_pool.py` & `najapy-1.3.1/tests/test_redis/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/tests/test_redis/test_distributed_event.py` & `najapy-1.3.1/tests/test_redis/test_distributed_event.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/tests/test_redis/test_lock.py` & `najapy-1.3.1/tests/test_redis/test_lock.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/tests/test_redis/test_pub_sub.py` & `najapy-1.3.1/tests/test_redis/test_pub_sub.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/tests/test_redis/test_share_cache.py` & `najapy-1.3.1/tests/test_redis/test_share_cache.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.0/tests/test_utils.py` & `najapy-1.3.1/tests/test_utils.py`

 * *Files identical despite different names*

