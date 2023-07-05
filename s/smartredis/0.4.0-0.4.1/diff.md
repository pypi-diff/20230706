# Comparing `tmp/smartredis-0.4.0.tar.gz` & `tmp/smartredis-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartredis-0.4.0.tar", last modified: Wed Apr 12 19:48:02 2023, max compression
+gzip compressed data, was "smartredis-0.4.1.tar", last modified: Wed Jul  5 22:12:32 2023, max compression
```

## Comparing `smartredis-0.4.0.tar` & `smartredis-0.4.1.tar`

### file list

```diff
@@ -1,187 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-12 19:47:54.000000 smartredis-0.4.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 19:47:54.000000 smartredis-0.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 19:47:54.000000 smartredis-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-04-12 19:47:54.000000 smartredis-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-12 19:48:02.582703 smartredis-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-12 19:47:54.000000 smartredis-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.570703 smartredis-0.4.0/build-scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-catch.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-keydb.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-lcov.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      583 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-redis.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      984 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-redisai-cpu.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2025 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build-redisai-gpu.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_c_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      548 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_cpp_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_cpp_unit_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_deps.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_fortran_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_lib.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_parallel_examples.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_serial_examples.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-04-12 19:47:54.000000 smartredis-0.4.0/build-scripts/build_test_deps.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.574703 smartredis-0.4.0/include/
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/address.h
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/addressallcommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/addressanycommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/addressatcommand.h
--rw-r--r--   0 runner    (1001) docker     (123)    80168 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/c_client.h
--rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/c_dataset.h
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/c_logcontext.h
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/c_logger.h
--rw-r--r--   0 runner    (1001) docker     (123)    84208 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/client.h
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/clusterinfocommand.h
--rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/command.h
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/command.tcc
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/commandlist.h
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/commandlist.tcc
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/commandreply.h
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/compoundcommand.h
--rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/dataset.h
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/dbinfocommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/dbnode.h
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/enum_fortran.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/gettensorcommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/keyedcommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/logcontext.h
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/logger.h
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/metadata.h
--rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/metadatabuffer.h
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/metadatafield.h
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/multikeycommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/nonkeyedcommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/pipelinereply.h
--rw-r--r--   0 runner    (1001) docker     (123)    46159 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/pyclient.h
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/pydataset.h
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/pylogcontext.h
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/pysrobject.h
--rw-r--r--   0 runner    (1001) docker     (123)    25115 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/redis.h
--rw-r--r--   0 runner    (1001) docker     (123)    34070 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/rediscluster.h
--rw-r--r--   0 runner    (1001) docker     (123)    30049 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/redisserver.h
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/scalarfield.h
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/scalarfield.tcc
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/sharedmemorylist.h
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/sharedmemorylist.tcc
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/singlekeycommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/sr_enums.h
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/srassert.h
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/srexception.h
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/srobject.h
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/stringfield.h
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/tensor.h
--rw-r--r--   0 runner    (1001) docker     (123)    15135 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/tensor.tcc
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/tensorbase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/tensorpack.h
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/threadpool.h
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-12 19:47:54.000000 smartredis-0.4.0/include/utility.h
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 19:47:54.000000 smartredis-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-12 19:47:54.000000 smartredis-0.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 19:47:54.000000 smartredis-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-12 19:48:02.586703 smartredis-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-12 19:47:54.000000 smartredis-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.566703 smartredis-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.574703 smartredis-0.4.0/src/c/
--rw-r--r--   0 runner    (1001) docker     (123)    45629 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/c/c_client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/c/c_dataset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/c/c_error.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/c/c_logcontext.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/c/c_logger.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.578703 smartredis-0.4.0/src/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/address.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/addressallcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/addressanycommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/addressatcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    75366 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/clusterinfocommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/command.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/commandlist.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/commandreply.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/compoundcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/dataset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/dbinfocommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/dbnode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/gettensorcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/keyedcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/logger.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23018 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/metadata.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/metadatafield.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/multikeycommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/nonkeyedcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/pipelinereply.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28292 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/redis.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    51252 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/rediscluster.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/redisserver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/singlekeycommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/srobject.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/stringfield.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/tensorbase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/tensorpack.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/threadpool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/cpp/utility.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.578703 smartredis-0.4.0/src/fortran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/fortran/client/
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/aggregation_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/client_dataset_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/client_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/ensemble_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/misc_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)    21033 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/model_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/put_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/put_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/script_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/unpack_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client/unpack_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (123)    91170 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/client.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/fortran/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/add_meta_scalar_common.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/add_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/dataset_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/get_meta_scalars_common.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/metadata_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (123)    26425 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/dataset.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/fortran/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/errors/errors_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/errors.F90
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/fortran_c_interop.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/fortran/logcontext/
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/logcontext/logcontext_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/logcontext.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/fortran/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/logger/logger_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/fortran/logger.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.566703 smartredis-0.4.0/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/python/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/bindings/bind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.566703 smartredis-0.4.0/src/python/module/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/python/module/smartredis/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69915 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/logcontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/srobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/module/smartredis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/python/module/smartredis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 19:48:02.000000 smartredis-0.4.0/src/python/module/smartredis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/src/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)    22479 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/src/pyclient.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/src/pydataset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/src/pylogcontext.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-12 19:47:54.000000 smartredis-0.4.0/src/python/src/pysrobject.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      726 2023-04-12 19:47:54.000000 smartredis-0.4.0/utils/check_redis.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:02.582703 smartredis-0.4.0/utils/create_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-12 19:47:54.000000 smartredis-0.4.0/utils/create_cluster/local_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-04-12 19:47:54.000000 smartredis-0.4.0/utils/create_cluster/slurm_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    71347 2023-04-12 19:47:54.000000 smartredis-0.4.0/utils/create_cluster/smartredisdb.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.786870 smartredis-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-07-05 22:12:24.000000 smartredis-0.4.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-05 22:12:24.000000 smartredis-0.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-05 22:12:24.000000 smartredis-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21880 2023-07-05 22:12:24.000000 smartredis-0.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-05 22:12:32.786870 smartredis-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-05 22:12:24.000000 smartredis-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.746869 smartredis-0.4.1/build-scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build-catch.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build-keydb.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build-lcov.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      583 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build-redis.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      984 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build-redisai-cpu.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2025 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build-redisai-gpu.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build_c_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      548 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build_cpp_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build_cpp_unit_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build_deps.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build_fortran_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build_lib.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build_parallel_examples.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build_serial_examples.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-07-05 22:12:24.000000 smartredis-0.4.1/build-scripts/build_test_deps.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.766870 smartredis-0.4.1/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/address.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/addressallcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/addressanycommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/addressatcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80168 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/c_client.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/c_configoptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/c_dataset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/c_logcontext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/c_logger.h
+-rw-r--r--   0 runner    (1001) docker     (123)    84208 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/client.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/clusterinfocommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/command.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/command.tcc
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/commandlist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/commandlist.tcc
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/commandreply.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/compoundcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/configoptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21100 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/dataset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/dbinfocommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/dbnode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/enum_fortran.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/gettensorcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/keyedcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/logcontext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/logger.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/metadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/metadatabuffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/metadatafield.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/multikeycommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/nonkeyedcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/pipelinereply.h
+-rw-r--r--   0 runner    (1001) docker     (123)    46159 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/pyclient.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/pyconfigoptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/pydataset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/pylogcontext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/pysrobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25115 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/redis.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34070 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/rediscluster.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30017 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/redisserver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/scalarfield.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/scalarfield.tcc
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/sharedmemorylist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/sharedmemorylist.tcc
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/singlekeycommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/sr_enums.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/srassert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/srexception.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/srobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/stringfield.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15135 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/tensor.tcc
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/tensorbase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/tensorpack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/threadpool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-05 22:12:24.000000 smartredis-0.4.1/include/utility.h
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-05 22:12:24.000000 smartredis-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-05 22:12:24.000000 smartredis-0.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 22:12:24.000000 smartredis-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-05 22:12:32.786870 smartredis-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-05 22:12:24.000000 smartredis-0.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-05 22:12:24.000000 smartredis-0.4.1/smartredis_defs.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.746869 smartredis-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.770870 smartredis-0.4.1/src/c/
+-rw-r--r--   0 runner    (1001) docker     (123)    45629 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/c/c_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/c/c_configoptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/c/c_dataset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/c/c_error.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/c/c_logcontext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/c/c_logger.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.778870 smartredis-0.4.1/src/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/addressallcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/addressanycommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/addressatcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    75366 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/clusterinfocommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/command.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/commandlist.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/commandreply.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/compoundcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/configoptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/dataset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/dbinfocommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/dbnode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/gettensorcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/keyedcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23018 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/metadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/metadatafield.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/multikeycommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/nonkeyedcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/pipelinereply.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28324 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/redis.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    51284 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/rediscluster.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/redisserver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/singlekeycommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/srobject.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/stringfield.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/tensorbase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/tensorpack.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/threadpool.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/cpp/utility.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.778870 smartredis-0.4.1/src/fortran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.782870 smartredis-0.4.1/src/fortran/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/aggregation_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/client_dataset_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/client_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/ensemble_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/misc_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    21033 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/model_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/put_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/put_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/script_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/unpack_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client/unpack_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    92158 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/client.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.782870 smartredis-0.4.1/src/fortran/configoptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/configoptions/configoptions_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/configoptions.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.782870 smartredis-0.4.1/src/fortran/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/dataset/add_meta_scalar_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/dataset/add_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/dataset/dataset_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/dataset/get_meta_scalars_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/dataset/metadata_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/dataset/tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/dataset.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.782870 smartredis-0.4.1/src/fortran/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/errors/errors_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/errors.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/fortran_c_interop.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.782870 smartredis-0.4.1/src/fortran/logcontext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/logcontext/logcontext_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/logcontext.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.782870 smartredis-0.4.1/src/fortran/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/logger/logger_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/fortran/logger.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.746869 smartredis-0.4.1/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.782870 smartredis-0.4.1/src/python/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/bindings/bind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.746869 smartredis-0.4.1/src/python/module/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.786870 smartredis-0.4.1/src/python/module/smartredis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/module/smartredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72577 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/module/smartredis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/module/smartredis/configoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/module/smartredis/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/module/smartredis/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/module/smartredis/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/module/smartredis/logcontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/module/smartredis/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/module/smartredis/srobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/module/smartredis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.786870 smartredis-0.4.1/src/python/module/smartredis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-05 22:12:32.000000 smartredis-0.4.1/src/python/module/smartredis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-05 22:12:32.000000 smartredis-0.4.1/src/python/module/smartredis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:12:32.000000 smartredis-0.4.1/src/python/module/smartredis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:12:32.000000 smartredis-0.4.1/src/python/module/smartredis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-05 22:12:32.000000 smartredis-0.4.1/src/python/module/smartredis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 22:12:32.000000 smartredis-0.4.1/src/python/module/smartredis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.786870 smartredis-0.4.1/src/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    22426 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/src/pyclient.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/src/pyconfigoptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/src/pydataset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/src/pylogcontext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-05 22:12:24.000000 smartredis-0.4.1/src/python/src/pysrobject.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.786870 smartredis-0.4.1/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      726 2023-07-05 22:12:24.000000 smartredis-0.4.1/utils/check_redis.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:12:32.786870 smartredis-0.4.1/utils/create_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-05 22:12:24.000000 smartredis-0.4.1/utils/create_cluster/local_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-05 22:12:24.000000 smartredis-0.4.1/utils/create_cluster/slurm_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71347 2023-07-05 22:12:24.000000 smartredis-0.4.1/utils/create_cluster/smartredisdb.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-05 22:12:24.000000 smartredis-0.4.1/utils/launch_redis.py
```

### Comparing `smartredis-0.4.0/CMakeLists.txt` & `smartredis-0.4.1/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,150 +20,178 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-project(SmartRedis)
+# Enable setting version in the project statement
+if (POLICY CMP0048)
+    cmake_policy(SET CMP0048 NEW)
+endif (POLICY CMP0048)
 
+# Project definition for the SmartRedis project
 cmake_minimum_required(VERSION 3.13)
+project(SmartRedis VERSION "0.4.0")
 
-option(BUILD_PYTHON  "Build the python module" ON)
-option(BUILD_FORTRAN "Build the fortran client library" OFF)
-option(COVERAGE "Build the fortran client library" OFF)
+# Configure options for the SmartRedis project
+option(SR_PYTHON  "Build the python module" OFF)
+option(SR_FORTRAN "Build the fortran client library" OFF)
+option(SR_PEDANTIC "Build with pickiest compiler settings" OFF)
 
-set(CMAKE_BUILD_TYPE RELEASE)
 set(CMAKE_CXX_STANDARD 17)
 set(CMAKE_INSTALL_PREFIX ${CMAKE_SOURCE_DIR}/install)
 set(CMAKE_CXX_VISIBILITY_PRESET default)
 set(THREADS_PREFER_PTHREAD_FLAG ON)
+set(CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR})
+include(smartredis_defs)
 
-if (BUILD_FORTRAN)
+# If we want to use Fortran, we have to tell CMake to use it
+if (SR_FORTRAN)
     enable_language(Fortran)
 endif()
 
-if (WERROR)
+# For now, we only support Pedantic on the main library build.
+# If/when we fine-tune the examples and test cases, move this block
+# to smartredis_defs.cmake
+if (SR_PEDANTIC)
     if((CMAKE_CXX_COMPILER_ID STREQUAL "GNU") AND (CMAKE_C_COMPILER_ID STREQUAL "GNU"))
         add_compile_options(-Wall -Werror)
     else()
-        message(WARNING "WERROR was specified, but the CMAKE compiler is not GCC")
+        message(WARNING "SR_PEDANTIC was specified, but the CMAKE compiler is not GCC")
     endif()
-endif()
-
-if (COVERAGE)
-    if((CMAKE_CXX_COMPILER_ID STREQUAL "GNU") AND (CMAKE_C_COMPILER_ID STREQUAL "GNU"))
-        add_compile_options(--coverage)
-        add_link_options(--coverage)
-    else()
-        message(WARNING "COVERAGE was specified, but the CMAKE compiler is not GCC")
+    if(CMAKE_Fortran_COMPILER_ID STREQUAL "GNU")
+        set(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS} -Wno-maybe-uninitialized")
     endif()
 endif()
 
-find_library(REDISPP redis++ PATHS ${CMAKE_SOURCE_DIR}/install/lib NO_DEFAULT_PATH REQUIRED)
-find_library(HIREDIS hiredis PATHS ${CMAKE_SOURCE_DIR}/install/lib NO_DEFAULT_PATH REQUIRED)
+# Bring in third-party libaries needed for the SmartRedis library
+find_library(REDISPP redis++
+    PATHS ${CMAKE_SOURCE_DIR}/install/lib NO_DEFAULT_PATH
+    REQUIRED STATIC
+)
+find_library(HIREDIS hiredis
+    PATHS ${CMAKE_SOURCE_DIR}/install/lib NO_DEFAULT_PATH
+    REQUIRED STATIC
+)
 find_package(Threads REQUIRED)
-
 set(EXT_CLIENT_LIBRARIES ${REDISPP} ${HIREDIS})
 
+# Define source code that goes into the SmartRedis library
 set(CLIENT_SRC
     src/c/c_client.cpp
+    src/c/c_configoptions.cpp
     src/c/c_dataset.cpp
     src/c/c_error.cpp
     src/c/c_logcontext.cpp
     src/c/c_logger.cpp
     src/cpp/address.cpp
+    src/cpp/addressallcommand.cpp
+    src/cpp/addressanycommand.cpp
+    src/cpp/addressatcommand.cpp
     src/cpp/client.cpp
-    src/cpp/dataset.cpp
+    src/cpp/clusterinfocommand.cpp
     src/cpp/command.cpp
-    src/cpp/keyedcommand.cpp
-    src/cpp/nonkeyedcommand.cpp
-    src/cpp/multikeycommand.cpp
-    src/cpp/singlekeycommand.cpp
+    src/cpp/commandlist.cpp
+    src/cpp/commandreply.cpp
     src/cpp/compoundcommand.cpp
-    src/cpp/addressatcommand.cpp
-    src/cpp/addressanycommand.cpp
-    src/cpp/addressallcommand.cpp
-    src/cpp/clusterinfocommand.cpp
+    src/cpp/configoptions.cpp
+    src/cpp/dataset.cpp
     src/cpp/dbinfocommand.cpp
+    src/cpp/dbnode.cpp
     src/cpp/gettensorcommand.cpp
-    src/cpp/commandlist.cpp
+    src/cpp/keyedcommand.cpp
+    src/cpp/logger.cpp
     src/cpp/metadata.cpp
-    src/cpp/tensorbase.cpp
-    src/cpp/tensorpack.cpp
-    src/cpp/dbnode.cpp
-    src/cpp/commandreply.cpp
-    src/cpp/redisserver.cpp
-    src/cpp/rediscluster.cpp
-    src/cpp/redis.cpp
     src/cpp/metadatafield.cpp
-    src/cpp/stringfield.cpp
+    src/cpp/multikeycommand.cpp
+    src/cpp/nonkeyedcommand.cpp
     src/cpp/pipelinereply.cpp
+    src/cpp/redis.cpp
+    src/cpp/rediscluster.cpp
+    src/cpp/redisserver.cpp
+    src/cpp/singlekeycommand.cpp
+    src/cpp/srobject.cpp
+    src/cpp/stringfield.cpp
+    src/cpp/tensorbase.cpp
+    src/cpp/tensorpack.cpp
     src/cpp/threadpool.cpp
     src/cpp/utility.cpp
-    src/cpp/logger.cpp
-    src/cpp/srobject.cpp
 )
 
+# Define include directories for header files
 include_directories(SYSTEM
     include
     install/include
 )
 
-if (BUILD_FORTRAN)
+# Build the Fortran library
+if (SR_FORTRAN)
     set(FORTRAN_SRC
         src/fortran/errors.F90
         src/fortran/client.F90
+        src/fortran/configoptions.F90
         src/fortran/dataset.F90
         src/fortran/fortran_c_interop.F90
         src/fortran/logcontext.F90
         src/fortran/logger.F90
     )
     include_directories(src/fortran)
     # Note the following has to be before ANY add_library command)
     set(CMAKE_Fortran_MODULE_DIRECTORY "${CMAKE_INSTALL_PREFIX}/include")
     # Fortran library
-    add_library(smartredis-fortran SHARED ${FORTRAN_SRC})
-    set_target_properties(smartredis-fortran PROPERTIES SUFFIX ".so")
+    add_library(smartredis-fortran ${SMARTREDIS_LINK_MODE} ${FORTRAN_SRC})
+    set_target_properties(smartredis-fortran PROPERTIES
+        SUFFIX ${SMARTREDIS_LINK_LIBRARY_SUFFIX}
+    )
+	set_target_properties(smartredis-fortran PROPERTIES
+		OUTPUT_NAME ${SMARTREDIS_FORTRAN_LIB}
+	)
     target_link_libraries(smartredis-fortran PUBLIC smartredis ${EXT_CLIENT_LIBRARIES})
     # Install dynamic library and headers
     install(TARGETS smartredis-fortran
     	LIBRARY DESTINATION lib)
 endif()
 
 
-# Build dynamic library
-add_library(smartredis SHARED ${CLIENT_SRC})
-set_target_properties(smartredis PROPERTIES SUFFIX ".so")
+# Build the main SmartRedis library
+add_library(smartredis ${SMARTREDIS_LINK_MODE} ${CLIENT_SRC})
+set_target_properties(smartredis PROPERTIES
+    SUFFIX ${SMARTREDIS_LINK_LIBRARY_SUFFIX}
+)
+set_target_properties(smartredis PROPERTIES
+    OUTPUT_NAME ${SMARTREDIS_LIB}
+)
 target_link_libraries(smartredis PUBLIC ${EXT_CLIENT_LIBRARIES} PRIVATE Threads::Threads)
 
+# Install SmartRedis header files
 install(DIRECTORY "${CMAKE_SOURCE_DIR}/include/"
         DESTINATION "include"
         FILES_MATCHING
         PATTERN "*.h" PATTERN "*.tcc" PATTERN "*.inc"
 )
 
 # Install dynamic library and headers
 install(TARGETS smartredis
      	LIBRARY DESTINATION lib)
 
-if(BUILD_PYTHON)
+# Build the Python library for SmartRedis
+if(SR_PYTHON)
 	message("-- Python client build enabled")
 	add_subdirectory(${CMAKE_SOURCE_DIR}/third-party/pybind
                      ${CMAKE_SOURCE_DIR}/third-party/pybind/build)
 
-    add_library(smartredis_static STATIC ${CLIENT_SRC})
-
 	pybind11_add_module(smartredisPy
-                        src/python/src/pysrobject.cpp
-                        src/python/src/pylogcontext.cpp
 	                    src/python/src/pyclient.cpp
+                        src/python/src/pyconfigoptions.cpp
                         src/python/src/pydataset.cpp
+                        src/python/src/pylogcontext.cpp
+                        src/python/src/pysrobject.cpp
                         ${CLIENT_SRC}
                         src/python/bindings/bind.cpp)
 
 	target_link_libraries(smartredisPy PUBLIC ${EXT_CLIENT_LIBRARIES})
-	install(TARGETS smartredisPy
-	        LIBRARY DESTINATION lib)
+	install(TARGETS smartredisPy LIBRARY DESTINATION lib)
+    install(TARGETS smartredisPy LIBRARY DESTINATION ../src/python/module/smartredis)
 else()
 	message("-- Skipping Python client build")
 endif()
```

### Comparing `smartredis-0.4.0/LICENSE.md` & `smartredis-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/PKG-INFO` & `smartredis-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartredis
-Version: 0.4.0
+Version: 0.4.1
 Summary: RedisAI clients for SmartSim
 Home-page: https://github.com/CrayLabs/SmartRedis
 Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
 Author-email: craylabs@hpe.com
 License: BSD 2-Clause License
 Project-URL: Source, https://github.com/CrayLabs/SmartRedis
 Project-URL: Documentation, https://www.craylabs.org
@@ -38,20 +38,20 @@
         # SmartRedis
         
         SmartRedis is a collection of Redis clients that support
         RedisAI capabilities and include additional
         features for high performance computing (HPC) applications.
         SmartRedis provides clients in the following languages:
         
-        | Language   | Version/Standard  |
-        |------------|:-----------------:|
-        | Python     |   3.7, 3.8, 3.9   |
-        | C++        |   C++17           |
-        | C          |   C99             |
-        | Fortran    |   Fortran 2018    |
+        | Language   | Version/Standard                               |
+        |------------|:----------------------------------------------:|
+        | Python     |   3.7, 3.8, 3.9, 3.10                          |
+        | C++        |   C++17                                        |
+        | C          |   C99                                          |
+        | Fortran    |   Fortran 2018 (GNU/Intel), 2003 (PGI/Nvidia)  |
         
         SmartRedis is used in the [SmartSim library](https://github.com/CrayLabs/SmartSim).
         SmartSim makes it easier to use common Machine Learning (ML) libraries like
         PyTorch and TensorFlow in numerical simulations at scale.  SmartRedis connects
         these simulations to a Redis database or Redis database cluster for
         data storage, script execution, and model evaluation.  While SmartRedis
         contains features for simulation workflows on supercomputers, SmartRedis
@@ -63,54 +63,60 @@
         SmartRedis installation instructions are currently hosted as part of the
         [SmartSim library installation instructions](https://www.craylabs.org/docs/installation.html#smartredis)
         Additionally, detailed [API documents](https://www.craylabs.org/docs/api/smartredis_api.html) are also available as
         part of the SmartSim documentation.
         
         ## Dependencies
         
-        SmartRedis utilizes the following libraries.
+        SmartRedis utilizes the following libraries:
         
          - [NumPy](https://github.com/numpy/numpy)
-         - [Hiredis](https://github.com/redis/hiredis) 1.0.0
-         - [Redis-plus-plus](https://github.com/sewenew/redis-plus-plus)  1.2.3
+         - [Hiredis](https://github.com/redis/hiredis) 1.1.0
+         - [Redis-plus-plus](https://github.com/sewenew/redis-plus-plus) 1.3.5
         
         ## Publications
         
         The following are public presentations or publications using SmartRedis
         
          - [Collaboration with NCAR - CGD Seminar](https://www.youtube.com/watch?v=2e-5j427AS0)
-         - [Using Machine Learning in HPC Simulations - paper (pre-print)](https://arxiv.org/abs/2104.09355)
+         - [Using Machine Learning in HPC Simulations - paper](https://www.sciencedirect.com/science/article/pii/S1877750322001065)
+         - [Relexi — A scalable open source reinforcement learning framework for high-performance computing - paper](https://www.sciencedirect.com/science/article/pii/S2665963822001063)
         
         ## Cite
         
-        Please use the following citation when referencing SmartSim, SmartRedis, or any SmartSim related work.
+        Please use the following citation when referencing SmartSim, SmartRedis, or any SmartSim related work:
         
-        
-        Partee et al., “Using Machine Learning at Scale in HPC Simulations with SmartSim:
-        An Application to Ocean Climate Modeling,” arXiv:2104.09355, Apr. 2021,
-        [Online]. Available: http://arxiv.org/abs/2104.09355.
+            Partee et al., "Using Machine Learning at scale in numerical simulations with SmartSim:
+            An application to ocean climate modeling",
+            Journal of Computational Science, Volume 62, 2022, 101707, ISSN 1877-7503.
+            Open Access: https://doi.org/10.1016/j.jocs.2022.101707.
         
         ### bibtex
         
-            ```latex
-            @misc{partee2021using,
-                  title={Using Machine Learning at Scale in HPC Simulations with SmartSim: An Application to Ocean Climate Modeling},
-                  author={Sam Partee and Matthew Ellis and Alessandro Rigazzi and Scott Bachman and Gustavo Marques and Andrew Shao and Benjamin Robbins},
-                  year={2021},
-                  eprint={2104.09355},
-                  archivePrefix={arXiv},
-                  primaryClass={cs.CE}
-            }
-            ```
+            @article{PARTEE2022101707,
+                title = {Using Machine Learning at scale in numerical simulations with SmartSim:
+                An application to ocean climate modeling},
+                journal = {Journal of Computational Science},
+                volume = {62},
+                pages = {101707},
+                year = {2022},
+                issn = {1877-7503},
+                doi = {https://doi.org/10.1016/j.jocs.2022.101707},
+                url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
+                author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E. Shao
+                and Scott Bachman and Gustavo Marques and Benjamin Robbins},
+                keywords = {Deep learning, Numerical simulation, Climate modeling, High performance computing, SmartSim},
+                }
         
 Keywords: redis,clients,hpc,ai,deep learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartredis Version: 0.4.0 Summary: RedisAI clients
+Metadata-Version: 2.1 Name: smartredis Version: 0.4.1 Summary: RedisAI clients
 for SmartSim Home-page: https://github.com/CrayLabs/SmartRedis Author:
 CrayLabs, a Hewlett Packard Enterprise OSS Organization Author-email:
 craylabs@hpe.com License: BSD 2-Clause License Project-URL: Source, https://
 github.com/CrayLabs/SmartRedis Project-URL: Documentation, https://
 www.craylabs.org Description:
     [https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/
                           SmartSim_Large.png][Image]
@@ -20,43 +20,52 @@
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![codecov](https://codecov.io/gh/CrayLabs/SmartRedis/
 branch/develop/graph/badge.svg?token=XSS8CCJ2KR)](https://codecov.io/gh/
 CrayLabs/SmartRedis) ---------- # SmartRedis SmartRedis is a collection of
 Redis clients that support RedisAI capabilities and include additional features
 for high performance computing (HPC) applications. SmartRedis provides clients
 in the following languages: | Language | Version/Standard | |------------|:----
--------------:| | Python | 3.7, 3.8, 3.9 | | C++ | C++17 | | C | C99 | |
-Fortran | Fortran 2018 | SmartRedis is used in the [SmartSim library](https://
-github.com/CrayLabs/SmartSim). SmartSim makes it easier to use common Machine
-Learning (ML) libraries like PyTorch and TensorFlow in numerical simulations at
-scale. SmartRedis connects these simulations to a Redis database or Redis
-database cluster for data storage, script execution, and model evaluation.
-While SmartRedis contains features for simulation workflows on supercomputers,
+------------------------------------------:| | Python | 3.7, 3.8, 3.9, 3.10 | |
+C++ | C++17 | | C | C99 | | Fortran | Fortran 2018 (GNU/Intel), 2003 (PGI/
+Nvidia) | SmartRedis is used in the [SmartSim library](https://github.com/
+CrayLabs/SmartSim). SmartSim makes it easier to use common Machine Learning
+(ML) libraries like PyTorch and TensorFlow in numerical simulations at scale.
+SmartRedis connects these simulations to a Redis database or Redis database
+cluster for data storage, script execution, and model evaluation. While
+SmartRedis contains features for simulation workflows on supercomputers,
 SmartRedis is fully functional as a RedisAI client library and can be used
 without SmartSim in any Python, C++, C, or Fortran project. ## Using SmartRedis
 SmartRedis installation instructions are currently hosted as part of the
 [SmartSim library installation instructions](https://www.craylabs.org/docs/
 installation.html#smartredis) Additionally, detailed [API documents](https://
 www.craylabs.org/docs/api/smartredis_api.html) are also available as part of
 the SmartSim documentation. ## Dependencies SmartRedis utilizes the following
-libraries. - [NumPy](https://github.com/numpy/numpy) - [Hiredis](https://
-github.com/redis/hiredis) 1.0.0 - [Redis-plus-plus](https://github.com/sewenew/
-redis-plus-plus) 1.2.3 ## Publications The following are public presentations
+libraries: - [NumPy](https://github.com/numpy/numpy) - [Hiredis](https://
+github.com/redis/hiredis) 1.1.0 - [Redis-plus-plus](https://github.com/sewenew/
+redis-plus-plus) 1.3.5 ## Publications The following are public presentations
 or publications using SmartRedis - [Collaboration with NCAR - CGD Seminar]
 (https://www.youtube.com/watch?v=2e-5j427AS0) - [Using Machine Learning in HPC
-Simulations - paper (pre-print)](https://arxiv.org/abs/2104.09355) ## Cite
-Please use the following citation when referencing SmartSim, SmartRedis, or any
-SmartSim related work. Partee et al., âUsing Machine Learning at Scale in HPC
-Simulations with SmartSim: An Application to Ocean Climate Modeling,â arXiv:
-2104.09355, Apr. 2021, [Online]. Available: http://arxiv.org/abs/2104.09355.
-### bibtex ```latex @misc{partee2021using, title={Using Machine Learning at
-Scale in HPC Simulations with SmartSim: An Application to Ocean Climate
-Modeling}, author={Sam Partee and Matthew Ellis and Alessandro Rigazzi and
-Scott Bachman and Gustavo Marques and Andrew Shao and Benjamin Robbins}, year=
-{2021}, eprint={2104.09355}, archivePrefix={arXiv}, primaryClass={cs.CE} } ```
-Keywords: redis,clients,hpc,ai,deep learning Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Simulations - paper](https://www.sciencedirect.com/science/article/pii/
+S1877750322001065) - [Relexi â A scalable open source reinforcement learning
+framework for high-performance computing - paper](https://
+www.sciencedirect.com/science/article/pii/S2665963822001063) ## Cite Please use
+the following citation when referencing SmartSim, SmartRedis, or any SmartSim
+related work: Partee et al., "Using Machine Learning at scale in numerical
+simulations with SmartSim: An application to ocean climate modeling", Journal
+of Computational Science, Volume 62, 2022, 101707, ISSN 1877-7503. Open Access:
+https://doi.org/10.1016/j.jocs.2022.101707. ### bibtex @article
+{PARTEE2022101707, title = {Using Machine Learning at scale in numerical
+simulations with SmartSim: An application to ocean climate modeling}, journal =
+{Journal of Computational Science}, volume = {62}, pages = {101707}, year =
+{2022}, issn = {1877-7503}, doi = {https://doi.org/10.1016/j.jocs.2022.101707},
+url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
+author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E.
+Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins}, keywords =
+{Deep learning, Numerical simulation, Climate modeling, High performance
+computing, SmartSim}, } Keywords: redis,clients,hpc,ai,deep learning Platform:
+UNKNOWN Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 License :: OSI Approved :: BSD License Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Scientific/Engineering Requires-Python:
 <3.11,>=3.7 Description-Content-Type: text/markdown Provides-Extra: dev
 Provides-Extra: doc Provides-Extra: xarray
```

### Comparing `smartredis-0.4.0/README.md` & `smartredis-0.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 # SmartRedis
 
 SmartRedis is a collection of Redis clients that support
 RedisAI capabilities and include additional
 features for high performance computing (HPC) applications.
 SmartRedis provides clients in the following languages:
 
-| Language   | Version/Standard  |
-|------------|:-----------------:|
-| Python     |   3.7, 3.8, 3.9   |
-| C++        |   C++17           |
-| C          |   C99             |
-| Fortran    |   Fortran 2018    |
+| Language   | Version/Standard                               |
+|------------|:----------------------------------------------:|
+| Python     |   3.7, 3.8, 3.9, 3.10                          |
+| C++        |   C++17                                        |
+| C          |   C99                                          |
+| Fortran    |   Fortran 2018 (GNU/Intel), 2003 (PGI/Nvidia)  |
 
 SmartRedis is used in the [SmartSim library](https://github.com/CrayLabs/SmartSim).
 SmartSim makes it easier to use common Machine Learning (ML) libraries like
 PyTorch and TensorFlow in numerical simulations at scale.  SmartRedis connects
 these simulations to a Redis database or Redis database cluster for
 data storage, script execution, and model evaluation.  While SmartRedis
 contains features for simulation workflows on supercomputers, SmartRedis
@@ -53,41 +53,46 @@
 SmartRedis installation instructions are currently hosted as part of the
 [SmartSim library installation instructions](https://www.craylabs.org/docs/installation.html#smartredis)
 Additionally, detailed [API documents](https://www.craylabs.org/docs/api/smartredis_api.html) are also available as
 part of the SmartSim documentation.
 
 ## Dependencies
 
-SmartRedis utilizes the following libraries.
+SmartRedis utilizes the following libraries:
 
  - [NumPy](https://github.com/numpy/numpy)
- - [Hiredis](https://github.com/redis/hiredis) 1.0.0
- - [Redis-plus-plus](https://github.com/sewenew/redis-plus-plus)  1.2.3
+ - [Hiredis](https://github.com/redis/hiredis) 1.1.0
+ - [Redis-plus-plus](https://github.com/sewenew/redis-plus-plus) 1.3.5
 
 ## Publications
 
 The following are public presentations or publications using SmartRedis
 
  - [Collaboration with NCAR - CGD Seminar](https://www.youtube.com/watch?v=2e-5j427AS0)
- - [Using Machine Learning in HPC Simulations - paper (pre-print)](https://arxiv.org/abs/2104.09355)
+ - [Using Machine Learning in HPC Simulations - paper](https://www.sciencedirect.com/science/article/pii/S1877750322001065)
+ - [Relexi — A scalable open source reinforcement learning framework for high-performance computing - paper](https://www.sciencedirect.com/science/article/pii/S2665963822001063)
 
 ## Cite
 
-Please use the following citation when referencing SmartSim, SmartRedis, or any SmartSim related work.
+Please use the following citation when referencing SmartSim, SmartRedis, or any SmartSim related work:
 
-
-Partee et al., “Using Machine Learning at Scale in HPC Simulations with SmartSim:
-An Application to Ocean Climate Modeling,” arXiv:2104.09355, Apr. 2021,
-[Online]. Available: http://arxiv.org/abs/2104.09355.
+    Partee et al., "Using Machine Learning at scale in numerical simulations with SmartSim:
+    An application to ocean climate modeling",
+    Journal of Computational Science, Volume 62, 2022, 101707, ISSN 1877-7503.
+    Open Access: https://doi.org/10.1016/j.jocs.2022.101707.
 
 ### bibtex
 
-    ```latex
-    @misc{partee2021using,
-          title={Using Machine Learning at Scale in HPC Simulations with SmartSim: An Application to Ocean Climate Modeling},
-          author={Sam Partee and Matthew Ellis and Alessandro Rigazzi and Scott Bachman and Gustavo Marques and Andrew Shao and Benjamin Robbins},
-          year={2021},
-          eprint={2104.09355},
-          archivePrefix={arXiv},
-          primaryClass={cs.CE}
-    }
-    ```
+    @article{PARTEE2022101707,
+        title = {Using Machine Learning at scale in numerical simulations with SmartSim:
+        An application to ocean climate modeling},
+        journal = {Journal of Computational Science},
+        volume = {62},
+        pages = {101707},
+        year = {2022},
+        issn = {1877-7503},
+        doi = {https://doi.org/10.1016/j.jocs.2022.101707},
+        url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
+        author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E. Shao
+        and Scott Bachman and Gustavo Marques and Benjamin Robbins},
+        keywords = {Deep learning, Numerical simulation, Climate modeling, High performance computing, SmartSim},
+        }
```

#### html2text {}

```diff
@@ -14,36 +14,45 @@
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![codecov](https://codecov.io/gh/CrayLabs/SmartRedis/
 branch/develop/graph/badge.svg?token=XSS8CCJ2KR)](https://codecov.io/gh/
 CrayLabs/SmartRedis) ---------- # SmartRedis SmartRedis is a collection of
 Redis clients that support RedisAI capabilities and include additional features
 for high performance computing (HPC) applications. SmartRedis provides clients
 in the following languages: | Language | Version/Standard | |------------|:----
--------------:| | Python | 3.7, 3.8, 3.9 | | C++ | C++17 | | C | C99 | |
-Fortran | Fortran 2018 | SmartRedis is used in the [SmartSim library](https://
-github.com/CrayLabs/SmartSim). SmartSim makes it easier to use common Machine
-Learning (ML) libraries like PyTorch and TensorFlow in numerical simulations at
-scale. SmartRedis connects these simulations to a Redis database or Redis
-database cluster for data storage, script execution, and model evaluation.
-While SmartRedis contains features for simulation workflows on supercomputers,
+------------------------------------------:| | Python | 3.7, 3.8, 3.9, 3.10 | |
+C++ | C++17 | | C | C99 | | Fortran | Fortran 2018 (GNU/Intel), 2003 (PGI/
+Nvidia) | SmartRedis is used in the [SmartSim library](https://github.com/
+CrayLabs/SmartSim). SmartSim makes it easier to use common Machine Learning
+(ML) libraries like PyTorch and TensorFlow in numerical simulations at scale.
+SmartRedis connects these simulations to a Redis database or Redis database
+cluster for data storage, script execution, and model evaluation. While
+SmartRedis contains features for simulation workflows on supercomputers,
 SmartRedis is fully functional as a RedisAI client library and can be used
 without SmartSim in any Python, C++, C, or Fortran project. ## Using SmartRedis
 SmartRedis installation instructions are currently hosted as part of the
 [SmartSim library installation instructions](https://www.craylabs.org/docs/
 installation.html#smartredis) Additionally, detailed [API documents](https://
 www.craylabs.org/docs/api/smartredis_api.html) are also available as part of
 the SmartSim documentation. ## Dependencies SmartRedis utilizes the following
-libraries. - [NumPy](https://github.com/numpy/numpy) - [Hiredis](https://
-github.com/redis/hiredis) 1.0.0 - [Redis-plus-plus](https://github.com/sewenew/
-redis-plus-plus) 1.2.3 ## Publications The following are public presentations
+libraries: - [NumPy](https://github.com/numpy/numpy) - [Hiredis](https://
+github.com/redis/hiredis) 1.1.0 - [Redis-plus-plus](https://github.com/sewenew/
+redis-plus-plus) 1.3.5 ## Publications The following are public presentations
 or publications using SmartRedis - [Collaboration with NCAR - CGD Seminar]
 (https://www.youtube.com/watch?v=2e-5j427AS0) - [Using Machine Learning in HPC
-Simulations - paper (pre-print)](https://arxiv.org/abs/2104.09355) ## Cite
-Please use the following citation when referencing SmartSim, SmartRedis, or any
-SmartSim related work. Partee et al., âUsing Machine Learning at Scale in HPC
-Simulations with SmartSim: An Application to Ocean Climate Modeling,â arXiv:
-2104.09355, Apr. 2021, [Online]. Available: http://arxiv.org/abs/2104.09355.
-### bibtex ```latex @misc{partee2021using, title={Using Machine Learning at
-Scale in HPC Simulations with SmartSim: An Application to Ocean Climate
-Modeling}, author={Sam Partee and Matthew Ellis and Alessandro Rigazzi and
-Scott Bachman and Gustavo Marques and Andrew Shao and Benjamin Robbins}, year=
-{2021}, eprint={2104.09355}, archivePrefix={arXiv}, primaryClass={cs.CE} } ```
+Simulations - paper](https://www.sciencedirect.com/science/article/pii/
+S1877750322001065) - [Relexi â A scalable open source reinforcement learning
+framework for high-performance computing - paper](https://
+www.sciencedirect.com/science/article/pii/S2665963822001063) ## Cite Please use
+the following citation when referencing SmartSim, SmartRedis, or any SmartSim
+related work: Partee et al., "Using Machine Learning at scale in numerical
+simulations with SmartSim: An application to ocean climate modeling", Journal
+of Computational Science, Volume 62, 2022, 101707, ISSN 1877-7503. Open Access:
+https://doi.org/10.1016/j.jocs.2022.101707. ### bibtex @article
+{PARTEE2022101707, title = {Using Machine Learning at scale in numerical
+simulations with SmartSim: An application to ocean climate modeling}, journal =
+{Journal of Computational Science}, volume = {62}, pages = {101707}, year =
+{2022}, issn = {1877-7503}, doi = {https://doi.org/10.1016/j.jocs.2022.101707},
+url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
+author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E.
+Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins}, keywords =
+{Deep learning, Numerical simulation, Climate modeling, High performance
+computing, SmartSim}, }
```

### Comparing `smartredis-0.4.0/build-scripts/build-keydb.sh` & `smartredis-0.4.1/build-scripts/build-keydb.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build-redis.sh` & `smartredis-0.4.1/build-scripts/build-redis.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build-redisai-cpu.sh` & `smartredis-0.4.1/build-scripts/build-redisai-cpu.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build-redisai-gpu.sh` & `smartredis-0.4.1/build-scripts/build-redisai-gpu.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build_c_tests.sh` & `smartredis-0.4.1/build-scripts/build_c_tests.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build_cpp_tests.sh` & `smartredis-0.4.1/build-scripts/build_cpp_tests.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build_cpp_unit_tests.sh` & `smartredis-0.4.1/build-scripts/build_cpp_unit_tests.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build_deps.sh` & `smartredis-0.4.1/build-scripts/build_deps.sh`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 #Install Redis-plus-plus
 if ls ../install/lib/libredis++.a 1>/dev/null 2>&1; then
     echo "Redis-plus-plus has already been installed"
 else
     if [[ ! -d "./redis-plus-plus" ]]; then
-        git clone https://github.com/sewenew/redis-plus-plus.git redis-plus-plus --branch 1.3.5 --depth=1
+        git clone https://github.com/sewenew/redis-plus-plus.git redis-plus-plus --branch 1.3.8 --depth=1
 	    echo "Redis-plus-plus downloaded"
     fi
     cd redis-plus-plus
     #ex -s -c '2i|SET_PROPERTY(GLOBAL PROPERTY TARGET_SUPPORTS_SHARED_LIBS TRUE)' -c x CMakeLists.txt
     mkdir compile
     cd compile
```

### Comparing `smartredis-0.4.0/build-scripts/build_fortran_tests.sh` & `smartredis-0.4.1/build-scripts/build_fortran_tests.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build_lib.sh` & `smartredis-0.4.1/build-scripts/build_lib.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build_parallel_examples.sh` & `smartredis-0.4.1/build-scripts/build_parallel_examples.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build_serial_examples.sh` & `smartredis-0.4.1/build-scripts/build_serial_examples.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/build-scripts/build_test_deps.sh` & `smartredis-0.4.1/build-scripts/build_test_deps.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/address.h` & `smartredis-0.4.1/include/address.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/addressallcommand.h` & `smartredis-0.4.1/include/addressallcommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/addressanycommand.h` & `smartredis-0.4.1/include/addressanycommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/addressatcommand.h` & `smartredis-0.4.1/include/addressatcommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/c_client.h` & `smartredis-0.4.1/include/c_client.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/c_dataset.h` & `smartredis-0.4.1/include/c_dataset.h`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 /*!
 *   \brief C-DataSet destructor
 *   \param dataset A pointer to the dataset to release. The dataset is
 *                  set to NULL on completion
 *   \return Returns SRNoError on success or an error code on failure
 */
-SRError DeallocateeDataSet(void** dataset);
+SRError DeallocateDataSet(void** dataset);
 
 /*!
 *   \brief Add a tensor to the DataSet.
 *   \param dataset The dataset to use for this operation
 *   \param name The name by which this tensor should be referenced
 *               in the DataSet
 *   \param name_length The length of the dataset name string,
```

### Comparing `smartredis-0.4.0/include/c_logcontext.h` & `smartredis-0.4.1/include/c_logcontext.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/c_logger.h` & `smartredis-0.4.1/include/c_logger.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/client.h` & `smartredis-0.4.1/include/client.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/clusterinfocommand.h` & `smartredis-0.4.1/include/clusterinfocommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/command.h` & `smartredis-0.4.1/include/command.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/command.tcc` & `smartredis-0.4.1/include/command.tcc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/commandlist.h` & `smartredis-0.4.1/include/commandlist.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/commandlist.tcc` & `smartredis-0.4.1/include/commandlist.tcc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/commandreply.h` & `smartredis-0.4.1/include/commandreply.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/compoundcommand.h` & `smartredis-0.4.1/include/compoundcommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/dataset.h` & `smartredis-0.4.1/include/dataset.h`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 #include "sharedmemorylist.h"
 #include "sr_enums.h"
 
 ///@file
 
 namespace SmartRedis {
 
-///@file
 /*!
 *   \brief The DataSet class aggregates tensors
 *          and metadata into a nested data structure
 *          for storage.
 *   \details Tensors in the DataSet can be used in
 *            Client commands such as Client.run_model()
 *            and Client.run_script() as inputs or outputs
```

### Comparing `smartredis-0.4.0/include/dbinfocommand.h` & `smartredis-0.4.1/include/dbinfocommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/dbnode.h` & `smartredis-0.4.1/include/dbnode.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/enum_fortran.inc` & `smartredis-0.4.1/include/enum_fortran.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/gettensorcommand.h` & `smartredis-0.4.1/include/gettensorcommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/keyedcommand.h` & `smartredis-0.4.1/include/keyedcommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/logcontext.h` & `smartredis-0.4.1/include/logcontext.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/logger.h` & `smartredis-0.4.1/include/logger.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/metadata.h` & `smartredis-0.4.1/include/metadata.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/metadatabuffer.h` & `smartredis-0.4.1/include/metadatabuffer.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/metadatafield.h` & `smartredis-0.4.1/include/metadatafield.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/multikeycommand.h` & `smartredis-0.4.1/include/multikeycommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/nonkeyedcommand.h` & `smartredis-0.4.1/include/nonkeyedcommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/pipelinereply.h` & `smartredis-0.4.1/include/pipelinereply.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/pyclient.h` & `smartredis-0.4.1/include/pyclient.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/pydataset.h` & `smartredis-0.4.1/include/pydataset.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/pylogcontext.h` & `smartredis-0.4.1/include/pylogcontext.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/pysrobject.h` & `smartredis-0.4.1/include/pysrobject.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/redis.h` & `smartredis-0.4.1/include/redis.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/rediscluster.h` & `smartredis-0.4.1/include/rediscluster.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/redisserver.h` & `smartredis-0.4.1/include/redisserver.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 #ifndef SMARTREDIS_REDISSERVER_H
 #define SMARTREDIS_REDISSERVER_H
 
 #include <thread>
 #include <iostream>
 #include <random>
 #include <limits.h>
-#include <sw/redis++/redis++.h>
 
 #include "command.h"
 #include "commandreply.h"
 #include "commandlist.h"
 #include "tensorbase.h"
 #include "dbnode.h"
 #include "nonkeyedcommand.h"
```

### Comparing `smartredis-0.4.0/include/scalarfield.h` & `smartredis-0.4.1/include/scalarfield.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/scalarfield.tcc` & `smartredis-0.4.1/include/scalarfield.tcc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/sharedmemorylist.h` & `smartredis-0.4.1/include/sharedmemorylist.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/sharedmemorylist.tcc` & `smartredis-0.4.1/include/sharedmemorylist.tcc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/singlekeycommand.h` & `smartredis-0.4.1/include/singlekeycommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/sr_enums.h` & `smartredis-0.4.1/include/sr_enums.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/srassert.h` & `smartredis-0.4.1/include/srassert.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/srexception.h` & `smartredis-0.4.1/include/srexception.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/srobject.h` & `smartredis-0.4.1/include/srobject.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/stringfield.h` & `smartredis-0.4.1/include/stringfield.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/tensor.h` & `smartredis-0.4.1/include/tensor.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/tensor.tcc` & `smartredis-0.4.1/include/tensor.tcc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/tensorbase.h` & `smartredis-0.4.1/include/tensorbase.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/tensorpack.h` & `smartredis-0.4.1/include/tensorpack.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/include/threadpool.h` & `smartredis-0.4.1/include/threadpool.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/setup.cfg` & `smartredis-0.4.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smartredis
-version = 0.4.0
+version = 0.4.1
 description = RedisAI clients for SmartSim
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrayLabs/SmartRedis
 project_urls = 
 	Source = https://github.com/CrayLabs/SmartRedis
 	Documentation = https://www.craylabs.org
@@ -14,37 +14,39 @@
 contact_email = craylabs@hpe.com
 license = BSD 2-Clause License
 keywords = redis, clients, hpc, ai, deep learning
 classifiers = 
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: BSD License
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 
 [options]
 package_dir = 
 	=src/python/module
 packages = find:
 setup_requires = 
-	setuptools>=39.2
+	setuptools>=42
 include_package_data = True
 install_requires = 
 	numpy>=1.18.2
 python_requires = >=3.7,<3.11
 
 [options.extras_require]
 dev = 
 	pytest>=6.0.0
 	pytest-cov==2.10.1
 	black==20.8b1
 	isort==5.6.4
 	pylint==2.6.0
-	torch==1.7.1
+	torch>=1.7.1
+	mypy>=1.4.0
 doc = 
 	sphinx==3.1.1
 	sphinx-fortran==1.1.1
 	sphinx_rtd_theme>=0.5.0
 	breathe==4.25.1
 xarray = 
 	xarray>=0.14.1
```

### Comparing `smartredis-0.4.0/setup.py` & `smartredis-0.4.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 import subprocess
 import shutil
 from pathlib import Path
 import multiprocessing as mp
 
 from setuptools import setup, Extension, find_packages
 from setuptools.command.build_ext import build_ext
-from distutils.version import LooseVersion
 
 # get number of processors
 NPROC = mp.cpu_count()
 
 class CMakeExtension(Extension):
     def __init__(self, name):
         Extension.__init__(self, name, sources=[])
@@ -46,97 +45,100 @@
 
     @property
     def cmake(self):
         """Find and use installed cmake"""
         cmake_cmd = shutil.which("cmake")
         return cmake_cmd
 
+    @property
+    def make(self):
+        """Find and use installed cmake"""
+        make_cmd = shutil.which("make")
+        return make_cmd
+
     def run(self):
+        # Validate dependencies
+        check_prereq("cmake")
         check_prereq("make")
         check_prereq("gcc")
         check_prereq("g++")
 
+        # Set up parameters
+        source_directory = Path(__file__).parent.resolve()
         build_directory = Path(self.build_temp).resolve()
-        cmake_args = [
-            '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=' + str(build_directory),
-            '-DPYTHON_EXECUTABLE=' + sys.executable
-        ]
-
         cfg = 'Debug' if self.debug else 'Release'
-        build_args = ['--config', cfg]
-        build_args += ['--', f'-j{str(NPROC)}']
-        self.build_args = build_args
 
-        cmake_args += ['-DCMAKE_BUILD_TYPE=' + cfg]
-
-        # setup build environment
+        # Setup build environment
         env = os.environ.copy()
         env['CXXFLAGS'] = '{} -DVERSION_INFO=\\"{}\\"'.format(
             env.get('CXXFLAGS', ''),
             self.distribution.get_version())
 
-        # make tmp dir
-        if not build_directory.is_dir():
-            os.makedirs(self.build_temp)
-
-        print('-'*10, 'Building C dependencies', '-'*40)
-        make_cmd = shutil.which("make")
-        setup_path = Path(os.path.abspath(os.path.dirname(__file__))).resolve()
-
-        # build dependencies
-        subprocess.check_call([f"{make_cmd} deps"],
-                              cwd=setup_path,
-                              shell=True)
-
-        # run cmake prep step
-        print('-'*10, 'Running CMake prepare', '-'*40)
-        subprocess.check_call([self.cmake, setup_path] + cmake_args,
-                              cwd=build_directory,
-                              env=env)
-
-
-        print('-'*10, 'Building extensions', '-'*40)
-        cmake_cmd = [self.cmake, '--build', '.'] + self.build_args
-        subprocess.check_call(cmake_cmd,
-                              cwd=build_directory)
-
-        shutil.copytree(setup_path.joinpath("install"),
-                        build_directory.joinpath("install"))
+        # Build dependencies
+        print('-'*10, 'Building third-party dependencies', '-'*40)
+        subprocess.check_call(
+            [self.make, "deps"],
+            cwd=source_directory,
+            shell=False
+        )
+
+        # Run CMake config step
+        print('-'*10, 'Configuring build', '-'*40)
+        config_args = [
+            '-S.',
+            f'-B{str(build_directory)}',
+            '-DSR_BUILD=' + cfg,
+            '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=' + str(build_directory),
+            '-DPYTHON_EXECUTABLE=' + sys.executable,
+            '-DSR_PYTHON=ON',
+        ]
+        subprocess.check_call(
+            [self.cmake] + config_args,
+            cwd=source_directory,
+            env=env
+        )
+
+        # Run CMake build step
+        print('-'*10, 'Building library', '-'*40)
+        build_args = [
+            '--build',
+            str(build_directory),
+            '--',
+            f'-j{str(NPROC)}'
+        ]
+        subprocess.check_call(
+            [self.cmake] + build_args,
+            cwd=build_directory,
+            env=env
+        )
 
         # Move from build temp to final position
+        # (Note that we skip the CMake install step because
+        # we configured the library to be built directly into the
+        # build directory)
         for ext in self.extensions:
             self.move_output(ext)
 
     def move_output(self, ext):
         build_temp = Path(self.build_temp).resolve()
         dest = Path(self.get_ext_fullpath(ext.name)).parent.absolute()
         dest_path = dest.joinpath("smartredis")
         source_path = build_temp / self.get_ext_filename(ext.name)
         dest_directory = dest_path.parents[0]
         dest_directory.mkdir(parents=True, exist_ok=True)
         self.copy_file(source_path, dest_path)
 
 # check that certain dependencies are installed
-# TODO: Check versions for compatible versions
 def check_prereq(command):
     try:
-        out = subprocess.check_output([command, '--version'])
+        _ = subprocess.check_output([command, '--version'])
     except OSError:
         raise RuntimeError(
             f"{command} must be installed to build SmartRedis")
 
-# update existing env var
-def update_env_var(var, new):
-    try:
-        value = os.environ[var]
-        value = ":".join((value, str(new)))
-        return value
-    except KeyError:
-        return new
-
 ext_modules = [
     CMakeExtension('smartredisPy'),
 ]
 
 setup(
  # ... in setup.cfg
     packages=find_packages(),
```

### Comparing `smartredis-0.4.0/src/c/c_client.cpp` & `smartredis-0.4.1/src/c/c_client.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/c/c_dataset.cpp` & `smartredis-0.4.1/src/c/c_dataset.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     catch (const std::bad_alloc& e) {
       SRSetLastError(SRBadAllocException("dataset allocation"));
     }
   });
 }
 
 // Deallocate a DataSet
-extern "C" SRError DeallocateeDataSet(void** dataset)
+extern "C" SRError DeallocateDataSet(void** dataset)
 {
   return MAKE_DATASET_API({
     // Sanity check params
     SR_CHECK_PARAMS(dataset != NULL);
 
     DataSet* d = reinterpret_cast<DataSet*>(*dataset);
     delete d;
```

### Comparing `smartredis-0.4.0/src/c/c_error.cpp` & `smartredis-0.4.1/src/c/c_error.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/c/c_logcontext.cpp` & `smartredis-0.4.1/src/c/c_logcontext.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/c/c_logger.cpp` & `smartredis-0.4.1/src/c/c_logger.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/address.cpp` & `smartredis-0.4.1/src/cpp/address.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/addressallcommand.cpp` & `smartredis-0.4.1/src/cpp/addressallcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/addressanycommand.cpp` & `smartredis-0.4.1/src/cpp/addressanycommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/addressatcommand.cpp` & `smartredis-0.4.1/src/cpp/addressatcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/client.cpp` & `smartredis-0.4.1/src/cpp/client.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/clusterinfocommand.cpp` & `smartredis-0.4.1/src/cpp/clusterinfocommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/command.cpp` & `smartredis-0.4.1/src/cpp/command.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/commandlist.cpp` & `smartredis-0.4.1/src/cpp/commandlist.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/commandreply.cpp` & `smartredis-0.4.1/src/cpp/commandreply.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/compoundcommand.cpp` & `smartredis-0.4.1/src/cpp/compoundcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/dataset.cpp` & `smartredis-0.4.1/src/cpp/dataset.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/dbinfocommand.cpp` & `smartredis-0.4.1/src/cpp/dbinfocommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/dbnode.cpp` & `smartredis-0.4.1/src/cpp/dbnode.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/gettensorcommand.cpp` & `smartredis-0.4.1/src/cpp/gettensorcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/keyedcommand.cpp` & `smartredis-0.4.1/src/cpp/keyedcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/logger.cpp` & `smartredis-0.4.1/src/cpp/logger.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 // Set up logging for the current client
 void Logger::configure_logging()
 {
     // Mark ourselves as initialized now
     _initialized = true;
 
     // Get the logfile
-    get_config_string(_logfile, "SR_LOG_FILE", "", true);
+    get_config_string(_logfile, "SR_LOG_FILE", "", flag_suppress_warning);
     std::string requestedLogfile(_logfile);
     bool missingLogFile = _logfile.length() == 0;
 
     // Make sure it can be written to
     bool badLogFile = false;
     if (_logfile.length() > 0) {
         std::ofstream logstream;
@@ -73,15 +73,15 @@
         // Switch to STDOUT if we can't write to the specified file
         if (badLogFile)
             _logfile = "";
     }
 
     // Get the logging level
     std::string level;
-    get_config_string(level, "SR_LOG_LEVEL", "", true);
+    get_config_string(level, "SR_LOG_LEVEL", "", flag_suppress_warning);
     bool missingLogLevel = level.length() == 0;
     bool badLogLevel = false;
     if (level.length() > 0) {
         str_to_lower(level);
         if (level.compare("quiet") == 0)
             _log_level = LLQuiet;
         else if (level.compare("info") == 0)
```

### Comparing `smartredis-0.4.0/src/cpp/metadata.cpp` & `smartredis-0.4.1/src/cpp/metadata.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/metadatafield.cpp` & `smartredis-0.4.1/src/cpp/metadatafield.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/multikeycommand.cpp` & `smartredis-0.4.1/src/cpp/multikeycommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/nonkeyedcommand.cpp` & `smartredis-0.4.1/src/cpp/nonkeyedcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/pipelinereply.cpp` & `smartredis-0.4.1/src/cpp/pipelinereply.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/redis.cpp` & `smartredis-0.4.1/src/cpp/redis.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
+#include <sw/redis++/redis++.h>
 #include "redis.h"
 #include "srexception.h"
 #include "utility.h"
 #include "srobject.h"
 
 using namespace SmartRedis;
```

### Comparing `smartredis-0.4.0/src/cpp/rediscluster.cpp` & `smartredis-0.4.1/src/cpp/rediscluster.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
  * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
+#include <sw/redis++/redis++.h>
 #include "rediscluster.h"
 #include "nonkeyedcommand.h"
 #include "keyedcommand.h"
 #include "srexception.h"
 #include "utility.h"
 #include "srobject.h"
```

### Comparing `smartredis-0.4.0/src/cpp/redisserver.cpp` & `smartredis-0.4.1/src/cpp/redisserver.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #include <ctype.h>
+#include <sw/redis++/redis++.h>
 #include "redisserver.h"
 #include "srexception.h"
 #include "utility.h"
 #include "srobject.h"
 
 using namespace SmartRedis;
```

### Comparing `smartredis-0.4.0/src/cpp/singlekeycommand.cpp` & `smartredis-0.4.1/src/cpp/singlekeycommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/srobject.cpp` & `smartredis-0.4.1/src/cpp/srobject.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/stringfield.cpp` & `smartredis-0.4.1/src/cpp/stringfield.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/tensorbase.cpp` & `smartredis-0.4.1/src/cpp/tensorbase.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/tensorpack.cpp` & `smartredis-0.4.1/src/cpp/tensorpack.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/threadpool.cpp` & `smartredis-0.4.1/src/cpp/threadpool.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/cpp/utility.cpp` & `smartredis-0.4.1/src/cpp/utility.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -23,63 +23,66 @@
  * SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  * CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #include <cstdlib>
+#include <cctype>
+#include <algorithm>
 #include <string>
 #include <cstring>
 #include <stdio.h>
 #include <stdexcept>
 #include "srexception.h"
 #include "utility.h"
 #include "logger.h"
 
 namespace SmartRedis {
 
-/*!
-*   \brief Initialize an integer from configuration, such as an
-*          environment variable
-*   \param value Receives the configuration value
-*   \param cfg_key The key to query for the configuration variable
-*   \param default_value Default if configuration key is not set
-*   \param suppress_warning Do not issue a warning if the variable
-*                           is not set
-*/
+// Initialize an integer from an environment variable
 void get_config_integer(int& value,
                         const std::string& cfg_key,
                         const int default_value,
-                        bool suppress_warning /*= false*/)
+                        int flags /* = 0 */)
 {
-    value = default_value;
+    bool suppress_warning = 0 != (flags & flag_suppress_warning);
+    bool keyerror_on_absent = 0 != (flags & throw_on_absent);
+
+    int result = default_value;
     std::string message = "Getting value for " + cfg_key;
     log_data("SmartRedis Library", LLDebug, message);
 
     char* cfg_val = std::getenv(cfg_key.c_str());
     message = "Retrieved value \"";
     message += cfg_val == NULL ? "<NULL>" : cfg_val;
     message += "\"";
-    if (NULL == cfg_val)
+    if ((NULL == cfg_val) && !keyerror_on_absent)
         message += ". Using default value of " + std::to_string(default_value);
     log_data("SmartRedis Library", LLDebug, message);
 
+    if ((cfg_val == NULL) && keyerror_on_absent) {
+        std::string msg("No value found for key ");
+        msg += cfg_key;
+        throw SRKeyException(msg);
+    }
+
     if (cfg_val != NULL && std::strlen(cfg_val) > 0) {
         // Enforce that all characters are digits because std::stoi
         // will truncate a string like "10xy" to 10.
         // We want to guard users from input errors they might have.
         for (char* c = cfg_val; *c != '\0'; c++) {
             if (!isdigit(*c) && !(*c == '-' && c == cfg_val)) {
                 throw SRParameterException("The value of " + cfg_key +
                                            " must be a valid number.");
             }
         }
 
         try {
-            value = std::stoi(cfg_val);
+            result = std::stoi(cfg_val);
         }
         catch (std::invalid_argument& e) {
             throw SRParameterException("The value of " + cfg_key + " could "\
                                        "not be converted to type integer.");
         }
         catch (std::out_of_range& e) {
             throw SRParameterException("The value of " + cfg_key + " is too "\
@@ -97,54 +100,57 @@
         log_warning(
             "SmartRedis Library",
             LLDebug,
             "Configuration variable " + cfg_key + " not set"
         );
     }
 
+    value = result;
     message = "Exiting with value \"" + std::to_string(value) + "\"";
     log_data("SmartRedis Library", LLDebug, message);
 }
 
-/*!
-*   \brief Initialize an string from configuration, such as an
-*          environment variable
-*   \param value Receives the configuration value
-*   \param cfg_key The key to query for the configuration variable
-*   \param default_value Default if configuration key is not set
-*   \param suppress_warning Do not issue a warning if the variable
-*                           is not set
-*/
+// Initialize a string from an environment variable
 void get_config_string(std::string& value,
                        const std::string& cfg_key,
                        const std::string& default_value,
-                       bool suppress_warning /*= false*/)
+                       int flags /* = 0 */)
 {
-    value = default_value;
+    bool suppress_warning = 0 != (flags & flag_suppress_warning);
+    bool keyerror_on_absent = 0 != (flags & throw_on_absent);
+
+    std::string result = default_value;
     std::string message = "Getting value for " + cfg_key;
     log_data("SmartRedis Library", LLDebug, message);
 
     char* cfg_val = std::getenv(cfg_key.c_str());
     message = "Retrieved value \"";
     message += cfg_val == NULL ? "<NULL>" : cfg_val;
     message += "\"";
-    if (NULL == cfg_val)
-        message += ". Using default value of \"" + default_value + "\"";
+    if ((NULL == cfg_val) && !keyerror_on_absent)
+        message += ". Using default value of " + default_value;
     log_data("SmartRedis Library", LLDebug, message);
 
+    if ((cfg_val == NULL) && keyerror_on_absent) {
+        std::string msg("No value found for key ");
+        msg += cfg_key;
+        throw SRKeyException(msg);
+    }
+
     if (cfg_val != NULL && std::strlen(cfg_val) > 0)
-        value = cfg_val;
+        result = cfg_val;
     else if (!suppress_warning) {
         log_warning(
             "SmartRedis Library",
             LLDebug,
             "Configuration variable " + cfg_key + " not set"
         );
     }
 
+    value = result;
     message = "Exiting with value \"" + value + "\"";
     log_data("SmartRedis Library", LLDebug, message);
 }
 
 // Create a string representation of a tensor type
 std::string to_string(SRTensorType ttype)
 {
```

### Comparing `smartredis-0.4.0/src/fortran/client/aggregation_interfaces.inc` & `smartredis-0.4.1/src/fortran/client/aggregation_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client/client_dataset_interfaces.inc` & `smartredis-0.4.1/src/fortran/client/client_dataset_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client/client_interfaces.inc` & `smartredis-0.4.1/src/fortran/client/client_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client/ensemble_interfaces.inc` & `smartredis-0.4.1/src/fortran/client/ensemble_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client/misc_tensor_interfaces.inc` & `smartredis-0.4.1/src/fortran/client/misc_tensor_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client/model_interfaces.inc` & `smartredis-0.4.1/src/fortran/client/model_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client/put_tensor_interfaces.inc` & `smartredis-0.4.1/src/fortran/client/put_tensor_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client/put_tensor_methods_common.inc` & `smartredis-0.4.1/src/fortran/client/put_tensor_methods_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client/script_interfaces.inc` & `smartredis-0.4.1/src/fortran/client/script_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client/unpack_tensor_interfaces.inc` & `smartredis-0.4.1/src/fortran/client/unpack_tensor_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client/unpack_tensor_methods_common.inc` & `smartredis-0.4.1/src/fortran/client/unpack_tensor_methods_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/client.F90` & `smartredis-0.4.1/src/fortran/client.F90`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,23 @@
 ! FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 ! DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 ! SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 ! CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 ! OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+! Note the below macros are here to allow compilation with Nvidia drivers
+! While assumed size should be sufficient, this does not seem to work with
+! Intel and GNU (however those have support for assumed rank)
+#ifdef __NVCOMPILER
+#define DIM_RANK_SPEC dimension(*)
+#else
+#define DIM_RANK_SPEC dimension(..)
+#endif
+
 module smartredis_client
 
 use iso_c_binding, only : c_ptr, c_bool, c_null_ptr, c_char, c_int
 use iso_c_binding, only : c_int8_t, c_int16_t, c_int32_t, c_int64_t, c_float, c_double, c_size_t
 use iso_c_binding, only : c_loc, c_f_pointer
 
 use, intrinsic :: iso_fortran_env, only: stderr => error_unit
@@ -287,168 +296,184 @@
   get_c_pointer = self%client_ptr
 end function get_c_pointer
 
 !> Check if the specified key exists in the database
 function key_exists(self, key, exists)
   class(client_type),   intent(in)  :: self   !< The client
   character(len=*),     intent(in)  :: key    !< The key to check
-  logical(kind=c_bool), intent(out) :: exists !< Receives whether the key exists
+  logical,              intent(out) :: exists !< Receives whether the key exists
   integer(kind=enum_kind)           :: key_exists
 
   ! Local variables
   character(kind=c_char, len=len_trim(key)) :: c_key
   integer(kind=c_size_t) :: c_key_length
+  logical(kind=c_bool) :: c_exists
 
   c_key = trim(key)
   c_key_length = len_trim(key)
 
-  key_exists = key_exists_c(self%client_ptr, c_key, c_key_length, exists)
+  key_exists = key_exists_c(self%client_ptr, c_key, c_key_length, c_exists)
+  exists = c_exists
 end function key_exists
 
 !> Check if the specified model exists in the database
 function model_exists(self, model_name, exists) result(code)
   class(client_type),   intent(in)  :: self       !< The client
   character(len=*),     intent(in)  :: model_name !< The model to check
-  logical(kind=c_bool), intent(out) :: exists     !< Receives whether the model exists
+  logical,              intent(out) :: exists     !< Receives whether the model exists
   integer(kind=enum_kind)           :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(model_name)) :: c_model_name
   integer(kind=c_size_t) :: c_model_name_length
+  logical(kind=c_bool) :: c_exists
 
   c_model_name = trim(model_name)
   c_model_name_length = len_trim(model_name)
 
-  code = model_exists_c(self%client_ptr, c_model_name, c_model_name_length, exists)
+  code = model_exists_c(self%client_ptr, c_model_name, c_model_name_length, c_exists)
+  exists = c_exists
 end function model_exists
 
 !> Check if the specified tensor exists in the database
 function tensor_exists(self, tensor_name, exists) result(code)
   class(client_type),   intent(in)  :: self        !< The client
   character(len=*),     intent(in)  :: tensor_name !< The tensor to check
-  logical(kind=c_bool), intent(out) :: exists      !< Receives whether the model exists
+  logical,              intent(out) :: exists      !< Receives whether the model exists
   integer(kind=enum_kind)           :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(tensor_name)) :: c_tensor_name
   integer(kind=c_size_t) :: c_tensor_name_length
+  logical(kind=c_bool) :: c_exists
 
   c_tensor_name = trim(tensor_name)
   c_tensor_name_length = len_trim(tensor_name)
 
-  code = tensor_exists_c(self%client_ptr, c_tensor_name, c_tensor_name_length, exists)
+  code = tensor_exists_c(self%client_ptr, c_tensor_name, c_tensor_name_length, c_exists)
+  exists = c_exists
 end function tensor_exists
 
 !> Check if the specified dataset exists in the database
 function dataset_exists(this, dataset_name, exists) result(code)
   class(client_type),   intent(in)  :: this          !< The client
   character(len=*),     intent(in)  :: dataset_name  !< The dataset to check
-  logical(kind=c_bool), intent(out) :: exists        !< Receives whether the model exists
+  logical,              intent(out) :: exists        !< Receives whether the model exists
   integer(kind=enum_kind)           :: code
 
   character(kind=c_char, len=len_trim(dataset_name)) :: c_dataset_name
   integer(kind=c_size_t) :: c_dataset_name_length
+  logical(kind=c_bool) :: c_exists
 
   c_dataset_name = trim(dataset_name)
   c_dataset_name_length = len_trim(dataset_name)
 
-  code = dataset_exists_c(this%client_ptr, c_dataset_name, c_dataset_name_length, exists)
+  code = dataset_exists_c(this%client_ptr, c_dataset_name, c_dataset_name_length, c_exists)
+  exists = c_exists
 end function dataset_exists
 
 !> Repeatedly poll the database until the tensor exists or the number of tries is exceeded
 function poll_tensor(self, tensor_name, poll_frequency_ms, num_tries, exists) result(code)
   class(client_type),   intent(in)  :: self              !< The client
   character(len=*),     intent(in)  :: tensor_name       !< name in the database to poll
   integer,              intent(in)  :: poll_frequency_ms !< Frequency at which to poll the database (ms)
   integer,              intent(in)  :: num_tries         !< Number of times to poll the database before failing
-  logical(kind=c_bool), intent(out) :: exists            !< Receives whether the tensor exists
+  logical,              intent(out) :: exists            !< Receives whether the tensor exists
   integer(kind=enum_kind)           :: code
 
   ! Local variables
   character(kind=c_char,len=len_trim(tensor_name)) :: c_tensor_name
   integer(kind=c_size_t) :: c_tensor_name_length
   integer(kind=c_int) :: c_poll_frequency, c_num_tries
+  logical(kind=c_bool) :: c_exists
 
   c_tensor_name = trim(tensor_name)
   c_tensor_name_length = len_trim(tensor_name)
   c_num_tries = num_tries
   c_poll_frequency = poll_frequency_ms
 
-  code = poll_tensor_c(self%client_ptr, c_tensor_name, c_tensor_name_length, c_poll_frequency, c_num_tries, exists)
+  code = poll_tensor_c(self%client_ptr, c_tensor_name, c_tensor_name_length, c_poll_frequency, c_num_tries, c_exists)
+  exists = c_exists
 end function poll_tensor
 
 !> Repeatedly poll the database until the dataset exists or the number of tries is exceeded
 function poll_dataset(self, dataset_name, poll_frequency_ms, num_tries, exists)
   integer(kind=enum_kind)           :: poll_dataset
   class(client_type),   intent(in)  :: self              !< The client
   character(len=*),     intent(in)  :: dataset_name      !< Name in the database to poll
   integer,              intent(in)  :: poll_frequency_ms !< Frequency at which to poll the database (ms)
   integer,              intent(in)  :: num_tries         !< Number of times to poll the database before failing
-  logical(kind=c_bool), intent(out) :: exists            !< Receives whether the tensor exists
+  logical,              intent(out) :: exists            !< Receives whether the tensor exists
 
   ! Local variables
   character(kind=c_char,len=len_trim(dataset_name)) :: c_dataset_name
   integer(kind=c_size_t) :: c_dataset_name_length
   integer(kind=c_int) :: c_poll_frequency, c_num_tries
+  logical(kind=c_bool) :: c_exists
 
   c_dataset_name = trim(dataset_name)
   c_dataset_name_length = len_trim(dataset_name)
   c_num_tries = num_tries
   c_poll_frequency = poll_frequency_ms
 
-  poll_dataset = poll_dataset_c(self%client_ptr, c_dataset_name, c_dataset_name_length, c_poll_frequency, c_num_tries, exists)
+  poll_dataset = poll_dataset_c(self%client_ptr, c_dataset_name, c_dataset_name_length, c_poll_frequency, c_num_tries, c_exists)
+  exists = c_exists
 end function poll_dataset
 
 !> Repeatedly poll the database until the model exists or the number of tries is exceeded
 function poll_model(self, model_name, poll_frequency_ms, num_tries, exists) result(code)
   class(client_type),   intent(in)  :: self              !< The client
   character(len=*),     intent(in)  :: model_name        !< Name in the database to poll
   integer,              intent(in)  :: poll_frequency_ms !< Frequency at which to poll the database (ms)
   integer,              intent(in)  :: num_tries         !< Number of times to poll the database before failing
-  logical(kind=c_bool), intent(out) :: exists            !< Receives whether the model exists
+  logical,              intent(out) :: exists            !< Receives whether the model exists
   integer(kind=enum_kind)           :: code
 
   ! Local variables
   character(kind=c_char,len=len_trim(model_name)) :: c_model_name
   integer(kind=c_size_t) :: c_model_name_length
   integer(kind=c_int) :: c_poll_frequency, c_num_tries
+  logical(kind=c_bool) :: c_exists
 
   c_model_name = trim(model_name)
   c_model_name_length = len_trim(model_name)
   c_num_tries = num_tries
   c_poll_frequency = poll_frequency_ms
 
-  code = poll_model_c(self%client_ptr, c_model_name, c_model_name_length, c_poll_frequency, c_num_tries, exists)
+  code = poll_model_c(self%client_ptr, c_model_name, c_model_name_length, c_poll_frequency, c_num_tries, c_exists)
+  exists = c_exists
 end function poll_model
 
 !> Repeatedly poll the database until the key exists or the number of tries is exceeded
 function poll_key(self, key, poll_frequency_ms, num_tries, exists) result(code)
   class(client_type),   intent(in)  :: self               !< The client
   character(len=*),     intent(in)  :: key                !< Key in the database to poll
   integer,              intent(in)  :: poll_frequency_ms  !< Frequency at which to poll the database (ms)
   integer,              intent(in)  :: num_tries          !< Number of times to poll the database before failing
-  logical(kind=c_bool), intent(out) :: exists             !< Receives whether the key exists
+  logical,              intent(out) :: exists             !< Receives whether the key exists
   integer(kind=enum_kind)           :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(key)) :: c_key
   integer(kind=c_size_t) :: c_key_length
   integer(kind=c_int) :: c_poll_frequency, c_num_tries
+  logical(kind=c_bool) :: c_exists
 
   c_key = trim(key)
   c_key_length = len_trim(key)
   c_num_tries = num_tries
   c_poll_frequency = poll_frequency_ms
 
-  code = poll_key_c(self%client_ptr, c_key, c_key_length, c_poll_frequency, c_num_tries, exists)
+  code = poll_key_c(self%client_ptr, c_key, c_key_length, c_poll_frequency, c_num_tries, c_exists)
+  exists = c_exists
 end function poll_key
 
 !> Put a tensor whose Fortran type is the equivalent 'int8' C-type
 function put_tensor_i8(self, name, data, dims) result(code)
-  integer(kind=c_int8_t), dimension(..), target, intent(in) :: data !< Data to be sent
+  integer(kind=c_int8_t), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(client_type),                    intent(in) :: self !< Fortran SmartRedis client
   character(len=*),                      intent(in) :: name !< The unique name used to store in the database
   integer, dimension(:),                 intent(in) :: dims !< The length of each dimension
   integer(kind=enum_kind)                           :: code
 
   include 'client/put_tensor_methods_common.inc'
 
@@ -456,15 +481,15 @@
   data_type = tensor_int8
   code = put_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, &
     c_n_dims, data_type, c_fortran_contiguous)
 end function put_tensor_i8
 
 !> Put a tensor whose Fortran type is the equivalent 'int16' C-type
 function put_tensor_i16(self, name, data, dims) result(code)
-  integer(kind=c_int16_t), dimension(..), target, intent(in) :: data !< Data to be sent
+  integer(kind=c_int16_t), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(client_type),                    intent(in) :: self !< Fortran SmartRedis client
   character(len=*),                      intent(in) :: name !< The unique name used to store in the database
   integer, dimension(:),                 intent(in) :: dims !< The length of each dimension
   integer(kind=enum_kind)                           :: code
 
   include 'client/put_tensor_methods_common.inc'
 
@@ -472,15 +497,15 @@
   data_type = tensor_int16
   code = put_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, c_n_dims, &
     data_type, c_fortran_contiguous)
 end function put_tensor_i16
 
 !> Put a tensor whose Fortran type is the equivalent 'int32' C-type
 function put_tensor_i32(self, name, data, dims) result(code)
-  integer(kind=c_int32_t), dimension(..), target, intent(in) :: data !< Data to be sent
+  integer(kind=c_int32_t), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(client_type),                    intent(in) :: self !< Fortran SmartRedis client
   character(len=*),                      intent(in) :: name !< The unique name used to store in the database
   integer, dimension(:),                 intent(in) :: dims !< The length of each dimension
   integer(kind=enum_kind)                           :: code
 
   include 'client/put_tensor_methods_common.inc'
 
@@ -488,15 +513,15 @@
   data_type = tensor_int32
   code = put_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, c_n_dims, &
     data_type, c_fortran_contiguous)
 end function put_tensor_i32
 
 !> Put a tensor whose Fortran type is the equivalent 'int64' C-type
 function put_tensor_i64(self, name, data, dims) result(code)
-  integer(kind=c_int64_t), dimension(..), target, intent(in) :: data !< Data to be sent
+  integer(kind=c_int64_t), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(client_type),                    intent(in) :: self !< Fortran SmartRedis client
   character(len=*),                      intent(in) :: name !< The unique name used to store in the database
   integer, dimension(:),                 intent(in) :: dims !< The length of each dimension
   integer(kind=enum_kind)                           :: code
 
   include 'client/put_tensor_methods_common.inc'
 
@@ -504,15 +529,15 @@
   data_type = tensor_int64
   code = put_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, c_n_dims, &
     data_type, c_fortran_contiguous)
 end function put_tensor_i64
 
 !> Put a tensor whose Fortran type is the equivalent 'float' C-type
 function put_tensor_float(self, name, data, dims) result(code)
-  real(kind=c_float), dimension(..), target, intent(in) :: data !< Data to be sent
+  real(kind=c_float), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(client_type),                    intent(in) :: self !< Fortran SmartRedis client
   character(len=*),                      intent(in) :: name !< The unique name used to store in the database
   integer, dimension(:),                 intent(in) :: dims !< The length of each dimension
   integer(kind=enum_kind)                           :: code
 
   include 'client/put_tensor_methods_common.inc'
 
@@ -520,15 +545,15 @@
   data_type = tensor_flt
   code = put_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, c_n_dims, &
     data_type, c_fortran_contiguous)
 end function put_tensor_float
 
 !> Put a tensor whose Fortran type is the equivalent 'double' C-type
 function put_tensor_double(self, name, data, dims) result(code)
-  real(kind=c_double), dimension(..), target, intent(in) :: data !< Data to be sent
+  real(kind=c_double), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(client_type),                    intent(in) :: self !< Fortran SmartRedis client
   character(len=*),                      intent(in) :: name !< The unique name used to store in the database
   integer, dimension(:),                 intent(in) :: dims !< The length of each dimension
   integer(kind=enum_kind)                           :: code
 
   include 'client/put_tensor_methods_common.inc'
 
@@ -536,15 +561,15 @@
   data_type = tensor_dbl
   code = put_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, c_n_dims, &
     data_type, c_fortran_contiguous)
 end function put_tensor_double
 
 !> Put a tensor whose Fortran type is the equivalent 'int8' C-type
 function unpack_tensor_i8(self, name, result, dims) result(code)
-  integer(kind=c_int8_t), dimension(..), target, intent(out) :: result !< Data to be sent
+  integer(kind=c_int8_t), DIM_RANK_SPEC, target, intent(out) :: result !< Data to be sent
   class(client_type),                   intent(in) :: self  !< Pointer to the initialized client
   character(len=*),                     intent(in) :: name  !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims  !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'client/unpack_tensor_methods_common.inc'
 
@@ -552,15 +577,15 @@
   data_type = tensor_int8
   code = unpack_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, c_n_dims, &
     data_type, mem_layout)
 end function unpack_tensor_i8
 
 !> Put a tensor whose Fortran type is the equivalent 'int16' C-type
 function unpack_tensor_i16(self, name, result, dims) result(code)
-  integer(kind=c_int16_t), dimension(..), target, intent(out) :: result !< Data to be sent
+  integer(kind=c_int16_t), DIM_RANK_SPEC, target, intent(out) :: result !< Data to be sent
   class(client_type),                   intent(in) :: self  !< Pointer to the initialized client
   character(len=*),                     intent(in) :: name  !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims  !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'client/unpack_tensor_methods_common.inc'
 
@@ -568,15 +593,15 @@
   data_type = tensor_int16
   code = unpack_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, c_n_dims, &
     data_type, mem_layout)
 end function unpack_tensor_i16
 
 !> Put a tensor whose Fortran type is the equivalent 'int32' C-type
 function unpack_tensor_i32(self, name, result, dims) result(code)
-  integer(kind=c_int32_t), dimension(..), target, intent(out) :: result !< Data to be sent
+  integer(kind=c_int32_t), DIM_RANK_SPEC, target, intent(out) :: result !< Data to be sent
   class(client_type),                   intent(in) :: self  !< Pointer to the initialized client
   character(len=*),                     intent(in) :: name  !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims  !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'client/unpack_tensor_methods_common.inc'
 
@@ -584,15 +609,15 @@
   data_type = tensor_int32
   code = unpack_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, c_n_dims, &
     data_type, mem_layout)
 end function unpack_tensor_i32
 
 !> Put a tensor whose Fortran type is the equivalent 'int64' C-type
 function unpack_tensor_i64(self, name, result, dims) result(code)
-  integer(kind=c_int64_t), dimension(..), target, intent(out) :: result !< Data to be sent
+  integer(kind=c_int64_t), DIM_RANK_SPEC, target, intent(out) :: result !< Data to be sent
   class(client_type),                   intent(in) :: self  !< Pointer to the initialized client
   character(len=*),                     intent(in) :: name  !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims  !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'client/unpack_tensor_methods_common.inc'
 
@@ -600,15 +625,15 @@
   data_type = tensor_int64
   code = unpack_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, &
     c_n_dims, data_type, mem_layout)
 end function unpack_tensor_i64
 
 !> Put a tensor whose Fortran type is the equivalent 'float' C-type
 function unpack_tensor_float(self, name, result, dims) result(code)
-  real(kind=c_float), dimension(..), target, intent(out) :: result !< Data to be sent
+  real(kind=c_float), DIM_RANK_SPEC, target, intent(out) :: result !< Data to be sent
   class(client_type),                   intent(in) :: self  !< Pointer to the initialized client
   character(len=*),                     intent(in) :: name  !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims  !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'client/unpack_tensor_methods_common.inc'
 
@@ -616,15 +641,15 @@
   data_type = tensor_flt
   code = unpack_tensor_c(self%client_ptr, c_name, name_length, data_ptr, c_dims_ptr, &
     c_n_dims, data_type, mem_layout)
 end function unpack_tensor_float
 
 !> Put a tensor whose Fortran type is the equivalent 'double' C-type
 function unpack_tensor_double(self, name, result, dims) result(code)
-  real(kind=c_double), dimension(..), target, intent(out) :: result !< Data to be sent
+  real(kind=c_double), DIM_RANK_SPEC, target, intent(out) :: result !< Data to be sent
   class(client_type),                   intent(in) :: self  !< Pointer to the initialized client
   character(len=*),                     intent(in) :: name  !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims  !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'client/unpack_tensor_methods_common.inc'
 
@@ -1675,80 +1700,86 @@
 !> Get the length of the aggregation list
 function poll_list_length(self, list_name, list_length, poll_frequency_ms, num_tries, poll_result) result(code)
   class(client_type),   intent(in   ) :: self               !< An initialized SmartRedis client
   character(len=*),     intent(in   ) :: list_name          !< Name of the dataset to get
   integer,              intent(in   ) :: list_length        !< The desired length of the list
   integer,              intent(in   ) :: poll_frequency_ms  !< Frequency at which to poll the database (ms)
   integer,              intent(in   ) :: num_tries          !< Number of times to poll the database before failing
-  logical(kind=c_bool), intent(  out) :: poll_result        !< True if the list is the requested length, False if not after num_tries.
+  logical,              intent(  out) :: poll_result        !< True if the list is the requested length, False if not after num_tries.
   integer(kind=enum_kind)             :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(list_name)) :: list_name_c
   integer(kind=c_size_t) :: list_name_length
   integer(kind=c_int) :: c_poll_frequency, c_num_tries, c_list_length
+  logical(kind=c_bool) :: c_poll_result
 
   list_name_c = trim(list_name)
   list_name_length = len_trim(list_name)
   c_num_tries = num_tries
   c_poll_frequency = poll_frequency_ms
   c_list_length = list_length
 
   code = poll_list_length_c(self%client_ptr, list_name_c, list_name_length, &
-                            c_list_length, c_poll_frequency, c_num_tries, poll_result)
+                            c_list_length, c_poll_frequency, c_num_tries, c_poll_result)
+  poll_result = c_poll_result
 end function poll_list_length
 
 !> Get the length of the aggregation list
 function poll_list_length_gte(self, list_name, list_length, poll_frequency_ms, num_tries, poll_result) result(code)
   class(client_type),   intent(in   ) :: self               !< An initialized SmartRedis client
   character(len=*),     intent(in   ) :: list_name          !< Name of the dataset to get
   integer,              intent(in   ) :: list_length        !< The desired length of the list
   integer,              intent(in   ) :: poll_frequency_ms  !< Frequency at which to poll the database (ms)
   integer,              intent(in   ) :: num_tries          !< Number of times to poll the database before failing
-  logical(kind=c_bool), intent(  out) :: poll_result        !< True if the list is the requested length, False if not after num_tries.
+  logical,              intent(  out) :: poll_result        !< True if the list is the requested length, False if not after num_tries.
   integer(kind=enum_kind)          :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(list_name)) :: list_name_c
   integer(kind=c_size_t) :: list_name_length
   integer(kind=c_int) :: c_poll_frequency, c_num_tries, c_list_length
+  logical(kind=c_bool) :: c_poll_result
 
   list_name_c = trim(list_name)
   list_name_length = len_trim(list_name)
   c_num_tries = num_tries
   c_poll_frequency = poll_frequency_ms
   c_list_length = list_length
 
   code = poll_list_length_gte_c(self%client_ptr, list_name_c, list_name_length, &
-                            c_list_length, c_poll_frequency, c_num_tries, poll_result)
+                            c_list_length, c_poll_frequency, c_num_tries, c_poll_result)
+  poll_result = c_poll_result
 end function poll_list_length_gte
 
 !> Get the length of the aggregation list
 function poll_list_length_lte(self, list_name, list_length, poll_frequency_ms, num_tries, poll_result) result(code)
   class(client_type),   intent(in) :: self                !< An initialized SmartRedis client
   character(len=*),     intent(in) :: list_name           !< Name of the dataset to get
   integer,              intent(in)  :: list_length        !< The desired length of the list
   integer,              intent(in)  :: poll_frequency_ms  !< Frequency at which to poll the database (ms)
   integer,              intent(in)  :: num_tries          !< Number of times to poll the database before failing
-  logical(kind=c_bool), intent(out) :: poll_result        !< True if the list is the requested length, False if not after num_tries.
+  logical,              intent(out) :: poll_result        !< True if the list is the requested length, False if not after num_tries.
   integer(kind=enum_kind)          :: code
 
   ! Local variables
   character(kind=c_char, len=len_trim(list_name)) :: list_name_c
   integer(kind=c_size_t) :: list_name_length
   integer(kind=c_int) :: c_poll_frequency, c_num_tries, c_list_length
+  logical(kind=c_bool) :: c_poll_result
 
   list_name_c = trim(list_name)
   list_name_length = len_trim(list_name)
   c_num_tries = num_tries
   c_poll_frequency = poll_frequency_ms
   c_list_length = list_length
 
   code = poll_list_length_lte_c(self%client_ptr, list_name_c, list_name_length, &
-                            c_list_length, c_poll_frequency, c_num_tries, poll_result)
+                            c_list_length, c_poll_frequency, c_num_tries, c_poll_result)
+  poll_result = c_poll_result
 end function poll_list_length_lte
 
 !> Get datasets from an aggregation list. Note that this will deallocate an existing list.
 !! NOTE: This potentially be less performant than get_datasets_from_list_range due to an
 !! extra query to the database to get the list length. This is for now necessary because
 !! difficulties in allocating memory for Fortran alloctables from within C.
 function get_datasets_from_list(self, list_name, datasets, num_datasets) result(code)
```

### Comparing `smartredis-0.4.0/src/fortran/dataset/add_meta_scalar_common.inc` & `smartredis-0.4.1/src/fortran/dataset/add_meta_scalar_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/dataset/add_tensor_methods_common.inc` & `smartredis-0.4.1/src/fortran/dataset/add_tensor_methods_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/dataset/dataset_interfaces.inc` & `smartredis-0.4.1/src/fortran/dataset/dataset_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/dataset/get_meta_scalars_common.inc` & `smartredis-0.4.1/src/fortran/dataset/get_meta_scalars_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/dataset/metadata_interfaces.inc` & `smartredis-0.4.1/src/fortran/dataset/metadata_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/dataset/tensor_interfaces.inc` & `smartredis-0.4.1/src/fortran/dataset/tensor_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc` & `smartredis-0.4.1/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc` & `smartredis-0.4.1/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/dataset.F90` & `smartredis-0.4.1/src/fortran/dataset.F90`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,26 @@
 ! FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 ! DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 ! SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 ! CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 ! OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 ! OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+! Note the below macros are here to allow compilation with Nvidia drivers
+! While assumed size should be sufficient, this does not seem to work with
+! Intel and GNU (however those have support for assumed rank)
+#ifdef __NVCOMPILER
+#define DIM_RANK_SPEC dimension(*)
+#else
+#define DIM_RANK_SPEC dimension(..)
+#endif
+
 module smartredis_dataset
 
-use iso_c_binding,   only : c_ptr, c_bool, c_null_ptr, c_char, c_int
+use iso_c_binding,   only : c_ptr, c_char, c_int
 use iso_c_binding,   only : c_int8_t, c_int16_t, c_int32_t, c_int64_t, c_float, c_double, c_size_t
 use iso_c_binding,   only : c_loc, c_f_pointer
 
 use, intrinsic :: iso_fortran_env, only: stderr => error_unit
 
 use fortran_c_interop, only : enum_kind
 
@@ -52,15 +61,15 @@
 type, public :: dataset_type
   type(c_ptr) :: dataset_ptr !< A pointer to the initialized dataset object
 
   contains
 
   !> Initialize a new dataset with a given name
   procedure :: initialize => initialize_dataset
-  !> Access the raw C pointer for the client
+  !> Access the raw C pointer for the dataset
   procedure :: get_c_pointer
 
   ! Metadata procedures
   !> Add metadata to the dataset with a given field and string
   procedure :: add_meta_string
   ! Retrieve the strings associated with a metadata string field
   !> procedure :: get_meta_strings ! Not supported currently
@@ -140,15 +149,15 @@
   type(c_ptr)                     :: get_c_pointer
   class(dataset_type), intent(in) :: self
   get_c_pointer = self%dataset_ptr
 end function get_c_pointer
 
 !> Add a tensor to a dataset whose Fortran type is the equivalent 'int8' C-type
 function add_tensor_i8(self, name, data, dims) result(code)
-  integer(kind=c_int8_t), dimension(..), target, intent(in) :: data !< Data to be sent
+  integer(kind=c_int8_t), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(dataset_type),   intent(in)  :: self !< Fortran SmartRedis dataset
   character(len=*),      intent(in)  :: name !< The unique name used to store in the database
   integer, dimension(:), intent(in)  :: dims !< The length of each dimension
   integer(kind=enum_kind)            :: code !< Result of the operation
 
   include 'dataset/add_tensor_methods_common.inc'
 
@@ -156,15 +165,15 @@
   data_type = tensor_int8
   code = add_tensor_c(self%dataset_ptr, c_name, name_length, data_ptr, &
        c_dims_ptr, c_n_dims, data_type, c_fortran_contiguous)
 end function add_tensor_i8
 
 !> Add a tensor to a dataset whose Fortran type is the equivalent 'int16' C-type
 function add_tensor_i16(self, name, data, dims) result(code)
-  integer(kind=c_int16_t), dimension(..), target, intent(in) :: data !< Data to be sent
+  integer(kind=c_int16_t), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(dataset_type),   intent(in)  :: self !< Fortran SmartRedis dataset
   character(len=*),      intent(in)  :: name !< The unique name used to store in the database
   integer, dimension(:), intent(in)  :: dims !< The length of each dimension
   integer(kind=enum_kind)            :: code !< Result of the operation
 
   include 'dataset/add_tensor_methods_common.inc'
 
@@ -172,15 +181,15 @@
   data_type = tensor_int16
   code = add_tensor_c(self%dataset_ptr, c_name, name_length, data_ptr, &
        c_dims_ptr, c_n_dims, data_type, c_fortran_contiguous)
 end function add_tensor_i16
 
 !> Add a tensor to a dataset whose Fortran type is the equivalent 'int32' C-type
 function add_tensor_i32(self, name, data, dims) result(code)
-  integer(kind=c_int32_t), dimension(..), target, intent(in) :: data !< Data to be sent
+  integer(kind=c_int32_t), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(dataset_type),   intent(in)  :: self !< Fortran SmartRedis dataset
   character(len=*),      intent(in)  :: name !< The unique name used to store in the database
   integer, dimension(:), intent(in)  :: dims !< The length of each dimension
   integer(kind=enum_kind)            :: code !< Result of the operation
 
   include 'dataset/add_tensor_methods_common.inc'
 
@@ -188,15 +197,15 @@
   data_type = tensor_int32
   code = add_tensor_c(self%dataset_ptr, c_name, name_length, data_ptr, &
        c_dims_ptr, c_n_dims, data_type, c_fortran_contiguous)
 end function add_tensor_i32
 
 !> Add a tensor to a dataset whose Fortran type is the equivalent 'int64' C-type
 function add_tensor_i64(self, name, data, dims) result(code)
-  integer(kind=c_int64_t), dimension(..), target, intent(in) :: data !< Data to be sent
+  integer(kind=c_int64_t), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(dataset_type),   intent(in)  :: self !< Fortran SmartRedis dataset
   character(len=*),      intent(in)  :: name !< The unique name used to store in the database
   integer, dimension(:), intent(in)  :: dims !< The length of each dimension
   integer(kind=enum_kind)            :: code !< Result of the operation
 
   include 'dataset/add_tensor_methods_common.inc'
 
@@ -204,15 +213,15 @@
   data_type = tensor_int64
   code = add_tensor_c(self%dataset_ptr, c_name, name_length, data_ptr, &
        c_dims_ptr, c_n_dims, data_type, c_fortran_contiguous)
 end function add_tensor_i64
 
 !> Add a tensor to a dataset whose Fortran type is the equivalent 'float' C-type
 function add_tensor_float(self, name, data, dims) result(code)
-  real(kind=c_float), dimension(..), target, intent(in) :: data !< Data to be sent
+  real(kind=c_float), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(dataset_type),   intent(in)  :: self !< Fortran SmartRedis dataset
   character(len=*),      intent(in)  :: name !< The unique name used to store in the database
   integer, dimension(:), intent(in)  :: dims !< The length of each dimension
   integer(kind=enum_kind)            :: code !< Result of the operation
 
   include 'dataset/add_tensor_methods_common.inc'
 
@@ -220,15 +229,15 @@
   data_type = tensor_flt
   code = add_tensor_c(self%dataset_ptr, c_name, name_length, data_ptr, &
        c_dims_ptr, c_n_dims, data_type, c_fortran_contiguous)
 end function add_tensor_float
 
 !> Add a tensor to a dataset whose Fortran type is the equivalent 'double' C-type
 function add_tensor_double(self, name, data, dims) result(code)
-  real(kind=c_double), dimension(..), target, intent(in) :: data !< Data to be sent
+  real(kind=c_double), DIM_RANK_SPEC, target, intent(in) :: data !< Data to be sent
   class(dataset_type),   intent(in)  :: self !< Fortran SmartRedis dataset
   character(len=*),      intent(in)  :: name !< The unique name used to store in the database
   integer, dimension(:), intent(in)  :: dims !< The length of each dimension
   integer(kind=enum_kind)            :: code !< Result of the operation
 
   include 'dataset/add_tensor_methods_common.inc'
 
@@ -237,15 +246,15 @@
   code = add_tensor_c(self%dataset_ptr, c_name, name_length, data_ptr, &
        c_dims_ptr, c_n_dims, data_type, c_fortran_contiguous)
 end function add_tensor_double
 
 
 !> Unpack a tensor into already allocated memory whose Fortran type is the equivalent 'int8' C-type
 function unpack_dataset_tensor_i8(self, name, result, dims) result(code)
-  integer(kind=c_int8_t), dimension(..), target, intent(out) :: result !< Array to be populated with data
+  integer(kind=c_int8_t), DIM_RANK_SPEC, target, intent(out) :: result !< Array to be populated with data
   class(dataset_type),                  intent(in) :: self !< Pointer to the initialized dataset
   character(len=*),                     intent(in) :: name !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'dataset/unpack_dataset_tensor_methods_common.inc'
 
@@ -253,15 +262,15 @@
   data_type = tensor_int8
   code = unpack_dataset_tensor_c(self%dataset_ptr, c_name, name_length, &
        data_ptr, c_dims_ptr, c_n_dims, data_type, mem_layout)
 end function unpack_dataset_tensor_i8
 
 !> Unpack a tensor into already allocated memory whose Fortran type is the equivalent 'int16' C-type
 function unpack_dataset_tensor_i16(self, name, result, dims) result(code)
-  integer(kind=c_int16_t), dimension(..), target, intent(out) :: result !< Array to be populated with data
+  integer(kind=c_int16_t), DIM_RANK_SPEC, target, intent(out) :: result !< Array to be populated with data
   class(dataset_type),                  intent(in) :: self !< Pointer to the initialized dataset
   character(len=*),                     intent(in) :: name !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'dataset/unpack_dataset_tensor_methods_common.inc'
 
@@ -269,15 +278,15 @@
   data_type = tensor_int16
   code = unpack_dataset_tensor_c(self%dataset_ptr, c_name, name_length, &
        data_ptr, c_dims_ptr, c_n_dims, data_type, mem_layout)
 end function unpack_dataset_tensor_i16
 
 !> Unpack a tensor into already allocated memory whose Fortran type is the equivalent 'int32' C-type
 function unpack_dataset_tensor_i32(self, name, result, dims) result(code)
-  integer(kind=c_int32_t), dimension(..), target, intent(out) :: result !< Array to be populated with data
+  integer(kind=c_int32_t), DIM_RANK_SPEC, target, intent(out) :: result !< Array to be populated with data
   class(dataset_type),                  intent(in) :: self !< Pointer to the initialized dataset
   character(len=*),                     intent(in) :: name !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'dataset/unpack_dataset_tensor_methods_common.inc'
 
@@ -285,15 +294,15 @@
   data_type = tensor_int32
   code = unpack_dataset_tensor_c(self%dataset_ptr, c_name, name_length, &
        data_ptr, c_dims_ptr, c_n_dims, data_type, mem_layout)
 end function unpack_dataset_tensor_i32
 
 !> Unpack a tensor into already allocated memory whose Fortran type is the equivalent 'int64' C-type
 function unpack_dataset_tensor_i64(self, name, result, dims) result(code)
-  integer(kind=c_int64_t), dimension(..), target, intent(out) :: result !< Array to be populated with data
+  integer(kind=c_int64_t), DIM_RANK_SPEC, target, intent(out) :: result !< Array to be populated with data
   class(dataset_type),                  intent(in) :: self !< Pointer to the initialized dataset
   character(len=*),                     intent(in) :: name !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'dataset/unpack_dataset_tensor_methods_common.inc'
 
@@ -301,15 +310,15 @@
   data_type = tensor_int64
   code = unpack_dataset_tensor_c(self%dataset_ptr, c_name, name_length, &
        data_ptr, c_dims_ptr, c_n_dims, data_type, mem_layout)
 end function unpack_dataset_tensor_i64
 
 !> Unpack a tensor into already allocated memory whose Fortran type is the equivalent 'float' C-type
 function unpack_dataset_tensor_float(self, name, result, dims) result(code)
-  real(kind=c_float), dimension(..), target, intent(out) :: result !< Array to be populated with data
+  real(kind=c_float), DIM_RANK_SPEC, target, intent(out) :: result !< Array to be populated with data
   class(dataset_type),                  intent(in) :: self !< Pointer to the initialized dataset
   character(len=*),                     intent(in) :: name !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'dataset/unpack_dataset_tensor_methods_common.inc'
 
@@ -317,15 +326,15 @@
   data_type = tensor_flt
   code = unpack_dataset_tensor_c(self%dataset_ptr, c_name, name_length, &
        data_ptr, c_dims_ptr, c_n_dims, data_type, mem_layout)
 end function unpack_dataset_tensor_float
 
 !> Unpack a tensor into already allocated memory whose Fortran type is the equivalent 'double' C-type
 function unpack_dataset_tensor_double(self, name, result, dims) result(code)
-  real(kind=c_double), dimension(..), target, intent(out) :: result !< Array to be populated with data
+  real(kind=c_double), DIM_RANK_SPEC, target, intent(out) :: result !< Array to be populated with data
   class(dataset_type),                  intent(in) :: self !< Pointer to the initialized dataset
   character(len=*),                     intent(in) :: name !< The name to use to place the tensor
   integer, dimension(:),                intent(in) :: dims !< Length along each dimension of the tensor
   integer(kind=enum_kind)                          :: code
 
   include 'dataset/unpack_dataset_tensor_methods_common.inc'
```

### Comparing `smartredis-0.4.0/src/fortran/errors/errors_interfaces.inc` & `smartredis-0.4.1/src/fortran/errors/errors_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/errors.F90` & `smartredis-0.4.1/src/fortran/errors.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/fortran_c_interop.F90` & `smartredis-0.4.1/src/fortran/fortran_c_interop.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/logcontext/logcontext_interfaces.inc` & `smartredis-0.4.1/src/fortran/logcontext/logcontext_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/logcontext.F90` & `smartredis-0.4.1/src/fortran/logcontext.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/logger/logger_interfaces.inc` & `smartredis-0.4.1/src/fortran/logger/logger_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/fortran/logger.F90` & `smartredis-0.4.1/src/fortran/logger.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/python/bindings/bind.cpp` & `smartredis-0.4.1/src/python/bindings/bind.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -27,36 +27,40 @@
  */
 
 #include "pysrobject.h"
 #include "pyclient.h"
 #include "pydataset.h"
 #include "pylogcontext.h"
 #include "srexception.h"
+#include "pyconfigoptions.h"
 #include "logger.h"
 
 using namespace SmartRedis;
 namespace py = pybind11;
 
 
 PYBIND11_MODULE(smartredisPy, m) {
+#define CLASS_METHOD(class, name) def(#name, &class::name)
+
     m.doc() = "smartredis client"; // optional module docstring
 
     // Python SRObject class
+    #define SROBJECT_METHOD(name) CLASS_METHOD(PySRObject, name)
     py::class_<PySRObject>(m, "PySRObject")
         .def(py::init<std::string&>())
-        .def("log_data", &PySRObject::log_data)
-        .def("log_warning", &PySRObject::log_warning)
-        .def("log_error", &PySRObject::log_error);
+        .SROBJECT_METHOD(log_data)
+        .SROBJECT_METHOD(log_warning)
+        .SROBJECT_METHOD(log_error);
 
     // Python LogContext class
     py::class_<PyLogContext, PySRObject>(m, "PyLogContext")
         .def(py::init<std::string&>());
 
     // Python client class
-    #define CLIENT_METHOD(name)  def(#name, &PyClient::name)
+    #define CLIENT_METHOD(name) CLASS_METHOD(PyClient, name)
     py::class_<PyClient, PySRObject>(m, "PyClient")
         .def(py::init<bool, const std::string&>())
         .CLIENT_METHOD(put_tensor)
         .CLIENT_METHOD(get_tensor)
         .CLIENT_METHOD(delete_tensor)
         .CLIENT_METHOD(copy_tensor)
         .CLIENT_METHOD(rename_tensor)
@@ -113,15 +117,15 @@
         .CLIENT_METHOD(poll_list_length_lte)
         .CLIENT_METHOD(get_datasets_from_list)
         .CLIENT_METHOD(get_dataset_list_range)
         .CLIENT_METHOD(to_string)
     ;
 
     // Python Dataset class
-    #define DATASET_METHOD(name) def(#name, &PyDataset::name)
+    #define DATASET_METHOD(name) CLASS_METHOD(PyDataset, name)
     py::class_<PyDataset, PySRObject>(m, "PyDataset")
         .def(py::init<std::string&>())
         .DATASET_METHOD(add_tensor)
         .DATASET_METHOD(get_tensor)
         .DATASET_METHOD(add_meta_scalar)
         .DATASET_METHOD(add_meta_string)
         .DATASET_METHOD(get_meta_scalars)
@@ -131,14 +135,27 @@
         .DATASET_METHOD(get_metadata_field_type)
         .DATASET_METHOD(get_tensor_type)
         .DATASET_METHOD(get_tensor_names)
         .DATASET_METHOD(get_tensor_dims)
         .DATASET_METHOD(to_string)
     ;
 
+    // Python ConfigOptions class
+    #define CONFIGOPTIONS_METHOD(name) CLASS_METHOD(PyConfigOptions, name)
+    py::class_<PyConfigOptions>(m, "PyConfigOptions")
+        .def_static("create_from_environment",
+                    static_cast<PyConfigOptions* (*)(const std::string&)>(
+                        &PyConfigOptions::create_from_environment))
+        .CONFIGOPTIONS_METHOD(get_integer_option)
+        .CONFIGOPTIONS_METHOD(get_string_option)
+        .CONFIGOPTIONS_METHOD(is_configured)
+        .CONFIGOPTIONS_METHOD(override_integer_option)
+        .CONFIGOPTIONS_METHOD(override_string_option)
+    ;
+
     // Logging functions
     m.def("cpp_log_data", py::overload_cast<const std::string&, SRLoggingLevel, const std::string&>(&log_data))
      .def("cpp_log_data", py::overload_cast<const SRObject*, SRLoggingLevel, const std::string&>(&log_data))
      .def("cpp_log_warning", py::overload_cast<const std::string&, SRLoggingLevel, const std::string&>(&log_warning))
      .def("cpp_log_warning", py::overload_cast<const SRObject*, SRLoggingLevel, const std::string&>(&log_warning))
      .def("cpp_log_error", py::overload_cast<const std::string&, SRLoggingLevel, const std::string&>(&log_error))
      .def("cpp_log_error", py::overload_cast<const SRObject*, SRLoggingLevel, const std::string&>(&log_error));
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis/__init__.py` & `smartredis-0.4.1/src/python/module/smartredis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,31 +22,29 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 __all__ = [
     "Client",
+    "ConfigOptions",
     "Dataset",
     "SRObject",
     "LogContext",
     "DatasetConverter",
     "log_data",
     "log_warning",
     "log_error",
     "LLQuiet",
     "LLInfo",
     "LLDebug",
     "LLDeveloper",
 ]
 
 from .client import Client
+from .configoptions import ConfigOptions
 from .dataset import Dataset
 from .dataset_utils import DatasetConverter
-from .logger import (
-    log_data, log_warning, log_error
-)
+from .logger import log_data, log_warning, log_error
 from .srobject import SRObject
 from .logcontext import LogContext
-from .smartredisPy import (
-    LLQuiet, LLInfo, LLDebug, LLDeveloper
-)
+from .smartredisPy import LLQuiet, LLInfo, LLDebug, LLDeveloper
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis/client.py` & `smartredis-0.4.1/src/python/module/smartredis/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,28 +23,34 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import inspect
 import os
 import os.path as osp
-import functools
 
+import typing as t
 import numpy as np
 
 from .dataset import Dataset
 from .srobject import SRObject
 from .smartredisPy import PyClient
 from .util import Dtypes, init_default, exception_handler, typecheck
 
 from .error import *
 from .smartredisPy import RedisReplyError as PybindRedisReplyError
 
+
 class Client(SRObject):
-    def __init__(self, address=None, cluster=False, logger_name="default"):
+    def __init__(
+        self,
+        address: t.Optional[str] = None,
+        cluster: bool = False,
+        logger_name: str = "default",
+    ) -> None:
         """Initialize a RedisAI client
 
         For clusters, the address can be a single tcp/ip address and port
         of a database node. The rest of the cluster will be discovered
         by the client itself. (e.g. address="127.0.0.1:6379")
 
         If an address is not set, the client will look for the environment
@@ -64,30 +70,29 @@
         try:
             super().__init__(PyClient(cluster, logger_name))
         except PybindRedisReplyError as e:
             raise RedisConnectionError(str(e)) from None
         except RuntimeError as e:
             raise RedisConnectionError(str(e)) from None
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Create a string representation of the client
 
         :return: A string representation of the client
         :rtype: str
         """
         return self._client.to_string()
 
     @property
-    def _client(self):
-        """Alias _srobject to _client
-        """
+    def _client(self) -> PyClient:
+        """Alias _srobject to _client"""
         return self._srobject
 
     @exception_handler
-    def put_tensor(self, name, data):
+    def put_tensor(self, name: str, data: np.ndarray) -> None:
         """Put a tensor to a Redis database
 
         The final tensor key under which the tensor is stored
         may be formed by applying a prefix to the supplied
         name. See use_tensor_ensemble_prefix() for more details.
 
         :param name: name for tensor for be stored at
@@ -98,15 +103,15 @@
         """
         typecheck(name, "name", str)
         typecheck(data, "data", np.ndarray)
         dtype = Dtypes.tensor_from_numpy(data)
         self._client.put_tensor(name, dtype, data)
 
     @exception_handler
-    def get_tensor(self, name):
+    def get_tensor(self, name: str) -> np.ndarray:
         """Get a tensor from the database
 
         The tensor key used to locate the tensor
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
         and use_tensor_ensemble_prefix() for more details.
 
@@ -116,15 +121,15 @@
         :return: numpy array of tensor data
         :rtype: np.array
         """
         typecheck(name, "name", str)
         return self._client.get_tensor(name)
 
     @exception_handler
-    def delete_tensor(self, name):
+    def delete_tensor(self, name: str) -> None:
         """Delete a tensor from the database
 
         The tensor key used to locate the tensor to be deleted
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
         and use_tensor_ensemble_prefix() for more details.
 
@@ -132,15 +137,15 @@
         :type name: str
         :raises RedisReplyError: if deletion fails
         """
         typecheck(name, "name", str)
         self._client.delete_tensor(name)
 
     @exception_handler
-    def copy_tensor(self, src_name, dest_name):
+    def copy_tensor(self, src_name: str, dest_name: str) -> None:
         """Copy a tensor at one name to another name
 
         The source and destination tensor keys used to locate
         and store the tensor may be formed by applying prefixes
         to the supplied src_name and dest_name. See set_data_source()
         and use_tensor_ensemble_prefix() for more details.
 
@@ -151,15 +156,15 @@
         :raises RedisReplyError: if copy operation fails
         """
         typecheck(src_name, "src_name", str)
         typecheck(dest_name, "dest_name", str)
         self._client.copy_tensor(src_name, dest_name)
 
     @exception_handler
-    def rename_tensor(self, old_name, new_name):
+    def rename_tensor(self, old_name: str, new_name: str) -> None:
         """Rename a tensor in the database
 
         The old and new tensor keys used to find and relocate
         the tensor may be formed by applying prefixes to the supplied
         old_name and new_name. See set_data_source()
         and use_tensor_ensemble_prefix() for more details.
 
@@ -170,15 +175,15 @@
         :raises RedisReplyError: if rename operation fails
         """
         typecheck(old_name, "old_name", str)
         typecheck(new_name, "new_name", str)
         self._client.rename_tensor(old_name, new_name)
 
     @exception_handler
-    def put_dataset(self, dataset):
+    def put_dataset(self, dataset: Dataset) -> None:
         """Put a Dataset instance into the database
 
         The final dataset key under which the dataset is stored
         is generated from the name that was supplied when the
         dataset was created and may be prefixed. See
         use_dataset_ensemble_prefix() for more details.
 
@@ -191,15 +196,15 @@
         :raises RedisReplyError: if update fails
         """
         typecheck(dataset, "dataset", Dataset)
         pybind_dataset = dataset.get_data()
         self._client.put_dataset(pybind_dataset)
 
     @exception_handler
-    def get_dataset(self, name):
+    def get_dataset(self, name: str) -> Dataset:
         """Get a dataset from the database
 
         The dataset key used to locate the dataset
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
         and use_dataset_ensemble_prefix() for more details.
 
@@ -211,15 +216,15 @@
         """
         typecheck(name, "name", str)
         dataset = self._client.get_dataset(name)
         python_dataset = Dataset.from_pybind(dataset)
         return python_dataset
 
     @exception_handler
-    def delete_dataset(self, name):
+    def delete_dataset(self, name: str) -> None:
         """Delete a dataset within the database
 
         The dataset key used to locate the dataset to be deleted
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
         and use_dataset_ensemble_prefix() for more details.
 
@@ -227,15 +232,15 @@
         :type name: str
         :raises RedisReplyError: if deletion fails
         """
         typecheck(name, "name", str)
         self._client.delete_dataset(name)
 
     @exception_handler
-    def copy_dataset(self, src_name, dest_name):
+    def copy_dataset(self, src_name: str, dest_name: str) -> None:
         """Copy a dataset from one key to another
 
         The source and destination dataset keys used to
         locate the dataset may be formed by applying prefixes
         to the supplied src_name and dest_name. See set_data_source()
         and use_dataset_ensemble_prefix() for more details.
 
@@ -246,15 +251,15 @@
         :raises RedisReplyError: if copy operation fails
         """
         typecheck(src_name, "src_name", str)
         typecheck(dest_name, "dest_name", str)
         self._client.copy_dataset(src_name, dest_name)
 
     @exception_handler
-    def rename_dataset(self, old_name, new_name):
+    def rename_dataset(self, old_name: str, new_name: str) -> None:
         """Rename a dataset in the database
 
         The old and new dataset keys used to find and relocate
         the dataset may be formed by applying prefixes to the supplied
         old_name and new_name. See set_data_source()
         and use_dataset_ensemble_prefix() for more details.
 
@@ -265,15 +270,17 @@
         :raises RedisReplyError: if rename operation fails
         """
         typecheck(old_name, "old_name", str)
         typecheck(new_name, "new_name", str)
         self._client.rename_dataset(old_name, new_name)
 
     @exception_handler
-    def set_function(self, name, function, device="CPU"):
+    def set_function(
+        self, name: str, function: t.Callable, device: str = "CPU"
+    ) -> None:
         """Set a callable function into the database
 
         The final script key used to store the function may be formed
         by applying a prefix to the supplied name.
         See use_model_ensemble_prefix() for more details.
 
         Function must be a callable TorchScript function and have at least
@@ -290,21 +297,25 @@
         :type device: str, optional
         :raises TypeError: if argument was not a callable function
         :raises RedisReplyError: if function failed to set
         """
         typecheck(name, "name", str)
         typecheck(device, "device", str)
         if not callable(function):
-            raise TypeError(f"Argument provided for function, {type(function)}, is not callable")
+            raise TypeError(
+                f"Argument provided for function, {type(function)}, is not callable"
+            )
         device = self.__check_device(device)
         fn_src = inspect.getsource(function)
         self._client.set_script(name, device, fn_src)
 
     @exception_handler
-    def set_function_multigpu(self, name, function, first_gpu, num_gpus):
+    def set_function_multigpu(
+        self, name: str, function: t.Callable, first_gpu: int, num_gpus: int
+    ) -> None:
         """Set a callable function into the database for use
         in a multi-GPU system
 
         The final script key used to store the function may be formed
         by applying a prefix to the supplied name.
         See use_model_ensemble_prefix() for more details.
 
@@ -323,20 +334,22 @@
         :raises TypeError: if argument was not a callable function
         :raises RedisReplyError: if function failed to set
         """
         typecheck(name, "name", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         if not callable(function):
-            raise TypeError(f"Argument provided for function, {type(function)}, is not callable")
+            raise TypeError(
+                f"Argument provided for function, {type(function)}, is not callable"
+            )
         fn_src = inspect.getsource(function)
         self._client.set_script_multigpu(name, fn_src, first_gpu, num_gpus)
 
     @exception_handler
-    def set_script(self, name, script, device="CPU"):
+    def set_script(self, name: str, script: str, device: str = "CPU") -> None:
         """Store a TorchScript at a key in the database
 
         The final script key used to store the script may be formed
         by applying a prefix to the supplied name.
         See use_model_ensemble_prefix() for more details.
 
         Device selection is either "GPU" or "CPU". If many GPUs are present,
@@ -353,15 +366,17 @@
         typecheck(name, "name", str)
         typecheck(script, "script", str)
         typecheck(device, "device", str)
         device = self.__check_device(device)
         self._client.set_script(name, device, script)
 
     @exception_handler
-    def set_script_multigpu(self, name, script, first_gpu, num_gpus):
+    def set_script_multigpu(
+        self, name: str, script: str, first_gpu: int, num_gpus: int
+    ) -> None:
         """Store a TorchScript at a key in the database
 
         The final script key used to store the script may be formed
         by applying a prefix to the supplied name.
         See use_model_ensemble_prefix() for more details.
 
         :param name: name to store the script under
@@ -377,15 +392,15 @@
         typecheck(name, "name", str)
         typecheck(script, "script", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         self._client.set_script_multigpu(name, script, first_gpu, num_gpus)
 
     @exception_handler
-    def set_script_from_file(self, name, file, device="CPU"):
+    def set_script_from_file(self, name: str, file: str, device: str = "CPU") -> None:
         """Same as Client.set_script, but from file
 
         The final script key used to store the script may be formed
         by applying a prefix to the supplied name.
         See use_model_ensemble_prefix() for more details.
 
         :param name: key to store script under
@@ -400,15 +415,17 @@
         typecheck(file, "file", str)
         typecheck(device, "device", str)
         device = self.__check_device(device)
         file_path = self.__check_file(file)
         self._client.set_script_from_file(name, device, file_path)
 
     @exception_handler
-    def set_script_from_file_multigpu(self, name, file, first_gpu, num_gpus):
+    def set_script_from_file_multigpu(
+        self, name: str, file: str, first_gpu: int, num_gpus: int
+    ) -> None:
         """Same as Client.set_script_multigpu, but from file
 
         The final script key used to store the script may be formed
         by applying a prefix to the supplied name.
         See use_model_ensemble_prefix() for more details.
 
         :param name: key to store script under
@@ -425,15 +442,15 @@
         typecheck(file, "file", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         file_path = self.__check_file(file)
         self._client.set_script_from_file_multigpu(name, file_path, first_gpu, num_gpus)
 
     @exception_handler
-    def get_script(self, name):
+    def get_script(self, name: str) -> str:
         """Retrieve a Torchscript stored in the database
 
         The script key used to locate the script
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and
         use_model_ensemble_prefix() for more details.
 
@@ -444,15 +461,17 @@
         :rtype: str
         """
         typecheck(name, "name", str)
         script = self._client.get_script(name)
         return script
 
     @exception_handler
-    def run_script(self, name, fn_name, inputs, outputs):
+    def run_script(
+        self, name: str, fn_name: str, inputs: t.List[str], outputs: t.List[str]
+    ) -> None:
         """Execute TorchScript stored inside the database
 
         The script key used to locate the script to be run
         may be formed by applying a prefix to the supplied
         name. Similarly, the tensor names in the
         input and output lists may be prefixed. See
         set_data_source(), use_model_ensemble_prefix(), and
@@ -473,15 +492,23 @@
         typecheck(inputs, "inputs", list)
         typecheck(outputs, "outputs", list)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
         self._client.run_script(name, fn_name, inputs, outputs)
 
     @exception_handler
     def run_script_multigpu(
-        self, name, fn_name, inputs, outputs, offset, first_gpu, num_gpus):
+        self,
+        name: str,
+        fn_name: str,
+        inputs: t.List[str],
+        outputs: t.List[str],
+        offset: int,
+        first_gpu: int,
+        num_gpus: int,
+    ) -> None:
         """Execute TorchScript stored inside the database
 
         The script key used to locate the script to be run
         may be formed by applying a prefix to the supplied
         name. Similarly, the tensor names in the
         input and output lists may be prefixed. See
         set_data_source(), use_model_ensemble_prefix(), and
@@ -509,18 +536,19 @@
         typecheck(inputs, "inputs", list)
         typecheck(outputs, "outputs", list)
         typecheck(offset, "offset", int)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
         self._client.run_script_multigpu(
-            name, fn_name, inputs, outputs, offset, first_gpu, num_gpus)
+            name, fn_name, inputs, outputs, offset, first_gpu, num_gpus
+        )
 
     @exception_handler
-    def delete_script(self, name):
+    def delete_script(self, name: str) -> None:
         """Remove a script from the database
 
         The script key used to locate the script to be run
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_model_ensemble_prefix()
         for more details
 
@@ -528,15 +556,15 @@
         :type name: str
         :raises RedisReplyError: if script deletion fails
         """
         typecheck(name, "name", str)
         self._client.delete_script(name)
 
     @exception_handler
-    def delete_script_multigpu(self, name, first_gpu, num_gpus):
+    def delete_script_multigpu(self, name: str, first_gpu: int, num_gpus: int) -> None:
         """Remove a script from the database
 
         The script key used to locate the script to be run
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_model_ensemble_prefix()
         for more details
 
@@ -550,15 +578,15 @@
         """
         typecheck(name, "name", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         self._client.delete_script_multigpu(name, first_gpu, num_gpus)
 
     @exception_handler
-    def get_model(self, name):
+    def get_model(self, name: str) -> bytes:
         """Get a stored model
 
         The model key used to locate the model
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
         and use_model_ensemble_prefix() for more details.
 
@@ -571,24 +599,24 @@
         typecheck(name, "name", str)
         model = self._client.get_model(name)
         return model
 
     @exception_handler
     def set_model(
         self,
-        name,
-        model,
-        backend,
-        device="CPU",
-        batch_size=0,
-        min_batch_size=0,
-        tag="",
-        inputs=None,
-        outputs=None,
-    ):
+        name: str,
+        model: bytes,
+        backend: str,
+        device: str = "CPU",
+        batch_size: int = 0,
+        min_batch_size: int = 0,
+        tag: str = "",
+        inputs: t.Optional[t.Union[str, t.List[str]]] = None,
+        outputs: t.Optional[t.Union[str, t.List[str]]] = None,
+    ) -> None:
         """Put a TF, TF-lite, PT, or ONNX model in the database
 
         The final model key used to store the model
         may be formed by applying a prefix to the supplied
         name. Similarly, the tensor names in the
         input and output nodes for TF models may be prefixed.
         See set_data_source(), use_model_ensemble_prefix(), and
@@ -607,17 +635,17 @@
         :param batch_size: batch size for execution, defaults to 0
         :type batch_size: int, optional
         :param min_batch_size: minimum batch size for model execution, defaults to 0
         :type min_batch_size: int, optional
         :param tag: additional tag for model information, defaults to ""
         :type tag: str, optional
         :param inputs: model inputs (TF only), defaults to None
-        :type inputs: list[str], optional
+        :type inputs: str | list[str] | None
         :param outputs: model outputs (TF only), defaults to None
-        :type outputs: list[str], optional
+        :type outputs: str | list[str] | None
         :raises RedisReplyError: if model fails to set
         """
         typecheck(name, "name", str)
         typecheck(backend, "backend", str)
         typecheck(device, "device", str)
         typecheck(batch_size, "batch_size", int)
         typecheck(min_batch_size, "min_batch_size", int)
@@ -636,25 +664,25 @@
             inputs,
             outputs,
         )
 
     @exception_handler
     def set_model_multigpu(
         self,
-        name,
-        model,
-        backend,
-        first_gpu,
-        num_gpus,
-        batch_size=0,
-        min_batch_size=0,
-        tag="",
-        inputs=None,
-        outputs=None
-    ):
+        name: str,
+        model: bytes,
+        backend: str,
+        first_gpu: int,
+        num_gpus: int,
+        batch_size: int = 0,
+        min_batch_size: int = 0,
+        tag: str = "",
+        inputs: t.Optional[t.Union[str, t.List[str]]] = None,
+        outputs: t.Optional[t.Union[str, t.List[str]]] = None,
+    ) -> None:
         """Put a TF, TF-lite, PT, or ONNX model in the database for use
         in a multi-GPU system
 
         The final model key used to store the model
         may be formed by applying a prefix to the supplied
         name. Similarly, the tensor names in the
         input and output nodes for TF models may be prefixed.
@@ -674,17 +702,17 @@
         :param batch_size: batch size for execution, defaults to 0
         :type batch_size: int, optional
         :param min_batch_size: minimum batch size for model execution, defaults to 0
         :type min_batch_size: int, optional
         :param tag: additional tag for model information, defaults to ""
         :type tag: str, optional
         :param inputs: model inputs (TF only), defaults to None
-        :type inputs: list[str], optional
+        :type inputs: str | list[str] | None
         :param outputs: model outputs (TF only), defaults to None
-        :type outputs: list[str], optional
+        :type outputs: str | list[str] | None
         :raises RedisReplyError: if model fails to set
         """
         typecheck(name, "name", str)
         typecheck(backend, "backend", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         typecheck(batch_size, "batch_size", int)
@@ -698,30 +726,30 @@
             backend,
             first_gpu,
             num_gpus,
             batch_size,
             min_batch_size,
             tag,
             inputs,
-            outputs
+            outputs,
         )
 
     @exception_handler
     def set_model_from_file(
         self,
-        name,
-        model_file,
-        backend,
-        device="CPU",
-        batch_size=0,
-        min_batch_size=0,
-        tag="",
-        inputs=None,
-        outputs=None,
-    ):
+        name: str,
+        model_file: str,
+        backend: str,
+        device: str = "CPU",
+        batch_size: int = 0,
+        min_batch_size: int = 0,
+        tag: str = "",
+        inputs: t.Optional[t.Union[str, t.List[str]]] = None,
+        outputs: t.Optional[t.Union[str, t.List[str]]] = None,
+    ) -> None:
         """Put a TF, TF-lite, PT, or ONNX model from file in the database
 
         The final model key used to store the model
         may be formed by applying a prefix to the supplied
         name. Similarly, the tensor names in the
         input and output nodes for TF models may be prefixed.
         See set_data_source(), use_model_ensemble_prefix(), and
@@ -740,17 +768,17 @@
         :param batch_size: batch size for execution, defaults to 0
         :type batch_size: int, optional
         :param min_batch_size: minimum batch size for model execution, defaults to 0
         :type min_batch_size: int, optional
         :param tag: additional tag for model information, defaults to ""
         :type tag: str, optional
         :param inputs: model inputs (TF only), defaults to None
-        :type inputs: list[str], optional
+        :type inputs: str | list[str] | None
         :param outputs: model outupts (TF only), defaults to None
-        :type outputs: list[str], optional
+        :type outputs: str | list[str] | None
         :raises RedisReplyError: if model fails to set
         """
         typecheck(name, "name", str)
         typecheck(model_file, "model_file", str)
         typecheck(backend, "backend", str)
         typecheck(device, "device", str)
         typecheck(batch_size, "batch_size", int)
@@ -771,25 +799,25 @@
             inputs,
             outputs,
         )
 
     @exception_handler
     def set_model_from_file_multigpu(
         self,
-        name,
-        model_file,
-        backend,
-        first_gpu,
-        num_gpus,
-        batch_size=0,
-        min_batch_size=0,
-        tag="",
-        inputs=None,
-        outputs=None,
-    ):
+        name: str,
+        model_file: str,
+        backend: str,
+        first_gpu: int,
+        num_gpus: int,
+        batch_size: int = 0,
+        min_batch_size: int = 0,
+        tag: str = "",
+        inputs: t.Optional[t.Union[str, t.List[str]]] = None,
+        outputs: t.Optional[t.Union[str, t.List[str]]] = None,
+    ) -> None:
         """Put a TF, TF-lite, PT, or ONNX model from file in the database
         for use in a multi-GPU system
 
         The final model key used to store the model
         may be formed by applying a prefix to the supplied
         name. Similarly, the tensor names in the
         input and output nodes for TF models may be prefixed.
@@ -809,17 +837,17 @@
         :param batch_size: batch size for execution, defaults to 0
         :type batch_size: int, optional
         :param min_batch_size: minimum batch size for model execution, defaults to 0
         :type min_batch_size: int, optional
         :param tag: additional tag for model information, defaults to ""
         :type tag: str, optional
         :param inputs: model inputs (TF only), defaults to None
-        :type inputs: list[str], optional
+        :type inputs: str | list[str] | None
         :param outputs: model outupts (TF only), defaults to None
-        :type outputs: list[str], optional
+        :type outputs: str | list[str] | None
         :raises RedisReplyError: if model fails to set
         """
         typecheck(name, "name", str)
         typecheck(model_file, "model_file", str)
         typecheck(backend, "backend", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
@@ -839,43 +867,49 @@
             min_batch_size,
             tag,
             inputs,
             outputs,
         )
 
     @exception_handler
-    def run_model(self, name, inputs=None, outputs=None):
+    def run_model(
+        self,
+        name: str,
+        inputs: t.Optional[t.Union[str, t.List[str]]] = None,
+        outputs: t.Optional[t.Union[str, t.List[str]]] = None,
+    ) -> None:
         """Execute a stored model
 
         The model key used to locate the model to be run
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
         and use_model_ensemble_prefix() for more details.
 
         :param name: name for stored model
         :type name: str
         :param inputs: names of stored inputs to provide model, defaults to None
-        :type inputs: list[str], optional
+        :type inputs: str | list[str] | None
         :param outputs: names to store outputs under, defaults to None
-        :type outputs: list[str], optional
+        :type outputs: str | list[str] | None
         :raises RedisReplyError: if model execution fails
         """
         typecheck(name, "name", str)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
         self._client.run_model(name, inputs, outputs)
 
     @exception_handler
     def run_model_multigpu(
         self,
-        name,
-        offset,
-        first_gpu,
-        num_gpus,
-        inputs=None,
-        outputs=None):
+        name: str,
+        offset: int,
+        first_gpu: int,
+        num_gpus: int,
+        inputs: t.Optional[t.Union[str, t.List[str]]] = None,
+        outputs: t.Optional[t.Union[str, t.List[str]]] = None,
+    ) -> None:
         """Execute a model stored for a multi-GPU system
 
         The model key used to locate the model to be run
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
         and use_model_ensemble_prefix() for more details.
 
@@ -885,28 +919,30 @@
                          or MPI rank
         :type offset: int
         :param first_gpu: the first GPU (zero-based) to use in processing this model
         :type first_gpu: int
         :param num_gpus: the number of gpus for which the model was stored
         :type num_gpus: int
         :param inputs: names of stored inputs to provide model, defaults to None
-        :type inputs: list[str], optional
+        :type inputs: str | list[str] | None
         :param outputs: names to store outputs under, defaults to None
-        :type outputs: list[str], optional
+        :type outputs: str | list[str] | None
         :raises RedisReplyError: if model execution fails
         """
         typecheck(name, "name", str)
         typecheck(offset, "offset", int)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         inputs, outputs = self.__check_tensor_args(inputs, outputs)
-        self._client.run_model_multigpu(name, inputs, outputs, offset, first_gpu, num_gpus)
+        self._client.run_model_multigpu(
+            name, inputs, outputs, offset, first_gpu, num_gpus
+        )
 
     @exception_handler
-    def delete_model(self, name):
+    def delete_model(self, name: str) -> None:
         """Remove a model from the database
 
         The model key used to locate the script to be run
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_model_ensemble_prefix()
         for more details
 
@@ -914,15 +950,15 @@
         :type name: str
         :raises RedisReplyError: if model deletion fails
         """
         typecheck(name, "name", str)
         self._client.delete_model(name)
 
     @exception_handler
-    def delete_model_multigpu(self, name, first_gpu, num_gpus):
+    def delete_model_multigpu(self, name: str, first_gpu: int, num_gpus: str) -> None:
         """Remove a model from the database that was stored for use with multiple GPUs
 
         The model key used to locate the script to be run
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_model_ensemble_prefix()
         for more details
 
@@ -936,15 +972,15 @@
         """
         typecheck(name, "name", str)
         typecheck(first_gpu, "first_gpu", int)
         typecheck(num_gpus, "num_gpus", int)
         self._client.delete_model_multigpu(name, first_gpu, num_gpus)
 
     @exception_handler
-    def tensor_exists(self, name):
+    def tensor_exists(self, name: str) -> bool:
         """Check if a tensor exists in the database
 
         The tensor key used to check for existence
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
         and use_tensor_ensemble_prefix() for more details.
 
@@ -954,15 +990,15 @@
         :rtype: bool
         :raises RedisReplyError: if checking for tensor existence causes an error
         """
         typecheck(name, "name", str)
         return self._client.tensor_exists(name)
 
     @exception_handler
-    def dataset_exists(self, name):
+    def dataset_exists(self, name: str) -> bool:
         """Check if a dataset exists in the database
 
         The dataset key used to check for existence
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
         and use_dataset_ensemble_prefix() for more details.
 
@@ -972,15 +1008,15 @@
         :rtype: bool
         :raises RedisReplyError: if `dataset_exists` fails (i.e. causes an error)
         """
         typecheck(name, "name", str)
         return self._client.dataset_exists(name)
 
     @exception_handler
-    def model_exists(self, name):
+    def model_exists(self, name: str) -> bool:
         """Check if a model or script exists in the database
 
         The model or script key used to check for existence
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
         and use_model_ensemble_prefix() for more details.
 
@@ -990,28 +1026,28 @@
         :rtype: bool
         :raises RedisReplyError: if `model_exists` fails (i.e. causes an error)
         """
         typecheck(name, "name", str)
         return self._client.model_exists(name)
 
     @exception_handler
-    def key_exists(self, key):
+    def key_exists(self, key: str) -> bool:
         """Check if the key exists in the database
 
         :param key: The key that will be checked in the database
         :type key: str
         :returns: Returns true if the key exists in the database
         :rtype: bool
         :raises RedisReplyError: if `key_exists` fails
         """
         typecheck(key, "key", str)
         return self._client.key_exists(key)
 
     @exception_handler
-    def poll_key(self, key, poll_frequency_ms, num_tries):
+    def poll_key(self, key: str, poll_frequency_ms: int, num_tries: int) -> bool:
         """Check if the key exists in the database
 
         The check is repeated at a specified polling interval and for
         a specified number of retries.
 
         :param key: The key that will be checked in the database
         :type key: str
@@ -1026,15 +1062,15 @@
         """
         typecheck(key, "key", str)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
         return self._client.poll_key(key, poll_frequency_ms, num_tries)
 
     @exception_handler
-    def poll_tensor(self, name, poll_frequency_ms, num_tries):
+    def poll_tensor(self, name: str, poll_frequency_ms: int, num_tries: int) -> bool:
         """Check if a tensor exists in the database
 
         The check is repeated at a specified polling interval and for
         a specified number of retries.
         The tensor key used to check for existence
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
@@ -1053,15 +1089,15 @@
         """
         typecheck(name, "name", str)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
         return self._client.poll_tensor(name, poll_frequency_ms, num_tries)
 
     @exception_handler
-    def poll_dataset(self, name, poll_frequency_ms, num_tries):
+    def poll_dataset(self, name: str, poll_frequency_ms: int, num_tries: int) -> bool:
         """Check if a dataset exists in the database
 
         The check is repeated at a specified polling interval and for
         a specified number of retries.
         The dataset key used to check for existence
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
@@ -1080,15 +1116,15 @@
         """
         typecheck(name, "name", str)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
         return self._client.poll_dataset(name, poll_frequency_ms, num_tries)
 
     @exception_handler
-    def poll_model(self, name, poll_frequency_ms, num_tries):
+    def poll_model(self, name: str, poll_frequency_ms: int, num_tries: int) -> bool:
         """Check if a model or script exists in the database
 
         The check is repeated at a specified polling interval and for
         a specified number of retries.
         The model or script key used to check for existence
         may be formed by applying a prefix to the supplied
         name. See set_data_source()
@@ -1107,15 +1143,15 @@
         """
         typecheck(name, "name", str)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
         return self._client.poll_model(name, poll_frequency_ms, num_tries)
 
     @exception_handler
-    def set_data_source(self, source_id):
+    def set_data_source(self, source_id: str) -> None:
         """Set the data source, a key prefix for future operations
 
         When running multiple applications, such as an ensemble
         computation, there is a risk that the same name is used
         for a tensor, dataset, script, or model by more than one
         executing entity. In order to prevent this sort of collision,
         SmartRedis affords the ability to add a prefix to names,
@@ -1136,15 +1172,15 @@
         :type source_id: str
         :raises RedisReplyError: if set data
         """
         typecheck(source_id, "source_id", str)
         return self._client.set_data_source(source_id)
 
     @exception_handler
-    def use_model_ensemble_prefix(self, use_prefix):
+    def use_model_ensemble_prefix(self, use_prefix: bool) -> None:
         """Control whether model and script keys are
            prefixed (e.g. in an ensemble) when forming database keys
 
         This function can be used to avoid key collisions in an ensemble
         by prepending the string value from the environment variable SSKEYIN
         to model and script names.
         Prefixes will only be used if they were previously set through
@@ -1159,15 +1195,15 @@
                            available.
         :type use_prefix: bool
         """
         typecheck(use_prefix, "use_prefix", bool)
         return self._client.use_model_ensemble_prefix(use_prefix)
 
     @exception_handler
-    def use_list_ensemble_prefix(self, use_prefix):
+    def use_list_ensemble_prefix(self, use_prefix: bool) -> None:
         """Control whether aggregation lists are prefixed
            when forming database keys
 
         This function can be used to avoid key collisions in an
         ensemble by prepending the string value from the
         environment variable SSKEYIN and/or SSKEYOUT to
         aggregation list names.  Prefixes will only be used if
@@ -1188,15 +1224,15 @@
                            available.
         :type use_prefix: bool
         """
         typecheck(use_prefix, "use_prefix", bool)
         return self._client.use_list_ensemble_prefix(use_prefix)
 
     @exception_handler
-    def use_tensor_ensemble_prefix(self, use_prefix):
+    def use_tensor_ensemble_prefix(self, use_prefix: bool) -> None:
         """Control whether tensor keys are prefixed (e.g. in an
         ensemble) when forming database keys
 
         This function can be used to avoid key collisions in an ensemble
         by prepending the string value from the environment variable SSKEYIN
         to tensor names.
         Prefixes will only be used if they were previously set through
@@ -1210,15 +1246,15 @@
                            will use a prefix, if available.
         :type use_prefix: bool
         """
         typecheck(use_prefix, "use_prefix", bool)
         return self._client.use_tensor_ensemble_prefix(use_prefix)
 
     @exception_handler
-    def use_dataset_ensemble_prefix(self, use_prefix):
+    def use_dataset_ensemble_prefix(self, use_prefix: bool) -> None:
         """Control whether dataset keys are prefixed (e.g. in an ensemble)
            when forming database keys
 
         This function can be used to avoid key collisions in an ensemble
         by prepending the string value from the environment variable SSKEYIN
         to dataset names.
         Prefixes will only be used if they were previously set through
@@ -1232,15 +1268,15 @@
                            will use a prefix, if available.
         :type use_prefix: bool
         """
         typecheck(use_prefix, "use_prefix", bool)
         return self._client.use_dataset_ensemble_prefix(use_prefix)
 
     @exception_handler
-    def get_db_node_info(self, addresses):
+    def get_db_node_info(self, addresses: t.List[str]) -> t.List[t.Dict]:
         """Returns information about given database nodes
 
         :param addresses: The addresses of the database nodes
         :type address: list[str]
         :returns: A list of dictionaries with each entry in the
                   list corresponding to an address reply
         :rtype: list[dict]
@@ -1255,15 +1291,15 @@
                 CLUSTER SLOTS commands can lead to RedisReplyError
                 being thrown.
         """
         typecheck(addresses, "addresses", list)
         return self._client.get_db_node_info(addresses)
 
     @exception_handler
-    def get_db_cluster_info(self, addresses):
+    def get_db_cluster_info(self, addresses: t.List[str]) -> t.List[t.Dict]:
         """Returns cluster information from a specified db node.
         If the address does not correspond to a cluster node,
         an empty dictionary is returned.
 
         :param addresses: The addresses of the database nodes
         :type address: list[str]
         :returns: A list of dictionaries with each entry in the
@@ -1281,15 +1317,17 @@
                 CLUSTER SLOTS commands can lead to RedisReplyError
                 being thrown.
         """
         typecheck(addresses, "addresses", list)
         return self._client.get_db_cluster_info(addresses)
 
     @exception_handler
-    def get_ai_info(self, address, key, reset_stat=False):
+    def get_ai_info(
+        self, address: t.List[str], key: str, reset_stat: bool = False
+    ) -> t.List[t.Dict]:
         """Returns AI.INFO command reply information for the
         script or model key at the provided addresses.
 
         :param addresses: The addresses of the database nodes
         :type address: list[str]
         :param key: The key associated with the model or script
         :type key: str
@@ -1305,15 +1343,15 @@
         """
         typecheck(address, "address", list)
         typecheck(key, "key", str)
         typecheck(reset_stat, "reset_stat", bool)
         return self._client.get_ai_info(address, key, reset_stat)
 
     @exception_handler
-    def flush_db(self, addresses):
+    def flush_db(self, addresses: t.List[str]) -> None:
         """Removes all keys from a specified db node.
 
         :param addresses: The addresses of the database nodes
         :type address: list[str]
         :raises RedisReplyError: if there is an error
                 in command execution or the address
                 is not reachable by the client.
@@ -1325,15 +1363,15 @@
                 CLUSTER SLOTS commands can lead to RedisReplyError
                 being thrown.
         """
         typecheck(addresses, "addresses", list)
         self._client.flush_db(addresses)
 
     @exception_handler
-    def config_get(self, expression, address):
+    def config_get(self, expression: str, address: t.List[str]) -> t.Dict:
         """Read the configuration parameters of a running server.
         If the address does not correspond to a cluster node,
         an empty dictionary is returned.
 
         :param expression: Parameter used in the configuration or a
                            glob pattern (Use '*' to retrieve all
                            configuration parameters)
@@ -1356,15 +1394,15 @@
                 being thrown.
         """
         typecheck(expression, "expression", str)
         typecheck(address, "address", str)
         return self._client.config_get(expression, address)
 
     @exception_handler
-    def config_set(self, config_param, value, address):
+    def config_set(self, config_param: str, value: str, address: str) -> None:
         """Reconfigure the server. It can change both trivial
         parameters or switch from one to another persistence option.
         All the configuration parameters set using this command are
         immediately loaded by Redis and will take effect starting with
         the next command executed.
         If the address does not correspond to a cluster node,
         an empty dictionary is returned.
@@ -1388,15 +1426,15 @@
         """
         typecheck(config_param, "config_param", str)
         typecheck(value, "value", str)
         typecheck(address, "address", str)
         self._client.config_set(config_param, value, address)
 
     @exception_handler
-    def save(self, addresses):
+    def save(self, addresses: t.List[str]) -> None:
         """Performs a synchronous save of the database shard
         producing a point in time snapshot of all the data
         inside the Redis instance, in the form of an RBD file.
 
         :param addresses: The addresses of the database nodes
         :type addresses: list[str]
         :raises RedisReplyError: if there is an error
@@ -1410,15 +1448,15 @@
                 CLUSTER SLOTS commands can lead to RedisReplyError
                 being thrown.
         """
         typecheck(addresses, "addresses", list)
         self._client.save(addresses)
 
     @exception_handler
-    def append_to_list(self, list_name, dataset):
+    def append_to_list(self, list_name: str, dataset: Dataset) -> None:
         """Appends a dataset to the aggregation list
 
         When appending a dataset to an aggregation list,
         the list will automatically be created if it does not
         exist (i.e. this is the first entry in the list).
         Aggregation lists work by referencing the dataset
         by storing its key, so appending a dataset
@@ -1437,15 +1475,15 @@
         """
         typecheck(list_name, "list_name", str)
         typecheck(dataset, "dataset", Dataset)
         pybind_dataset = dataset.get_data()
         self._client.append_to_list(list_name, pybind_dataset)
 
     @exception_handler
-    def delete_list(self, list_name):
+    def delete_list(self, list_name: str) -> None:
         """Delete an aggregation list
 
         The key used to locate the aggregation list to be
         deleted may be formed by applying a prefix to the
         supplied name. See set_data_source()
         and use_list_ensemble_prefix() for more details.
 
@@ -1454,15 +1492,15 @@
         :raises RedisReplyError: if there is an error
                 in command execution.
         """
         typecheck(list_name, "list_name", str)
         self._client.delete_list(list_name)
 
     @exception_handler
-    def copy_list(self, src_name, dest_name):
+    def copy_list(self, src_name: str, dest_name: str) -> None:
         """Copy an aggregation list
 
         The source and destination aggregation list keys used to
         locate and store the aggregation list may be formed by
         applying prefixes to the supplied src_name and dest_name.
         See set_data_source() and use_list_ensemble_prefix()
         for more details.
@@ -1475,15 +1513,15 @@
                 in command execution.
         """
         typecheck(src_name, "src_name", str)
         typecheck(dest_name, "dest_name", str)
         self._client.copy_list(src_name, dest_name)
 
     @exception_handler
-    def rename_list(self, src_name, dest_name):
+    def rename_list(self, src_name: str, dest_name: str) -> None:
         """Rename an aggregation list
 
         The old and new aggregation list key used to find and
         relocate the list may be formed by applying prefixes to
         the supplied old_name and new_name. See set_data_source()
         and use_list_ensemble_prefix() for more details.
 
@@ -1495,29 +1533,31 @@
                 in command execution.
         """
         typecheck(src_name, "src_name", str)
         typecheck(dest_name, "dest_name", str)
         self._client.rename_list(src_name, dest_name)
 
     @exception_handler
-    def get_list_length(self, list_name):
+    def get_list_length(self, list_name: str) -> int:
         """Get the number of entries in the list
 
         :param list_name: The list name
         :type list_name: str
         :return: The length of the list
         :rtype: int
         :raises RedisReplyError: if there is an error
                 in command execution.
         """
         typecheck(list_name, "list_name", str)
         return self._client.get_list_length(list_name)
 
     @exception_handler
-    def poll_list_length(self, name, list_length, poll_frequency_ms, num_tries):
+    def poll_list_length(
+        self, name: str, list_length: int, poll_frequency_ms: int, num_tries: int
+    ) -> bool:
         """Poll list length until length is equal
         to the provided length.  If maximum number of
         attempts is exceeded, returns False
 
         The aggregation list key used to check for list length
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_list_ensemble_prefix()
@@ -1538,18 +1578,21 @@
                 in command execution.
         """
         typecheck(name, "name", str)
         typecheck(list_length, "list_length", int)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
         return self._client.poll_list_length(
-            name, list_length, poll_frequency_ms, num_tries)
+            name, list_length, poll_frequency_ms, num_tries
+        )
 
     @exception_handler
-    def poll_list_length_gte(self, name, list_length, poll_frequency_ms, num_tries):
+    def poll_list_length_gte(
+        self, name: str, list_length: int, poll_frequency_ms: int, num_tries: int
+    ) -> bool:
         """Poll list length until length is greater than or equal
         to the user-provided length. If maximum number of
         attempts is exceeded, false is returned.
 
         The aggregation list key used to check for list length
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_list_ensemble_prefix()
@@ -1570,18 +1613,21 @@
                 in command execution.
         """
         typecheck(name, "name", str)
         typecheck(list_length, "list_length", int)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
         return self._client.poll_list_length_gte(
-            name, list_length, poll_frequency_ms, num_tries)
+            name, list_length, poll_frequency_ms, num_tries
+        )
 
     @exception_handler
-    def poll_list_length_lte(self, name, list_length, poll_frequency_ms, num_tries):
+    def poll_list_length_lte(
+        self, name: str, list_length: int, poll_frequency_ms: int, num_tries: int
+    ) -> bool:
         """Poll list length until length is less than or equal
         to the user-provided length. If maximum number of
         attempts is exceeded, false is returned.
 
         The aggregation list key used to check for list length
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_list_ensemble_prefix()
@@ -1602,18 +1648,19 @@
                 in command execution.
         """
         typecheck(name, "name", str)
         typecheck(list_length, "list_length", int)
         typecheck(poll_frequency_ms, "poll_frequency_ms", int)
         typecheck(num_tries, "num_tries", int)
         return self._client.poll_list_length_lte(
-            name, list_length, poll_frequency_ms, num_tries)
+            name, list_length, poll_frequency_ms, num_tries
+        )
 
     @exception_handler
-    def get_datasets_from_list(self, list_name):
+    def get_datasets_from_list(self, list_name: str) -> t.List[Dataset]:
         """Get datasets from an aggregation list
 
         The aggregation list key used to retrieve datasets
         may be formed by applying a prefix to the supplied
         name. See set_data_source() and use_list_ensemble_prefix()
         for more details.  An empty or nonexistant
         aggregation list returns an empty vector.
@@ -1624,15 +1671,17 @@
         :rtype: list[DataSet]
         :raises RedisReplyError: if there is an error in command execution.
         """
         typecheck(list_name, "list_name", str)
         return self._client.get_datasets_from_list(list_name)
 
     @exception_handler
-    def get_dataset_list_range(self, list_name, start_index, end_index):
+    def get_dataset_list_range(
+        self, list_name: str, start_index: int, end_index: int
+    ) -> t.List[Dataset]:
         """Get a range of datasets (by index) from an aggregation list
 
         The aggregation list key used to retrieve datasets
         may be formed by applying a prefix to the supplied
         name. See set_data_source()  and use_list_ensemble_prefix()
         for more details.  An empty or nonexistant aggregation
         list returns an empty vector.  If the provided
@@ -1657,49 +1706,52 @@
         :return: A list of DataSet objects.
         :rtype: list[DataSet]
         :raises RedisReplyError: if there is an error in command execution.
         """
         typecheck(list_name, "list_name", str)
         typecheck(start_index, "start_index", int)
         typecheck(end_index, "end_index", int)
-        return self._client.get_dataset_list_range(
-            list_name, start_index, end_index)
+        return self._client.get_dataset_list_range(list_name, start_index, end_index)
 
     # ---- helpers --------------------------------------------------------
 
     @staticmethod
-    def __check_tensor_args(inputs, outputs):
+    def __check_tensor_args(
+        inputs: t.Optional[t.Union[t.List[str], str]],
+        outputs: t.Optional[t.Union[t.List[str], str]],
+    ) -> t.Tuple[t.List[str], t.List[str]]:
         inputs = init_default([], inputs, (list, str))
         outputs = init_default([], outputs, (list, str))
+        assert inputs is not None and outputs is not None
         if isinstance(inputs, str):
             inputs = [inputs]
         if isinstance(outputs, str):
             outputs = [outputs]
         return inputs, outputs
 
     @staticmethod
-    def __check_backend(backend):
+    def __check_backend(backend: str) -> str:
         backend = backend.upper()
         if backend in ["TF", "TFLITE", "TORCH", "ONNX"]:
             return backend
         else:
             raise TypeError(f"Backend type {backend} unsupported")
 
     @staticmethod
-    def __check_file(file):
+    def __check_file(file: str) -> str:
         file_path = osp.abspath(file)
         if not osp.isfile(file_path):
             raise FileNotFoundError(file_path)
         return file_path
 
     @staticmethod
-    def __check_device(device):
+    def __check_device(device: str) -> str:
         device = device.upper()
         if not device.startswith("CPU") and not device.startswith("GPU"):
             raise TypeError("Device argument must start with either CPU or GPU")
         return device
 
     @staticmethod
-    def __set_address(address):
+    def __set_address(address: str) -> None:
         if "SSDB" in os.environ:
             del os.environ["SSDB"]
         os.environ["SSDB"] = address
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis/dataset.py` & `smartredis-0.4.1/src/python/module/smartredis/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,111 +22,113 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from numbers import Number
 
+import typing as t
 import numpy as np
 
 from .smartredisPy import PyDataset
 from .srobject import SRObject
 from .util import Dtypes, exception_handler, typecheck
 
 from .error import *
 
+
 class Dataset(SRObject):
-    def __init__(self, name):
+    def __init__(self, name: str) -> None:
         """Initialize a Dataset object
 
         :param name: name of dataset
         :type name: str
         """
         super().__init__(PyDataset(name))
         typecheck(name, "name", str)
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Create a string representation of the client
 
         :return: A string representation of the client
         :rtype: str
         """
         return self._data.to_string()
 
     @property
-    def _data(self):
-        """Alias _srobject to _data
-        """
+    def _data(self) -> PyDataset:
+        """Alias _srobject to _data"""
+        assert isinstance(self._srobject, PyDataset)
         return self._srobject
 
     @staticmethod
-    def from_pybind(dataset):
+    def from_pybind(dataset: PyDataset) -> "Dataset":
         """Initialize a Dataset object from
         a PyDataset object
 
         :param dataset: The pybind PyDataset object
                         to use for construction
         :type dataset: PyDataset
-        :return: The newly constructor Dataset from
+        :return: The newly constructed Dataset from
                  the PyDataset
         :rtype: Dataset
         """
         typecheck(dataset, "dataset", PyDataset)
         new_dataset = Dataset(dataset.get_name())
         new_dataset.set_data(dataset)
         return new_dataset
 
     @exception_handler
-    def get_data(self):
+    def get_data(self) -> PyDataset:
         """Return the PyDataset attribute
 
         :return: The PyDataset attribute containing
                  the dataset information
         :rtype: PyDataset
         """
         return self._data
 
     @exception_handler
-    def set_data(self, dataset):
+    def set_data(self, dataset: PyDataset) -> None:
         """Set the PyDataset attribute
 
         :param dataset: The PyDataset object
         :type dataset: PyDataset
         """
         typecheck(dataset, "dataset", PyDataset)
         self._srobject = dataset
 
     @exception_handler
-    def add_tensor(self, name, data):
+    def add_tensor(self, name: str, data: np.ndarray) -> None:
         """Add a named tensor to this dataset
 
         :param name: tensor name
         :type name: str
         :param data: tensor data
-        :type data: np.array
+        :type data: np.ndarray
         """
         typecheck(name, "name", str)
         typecheck(data, "data", np.ndarray)
         dtype = Dtypes.tensor_from_numpy(data)
         self._data.add_tensor(name, data, dtype)
 
     @exception_handler
-    def get_tensor(self, name):
+    def get_tensor(self, name: str) -> np.ndarray:
         """Get a tensor from the Dataset
 
         :param name: name of the tensor to get
         :type name: str
         :return: a numpy array of tensor data
-        :rtype: np.array
+        :rtype: np.ndarray
         """
         typecheck(name, "name", str)
         return self._data.get_tensor(name)
 
     @exception_handler
-    def add_meta_scalar(self, name, data):
+    def add_meta_scalar(self, name: str, data: t.Union[int, float]) -> None:
         """Add metadata scalar field (non-string) with value to the DataSet
 
             If the field does not exist, it will be created.
             If the field exists, the value
             will be appended to existing field.
 
         :param name: The name used to reference the metadata
@@ -142,100 +144,101 @@
         if data_as_array.size > 1:
             raise TypeError("Argument provided is not a scalar")
         # We keep dtype, in case data has a non-standard python format
         dtype = Dtypes.metadata_from_numpy(data_as_array)
         self._data.add_meta_scalar(name, data_as_array, dtype)
 
     @exception_handler
-    def add_meta_string(self, name, data):
+    def add_meta_string(self, name: str, data: str) -> None:
         """Add metadata string field with value to the DataSet
 
         If the field does not exist, it will be created
         If the field exists the value will
         be appended to existing field.
 
-        :param name: The name used to reference the metadata
-                     field
+        :param name: The name used to reference the metadata field
         :type name: str
         :param data: The string to add to the field
         :type data: str
         """
         typecheck(name, "name", str)
         typecheck(data, "data", str)
         self._data.add_meta_string(name, data)
 
     @exception_handler
-    def get_meta_scalars(self, name):
+    def get_meta_scalars(self, name: str) -> t.Union[t.List[int], t.List[float]]:
         """Get the metadata scalar field values from the DataSet
 
         :param name: The name used to reference the metadata
                      field in the DataSet
         :type name: str
+        :rtype: list[int] | list[float]
         """
         typecheck(name, "name", str)
         return self._data.get_meta_scalars(name)
 
     @exception_handler
-    def get_meta_strings(self, name):
+    def get_meta_strings(self, name: str) -> t.List[str]:
         """Get the metadata scalar field values from the DataSet
 
         :param name: The name used to reference the metadata
-                        field in the DataSet
+                     field in the DataSet
         :type name: str
+        :rtype: list[str]
         """
         typecheck(name, "name", str)
         return self._data.get_meta_strings(name)
 
     @exception_handler
-    def get_metadata_field_names(self):
+    def get_metadata_field_names(self) -> t.List[str]:
         """Get the names of all metadata scalars and strings from the DataSet
 
         :return: a list of metadata field names
         :rtype: list[str]
         """
         return self._data.get_metadata_field_names()
 
     @exception_handler
-    def get_metadata_field_type(self, name):
+    def get_metadata_field_type(self, name: str) -> t.Type:
         """Get the names of all metadata scalars and strings from the DataSet
 
         :param name: The name used to reference the metadata
                      field in the DataSet
         :type name: str
         :return: the numpy type for the metadata field
         :rtype: type
         """
         typecheck(name, "name", str)
         type_str = self._data.get_metadata_field_type(name)
         return Dtypes.from_string(type_str)
 
     @exception_handler
-    def get_tensor_type(self, name):
+    def get_tensor_type(self, name: str) -> t.Type:
         """Get the type of a tensor in the DataSet
 
         :param name: The name used to reference the tensor in the DataSet
         :type name: str
         :return: the numpy type for the tensor
         :rtype: type
         """
         typecheck(name, "name", str)
         type_str = self._data.get_tensor_type(name)
         return Dtypes.from_string(type_str)
 
     @exception_handler
-    def get_tensor_names(self):
+    def get_tensor_names(self) -> t.List[str]:
         """Get the names of all tensors in the DataSet
 
         :return: a list of tensor names
         :rtype: list[str]
         """
         return self._data.get_tensor_names()
 
     @exception_handler
-    def get_tensor_dims(self, name):
+    def get_tensor_dims(self, name: str) -> t.List[int]:
         """Get the dimensions of a tensor in the DataSet
 
         :return: a list of the tensor dimensions
         :rtype: list[int]
         """
         typecheck(name, "name", str)
         return self._data.get_tensor_dims(name)
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis/dataset_utils.py` & `smartredis-0.4.1/src/python/module/smartredis/dataset_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,34 +21,41 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import functools
+import typing as t
 from typing import TYPE_CHECKING
 
 from .dataset import Dataset
 from .util import typecheck
 from itertools import permutations
 from .error import *
 
+
 if TYPE_CHECKING:  # pragma: no cover
     # Import optional deps for intellisense
     import xarray as xr
+
+    # Type hint magic bits
+    from typing_extensions import ParamSpec
+    _PR = ParamSpec("_PR")
+    _RT = t.TypeVar("_RT")
 else:
     # Leave optional deps as nullish
     xr = None
 
 # ----helper decorators -----
 
 
-def _requires_xarray(fn):
+def _requires_xarray(fn: "t.Callable[_PR, _RT]") -> "t.Callable[_PR, _RT]":
     @functools.wraps(fn)
-    def _import_xarray(*args, **kwargs):
+    def _import_xarray(*args: "_PR.args", **kwargs: "_PR.kwargs") -> "_RT":
         global xr
         try:
             import xarray as xr
         except ImportError as e:
             raise RedisRuntimeError(
                 "Optional package xarray must be installed; "
                 "Consider running `pip install smartredis[xarray]`"
@@ -57,32 +64,38 @@
 
     return _import_xarray
 
 
 # ----helper function -----
 
 
-def get_data(dataset, name, type):
-    return dataset.get_meta_strings(f"_xarray_{name}_{type}_names")[0].split(",")
+def get_data(dataset: Dataset, name: str, dtype: str) -> t.List[str]:
+    return dataset.get_meta_strings(f"_xarray_{name}_{dtype}_names")[0].split(",")
 
 
-def typecheck_stringlist(names, strings_name, string_name):
+def typecheck_stringlist(
+    names: t.List[str], strings_name: str, string_name: str
+) -> None:
     typecheck(names, strings_name, list)
     for name in names:
         typecheck(name, string_name, str)
         # Check if empty
         if string_name == "":
-            raise RedisRuntimeError
+            raise RedisRuntimeError("Empty string")
 
 
 class DatasetConverter:
     @staticmethod
     def add_metadata_for_xarray(
-        dataset, data_names, dim_names, coord_names=None, attr_names=None
-    ):
+        dataset: Dataset,
+        data_names: t.Union[t.List[str], str],
+        dim_names: t.Union[t.List[str], str],
+        coord_names: t.Optional[t.Union[t.List[str], str]] = None,
+        attr_names: t.Optional[t.Union[t.List[str], str]] = None,
+    ) -> None:
         """Extract metadata from a SmartRedis dataset and add it to
         dataformat specific fieldnames
 
         :param dataset: a Dataset instance
         :type dataset: Dataset
         :param data_names: variable data field name
         :type data_names: list[str] or str
@@ -90,21 +103,21 @@
         :type dim_names: list[str]
         :param coord_names: coordinate field names. Defaults to None.
         :type coord_names: list[str], optional
         :param attr_names: attribute field names. Defaults to None.
         :type attr_names: list[str], optional
         """
 
-        if type(data_names) == str:
+        if isinstance(data_names, str):
             data_names = [data_names]
-        if type(dim_names) == str:
+        if isinstance(dim_names, str):
             dim_names = [dim_names]
-        if type(coord_names) == str:
+        if isinstance(coord_names, str):
             coord_names = [coord_names]
-        if type(attr_names) == str:
+        if isinstance(attr_names, str):
             attr_names = [attr_names]
 
         typecheck(dataset, "dataset", Dataset)
         typecheck_stringlist(data_names, "data_names", "data_name")
         typecheck_stringlist(dim_names, "dim_names", "dim_name")
         if coord_names:
             typecheck_stringlist(coord_names, "coord_names", "coord_name")
@@ -112,30 +125,30 @@
             typecheck_stringlist(attr_names, "attr_names", "attr_name")
 
         args = [dim_names, coord_names, attr_names]
         sargs = ["dim_names", "coord_names", "attr_names"]
 
         for name in data_names:
             dataset.add_meta_string("_xarray_data_names", name)
-            for (arg, sarg) in zip(args, sargs):
+            for arg, sarg in zip(args, sargs):
                 if isinstance(arg, list):
                     values = []
                     for val in arg:
                         values.append(val)
                     arg_field = ",".join(values)
                     dataset.add_meta_string(f"_xarray_{name}_{sarg}", arg_field)
                 else:
                     if arg:
                         dataset.add_meta_string(f"_xarray_{name}_{sarg}", arg)
                     else:
                         dataset.add_meta_string(f"_xarray_{name}_{sarg}", "null")
 
     @staticmethod
     @_requires_xarray
-    def transform_to_xarray(dataset):
+    def transform_to_xarray(dataset: Dataset) -> t.Dict:
         """Transform a SmartRedis Dataset, with the appropriate metadata,
         to an Xarray Dataarray
 
         :param dataset: a Dataset instance
         :type dataset: Dataset
 
         :return: a dictionary of keys as the data field name and the
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis/error.py` & `smartredis-0.4.1/src/python/module/smartredis/error.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,63 +22,77 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from os import environ
 
-__all__ = ['RedisConnectionError', 'RedisReplyError', 'RedisRuntimeError',
-           'RedisBadAllocError', 'RedisDatabaseError', 'RedisInternalError',
-           'RedisTimeoutError', 'RedisKeyError']
+__all__ = [
+    "RedisConnectionError",
+    "RedisReplyError",
+    "RedisRuntimeError",
+    "RedisBadAllocError",
+    "RedisDatabaseError",
+    "RedisInternalError",
+    "RedisTimeoutError",
+    "RedisKeyError",
+]
+
 
 class RedisConnectionError(RuntimeError):
-    def __init__(self, cpp_error=""):
+    def __init__(self, cpp_error: str = "") -> None:
         super().__init__(self._set_message(cpp_error))
 
     @staticmethod
-    def _set_message(cpp_error):
+    def _set_message(cpp_error: str) -> str:
         msg = ""
         if cpp_error:
             msg = cpp_error + "\n"
         if "SSDB" in environ:
             msg += f"Could not connect to Orchestrator at {environ['SSDB']}"
         return msg
 
 
 class RedisReplyError(RuntimeError):
-    def __init__(self, cpp_error, method="", key=""):
+    def __init__(self, cpp_error: str, method: str = "", key: str = "") -> None:
         super().__init__(self._check_error(cpp_error, method, key))
 
     @staticmethod
-    def _check_error(cpp_error, method="", key=""):
+    def _check_error(cpp_error: str, method: str = "", key: str = "") -> str:
         msg = ""
         if method:
             msg = f"{method} execution failed\n"
         msg += cpp_error
         return msg
 
+
 class RedisRuntimeError(RedisReplyError):
     @staticmethod
-    def _check_error(cpp_error, method="", key=""):
+    def _check_error(cpp_error: str, method: str = "", key: str = "") -> str:
         msg = ""
         if method:
             msg = f"{method} execution failed\n"
         if "REDIS_REPLY_NIL" in cpp_error:
             msg += f"No Dataset stored at key: {key}"
             return msg
         msg += cpp_error
         return msg
 
+
 class RedisBadAllocError(RedisReplyError):
     pass
 
+
 class RedisDatabaseError(RedisReplyError):
     pass
 
+
 class RedisInternalError(RedisReplyError):
     pass
 
+
 class RedisTimeoutError(RedisReplyError):
     pass
 
+
 class RedisKeyError(RedisReplyError):
     pass
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis/logcontext.py` & `smartredis-0.4.1/src/python/module/smartredis/logcontext.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,36 +23,36 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from .smartredisPy import PyLogContext
 from .srobject import SRObject
 from .util import exception_handler, typecheck
-
 from .error import *
+import typing as t
+
 
 class LogContext(SRObject):
-    def __init__(self, context):
+    def __init__(self, context: str) -> None:
         """Initialize a LogContext object
 
         :param context: logging context
         :type name: str
         """
         super().__init__(PyLogContext(context))
         typecheck(context, "context", str)
         self._name = context
 
     @property
-    def _logcontext(self):
-        """Alias _srobject to _logcontext
-        """
+    def _logcontext(self) -> PyLogContext:
+        """Alias _srobject to _logcontext"""
         return self._srobject
 
     @staticmethod
-    def from_pybind(logcontext):
+    def from_pybind(logcontext: PyLogContext) -> "LogContext":
         """Initialize a LogContext object from
         a PyLogContext object
 
         :param logcontext: The pybind PyLogContext object
                            to use for construction
         :type logcontext: PyLogContext
         :return: The newly constructor LogContext from
@@ -61,25 +61,25 @@
         """
         typecheck(logcontext, "logcontext", PyLogContext)
         new_logcontext = LogContext(logcontext._name)
         new_logcontext.set_context(logcontext)
         return new_logcontext
 
     @exception_handler
-    def get_context(self):
+    def get_context(self) -> PyLogContext:
         """Return the PyLogContext attribute
 
         :return: The PyLogContext attribute containing
                  the logcontext information
         :rtype: PyLogContext
         """
         return self._logcontext
 
     @exception_handler
-    def set_context(self, logcontext):
+    def set_context(self, logcontext: PyLogContext) -> None:
         """Set the PyLogContext attribute
 
         :param logcontext: The PyLogContext object
         :type logcontext: PyLogContext
         """
         typecheck(logcontext, "logcontext", PyLogContext)
         self._srobject = logcontext
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis/logger.py` & `smartredis-0.4.1/src/python/module/smartredis/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,21 +24,22 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from .smartredisPy import cpp_log_data, cpp_log_warning, cpp_log_error, SRLoggingLevel
 from .util import exception_handler, typecheck
 
 # Logging levels
-#LLQuiet     = 1  # No logging at all
-#LLInfo      = 2  # Informational logging only
-#LLDebug     = 3  # Verbose logging for debugging purposes
-#LLDeveloper = 4  # Extra verbose logging for internal use
+# LLQuiet     = 1  # No logging at all
+# LLInfo      = 2  # Informational logging only
+# LLDebug     = 3  # Verbose logging for debugging purposes
+# LLDeveloper = 4  # Extra verbose logging for internal use
+
 
 @exception_handler
-def log_data(context, level, data):
+def log_data(context: str, level: SRLoggingLevel, data: str) -> None:
     """Log data to the SmartRedis logfile
 
     :param context: Logging context (string to prefix the log entry with)
     :type context: str
     :param level: minimum logging level for data to be logged with
     :type name: enum
     :param data: message data to log
@@ -46,16 +47,17 @@
     :raises RedisReplyError: if logging fails
     """
     typecheck(context, "context", str)
     typecheck(level, "level", SRLoggingLevel)
     typecheck(data, "data", str)
     cpp_log_data(context, level, data)
 
+
 @exception_handler
-def log_warning(context, level, data):
+def log_warning(context: str, level: SRLoggingLevel, data: str) -> None:
     """Log a warning to the SmartRedis logfile
 
     :param context: Logging context (string to prefix the log entry with)
     :type context: str
     :param level: minimum logging level for data to be logged with
     :type name: enum
     :param data: message data to log
@@ -63,24 +65,24 @@
     :raises RedisReplyError: if logging fails
     """
     typecheck(context, "context", str)
     typecheck(level, "level", SRLoggingLevel)
     typecheck(data, "data", str)
     cpp_log_warning(context, level, data)
 
+
 @exception_handler
-def log_error(context, level, data):
+def log_error(context: str, level: SRLoggingLevel, data: str) -> None:
     """Log an error to the SmartRedis logfile
 
     :param context: Logging context (string to prefix the log entry with)
     :type context: str
     :param level: minimum logging level for data to be logged with
     :type name: enum
     :param data: message data to log
     :type data: str
     :raises RedisReplyError: if logging fails
     """
     typecheck(context, "context", str)
     typecheck(level, "level", SRLoggingLevel)
     typecheck(data, "data", str)
     cpp_log_error(context, level, data)
-
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis/srobject.py` & `smartredis-0.4.1/src/python/module/smartredis/srobject.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,92 +25,78 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from .smartredisPy import PySRObject, SRLoggingLevel
 from .util import exception_handler, typecheck
 
 from .error import *
 
+
 class SRObject:
-    def __init__(self, context):
+    def __init__(self, context: str) -> None:
         """Initialize a SRObject object
 
         :param context: logging context
         :type name: str
         """
         typecheck(context, "context", (str, PySRObject))
         if isinstance(context, str):
             self._name = context
             self._srobject = PySRObject(context)
         else:
             self._srobject = context
 
-    @staticmethod
-    def from_pybind(srobject):
-        """Initialize a SRObject object from
-        a PySRObject object
-
-        :param srobject: The pybind PySRObject object to use for construction
-        :type srobject: PySRObject
-        :return: The newly constructed¸ SRObject from the PySRObject
-        :rtype: SRObject
-        """
-        typecheck(srobject, "srobject", PySRObject)
-        new_srobject = SRObject(srobject._name)
-        new_srobject.set_data(srobject)
-        return new_srobject
-
     @exception_handler
-    def get_srobject(self):
+    def get_srobject(self) -> PySRObject:
         """Return the PySRObject attribute
 
         :return: The PySRObject attribute containing the srobject information
         :rtype: PySRObject
         """
         return self._srobject
 
     @exception_handler
-    def set_srobject(self, srobject):
+    def set_srobject(self, srobject: PySRObject) -> None:
         """Set the PySRObject attribute
 
         :param srobject: The PySRObject object
         :type srobject: PySRObject
         """
         typecheck(srobject, "srobject", PySRObject)
         self._srobject = srobject
 
     @exception_handler
-    def log_data(self, level, data):
+    def log_data(self, level: SRLoggingLevel, data: str) -> None:
         """Conditionally log data if the logging level is high enough
 
         :param level: Minimum logging level for data to be logged
         :type name: enum
         :param data: Text of data to be logged
         :type name: str
         :raises RedisReplyError: if logging fails
         """
         typecheck(level, "level", SRLoggingLevel)
         typecheck(data, "data", str)
         self._srobject.log_data(level, data)
 
     @exception_handler
-    def log_warning(self, level, data):
+    def log_warning(self, level: SRLoggingLevel, data: str) -> None:
         """Conditionally log warning data if the logging level is high enough
 
         :param level: Minimum logging level for data to be logged
         :type name: enum
         :param data: Text of data to be logged
         :type name: str
         :raises RedisReplyError: if logging fails
         """
         typecheck(level, "level", SRLoggingLevel)
         typecheck(data, "data", str)
         self._srobject.log_warning(level, data)
 
     @exception_handler
-    def log_error(self, level, data):
+    def log_error(self, level: SRLoggingLevel, data: str) -> None:
         """Conditionally log error data if the logging level is high enough
 
         :param level: Minimum logging level for data to be logged
         :type name: enum
         :param data: Text of data to be logged
         :type name: str
         :raises RedisReplyError: if logging fails
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis/util.py` & `smartredis-0.4.1/src/python/module/smartredis/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,18 +25,26 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from .error import *
 from functools import wraps
 from .smartredisPy import RedisReplyError as PybindRedisReplyError
 from .smartredisPy import c_get_last_error_location
 import numpy as np
+import typing as t
+
+if t.TYPE_CHECKING:
+    # Type hint magic bits
+    from typing_extensions import ParamSpec
+    _PR = ParamSpec("_PR")
+    _RT = t.TypeVar("_RT")
+
 
 class Dtypes:
     @staticmethod
-    def tensor_from_numpy(array):
+    def tensor_from_numpy(array: np.ndarray) -> str:
         mapping = {
             "float64": "DOUBLE",
             "float32": "FLOAT",
             "uint8": "UINT8",
             "uint16": "UINT16",
             "int8": "INT8",
             "int16": "INT16",
@@ -45,95 +53,116 @@
         }
         dtype = str(array.dtype)
         if dtype in mapping:
             return mapping[dtype]
         raise TypeError(f"Incompatible tensor type provided {dtype}")
 
     @staticmethod
-    def metadata_from_numpy(array):
+    def metadata_from_numpy(array: np.ndarray) -> str:
         mapping = {
             "float64": "DOUBLE",
             "float32": "FLOAT",
             "uint32": "UINT32",
             "uint64": "UINT64",
             "int32": "INT32",
             "int64": "INT64",
         }
         dtype = str(array.dtype)
         if dtype in mapping:
             return mapping[dtype]
         raise TypeError(f"Incompatible metadata type provided {dtype}")
 
     @staticmethod
-    def from_string(type_name):
+    def from_string(type_name: str) -> t.Type:
         mapping = {
             "DOUBLE": np.double,
-            "FLOAT":  np.float64,
-            "UINT8":  np.uint8,
+            "FLOAT": np.float64,
+            "UINT8": np.uint8,
             "UINT16": np.uint16,
             "UINT32": np.uint32,
             "UINT64": np.uint64,
-            "INT8":   np.int8,
-            "INT16":  np.int16,
-            "INT32":  np.int32,
-            "INT64":  np.int64,
+            "INT8": np.int8,
+            "INT16": np.int16,
+            "INT32": np.int32,
+            "INT64": np.int64,
             "STRING": str,
         }
         if type_name in mapping:
             return mapping[type_name]
         raise TypeError(f"Unrecognized type name {type_name}")
 
-def init_default(default, init_value, expected_type=None):
+
+def init_default(
+    default: t.Any, init_value: t.Any, expected_type: t.Optional[t.Any] = None
+) -> t.Any:
     """Used for setting a mutable type to a default value.
 
     PEP standards forbid setting a default value to a mutable type
     Use this function to get around that.
     """
     if init_value is None:
         return default
     if expected_type is not None and not isinstance(init_value, expected_type):
         raise TypeError(f"Argument was of type {type(init_value)}, not {expected_type}")
     return init_value
 
-def exception_handler(func):
+
+def exception_handler(func: "t.Callable[_PR, _RT]") -> "t.Callable[_PR, _RT]":
     """Route exceptions raised in processing SmartRedis API calls to our
     Python wrappers
 
+    WARNING: using this decorator with a class' @staticmethod or with an
+    unbound function that takes a type as its first argument will fail
+    because that will make the decorator think it's working with a
+    @classmethod
+
     :param func: the API function to decorate with this wrapper
     :type func: function
     :raises RedisReplyError: if the wrapped function raised an exception
     """
+
     @wraps(func)
-    def smartredis_api_wrapper(*args, **kwargs):
+    def smartredis_api_wrapper(*args: "_PR.args", **kwargs: "_PR.kwargs") -> "_RT":
         try:
             return func(*args, **kwargs)
         # Catch RedisReplyErrors for additional processing (convert from
         # pyerror to our error module).
         # TypeErrors and ValueErrors we pass straight through
         except PybindRedisReplyError as cpp_error:
-            # query args[0] (i.e. 'self') for the class name
-            method_name = args[0].__class__.__name__ + "." + func.__name__
+            # get the class for the calling context.
+            # for a @classmethod, this will be args[0], but for
+            # a "normal" method, args[0] is a self pointer from
+            # which we can grab the __class__ attribute
+            src_class = args[0]
+            if not isinstance(src_class, type):
+                src_class = args[0].__class__
+            # Build the fully specified name of the calling context
+            method_name = src_class.__name__ + "." + func.__name__
             # Get our exception from the global symbol table.
             # The smartredis.error hierarchy exactly
             # parallels the one built via pybind to enable this
             exception_name = cpp_error.__class__.__name__
             error_loc = c_get_last_error_location()
             if error_loc == "unavailable":
                 cpp_error_str = str(cpp_error)
             else:
-                cpp_error_str = f"File {error_loc}, in SmartRedis library\n{str(cpp_error)}"
+                cpp_error_str = (
+                    f"File {error_loc}, in SmartRedis library\n{str(cpp_error)}"
+                )
             raise globals()[exception_name](cpp_error_str, method_name) from None
+
     return smartredis_api_wrapper
 
-def typecheck(arg, name, _type):
+
+def typecheck(arg: t.Any, name: str, _type: t.Union[t.Tuple, type]) -> None:
     """Validate that an argument is of a given type
 
     :param arg: the variable to be type tested
     :type arg: variable, expected to match _type
     :param name: the name of the variable
     :type name: str
     :param _type: the expected type for the variable
     :type _type: a Python type
     :raises TypeError exception if arg is not of type _type
     """
     if not isinstance(arg, _type):
-        raise TypeError(f"Argument {name} is of type {type(arg)}, not {_type}")
+        raise TypeError(f"Argument {name} is of type {type(arg)}, not {_type}")
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis.egg-info/PKG-INFO` & `smartredis-0.4.1/src/python/module/smartredis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartredis
-Version: 0.4.0
+Version: 0.4.1
 Summary: RedisAI clients for SmartSim
 Home-page: https://github.com/CrayLabs/SmartRedis
 Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
 Author-email: craylabs@hpe.com
 License: BSD 2-Clause License
 Project-URL: Source, https://github.com/CrayLabs/SmartRedis
 Project-URL: Documentation, https://www.craylabs.org
@@ -38,20 +38,20 @@
         # SmartRedis
         
         SmartRedis is a collection of Redis clients that support
         RedisAI capabilities and include additional
         features for high performance computing (HPC) applications.
         SmartRedis provides clients in the following languages:
         
-        | Language   | Version/Standard  |
-        |------------|:-----------------:|
-        | Python     |   3.7, 3.8, 3.9   |
-        | C++        |   C++17           |
-        | C          |   C99             |
-        | Fortran    |   Fortran 2018    |
+        | Language   | Version/Standard                               |
+        |------------|:----------------------------------------------:|
+        | Python     |   3.7, 3.8, 3.9, 3.10                          |
+        | C++        |   C++17                                        |
+        | C          |   C99                                          |
+        | Fortran    |   Fortran 2018 (GNU/Intel), 2003 (PGI/Nvidia)  |
         
         SmartRedis is used in the [SmartSim library](https://github.com/CrayLabs/SmartSim).
         SmartSim makes it easier to use common Machine Learning (ML) libraries like
         PyTorch and TensorFlow in numerical simulations at scale.  SmartRedis connects
         these simulations to a Redis database or Redis database cluster for
         data storage, script execution, and model evaluation.  While SmartRedis
         contains features for simulation workflows on supercomputers, SmartRedis
@@ -63,54 +63,60 @@
         SmartRedis installation instructions are currently hosted as part of the
         [SmartSim library installation instructions](https://www.craylabs.org/docs/installation.html#smartredis)
         Additionally, detailed [API documents](https://www.craylabs.org/docs/api/smartredis_api.html) are also available as
         part of the SmartSim documentation.
         
         ## Dependencies
         
-        SmartRedis utilizes the following libraries.
+        SmartRedis utilizes the following libraries:
         
          - [NumPy](https://github.com/numpy/numpy)
-         - [Hiredis](https://github.com/redis/hiredis) 1.0.0
-         - [Redis-plus-plus](https://github.com/sewenew/redis-plus-plus)  1.2.3
+         - [Hiredis](https://github.com/redis/hiredis) 1.1.0
+         - [Redis-plus-plus](https://github.com/sewenew/redis-plus-plus) 1.3.5
         
         ## Publications
         
         The following are public presentations or publications using SmartRedis
         
          - [Collaboration with NCAR - CGD Seminar](https://www.youtube.com/watch?v=2e-5j427AS0)
-         - [Using Machine Learning in HPC Simulations - paper (pre-print)](https://arxiv.org/abs/2104.09355)
+         - [Using Machine Learning in HPC Simulations - paper](https://www.sciencedirect.com/science/article/pii/S1877750322001065)
+         - [Relexi — A scalable open source reinforcement learning framework for high-performance computing - paper](https://www.sciencedirect.com/science/article/pii/S2665963822001063)
         
         ## Cite
         
-        Please use the following citation when referencing SmartSim, SmartRedis, or any SmartSim related work.
+        Please use the following citation when referencing SmartSim, SmartRedis, or any SmartSim related work:
         
-        
-        Partee et al., “Using Machine Learning at Scale in HPC Simulations with SmartSim:
-        An Application to Ocean Climate Modeling,” arXiv:2104.09355, Apr. 2021,
-        [Online]. Available: http://arxiv.org/abs/2104.09355.
+            Partee et al., "Using Machine Learning at scale in numerical simulations with SmartSim:
+            An application to ocean climate modeling",
+            Journal of Computational Science, Volume 62, 2022, 101707, ISSN 1877-7503.
+            Open Access: https://doi.org/10.1016/j.jocs.2022.101707.
         
         ### bibtex
         
-            ```latex
-            @misc{partee2021using,
-                  title={Using Machine Learning at Scale in HPC Simulations with SmartSim: An Application to Ocean Climate Modeling},
-                  author={Sam Partee and Matthew Ellis and Alessandro Rigazzi and Scott Bachman and Gustavo Marques and Andrew Shao and Benjamin Robbins},
-                  year={2021},
-                  eprint={2104.09355},
-                  archivePrefix={arXiv},
-                  primaryClass={cs.CE}
-            }
-            ```
+            @article{PARTEE2022101707,
+                title = {Using Machine Learning at scale in numerical simulations with SmartSim:
+                An application to ocean climate modeling},
+                journal = {Journal of Computational Science},
+                volume = {62},
+                pages = {101707},
+                year = {2022},
+                issn = {1877-7503},
+                doi = {https://doi.org/10.1016/j.jocs.2022.101707},
+                url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
+                author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E. Shao
+                and Scott Bachman and Gustavo Marques and Benjamin Robbins},
+                keywords = {Deep learning, Numerical simulation, Climate modeling, High performance computing, SmartSim},
+                }
         
 Keywords: redis,clients,hpc,ai,deep learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartredis Version: 0.4.0 Summary: RedisAI clients
+Metadata-Version: 2.1 Name: smartredis Version: 0.4.1 Summary: RedisAI clients
 for SmartSim Home-page: https://github.com/CrayLabs/SmartRedis Author:
 CrayLabs, a Hewlett Packard Enterprise OSS Organization Author-email:
 craylabs@hpe.com License: BSD 2-Clause License Project-URL: Source, https://
 github.com/CrayLabs/SmartRedis Project-URL: Documentation, https://
 www.craylabs.org Description:
     [https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/
                           SmartSim_Large.png][Image]
@@ -20,43 +20,52 @@
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![codecov](https://codecov.io/gh/CrayLabs/SmartRedis/
 branch/develop/graph/badge.svg?token=XSS8CCJ2KR)](https://codecov.io/gh/
 CrayLabs/SmartRedis) ---------- # SmartRedis SmartRedis is a collection of
 Redis clients that support RedisAI capabilities and include additional features
 for high performance computing (HPC) applications. SmartRedis provides clients
 in the following languages: | Language | Version/Standard | |------------|:----
--------------:| | Python | 3.7, 3.8, 3.9 | | C++ | C++17 | | C | C99 | |
-Fortran | Fortran 2018 | SmartRedis is used in the [SmartSim library](https://
-github.com/CrayLabs/SmartSim). SmartSim makes it easier to use common Machine
-Learning (ML) libraries like PyTorch and TensorFlow in numerical simulations at
-scale. SmartRedis connects these simulations to a Redis database or Redis
-database cluster for data storage, script execution, and model evaluation.
-While SmartRedis contains features for simulation workflows on supercomputers,
+------------------------------------------:| | Python | 3.7, 3.8, 3.9, 3.10 | |
+C++ | C++17 | | C | C99 | | Fortran | Fortran 2018 (GNU/Intel), 2003 (PGI/
+Nvidia) | SmartRedis is used in the [SmartSim library](https://github.com/
+CrayLabs/SmartSim). SmartSim makes it easier to use common Machine Learning
+(ML) libraries like PyTorch and TensorFlow in numerical simulations at scale.
+SmartRedis connects these simulations to a Redis database or Redis database
+cluster for data storage, script execution, and model evaluation. While
+SmartRedis contains features for simulation workflows on supercomputers,
 SmartRedis is fully functional as a RedisAI client library and can be used
 without SmartSim in any Python, C++, C, or Fortran project. ## Using SmartRedis
 SmartRedis installation instructions are currently hosted as part of the
 [SmartSim library installation instructions](https://www.craylabs.org/docs/
 installation.html#smartredis) Additionally, detailed [API documents](https://
 www.craylabs.org/docs/api/smartredis_api.html) are also available as part of
 the SmartSim documentation. ## Dependencies SmartRedis utilizes the following
-libraries. - [NumPy](https://github.com/numpy/numpy) - [Hiredis](https://
-github.com/redis/hiredis) 1.0.0 - [Redis-plus-plus](https://github.com/sewenew/
-redis-plus-plus) 1.2.3 ## Publications The following are public presentations
+libraries: - [NumPy](https://github.com/numpy/numpy) - [Hiredis](https://
+github.com/redis/hiredis) 1.1.0 - [Redis-plus-plus](https://github.com/sewenew/
+redis-plus-plus) 1.3.5 ## Publications The following are public presentations
 or publications using SmartRedis - [Collaboration with NCAR - CGD Seminar]
 (https://www.youtube.com/watch?v=2e-5j427AS0) - [Using Machine Learning in HPC
-Simulations - paper (pre-print)](https://arxiv.org/abs/2104.09355) ## Cite
-Please use the following citation when referencing SmartSim, SmartRedis, or any
-SmartSim related work. Partee et al., âUsing Machine Learning at Scale in HPC
-Simulations with SmartSim: An Application to Ocean Climate Modeling,â arXiv:
-2104.09355, Apr. 2021, [Online]. Available: http://arxiv.org/abs/2104.09355.
-### bibtex ```latex @misc{partee2021using, title={Using Machine Learning at
-Scale in HPC Simulations with SmartSim: An Application to Ocean Climate
-Modeling}, author={Sam Partee and Matthew Ellis and Alessandro Rigazzi and
-Scott Bachman and Gustavo Marques and Andrew Shao and Benjamin Robbins}, year=
-{2021}, eprint={2104.09355}, archivePrefix={arXiv}, primaryClass={cs.CE} } ```
-Keywords: redis,clients,hpc,ai,deep learning Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Simulations - paper](https://www.sciencedirect.com/science/article/pii/
+S1877750322001065) - [Relexi â A scalable open source reinforcement learning
+framework for high-performance computing - paper](https://
+www.sciencedirect.com/science/article/pii/S2665963822001063) ## Cite Please use
+the following citation when referencing SmartSim, SmartRedis, or any SmartSim
+related work: Partee et al., "Using Machine Learning at scale in numerical
+simulations with SmartSim: An application to ocean climate modeling", Journal
+of Computational Science, Volume 62, 2022, 101707, ISSN 1877-7503. Open Access:
+https://doi.org/10.1016/j.jocs.2022.101707. ### bibtex @article
+{PARTEE2022101707, title = {Using Machine Learning at scale in numerical
+simulations with SmartSim: An application to ocean climate modeling}, journal =
+{Journal of Computational Science}, volume = {62}, pages = {101707}, year =
+{2022}, issn = {1877-7503}, doi = {https://doi.org/10.1016/j.jocs.2022.101707},
+url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
+author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E.
+Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins}, keywords =
+{Deep learning, Numerical simulation, Climate modeling, High performance
+computing, SmartSim}, } Keywords: redis,clients,hpc,ai,deep learning Platform:
+UNKNOWN Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 License :: OSI Approved :: BSD License Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Scientific/Engineering Requires-Python:
 <3.11,>=3.7 Description-Content-Type: text/markdown Provides-Extra: dev
 Provides-Extra: doc Provides-Extra: xarray
```

### Comparing `smartredis-0.4.0/src/python/module/smartredis.egg-info/SOURCES.txt` & `smartredis-0.4.1/src/python/module/smartredis.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Makefile
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
+smartredis_defs.cmake
 build-scripts/build-catch.sh
 build-scripts/build-keydb.sh
 build-scripts/build-lcov.sh
 build-scripts/build-redis.sh
 build-scripts/build-redisai-cpu.sh
 build-scripts/build-redisai-gpu.sh
 build-scripts/build_c_tests.sh
@@ -24,25 +25,27 @@
 build-scripts/build_serial_examples.sh
 build-scripts/build_test_deps.sh
 include/address.h
 include/addressallcommand.h
 include/addressanycommand.h
 include/addressatcommand.h
 include/c_client.h
+include/c_configoptions.h
 include/c_dataset.h
 include/c_logcontext.h
 include/c_logger.h
 include/client.h
 include/clusterinfocommand.h
 include/command.h
 include/command.tcc
 include/commandlist.h
 include/commandlist.tcc
 include/commandreply.h
 include/compoundcommand.h
+include/configoptions.h
 include/dataset.h
 include/dbinfocommand.h
 include/dbnode.h
 include/enum_fortran.inc
 include/gettensorcommand.h
 include/keyedcommand.h
 include/logcontext.h
@@ -50,14 +53,15 @@
 include/metadata.h
 include/metadatabuffer.h
 include/metadatafield.h
 include/multikeycommand.h
 include/nonkeyedcommand.h
 include/pipelinereply.h
 include/pyclient.h
+include/pyconfigoptions.h
 include/pydataset.h
 include/pylogcontext.h
 include/pysrobject.h
 include/redis.h
 include/rediscluster.h
 include/redisserver.h
 include/scalarfield.h
@@ -73,28 +77,30 @@
 include/tensor.h
 include/tensor.tcc
 include/tensorbase.h
 include/tensorpack.h
 include/threadpool.h
 include/utility.h
 src/c/c_client.cpp
+src/c/c_configoptions.cpp
 src/c/c_dataset.cpp
 src/c/c_error.cpp
 src/c/c_logcontext.cpp
 src/c/c_logger.cpp
 src/cpp/address.cpp
 src/cpp/addressallcommand.cpp
 src/cpp/addressanycommand.cpp
 src/cpp/addressatcommand.cpp
 src/cpp/client.cpp
 src/cpp/clusterinfocommand.cpp
 src/cpp/command.cpp
 src/cpp/commandlist.cpp
 src/cpp/commandreply.cpp
 src/cpp/compoundcommand.cpp
+src/cpp/configoptions.cpp
 src/cpp/dataset.cpp
 src/cpp/dbinfocommand.cpp
 src/cpp/dbnode.cpp
 src/cpp/gettensorcommand.cpp
 src/cpp/keyedcommand.cpp
 src/cpp/logger.cpp
 src/cpp/metadata.cpp
@@ -109,14 +115,15 @@
 src/cpp/srobject.cpp
 src/cpp/stringfield.cpp
 src/cpp/tensorbase.cpp
 src/cpp/tensorpack.cpp
 src/cpp/threadpool.cpp
 src/cpp/utility.cpp
 src/fortran/client.F90
+src/fortran/configoptions.F90
 src/fortran/dataset.F90
 src/fortran/errors.F90
 src/fortran/fortran_c_interop.F90
 src/fortran/logcontext.F90
 src/fortran/logger.F90
 src/fortran/client/aggregation_interfaces.inc
 src/fortran/client/client_dataset_interfaces.inc
@@ -125,42 +132,46 @@
 src/fortran/client/misc_tensor_interfaces.inc
 src/fortran/client/model_interfaces.inc
 src/fortran/client/put_tensor_interfaces.inc
 src/fortran/client/put_tensor_methods_common.inc
 src/fortran/client/script_interfaces.inc
 src/fortran/client/unpack_tensor_interfaces.inc
 src/fortran/client/unpack_tensor_methods_common.inc
+src/fortran/configoptions/configoptions_interfaces.inc
 src/fortran/dataset/add_meta_scalar_common.inc
 src/fortran/dataset/add_tensor_methods_common.inc
 src/fortran/dataset/dataset_interfaces.inc
 src/fortran/dataset/get_meta_scalars_common.inc
 src/fortran/dataset/metadata_interfaces.inc
 src/fortran/dataset/tensor_interfaces.inc
 src/fortran/dataset/unpack_dataset_tensor_interfaces.inc
 src/fortran/dataset/unpack_dataset_tensor_methods_common.inc
 src/fortran/errors/errors_interfaces.inc
 src/fortran/logcontext/logcontext_interfaces.inc
 src/fortran/logger/logger_interfaces.inc
 src/python/bindings/bind.cpp
 src/python/module/smartredis/__init__.py
 src/python/module/smartredis/client.py
+src/python/module/smartredis/configoptions.py
 src/python/module/smartredis/dataset.py
 src/python/module/smartredis/dataset_utils.py
 src/python/module/smartredis/error.py
 src/python/module/smartredis/logcontext.py
 src/python/module/smartredis/logger.py
 src/python/module/smartredis/srobject.py
 src/python/module/smartredis/util.py
 src/python/module/smartredis.egg-info/PKG-INFO
 src/python/module/smartredis.egg-info/SOURCES.txt
 src/python/module/smartredis.egg-info/dependency_links.txt
 src/python/module/smartredis.egg-info/not-zip-safe
 src/python/module/smartredis.egg-info/requires.txt
 src/python/module/smartredis.egg-info/top_level.txt
 src/python/src/pyclient.cpp
+src/python/src/pyconfigoptions.cpp
 src/python/src/pydataset.cpp
 src/python/src/pylogcontext.cpp
 src/python/src/pysrobject.cpp
 utils/check_redis.sh
+utils/launch_redis.py
 utils/create_cluster/local_cluster.py
 utils/create_cluster/slurm_cluster.py
 utils/create_cluster/smartredisdb.conf
```

### Comparing `smartredis-0.4.0/src/python/src/pyclient.cpp` & `smartredis-0.4.1/src/python/src/pyclient.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,14 @@
         _client->rename_tensor(old_name, new_name);
     });
 }
 
 void PyClient::put_dataset(PyDataset& dataset)
 {
     MAKE_CLIENT_API({
-        std::cout << "Got the dataset" << std::endl;
         _client->put_dataset(*(dataset.get()));
     });
 }
 
 PyDataset* PyClient::get_dataset(const std::string& name)
 {
     return MAKE_CLIENT_API({
```

### Comparing `smartredis-0.4.0/src/python/src/pydataset.cpp` & `smartredis-0.4.1/src/python/src/pydataset.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/python/src/pylogcontext.cpp` & `smartredis-0.4.1/src/python/src/pylogcontext.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/src/python/src/pysrobject.cpp` & `smartredis-0.4.1/src/python/src/pysrobject.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/utils/check_redis.sh` & `smartredis-0.4.1/utils/check_redis.sh`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/utils/create_cluster/local_cluster.py` & `smartredis-0.4.1/utils/create_cluster/local_cluster.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/utils/create_cluster/slurm_cluster.py` & `smartredis-0.4.1/utils/create_cluster/slurm_cluster.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.4.0/utils/create_cluster/smartredisdb.conf` & `smartredis-0.4.1/utils/create_cluster/smartredisdb.conf`

 * *Files identical despite different names*

