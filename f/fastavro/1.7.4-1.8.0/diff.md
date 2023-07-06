# Comparing `tmp/fastavro-1.7.4.tar.gz` & `tmp/fastavro-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastavro-1.7.4.tar", last modified: Thu May  4 15:54:08 2023, max compression
+gzip compressed data, was "fastavro-1.8.0.tar", last modified: Thu Jul  6 15:53:50 2023, max compression
```

## Comparing `fastavro-1.7.4.tar` & `fastavro-1.8.0.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.976793 fastavro-1.7.4/
--rwxr-xr-x   0 sbelden    (501) staff       (20)     1625 2019-05-08 02:19:05.000000 fastavro-1.7.4/.azure_upload.sh
--rw-r--r--   0 sbelden    (501) staff       (20)       55 2020-12-23 03:10:46.000000 fastavro-1.7.4/.flake8.cython
--rw-r--r--   0 sbelden    (501) staff       (20)    26245 2023-05-04 14:38:48.000000 fastavro-1.7.4/ChangeLog
--rw-r--r--   0 sbelden    (501) staff       (20)      333 2022-10-26 14:14:35.000000 fastavro-1.7.4/Dockerfile
--rw-r--r--   0 sbelden    (501) staff       (20)     1068 2019-05-04 22:05:46.000000 fastavro-1.7.4/LICENSE
--rw-r--r--   0 sbelden    (501) staff       (20)      559 2022-08-11 13:05:27.000000 fastavro-1.7.4/MANIFEST.in
--rw-r--r--   0 sbelden    (501) staff       (20)      812 2022-08-11 13:05:27.000000 fastavro-1.7.4/Makefile
--rw-r--r--   0 sbelden    (501) staff       (20)      563 2019-05-04 22:05:46.000000 fastavro-1.7.4/NOTICE.txt
--rw-r--r--   0 sbelden    (501) staff       (20)     5250 2023-05-04 15:54:08.976914 fastavro-1.7.4/PKG-INFO
--rw-r--r--   0 sbelden    (501) staff       (20)     3870 2022-10-26 14:14:35.000000 fastavro-1.7.4/README.md
--rw-r--r--   0 sbelden    (501) staff       (20)      520 2023-05-04 13:14:43.000000 fastavro-1.7.4/developer_requirements.txt
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.867907 fastavro-1.7.4/docs/
--rw-r--r--   0 sbelden    (501) staff       (20)     5578 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/Makefile
--rw-r--r--   0 sbelden    (501) staff       (20)     1456 2019-05-04 22:05:46.000000 fastavro-1.7.4/docs/command_line_script.rst
--rw-r--r--   0 sbelden    (501) staff       (20)     8320 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/conf.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2502 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/index.rst
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.868853 fastavro-1.7.4/docs/io/
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/io/index.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/io/json_decoder.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/io/json_encoder.rst
--rw-r--r--   0 sbelden    (501) staff       (20)       88 2020-02-26 16:33:59.000000 fastavro-1.7.4/docs/json_reader.rst
--rw-r--r--   0 sbelden    (501) staff       (20)       91 2020-02-26 16:33:59.000000 fastavro-1.7.4/docs/json_writer.rst
--rw-r--r--   0 sbelden    (501) staff       (20)     4869 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/logical_types.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      256 2021-03-20 12:25:05.000000 fastavro-1.7.4/docs/reader.rst
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.869470 fastavro-1.7.4/docs/repository/
--rw-r--r--   0 sbelden    (501) staff       (20)      116 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/repository/base.rst
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/repository/index.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      405 2021-02-06 15:15:34.000000 fastavro-1.7.4/docs/schema.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      174 2021-03-13 13:43:47.000000 fastavro-1.7.4/docs/utils.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      149 2019-05-04 22:05:46.000000 fastavro-1.7.4/docs/validation.rst
--rw-r--r--   0 sbelden    (501) staff       (20)     3996 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/writer.rst
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.907334 fastavro-1.7.4/fastavro/
--rw-r--r--   0 sbelden    (501) staff       (20)     1750 2023-05-04 14:38:56.000000 fastavro-1.7.4/fastavro/__init__.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2423 2020-12-23 03:10:46.000000 fastavro-1.7.4/fastavro/__main__.py
--rw-r--r--   0 sbelden    (501) staff       (20)   262056 2023-05-04 15:54:04.000000 fastavro-1.7.4/fastavro/_logical_readers.c
--rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_logical_readers.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)     2792 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_logical_readers.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)     2813 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_logical_readers_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_logical_readers_py.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)   430913 2023-05-04 15:54:05.000000 fastavro-1.7.4/fastavro/_logical_writers.c
--rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.7.4/fastavro/_logical_writers.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)     8427 2022-10-06 12:45:33.000000 fastavro-1.7.4/fastavro/_logical_writers.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)     7830 2022-10-06 12:45:33.000000 fastavro-1.7.4/fastavro/_logical_writers_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.7.4/fastavro/_logical_writers_py.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)  1109567 2023-05-04 15:54:05.000000 fastavro-1.7.4/fastavro/_read.c
--rw-r--r--   0 sbelden    (501) staff       (20)     1827 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_read.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)    35286 2023-04-17 20:07:08.000000 fastavro-1.7.4/fastavro/_read.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)      703 2023-04-17 20:07:08.000000 fastavro-1.7.4/fastavro/_read_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)    35776 2023-04-17 20:07:08.000000 fastavro-1.7.4/fastavro/_read_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)   704359 2023-05-04 15:54:05.000000 fastavro-1.7.4/fastavro/_schema.c
--rw-r--r--   0 sbelden    (501) staff       (20)      950 2023-02-22 18:29:22.000000 fastavro-1.7.4/fastavro/_schema.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)    24103 2023-05-04 14:35:44.000000 fastavro-1.7.4/fastavro/_schema.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)     1421 2021-01-23 16:11:54.000000 fastavro-1.7.4/fastavro/_schema_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)    33011 2023-05-04 14:35:44.000000 fastavro-1.7.4/fastavro/_schema_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)   441134 2020-08-18 18:15:09.000000 fastavro-1.7.4/fastavro/_six.c
--rw-r--r--   0 sbelden    (501) staff       (20)      633 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_validate_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)   390961 2023-05-04 15:54:06.000000 fastavro-1.7.4/fastavro/_validation.c
--rw-r--r--   0 sbelden    (501) staff       (20)      338 2022-08-12 17:49:36.000000 fastavro-1.7.4/fastavro/_validation.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)     9403 2022-08-15 15:33:27.000000 fastavro-1.7.4/fastavro/_validation.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)    10757 2022-08-15 15:33:27.000000 fastavro-1.7.4/fastavro/_validation_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)  1717084 2023-05-04 15:54:07.000000 fastavro-1.7.4/fastavro/_write.c
--rw-r--r--   0 sbelden    (501) staff       (20)     1680 2022-08-15 15:33:27.000000 fastavro-1.7.4/fastavro/_write.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)    26702 2023-04-17 20:07:08.000000 fastavro-1.7.4/fastavro/_write.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)      619 2023-05-03 19:57:13.000000 fastavro-1.7.4/fastavro/_write_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)    26758 2023-04-17 20:07:08.000000 fastavro-1.7.4/fastavro/_write_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)      853 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/const.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.913799 fastavro-1.7.4/fastavro/io/
--rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-02-26 16:33:59.000000 fastavro-1.7.4/fastavro/io/__init__.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4319 2022-10-06 12:45:36.000000 fastavro-1.7.4/fastavro/io/binary_decoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1861 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/io/binary_encoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     6904 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/io/json_decoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     5674 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/io/json_encoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4980 2022-02-25 13:49:52.000000 fastavro-1.7.4/fastavro/io/parser.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2321 2021-01-22 04:19:07.000000 fastavro-1.7.4/fastavro/io/symbols.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1603 2023-03-16 19:48:58.000000 fastavro-1.7.4/fastavro/json_read.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2908 2022-08-15 15:33:27.000000 fastavro-1.7.4/fastavro/json_write.py
--rw-r--r--   0 sbelden    (501) staff       (20)      217 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/logical_readers.py
--rw-r--r--   0 sbelden    (501) staff       (20)      217 2020-12-23 03:10:46.000000 fastavro-1.7.4/fastavro/logical_writers.py
--rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-06-22 15:51:13.000000 fastavro-1.7.4/fastavro/py.typed
--rw-r--r--   0 sbelden    (501) staff       (20)      775 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/read.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.915607 fastavro-1.7.4/fastavro/repository/
--rw-r--r--   0 sbelden    (501) staff       (20)      210 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/repository/__init__.py
--rw-r--r--   0 sbelden    (501) staff       (20)      185 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/repository/base.py
--rw-r--r--   0 sbelden    (501) staff       (20)      764 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/repository/flat_dict.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1030 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/schema.py
--rw-r--r--   0 sbelden    (501) staff       (20)      419 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/types.py
--rw-r--r--   0 sbelden    (501) staff       (20)     7456 2023-02-01 14:56:04.000000 fastavro-1.7.4/fastavro/utils.py
--rw-r--r--   0 sbelden    (501) staff       (20)      422 2020-12-23 03:10:46.000000 fastavro-1.7.4/fastavro/validation.py
--rw-r--r--   0 sbelden    (501) staff       (20)      457 2021-02-27 20:10:59.000000 fastavro-1.7.4/fastavro/write.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.910355 fastavro-1.7.4/fastavro.egg-info/
--rw-r--r--   0 sbelden    (501) staff       (20)     5250 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/PKG-INFO
--rw-r--r--   0 sbelden    (501) staff       (20)     6017 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/SOURCES.txt
--rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/dependency_links.txt
--rw-r--r--   0 sbelden    (501) staff       (20)       52 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/entry_points.txt
--rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-03-16 16:53:53.000000 fastavro-1.7.4/fastavro.egg-info/not-zip-safe
--rw-r--r--   0 sbelden    (501) staff       (20)       96 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/requires.txt
--rw-r--r--   0 sbelden    (501) staff       (20)        9 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/top_level.txt
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2023-04-17 20:07:08.000000 fastavro-1.7.4/mypy.ini
--rwxr-xr-x   0 sbelden    (501) staff       (20)     1930 2023-03-16 18:04:24.000000 fastavro-1.7.4/publish.sh
--rw-r--r--   0 sbelden    (501) staff       (20)      204 2023-03-08 20:55:48.000000 fastavro-1.7.4/pyproject.toml
--rwxr-xr-x   0 sbelden    (501) staff       (20)       31 2019-05-04 22:05:46.000000 fastavro-1.7.4/pytest.ini
--rw-r--r--   0 sbelden    (501) staff       (20)      710 2022-09-20 17:48:57.000000 fastavro-1.7.4/run-tests.cmd
--rwxr-xr-x   0 sbelden    (501) staff       (20)     1050 2023-05-04 13:44:25.000000 fastavro-1.7.4/run-tests.sh
--rw-r--r--   0 sbelden    (501) staff       (20)      105 2023-05-04 15:54:08.977634 fastavro-1.7.4/setup.cfg
--rw-r--r--   0 sbelden    (501) staff       (20)     2796 2022-10-26 14:14:35.000000 fastavro-1.7.4/setup.py
--rwxr-xr-x   0 sbelden    (501) staff       (20)      169 2023-03-08 22:33:06.000000 fastavro-1.7.4/tag.sh
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.934647 fastavro-1.7.4/tests/
--rw-r--r--   0 sbelden    (501) staff       (20)        0 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/__init__.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.956336 fastavro-1.7.4/tests/avro-files/
--rw-r--r--   0 sbelden    (501) staff       (20)       55 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/Child.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/Child1.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      179 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/Parent.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      130 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/ParentMissingChild.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      447 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/a_triple_pair.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       79 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/bool.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.seperators.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.deflate.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       84 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.plain.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.zerojsonvalues.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     3293 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/deflate.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      276 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/double_float.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      234 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/error-type.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     8453 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/java-generated-uuid.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      299 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/lines.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      403 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/m.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      139 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/no-fields.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     3285 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/null.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       68 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/org.apache.avro.tool.TestDataFileTools.avro
--rwxr-xr-x   0 sbelden    (501) staff       (20)      321 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/part-00000.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      218 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/recursive.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      162 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/request.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/response.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     3296 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/snappy.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    12556 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-0.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-1-A.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-1.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-3-A.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     6112 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-6-B.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-9.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     6522 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-null-B.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    13289 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-null.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    13677 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-snappy.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      182 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       51 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/testDataFileMeta.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      690 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/avro-files/weather-legacy-generated.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      696 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/avro-files/weather-legacy-with-names.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      330 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/weather-snappy.avro
--rwxr-xr-x   0 sbelden    (501) staff       (20)      335 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/weather-sorted.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      358 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/weather.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      999 2021-03-13 13:43:47.000000 fastavro-1.7.4/tests/conftest.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.958155 fastavro-1.7.4/tests/load_schema_test/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test/C.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test/D.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.960082 fastavro-1.7.4/tests/load_schema_test_10/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_10/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_10/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_10/C.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_10/D.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.961957 fastavro-1.7.4/tests/load_schema_test_11/
--rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_11/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_11/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_11/C.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_11/D.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_11/E.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.962265 fastavro-1.7.4/tests/load_schema_test_12/
--rw-r--r--   0 sbelden    (501) staff       (20)      143 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_12/A.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.963016 fastavro-1.7.4/tests/load_schema_test_12/com/
--rw-r--r--   0 sbelden    (501) staff       (20)      137 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_12/com/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      187 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_12/com/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.963704 fastavro-1.7.4/tests/load_schema_test_12/com/namespace/
--rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_12/com/namespace/D.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_12/com/namespace/E.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.964621 fastavro-1.7.4/tests/load_schema_test_13/
--rw-r--r--   0 sbelden    (501) staff       (20)        3 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_13/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_13/B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.965146 fastavro-1.7.4/tests/load_schema_test_14/
--rw-r--r--   0 sbelden    (501) staff       (20)        8 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_14/A.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.966331 fastavro-1.7.4/tests/load_schema_test_15/
--rw-r--r--   0 sbelden    (501) staff       (20)       10 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_15/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_15/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_15/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.967059 fastavro-1.7.4/tests/load_schema_test_16/
--rw-r--r--   0 sbelden    (501) staff       (20)      225 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/load_schema_test_16/namespace.match.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      120 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/load_schema_test_16/namespace.team.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.968178 fastavro-1.7.4/tests/load_schema_test_2/
--rw-r--r--   0 sbelden    (501) staff       (20)      294 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test_2/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test_2/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test_2/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.969608 fastavro-1.7.4/tests/load_schema_test_3/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_3/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_3/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_3/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.970744 fastavro-1.7.4/tests/load_schema_test_4/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_4/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_4/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_4/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.971558 fastavro-1.7.4/tests/load_schema_test_5/
--rw-r--r--   0 sbelden    (501) staff       (20)      170 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_5/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_5/B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.972277 fastavro-1.7.4/tests/load_schema_test_6/
--rw-r--r--   0 sbelden    (501) staff       (20)      173 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_6/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_6/B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.973160 fastavro-1.7.4/tests/load_schema_test_7/
--rw-r--r--   0 sbelden    (501) staff       (20)      129 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_7/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      116 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_7/namespace.B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.974183 fastavro-1.7.4/tests/load_schema_test_8/
--rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_8/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      102 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_8/namespace.B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      110 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_8/namespace.C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.975313 fastavro-1.7.4/tests/load_schema_test_9/
--rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_9/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_9/namespace.B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_9/namespace.C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.975685 fastavro-1.7.4/tests/repository/
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.976436 fastavro-1.7.4/tests/repository/flat_dict_test/
--rw-r--r--   0 sbelden    (501) staff       (20)       11 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/repository/flat_dict_test/InvalidJson.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      111 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/repository/flat_dict_test/Valid.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)     1153 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/repository/test_flat_dict.py
--rw-r--r--   0 sbelden    (501) staff       (20)     3678 2021-03-13 13:43:47.000000 fastavro-1.7.4/tests/test_aliases.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2185 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/test_appendable.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2533 2023-02-01 14:55:54.000000 fastavro-1.7.4/tests/test_block_reader.py
--rw-r--r--   0 sbelden    (501) staff       (20)    14428 2021-01-22 17:21:26.000000 fastavro-1.7.4/tests/test_canonical_form.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4768 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_complex.py
--rw-r--r--   0 sbelden    (501) staff       (20)     5623 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/test_compression.py
--rw-r--r--   0 sbelden    (501) staff       (20)    98991 2023-04-17 20:07:08.000000 fastavro-1.7.4/tests/test_fastavro.py
--rw-r--r--   0 sbelden    (501) staff       (20)    33787 2021-01-23 16:11:54.000000 fastavro-1.7.4/tests/test_fingerprint.py
--rw-r--r--   0 sbelden    (501) staff       (20)    27587 2023-03-16 19:48:58.000000 fastavro-1.7.4/tests/test_json.py
--rw-r--r--   0 sbelden    (501) staff       (20)    16587 2022-10-26 14:14:35.000000 fastavro-1.7.4/tests/test_logical_types.py
--rw-r--r--   0 sbelden    (501) staff       (20)     3483 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_main_cli.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2229 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_promotion.py
--rw-r--r--   0 sbelden    (501) staff       (20)    40285 2023-05-04 14:35:44.000000 fastavro-1.7.4/tests/test_schema.py
--rw-r--r--   0 sbelden    (501) staff       (20)    22495 2023-02-01 14:56:44.000000 fastavro-1.7.4/tests/test_schema_evolution.py
--rw-r--r--   0 sbelden    (501) staff       (20)     8069 2022-09-09 20:03:51.000000 fastavro-1.7.4/tests/test_schemaless.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1224 2021-03-13 13:43:47.000000 fastavro-1.7.4/tests/test_str_py3.py
--rw-r--r--   0 sbelden    (501) staff       (20)     7148 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_timezone.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2653 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_types.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4503 2022-05-21 05:36:47.000000 fastavro-1.7.4/tests/test_utils.py
--rw-r--r--   0 sbelden    (501) staff       (20)    15273 2022-08-12 17:49:36.000000 fastavro-1.7.4/tests/test_validation.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1653 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_write_block.py
--rw-r--r--   0 sbelden    (501) staff       (20)      253 2022-10-26 15:21:05.000000 fastavro-1.7.4/tox.ini
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.594318 fastavro-1.8.0/
+-rwxr-xr-x   0 sbelden    (501) staff       (20)     1625 2019-05-08 02:19:05.000000 fastavro-1.8.0/.azure_upload.sh
+-rw-r--r--   0 sbelden    (501) staff       (20)       55 2020-12-23 03:10:46.000000 fastavro-1.8.0/.flake8.cython
+-rw-r--r--   0 sbelden    (501) staff       (20)    26345 2023-07-06 15:00:48.000000 fastavro-1.8.0/ChangeLog
+-rw-r--r--   0 sbelden    (501) staff       (20)      333 2022-10-26 14:14:35.000000 fastavro-1.8.0/Dockerfile
+-rw-r--r--   0 sbelden    (501) staff       (20)     1068 2019-05-04 22:05:46.000000 fastavro-1.8.0/LICENSE
+-rw-r--r--   0 sbelden    (501) staff       (20)      559 2022-08-11 13:05:27.000000 fastavro-1.8.0/MANIFEST.in
+-rw-r--r--   0 sbelden    (501) staff       (20)      812 2022-08-11 13:05:27.000000 fastavro-1.8.0/Makefile
+-rw-r--r--   0 sbelden    (501) staff       (20)      563 2019-05-04 22:05:46.000000 fastavro-1.8.0/NOTICE.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)     5250 2023-07-06 15:53:50.594465 fastavro-1.8.0/PKG-INFO
+-rw-r--r--   0 sbelden    (501) staff       (20)     3870 2022-10-26 14:14:35.000000 fastavro-1.8.0/README.md
+-rw-r--r--   0 sbelden    (501) staff       (20)      520 2023-05-04 13:14:43.000000 fastavro-1.8.0/developer_requirements.txt
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.494680 fastavro-1.8.0/docs/
+-rw-r--r--   0 sbelden    (501) staff       (20)     5578 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/Makefile
+-rw-r--r--   0 sbelden    (501) staff       (20)     1456 2019-05-04 22:05:46.000000 fastavro-1.8.0/docs/command_line_script.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)     8320 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/conf.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2502 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/index.rst
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.495976 fastavro-1.8.0/docs/io/
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/io/index.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/io/json_decoder.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/io/json_encoder.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)       88 2020-02-26 16:33:59.000000 fastavro-1.8.0/docs/json_reader.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)       91 2020-02-26 16:33:59.000000 fastavro-1.8.0/docs/json_writer.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)     4869 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/logical_types.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      256 2021-03-20 12:25:05.000000 fastavro-1.8.0/docs/reader.rst
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.496914 fastavro-1.8.0/docs/repository/
+-rw-r--r--   0 sbelden    (501) staff       (20)      116 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/repository/base.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/repository/index.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      405 2021-02-06 15:15:34.000000 fastavro-1.8.0/docs/schema.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      174 2021-03-13 13:43:47.000000 fastavro-1.8.0/docs/utils.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      149 2019-05-04 22:05:46.000000 fastavro-1.8.0/docs/validation.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)     3996 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/writer.rst
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.531576 fastavro-1.8.0/fastavro/
+-rw-r--r--   0 sbelden    (501) staff       (20)     1750 2023-07-06 14:59:31.000000 fastavro-1.8.0/fastavro/__init__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2423 2020-12-23 03:10:46.000000 fastavro-1.8.0/fastavro/__main__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   262056 2023-07-06 15:53:45.000000 fastavro-1.8.0/fastavro/_logical_readers.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/_logical_readers.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)     2792 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/_logical_readers.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)     2813 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/_logical_readers_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/_logical_readers_py.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)   430913 2023-07-06 15:53:46.000000 fastavro-1.8.0/fastavro/_logical_writers.c
+-rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.8.0/fastavro/_logical_writers.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)     8427 2022-10-06 12:45:33.000000 fastavro-1.8.0/fastavro/_logical_writers.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)     7830 2022-10-06 12:45:33.000000 fastavro-1.8.0/fastavro/_logical_writers_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.8.0/fastavro/_logical_writers_py.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)  1104218 2023-07-06 15:53:46.000000 fastavro-1.8.0/fastavro/_read.c
+-rw-r--r--   0 sbelden    (501) staff       (20)     2070 2023-07-06 14:53:47.000000 fastavro-1.8.0/fastavro/_read.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)    34172 2023-07-06 14:53:47.000000 fastavro-1.8.0/fastavro/_read.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)      703 2023-04-17 20:07:08.000000 fastavro-1.8.0/fastavro/_read_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    34680 2023-07-06 14:53:47.000000 fastavro-1.8.0/fastavro/_read_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   704359 2023-07-06 15:53:47.000000 fastavro-1.8.0/fastavro/_schema.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      950 2023-02-22 18:29:22.000000 fastavro-1.8.0/fastavro/_schema.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)    24103 2023-05-04 14:35:44.000000 fastavro-1.8.0/fastavro/_schema.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)     1421 2021-01-23 16:11:54.000000 fastavro-1.8.0/fastavro/_schema_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    33011 2023-05-04 14:35:44.000000 fastavro-1.8.0/fastavro/_schema_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   441134 2020-08-18 18:15:09.000000 fastavro-1.8.0/fastavro/_six.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      633 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/_validate_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   390961 2023-07-06 15:53:47.000000 fastavro-1.8.0/fastavro/_validation.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      338 2022-08-12 17:49:36.000000 fastavro-1.8.0/fastavro/_validation.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)     9403 2022-08-15 15:33:27.000000 fastavro-1.8.0/fastavro/_validation.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)    10757 2022-08-15 15:33:27.000000 fastavro-1.8.0/fastavro/_validation_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)  1717084 2023-07-06 15:53:49.000000 fastavro-1.8.0/fastavro/_write.c
+-rw-r--r--   0 sbelden    (501) staff       (20)     1680 2022-08-15 15:33:27.000000 fastavro-1.8.0/fastavro/_write.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)    26702 2023-04-17 20:07:08.000000 fastavro-1.8.0/fastavro/_write.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)      619 2023-05-03 19:57:13.000000 fastavro-1.8.0/fastavro/_write_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    26758 2023-04-17 20:07:08.000000 fastavro-1.8.0/fastavro/_write_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      853 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/const.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.536520 fastavro-1.8.0/fastavro/io/
+-rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-02-26 16:33:59.000000 fastavro-1.8.0/fastavro/io/__init__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4379 2023-07-06 14:53:47.000000 fastavro-1.8.0/fastavro/io/binary_decoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1861 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/io/binary_encoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     6936 2023-07-06 14:53:47.000000 fastavro-1.8.0/fastavro/io/json_decoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     5674 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/io/json_encoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4980 2022-02-25 13:49:52.000000 fastavro-1.8.0/fastavro/io/parser.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2321 2021-01-22 04:19:07.000000 fastavro-1.8.0/fastavro/io/symbols.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1603 2023-03-16 19:48:58.000000 fastavro-1.8.0/fastavro/json_read.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2908 2022-08-15 15:33:27.000000 fastavro-1.8.0/fastavro/json_write.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      217 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/logical_readers.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      217 2020-12-23 03:10:46.000000 fastavro-1.8.0/fastavro/logical_writers.py
+-rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-06-22 15:51:13.000000 fastavro-1.8.0/fastavro/py.typed
+-rw-r--r--   0 sbelden    (501) staff       (20)      775 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/read.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.538089 fastavro-1.8.0/fastavro/repository/
+-rw-r--r--   0 sbelden    (501) staff       (20)      210 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/repository/__init__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      185 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/repository/base.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      764 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/repository/flat_dict.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1030 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/schema.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      419 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/types.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     7456 2023-02-01 14:56:04.000000 fastavro-1.8.0/fastavro/utils.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      422 2020-12-23 03:10:46.000000 fastavro-1.8.0/fastavro/validation.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      457 2021-02-27 20:10:59.000000 fastavro-1.8.0/fastavro/write.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.534059 fastavro-1.8.0/fastavro.egg-info/
+-rw-r--r--   0 sbelden    (501) staff       (20)     5250 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/PKG-INFO
+-rw-r--r--   0 sbelden    (501) staff       (20)     6017 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/SOURCES.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/dependency_links.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)       52 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/entry_points.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-07-05 18:01:12.000000 fastavro-1.8.0/fastavro.egg-info/not-zip-safe
+-rw-r--r--   0 sbelden    (501) staff       (20)       96 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/requires.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)        9 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/top_level.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2023-04-17 20:07:08.000000 fastavro-1.8.0/mypy.ini
+-rwxr-xr-x   0 sbelden    (501) staff       (20)     1439 2023-07-06 15:52:36.000000 fastavro-1.8.0/publish.sh
+-rw-r--r--   0 sbelden    (501) staff       (20)      204 2023-03-08 20:55:48.000000 fastavro-1.8.0/pyproject.toml
+-rwxr-xr-x   0 sbelden    (501) staff       (20)       31 2019-05-04 22:05:46.000000 fastavro-1.8.0/pytest.ini
+-rw-r--r--   0 sbelden    (501) staff       (20)      710 2022-09-20 17:48:57.000000 fastavro-1.8.0/run-tests.cmd
+-rwxr-xr-x   0 sbelden    (501) staff       (20)     1054 2023-07-05 17:54:02.000000 fastavro-1.8.0/run-tests.sh
+-rw-r--r--   0 sbelden    (501) staff       (20)      105 2023-07-06 15:53:50.594914 fastavro-1.8.0/setup.cfg
+-rw-r--r--   0 sbelden    (501) staff       (20)     2796 2022-10-26 14:14:35.000000 fastavro-1.8.0/setup.py
+-rwxr-xr-x   0 sbelden    (501) staff       (20)      169 2023-03-08 22:33:06.000000 fastavro-1.8.0/tag.sh
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.552393 fastavro-1.8.0/tests/
+-rw-r--r--   0 sbelden    (501) staff       (20)        0 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/__init__.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.571904 fastavro-1.8.0/tests/avro-files/
+-rw-r--r--   0 sbelden    (501) staff       (20)       55 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/Child.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/Child1.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      179 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/Parent.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      130 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/ParentMissingChild.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      447 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/a_triple_pair.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       79 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/bool.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.seperators.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.deflate.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       84 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.plain.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.zerojsonvalues.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     3293 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/deflate.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      276 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/double_float.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      234 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/error-type.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     8453 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/java-generated-uuid.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      299 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/lines.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      403 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/m.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      139 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/no-fields.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     3285 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/null.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       68 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/org.apache.avro.tool.TestDataFileTools.avro
+-rwxr-xr-x   0 sbelden    (501) staff       (20)      321 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/part-00000.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      218 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/recursive.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      162 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/request.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/response.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     3296 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/snappy.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    12556 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-0.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-1-A.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-1.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-3-A.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     6112 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-6-B.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-9.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     6522 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-null-B.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    13289 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-null.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    13677 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-snappy.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      182 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       51 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/testDataFileMeta.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      690 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/avro-files/weather-legacy-generated.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      696 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/avro-files/weather-legacy-with-names.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      330 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/weather-snappy.avro
+-rwxr-xr-x   0 sbelden    (501) staff       (20)      335 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/weather-sorted.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      358 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/weather.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      999 2021-03-13 13:43:47.000000 fastavro-1.8.0/tests/conftest.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.574424 fastavro-1.8.0/tests/load_schema_test/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test/C.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test/D.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.576920 fastavro-1.8.0/tests/load_schema_test_10/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_10/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_10/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_10/C.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_10/D.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.578842 fastavro-1.8.0/tests/load_schema_test_11/
+-rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_11/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_11/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_11/C.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_11/D.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_11/E.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.579216 fastavro-1.8.0/tests/load_schema_test_12/
+-rw-r--r--   0 sbelden    (501) staff       (20)      143 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_12/A.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.579969 fastavro-1.8.0/tests/load_schema_test_12/com/
+-rw-r--r--   0 sbelden    (501) staff       (20)      137 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_12/com/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      187 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_12/com/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.580693 fastavro-1.8.0/tests/load_schema_test_12/com/namespace/
+-rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_12/com/namespace/D.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_12/com/namespace/E.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.581558 fastavro-1.8.0/tests/load_schema_test_13/
+-rw-r--r--   0 sbelden    (501) staff       (20)        3 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_13/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_13/B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.582021 fastavro-1.8.0/tests/load_schema_test_14/
+-rw-r--r--   0 sbelden    (501) staff       (20)        8 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_14/A.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.582946 fastavro-1.8.0/tests/load_schema_test_15/
+-rw-r--r--   0 sbelden    (501) staff       (20)       10 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_15/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_15/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_15/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.583623 fastavro-1.8.0/tests/load_schema_test_16/
+-rw-r--r--   0 sbelden    (501) staff       (20)      225 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/load_schema_test_16/namespace.match.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      120 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/load_schema_test_16/namespace.team.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.584717 fastavro-1.8.0/tests/load_schema_test_2/
+-rw-r--r--   0 sbelden    (501) staff       (20)      294 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test_2/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test_2/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test_2/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.586139 fastavro-1.8.0/tests/load_schema_test_3/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_3/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_3/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_3/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.587468 fastavro-1.8.0/tests/load_schema_test_4/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_4/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_4/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_4/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.588318 fastavro-1.8.0/tests/load_schema_test_5/
+-rw-r--r--   0 sbelden    (501) staff       (20)      170 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_5/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_5/B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.589348 fastavro-1.8.0/tests/load_schema_test_6/
+-rw-r--r--   0 sbelden    (501) staff       (20)      173 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_6/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_6/B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.590455 fastavro-1.8.0/tests/load_schema_test_7/
+-rw-r--r--   0 sbelden    (501) staff       (20)      129 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_7/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      116 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_7/namespace.B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.591750 fastavro-1.8.0/tests/load_schema_test_8/
+-rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_8/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      102 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_8/namespace.B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      110 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_8/namespace.C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.592987 fastavro-1.8.0/tests/load_schema_test_9/
+-rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_9/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_9/namespace.B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_9/namespace.C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.593328 fastavro-1.8.0/tests/repository/
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.594005 fastavro-1.8.0/tests/repository/flat_dict_test/
+-rw-r--r--   0 sbelden    (501) staff       (20)       11 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/repository/flat_dict_test/InvalidJson.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      111 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/repository/flat_dict_test/Valid.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)     1153 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/repository/test_flat_dict.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     3678 2021-03-13 13:43:47.000000 fastavro-1.8.0/tests/test_aliases.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2185 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/test_appendable.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2533 2023-02-01 14:55:54.000000 fastavro-1.8.0/tests/test_block_reader.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    14428 2021-01-22 17:21:26.000000 fastavro-1.8.0/tests/test_canonical_form.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4768 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_complex.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     5623 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/test_compression.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    98991 2023-07-05 18:24:15.000000 fastavro-1.8.0/tests/test_fastavro.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    33787 2021-01-23 16:11:54.000000 fastavro-1.8.0/tests/test_fingerprint.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    27597 2023-07-06 14:53:47.000000 fastavro-1.8.0/tests/test_json.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    16587 2022-10-26 14:14:35.000000 fastavro-1.8.0/tests/test_logical_types.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     3483 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_main_cli.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2229 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_promotion.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    40285 2023-05-04 14:35:44.000000 fastavro-1.8.0/tests/test_schema.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    22495 2023-02-01 14:56:44.000000 fastavro-1.8.0/tests/test_schema_evolution.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     8733 2023-07-06 14:53:47.000000 fastavro-1.8.0/tests/test_schemaless.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1224 2021-03-13 13:43:47.000000 fastavro-1.8.0/tests/test_str_py3.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     7148 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_timezone.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2653 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_types.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4503 2022-05-21 05:36:47.000000 fastavro-1.8.0/tests/test_utils.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    15273 2022-08-12 17:49:36.000000 fastavro-1.8.0/tests/test_validation.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1653 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_write_block.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      253 2022-10-26 15:21:05.000000 fastavro-1.8.0/tox.ini
```

### Comparing `fastavro-1.7.4/.azure_upload.sh` & `fastavro-1.8.0/.azure_upload.sh`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/ChangeLog` & `fastavro-1.8.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-06 version 1.8.0
+* Add ability to override unicode decode errors (@scottbelden in PR #696)
+
 2023-05-04 version 1.7.4
 * Fix parsing of namespaces (@scottbelden in PR #692)
 * Be able to specify a reader schema in the json_reader (@scottbelden in PR #681)
 
 2023-03-08 version 1.7.3
 * Create musllinux wheels (@scottbelden in PR #679)
```

### Comparing `fastavro-1.7.4/LICENSE` & `fastavro-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/MANIFEST.in` & `fastavro-1.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/Makefile` & `fastavro-1.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/NOTICE.txt` & `fastavro-1.8.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/PKG-INFO` & `fastavro-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastavro
-Version: 1.7.4
+Version: 1.8.0
 Summary: Fast read/write of AVRO files
 Home-page: https://github.com/fastavro/fastavro
 Author: Miki Tebeka
 Author-email: miki.tebeka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fastavro-1.7.4/README.md` & `fastavro-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/developer_requirements.txt` & `fastavro-1.8.0/developer_requirements.txt`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/docs/Makefile` & `fastavro-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/docs/command_line_script.rst` & `fastavro-1.8.0/docs/command_line_script.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/docs/conf.py` & `fastavro-1.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/docs/index.rst` & `fastavro-1.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/docs/logical_types.rst` & `fastavro-1.8.0/docs/logical_types.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/docs/writer.rst` & `fastavro-1.8.0/docs/writer.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/__init__.py` & `fastavro-1.8.0/fastavro/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         {u'station': u'012650-99999', u'temp': 111, u'time': 1433275478},
     ]
 
     with open('weather.avro', 'wb') as out:
         writer(out, schema, records)
 """
 
-__version_info__ = (1, 7, 4)
+__version_info__ = (1, 8, 0)
 __version__ = "%s.%s.%s" % __version_info__
 
 
 import fastavro.read
 import fastavro.write
 import fastavro.schema
 import fastavro.validation
```

### Comparing `fastavro-1.7.4/fastavro/__main__.py` & `fastavro-1.8.0/fastavro/__main__.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_logical_readers.c` & `fastavro-1.8.0/fastavro/_logical_readers.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_logical_readers.pyx` & `fastavro-1.8.0/fastavro/_logical_readers.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_logical_readers_py.py` & `fastavro-1.8.0/fastavro/_logical_readers_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_logical_writers.c` & `fastavro-1.8.0/fastavro/_logical_writers.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_logical_writers.pyx` & `fastavro-1.8.0/fastavro/_logical_writers.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_logical_writers_py.py` & `fastavro-1.8.0/fastavro/_logical_writers_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_read.c` & `fastavro-1.8.0/fastavro/_read.c`

 * *Files 6% similar despite different names*

```diff
@@ -991,20 +991,23 @@
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8fastavro_5_read___pyx_scope_struct___iter_avro_records;
 struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks;
 struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_2___iter__;
 union __pyx_t_8fastavro_5_read_float_uint32;
 union __pyx_t_8fastavro_5_read_double_ulong64;
+struct __pyx_opt_args_8fastavro_5_read_read_utf8;
 struct __pyx_opt_args_8fastavro_5_read_read_array;
 struct __pyx_opt_args_8fastavro_5_read_read_map;
 struct __pyx_opt_args_8fastavro_5_read_read_union;
 struct __pyx_opt_args_8fastavro_5_read_read_record;
 struct __pyx_opt_args_8fastavro_5_read__read_data;
 struct __pyx_opt_args_8fastavro_5_read_schemaless_reader;
+struct __pyx_defaults;
+typedef struct __pyx_defaults __pyx_defaults;
 
 /* "fastavro/_read.pyx":195
  * 
  * 
  * cdef union float_uint32:             # <<<<<<<<<<<<<<
  *     float f
  *     uint32 n
@@ -1022,99 +1025,110 @@
  *     ulong64 n
  */
 union __pyx_t_8fastavro_5_read_double_ulong64 {
   double d;
   __pyx_t_8fastavro_5_read_ulong64 n;
 };
 
+/* "fastavro/_read.pyx":284
+ * 
+ * 
+ * cpdef unicode read_utf8(fo, handle_unicode_errors="strict"):             # <<<<<<<<<<<<<<
+ *     """A string is encoded as a long followed by that many bytes of UTF-8
+ *     encoded character data.
+ */
+struct __pyx_opt_args_8fastavro_5_read_read_utf8 {
+  int __pyx_n;
+  PyObject *handle_unicode_errors;
+};
+
 /* "fastavro/_read.pyx":338
  * 
  * cpdef read_array(
  *     fo,             # <<<<<<<<<<<<<<
  *     writer_schema,
  *     named_schemas,
  */
 struct __pyx_opt_args_8fastavro_5_read_read_array {
   int __pyx_n;
   PyObject *reader_schema;
-  PyObject *return_record_name;
-  PyObject *return_record_name_override;
+  PyObject *options;
 };
 
-/* "fastavro/_read.pyx":422
+/* "fastavro/_read.pyx":419
  * 
  * cpdef read_map(
  *     fo,             # <<<<<<<<<<<<<<
  *     writer_schema,
  *     named_schemas,
  */
 struct __pyx_opt_args_8fastavro_5_read_read_map {
   int __pyx_n;
   PyObject *reader_schema;
-  PyObject *return_record_name;
-  PyObject *return_record_name_override;
+  PyObject *options;
 };
 
-/* "fastavro/_read.pyx":507
+/* "fastavro/_read.pyx":501
  * 
  * cpdef read_union(
  *     fo,             # <<<<<<<<<<<<<<
  *     writer_schema,
  *     named_schemas,
  */
 struct __pyx_opt_args_8fastavro_5_read_read_union {
   int __pyx_n;
   PyObject *reader_schema;
-  PyObject *return_record_name;
-  PyObject *return_record_name_override;
+  PyObject *options;
 };
 
-/* "fastavro/_read.pyx":592
+/* "fastavro/_read.pyx":578
  * 
  * cpdef read_record(
  *     fo,             # <<<<<<<<<<<<<<
  *     writer_schema,
  *     named_schemas,
  */
 struct __pyx_opt_args_8fastavro_5_read_read_record {
   int __pyx_n;
   PyObject *reader_schema;
-  PyObject *return_record_name;
-  PyObject *return_record_name_override;
+  PyObject *options;
 };
 
-/* "fastavro/_read.pyx":688
+/* "fastavro/_read.pyx":671
  * 
  * cpdef _read_data(
  *     fo,             # <<<<<<<<<<<<<<
  *     writer_schema,
  *     named_schemas,
  */
 struct __pyx_opt_args_8fastavro_5_read__read_data {
   int __pyx_n;
   PyObject *reader_schema;
-  PyObject *return_record_name;
-  PyObject *return_record_name_override;
+  PyObject *options;
 };
 
-/* "fastavro/_read.pyx":1107
+/* "fastavro/_read.pyx":1100
  * 
- * 
- * cpdef schemaless_reader(fo, writer_schema, reader_schema=None,             # <<<<<<<<<<<<<<
- *                         return_record_name=False,
- *                         return_record_name_override=False):
+ * cpdef schemaless_reader(
+ *     fo,             # <<<<<<<<<<<<<<
+ *     writer_schema,
+ *     reader_schema=None,
  */
 struct __pyx_opt_args_8fastavro_5_read_schemaless_reader {
   int __pyx_n;
   PyObject *reader_schema;
   PyObject *return_record_name;
   PyObject *return_record_name_override;
+  PyObject *handle_unicode_errors;
+};
+struct __pyx_defaults {
+  PyObject *__pyx_arg_options;
 };
 
-/* "fastavro/_read.pyx":904
+/* "fastavro/_read.pyx":881
  * 
  * 
  * def _iter_avro_records(             # <<<<<<<<<<<<<<
  *     fo,
  *     header,
  */
 struct __pyx_obj_8fastavro_5_read___pyx_scope_struct___iter_avro_records {
@@ -1122,27 +1136,26 @@
   __pyx_t_8fastavro_5_read_long64 __pyx_v_block_count;
   PyObject *__pyx_v_block_fo;
   PyObject *__pyx_v_codec;
   PyObject *__pyx_v_fo;
   PyObject *__pyx_v_header;
   __pyx_t_8fastavro_5_read_int32 __pyx_v_i;
   PyObject *__pyx_v_named_schemas;
+  PyObject *__pyx_v_options;
   PyObject *__pyx_v_read_block;
   PyObject *__pyx_v_reader_schema;
-  PyObject *__pyx_v_return_record_name;
-  PyObject *__pyx_v_return_record_name_override;
   PyObject *__pyx_v_sync_marker;
   PyObject *__pyx_v_writer_schema;
   __pyx_t_8fastavro_5_read_long64 __pyx_t_0;
   __pyx_t_8fastavro_5_read_long64 __pyx_t_1;
   __pyx_t_8fastavro_5_read_int32 __pyx_t_2;
 };
 
 
-/* "fastavro/_read.pyx":940
+/* "fastavro/_read.pyx":915
  * 
  * 
  * def _iter_avro_blocks(             # <<<<<<<<<<<<<<
  *     fo,
  *     header,
  */
 struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks {
@@ -1150,26 +1163,25 @@
   PyObject *__pyx_v_block_bytes;
   PyObject *__pyx_v_codec;
   PyObject *__pyx_v_fo;
   PyObject *__pyx_v_header;
   PyObject *__pyx_v_named_schemas;
   __pyx_t_8fastavro_5_read_long64 __pyx_v_num_block_records;
   PyObject *__pyx_v_offset;
+  PyObject *__pyx_v_options;
   PyObject *__pyx_v_read_block;
   PyObject *__pyx_v_reader_schema;
-  PyObject *__pyx_v_return_record_name;
-  PyObject *__pyx_v_return_record_name_override;
   PyObject *__pyx_v_size;
   PyObject *__pyx_v_sync_marker;
   PyObject *__pyx_v_writer_schema;
 };
 
 
-/* "fastavro/_read.pyx":999
- *         self.return_record_name_override = return_record_name_override
+/* "fastavro/_read.pyx":972
+ *         self.options = options
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         for i in range(self.num_records):
  *             yield _read_data(
  */
 struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_2___iter__ {
   PyObject_HEAD
@@ -1531,21 +1543,14 @@
 /* BuildPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
                                                 int prepend_sign, char padding_char);
 
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_Py_ssize_t(Py_ssize_t value, Py_ssize_t width, char padding_char, char format_char);
 
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
@@ -1610,14 +1615,21 @@
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
 
 /* IterFinish.proto */
 static CYTHON_INLINE int __Pyx_IterFinish(void);
 
+/* PyObjectCallNoArg.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+#else
+#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+#endif
+
 /* PyObjectGetMethod.proto */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
 /* PyObjectCallMethod0.proto */
 static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
 
 /* RaiseNeedMoreValuesToUnpack.proto */
@@ -1940,15 +1952,15 @@
 static PyObject *__pyx_f_8fastavro_5_read_skip_int(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_read_float(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_skip_float(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_read_double(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_skip_double(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_read_bytes(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_skip_bytes(PyObject *, int __pyx_skip_dispatch); /*proto*/
-static PyObject *__pyx_f_8fastavro_5_read_read_utf8(PyObject *, int __pyx_skip_dispatch); /*proto*/
+static PyObject *__pyx_f_8fastavro_5_read_read_utf8(PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_8fastavro_5_read_read_utf8 *__pyx_optional_args); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_skip_utf8(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_read_fixed(PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_skip_fixed(PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_read_enum(PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_skip_enum(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_read_array(PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_8fastavro_5_read_read_array *__pyx_optional_args); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_skip_array(PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
@@ -1986,19 +1998,19 @@
 static PyObject *__pyx_builtin_NotImplementedError;
 static PyObject *__pyx_builtin_super;
 static PyObject *__pyx_builtin_open;
 static const char __pyx_k_[] = ".";
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_k[] = "k";
 static const char __pyx_k_v[] = "v";
-static const char __pyx_k__6[] = "+";
 static const char __pyx_k_fo[] = "fo";
 static const char __pyx_k_io[] = "io";
 static const char __pyx_k_rb[] = "rb";
 static const char __pyx_k_xz[] = "xz";
+static const char __pyx_k__12[] = "+";
 static const char __pyx_k_bz2[] = "bz2";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_lz4[] = "lz4";
 static const char __pyx_k_map[] = "map";
 static const char __pyx_k_str[] = "__str__";
@@ -2050,40 +2062,43 @@
 static const char __pyx_k_split[] = "split";
 static const char __pyx_k_super[] = "super";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_union[] = "union";
 static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_double[] = "double";
 static const char __pyx_k_encode[] = "encode";
+static const char __pyx_k_errors[] = "errors";
 static const char __pyx_k_fields[] = "fields";
 static const char __pyx_k_header[] = "header";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_is_not[] = " is not ";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_offset[] = "offset";
 static const char __pyx_k_reader[] = "reader";
 static const char __pyx_k_record[] = "record";
 static const char __pyx_k_schema[] = "_schema";
 static const char __pyx_k_size_2[] = " size";
 static const char __pyx_k_snappy[] = "snappy";
+static const char __pyx_k_strict[] = "strict";
 static const char __pyx_k_string[] = "string";
 static const char __pyx_k_tzinfo[] = "tzinfo";
 static const char __pyx_k_values[] = "values";
 static const char __pyx_k_writer[] = "writer";
 static const char __pyx_k_BytesIO[] = "BytesIO";
 static const char __pyx_k_Context[] = "Context";
 static const char __pyx_k_aliases[] = "aliases";
 static const char __pyx_k_boolean[] = "boolean";
 static const char __pyx_k_bytes_2[] = "bytes_";
 static const char __pyx_k_bytes_3[] = " bytes, ";
 static const char __pyx_k_codec_2[] = "codec: ";
 static const char __pyx_k_decimal[] = "decimal";
 static const char __pyx_k_default[] = "default";
 static const char __pyx_k_deflate[] = "deflate";
+static const char __pyx_k_options[] = "options";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_records[] = " records, ";
 static const char __pyx_k_symbols[] = "symbols";
 static const char __pyx_k_EOFError[] = "EOFError";
 static const char __pyx_k_Expected[] = "Expected ";
 static const char __pyx_k_block_fo[] = "block_fo";
 static const char __pyx_k_datetime[] = "datetime";
@@ -2173,14 +2188,15 @@
 static const char __pyx_k_block_reader___init[] = "block_reader.__init__";
 static const char __pyx_k_extract_record_type[] = "extract_record_type";
 static const char __pyx_k_No_default_value_for[] = "No default value for ";
 static const char __pyx_k_extract_logical_type[] = "extract_logical_type";
 static const char __pyx_k_ignore_default_error[] = "_ignore_default_error";
 static const char __pyx_k_zstandard_read_block[] = "zstandard_read_block";
 static const char __pyx_k_SchemaResolutionError[] = "SchemaResolutionError";
+static const char __pyx_k_handle_unicode_errors[] = "handle_unicode_errors";
 static const char __pyx_k_ignore_default_error_2[] = "ignore_default_error";
 static const char __pyx_k_size_is_different_than[] = " size is different than ";
 static const char __pyx_k_return_record_name_override[] = "return_record_name_override";
 static const char __pyx_k_expected_sync_marker_not_found[] = "expected sync marker not found";
 static const char __pyx_k_not_found_in_reader_symbol_list[] = " not found in reader symbol list ";
 static const char __pyx_k_Python_code_for_reading_AVRO_fil[] = "Python code for reading AVRO files";
 static const char __pyx_k_The_schema_attribute_is_deprecat[] = "The 'schema' attribute is deprecated. Please use 'writer_schema'";
@@ -2211,15 +2227,15 @@
 static PyObject *__pyx_n_s_SchemaResolutionError;
 static PyObject *__pyx_kp_u_Schema_mismatch;
 static PyObject *__pyx_n_s_StopIteration;
 static PyObject *__pyx_kp_u_The_schema_attribute_is_deprecat;
 static PyObject *__pyx_kp_u_Unrecognized_codec;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_ZstdDecompressor;
-static PyObject *__pyx_kp_u__6;
+static PyObject *__pyx_kp_u__12;
 static PyObject *__pyx_n_u_aliases;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_u_array;
 static PyObject *__pyx_kp_u_avro_codec;
 static PyObject *__pyx_kp_u_avro_schema;
 static PyObject *__pyx_n_s_block;
 static PyObject *__pyx_n_s_block_bytes;
@@ -2257,14 +2273,15 @@
 static PyObject *__pyx_n_s_elems;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_u_enum;
 static PyObject *__pyx_n_s_epoch;
 static PyObject *__pyx_n_s_epoch_naive;
 static PyObject *__pyx_n_u_error;
 static PyObject *__pyx_n_u_error_union;
+static PyObject *__pyx_n_s_errors;
 static PyObject *__pyx_kp_u_expected_sync_marker_not_found;
 static PyObject *__pyx_n_s_extract_logical_type;
 static PyObject *__pyx_n_s_extract_record_type;
 static PyObject *__pyx_n_s_fastavro__read;
 static PyObject *__pyx_kp_s_fastavro__read_pyx;
 static PyObject *__pyx_n_u_fields;
 static PyObject *__pyx_n_s_file_reader;
@@ -2274,14 +2291,16 @@
 static PyObject *__pyx_n_s_file_reader_schema;
 static PyObject *__pyx_n_u_fixed;
 static PyObject *__pyx_n_u_float;
 static PyObject *__pyx_n_s_fo;
 static PyObject *__pyx_n_s_force;
 static PyObject *__pyx_kp_u_from;
 static PyObject *__pyx_n_s_get;
+static PyObject *__pyx_n_s_handle_unicode_errors;
+static PyObject *__pyx_n_u_handle_unicode_errors;
 static PyObject *__pyx_n_s_header;
 static PyObject *__pyx_n_s_header_2;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_ignore_default_error;
 static PyObject *__pyx_n_s_ignore_default_error_2;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_init;
@@ -2321,14 +2340,15 @@
 static PyObject *__pyx_kp_u_not_found_in_reader_symbol_list;
 static PyObject *__pyx_n_u_null;
 static PyObject *__pyx_n_s_null_read_block;
 static PyObject *__pyx_n_s_num_block_records;
 static PyObject *__pyx_n_s_num_records;
 static PyObject *__pyx_n_s_offset;
 static PyObject *__pyx_n_s_open;
+static PyObject *__pyx_n_s_options;
 static PyObject *__pyx_n_s_parse_schema;
 static PyObject *__pyx_kp_u_position;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_property;
 static PyObject *__pyx_kp_u_python_snappy;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_r_schema;
@@ -2341,29 +2361,32 @@
 static PyObject *__pyx_n_u_reader;
 static PyObject *__pyx_n_s_reader___init;
 static PyObject *__pyx_n_s_reader_schema;
 static PyObject *__pyx_n_s_reader_type;
 static PyObject *__pyx_n_u_record;
 static PyObject *__pyx_kp_u_records;
 static PyObject *__pyx_n_s_return_record_name;
+static PyObject *__pyx_n_u_return_record_name;
 static PyObject *__pyx_n_s_return_record_name_override;
+static PyObject *__pyx_n_u_return_record_name_override;
 static PyObject *__pyx_n_s_schema;
 static PyObject *__pyx_n_s_schema_2;
 static PyObject *__pyx_kp_u_schema_mismatch;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_send;
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_u_size;
 static PyObject *__pyx_kp_u_size_2;
 static PyObject *__pyx_kp_u_size_is_different_than;
 static PyObject *__pyx_n_s_snappy;
 static PyObject *__pyx_n_u_snappy;
 static PyObject *__pyx_n_s_snappy_read_block;
 static PyObject *__pyx_n_s_split;
 static PyObject *__pyx_n_s_str;
+static PyObject *__pyx_n_u_strict;
 static PyObject *__pyx_n_u_string;
 static PyObject *__pyx_n_s_super;
 static PyObject *__pyx_n_u_symbols;
 static PyObject *__pyx_n_u_sync;
 static PyObject *__pyx_n_s_sync_marker;
 static PyObject *__pyx_n_s_tell;
 static PyObject *__pyx_n_s_test;
@@ -2400,95 +2423,100 @@
 static PyObject *__pyx_pf_8fastavro_5_read_16skip_int(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_18read_float(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_20skip_float(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_22read_double(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_24skip_double(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_26read_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_28skip_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_30read_utf8(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_30read_utf8(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_handle_unicode_errors); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_32skip_utf8(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_34read_fixed(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_36skip_fixed(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_38read_enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_reader_schema); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_40skip_enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_42read_array(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_42read_array(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_44skip_array(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_46read_map(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_46read_map(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_48skip_map(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_50read_union(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_50read_union(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_52skip_union(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_54read_record(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_54read_record(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_56skip_record(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_58maybe_promote(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_writer_type, PyObject *__pyx_v_reader_type); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_60_read_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_60_read_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_62_skip_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_64skip_sync(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_sync_marker); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_66null_read_block(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_68deflate_read_block(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_70bzip2_read_block(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_72xz_read_block(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_74snappy_read_block(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_76zstandard_read_block(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_78lz4_read_block(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_80_iter_avro_records(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_header, PyObject *__pyx_v_codec, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_83_iter_avro_blocks(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_header, PyObject *__pyx_v_codec, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_5Block___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_bytes_, PyObject *__pyx_v_num_records, PyObject *__pyx_v_codec, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_offset, PyObject *__pyx_v_size, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_80_iter_avro_records(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_header, PyObject *__pyx_v_codec, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_83_iter_avro_blocks(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_header, PyObject *__pyx_v_codec, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_5Block___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_bytes_, PyObject *__pyx_v_num_records, PyObject *__pyx_v_codec, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_offset, PyObject *__pyx_v_size, PyObject *__pyx_v_options); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_5Block_2__iter__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_5Block_5__str__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_11file_reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_90__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_11file_reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_11file_reader_2schema(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_11file_reader_4__iter__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_11file_reader_6__next__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_6reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_12block_reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
-static PyObject *__pyx_pf_8fastavro_5_read_86schemaless_reader(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_6reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override, PyObject *__pyx_v_handle_unicode_errors); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_12block_reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override, PyObject *__pyx_v_handle_unicode_errors); /* proto */
+static PyObject *__pyx_pf_8fastavro_5_read_86schemaless_reader(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override, PyObject *__pyx_v_handle_unicode_errors); /* proto */
 static PyObject *__pyx_pf_8fastavro_5_read_88is_avro(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path_or_buffer); /* proto */
 static PyObject *__pyx_tp_new_8fastavro_5_read___pyx_scope_struct___iter_avro_records(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_8fastavro_5_read___pyx_scope_struct_2___iter__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, &__pyx_n_s_get, 0, 0, 0};
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_4;
 static PyObject *__pyx_int_8;
 static PyObject *__pyx_int_1970;
 static PyObject *__pyx_int_neg_15;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_k__2;
+static PyObject *__pyx_k__3;
+static PyObject *__pyx_k__5;
+static PyObject *__pyx_k__6;
+static PyObject *__pyx_k__7;
+static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__11;
-static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
+static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
+static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__33;
-static PyObject *__pyx_tuple__34;
-static PyObject *__pyx_tuple__36;
-static PyObject *__pyx_codeobj__3;
-static PyObject *__pyx_codeobj__4;
-static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__21;
+static PyObject *__pyx_tuple__35;
+static PyObject *__pyx_tuple__37;
+static PyObject *__pyx_tuple__38;
+static PyObject *__pyx_tuple__40;
+static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__10;
+static PyObject *__pyx_codeobj__11;
 static PyObject *__pyx_codeobj__23;
 static PyObject *__pyx_codeobj__26;
 static PyObject *__pyx_codeobj__28;
 static PyObject *__pyx_codeobj__30;
 static PyObject *__pyx_codeobj__32;
-static PyObject *__pyx_codeobj__35;
+static PyObject *__pyx_codeobj__34;
+static PyObject *__pyx_codeobj__36;
+static PyObject *__pyx_codeobj__39;
 /* Late includes */
 
 /* "fastavro/_read.pyx":46
  * 
  * 
  * cpdef match_types(writer_type, reader_type):             # <<<<<<<<<<<<<<
  *     if isinstance(writer_type, list) or isinstance(reader_type, list):
@@ -6045,68 +6073,66 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "fastavro/_read.pyx":284
  * 
  * 
- * cpdef unicode read_utf8(fo):             # <<<<<<<<<<<<<<
+ * cpdef unicode read_utf8(fo, handle_unicode_errors="strict"):             # <<<<<<<<<<<<<<
  *     """A string is encoded as a long followed by that many bytes of UTF-8
  *     encoded character data.
  */
 
-static PyObject *__pyx_pw_8fastavro_5_read_31read_utf8(PyObject *__pyx_self, PyObject *__pyx_v_fo); /*proto*/
-static PyObject *__pyx_f_8fastavro_5_read_read_utf8(PyObject *__pyx_v_fo, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_8fastavro_5_read_31read_utf8(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_f_8fastavro_5_read_read_utf8(PyObject *__pyx_v_fo, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_8fastavro_5_read_read_utf8 *__pyx_optional_args) {
+  PyObject *__pyx_v_handle_unicode_errors = ((PyObject *)__pyx_n_u_strict);
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_utf8", 0);
+  if (__pyx_optional_args) {
+    if (__pyx_optional_args->__pyx_n > 0) {
+      __pyx_v_handle_unicode_errors = __pyx_optional_args->handle_unicode_errors;
+    }
+  }
 
   /* "fastavro/_read.pyx":288
  *     encoded character data.
  *     """
- *     return read_bytes(fo).decode()             # <<<<<<<<<<<<<<
+ *     return read_bytes(fo).decode(errors=handle_unicode_errors)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_f_8fastavro_5_read_read_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_decode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_errors, __pyx_v_handle_unicode_errors) < 0) __PYX_ERR(0, 288, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 288, __pyx_L1_error)
-  __pyx_r = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 288, __pyx_L1_error)
+  __pyx_r = ((PyObject*)__pyx_t_3);
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "fastavro/_read.pyx":284
  * 
  * 
- * cpdef unicode read_utf8(fo):             # <<<<<<<<<<<<<<
+ * cpdef unicode read_utf8(fo, handle_unicode_errors="strict"):             # <<<<<<<<<<<<<<
  *     """A string is encoded as a long followed by that many bytes of UTF-8
  *     encoded character data.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -6117,37 +6143,95 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8fastavro_5_read_31read_utf8(PyObject *__pyx_self, PyObject *__pyx_v_fo); /*proto*/
+static PyObject *__pyx_pw_8fastavro_5_read_31read_utf8(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_8fastavro_5_read_30read_utf8[] = "A string is encoded as a long followed by that many bytes of UTF-8\n    encoded character data.\n    ";
-static PyObject *__pyx_pw_8fastavro_5_read_31read_utf8(PyObject *__pyx_self, PyObject *__pyx_v_fo) {
+static PyObject *__pyx_pw_8fastavro_5_read_31read_utf8(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_fo = 0;
+  PyObject *__pyx_v_handle_unicode_errors = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_utf8 (wrapper)", 0);
-  __pyx_r = __pyx_pf_8fastavro_5_read_30read_utf8(__pyx_self, ((PyObject *)__pyx_v_fo));
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_handle_unicode_errors,0};
+    PyObject* values[2] = {0,0};
+    values[1] = ((PyObject *)__pyx_n_u_strict);
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_handle_unicode_errors);
+          if (value) { values[1] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_utf8") < 0)) __PYX_ERR(0, 284, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_fo = values[0];
+    __pyx_v_handle_unicode_errors = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("read_utf8", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 284, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("fastavro._read.read_utf8", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8fastavro_5_read_30read_utf8(__pyx_self, __pyx_v_fo, __pyx_v_handle_unicode_errors);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_30read_utf8(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo) {
+static PyObject *__pyx_pf_8fastavro_5_read_30read_utf8(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_handle_unicode_errors) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  struct __pyx_opt_args_8fastavro_5_read_read_utf8 __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_utf8", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_utf8(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_2.__pyx_n = 1;
+  __pyx_t_2.handle_unicode_errors = __pyx_v_handle_unicode_errors;
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_utf8(__pyx_v_fo, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7130,36 +7214,19 @@
 static PyObject *__pyx_pw_8fastavro_5_read_43read_array(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_read_array(PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_8fastavro_5_read_read_array *__pyx_optional_args) {
 
   /* "fastavro/_read.pyx":341
  *     writer_schema,
  *     named_schemas,
  *     reader_schema=None,             # <<<<<<<<<<<<<<
- *     return_record_name=False,
- *     return_record_name_override=False,
- */
-  PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
-
-  /* "fastavro/_read.pyx":342
- *     named_schemas,
- *     reader_schema=None,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
+ *     options={},
  * ):
  */
-  PyObject *__pyx_v_return_record_name = ((PyObject *)Py_False);
-
-  /* "fastavro/_read.pyx":343
- *     reader_schema=None,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
- * ):
- *     """Arrays are encoded as a series of blocks.
- */
-  PyObject *__pyx_v_return_record_name_override = ((PyObject *)Py_False);
+  PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
+  PyObject *__pyx_v_options = __pyx_k__2;
   PyObject *__pyx_v_read_items = 0;
   __pyx_t_8fastavro_5_read_long64 __pyx_v_block_count;
   CYTHON_UNUSED __pyx_t_8fastavro_5_read_long64 __pyx_v_i;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __pyx_t_8fastavro_5_read_long64 __pyx_t_2;
@@ -7174,218 +7241,213 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_array", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_reader_schema = __pyx_optional_args->reader_schema;
       if (__pyx_optional_args->__pyx_n > 1) {
-        __pyx_v_return_record_name = __pyx_optional_args->return_record_name;
-        if (__pyx_optional_args->__pyx_n > 2) {
-          __pyx_v_return_record_name_override = __pyx_optional_args->return_record_name_override;
-        }
+        __pyx_v_options = __pyx_optional_args->options;
       }
     }
   }
 
-  /* "fastavro/_read.pyx":359
+  /* "fastavro/_read.pyx":358
  *     cdef long64 i
  * 
  *     read_items = []             # <<<<<<<<<<<<<<
  * 
  *     block_count = read_long(fo)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_read_items = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":361
+  /* "fastavro/_read.pyx":360
  *     read_items = []
  * 
  *     block_count = read_long(fo)             # <<<<<<<<<<<<<<
  * 
  *     while block_count != 0:
  */
-  __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 360, __pyx_L1_error)
   __pyx_v_block_count = __pyx_t_2;
 
-  /* "fastavro/_read.pyx":363
+  /* "fastavro/_read.pyx":362
  *     block_count = read_long(fo)
  * 
  *     while block_count != 0:             # <<<<<<<<<<<<<<
  *         if block_count < 0:
  *             block_count = -block_count
  */
   while (1) {
     __pyx_t_3 = ((__pyx_v_block_count != 0) != 0);
     if (!__pyx_t_3) break;
 
-    /* "fastavro/_read.pyx":364
+    /* "fastavro/_read.pyx":363
  * 
  *     while block_count != 0:
  *         if block_count < 0:             # <<<<<<<<<<<<<<
  *             block_count = -block_count
  *             # Read block size, unused
  */
     __pyx_t_3 = ((__pyx_v_block_count < 0) != 0);
     if (__pyx_t_3) {
 
-      /* "fastavro/_read.pyx":365
+      /* "fastavro/_read.pyx":364
  *     while block_count != 0:
  *         if block_count < 0:
  *             block_count = -block_count             # <<<<<<<<<<<<<<
  *             # Read block size, unused
  *             read_long(fo)
  */
       __pyx_v_block_count = (-__pyx_v_block_count);
 
-      /* "fastavro/_read.pyx":367
+      /* "fastavro/_read.pyx":366
  *             block_count = -block_count
  *             # Read block size, unused
  *             read_long(fo)             # <<<<<<<<<<<<<<
  * 
  *         if reader_schema:
  */
-      __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 367, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L1_error)
 
-      /* "fastavro/_read.pyx":364
+      /* "fastavro/_read.pyx":363
  * 
  *     while block_count != 0:
  *         if block_count < 0:             # <<<<<<<<<<<<<<
  *             block_count = -block_count
  *             # Read block size, unused
  */
     }
 
-    /* "fastavro/_read.pyx":369
+    /* "fastavro/_read.pyx":368
  *             read_long(fo)
  * 
  *         if reader_schema:             # <<<<<<<<<<<<<<
  *             for i in range(block_count):
  *                 read_items.append(_read_data(
  */
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 368, __pyx_L1_error)
     if (__pyx_t_3) {
 
-      /* "fastavro/_read.pyx":370
+      /* "fastavro/_read.pyx":369
  * 
  *         if reader_schema:
  *             for i in range(block_count):             # <<<<<<<<<<<<<<
  *                 read_items.append(_read_data(
  *                     fo,
  */
       __pyx_t_2 = __pyx_v_block_count;
       __pyx_t_4 = __pyx_t_2;
       for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
         __pyx_v_i = __pyx_t_5;
 
-        /* "fastavro/_read.pyx":373
+        /* "fastavro/_read.pyx":372
  *                 read_items.append(_read_data(
  *                     fo,
  *                     writer_schema["items"],             # <<<<<<<<<<<<<<
  *                     named_schemas,
  *                     reader_schema["items"],
  */
-        __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_items); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_items); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
 
-        /* "fastavro/_read.pyx":375
+        /* "fastavro/_read.pyx":374
  *                     writer_schema["items"],
  *                     named_schemas,
  *                     reader_schema["items"],             # <<<<<<<<<<<<<<
- *                     return_record_name,
- *                     return_record_name_override,
+ *                     options,
+ *                 ))
  */
-        __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_reader_schema, __pyx_n_u_items); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 375, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_reader_schema, __pyx_n_u_items); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "fastavro/_read.pyx":371
+        /* "fastavro/_read.pyx":370
  *         if reader_schema:
  *             for i in range(block_count):
  *                 read_items.append(_read_data(             # <<<<<<<<<<<<<<
  *                     fo,
  *                     writer_schema["items"],
  */
-        __pyx_t_8.__pyx_n = 3;
+        __pyx_t_8.__pyx_n = 2;
         __pyx_t_8.reader_schema = __pyx_t_6;
-        __pyx_t_8.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_8.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_7 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_1, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 371, __pyx_L1_error)
+        __pyx_t_8.options = __pyx_v_options;
+        __pyx_t_7 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_1, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 370, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_read_items, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 371, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_read_items, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 370, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
 
-      /* "fastavro/_read.pyx":369
+      /* "fastavro/_read.pyx":368
  *             read_long(fo)
  * 
  *         if reader_schema:             # <<<<<<<<<<<<<<
  *             for i in range(block_count):
  *                 read_items.append(_read_data(
  */
       goto __pyx_L6;
     }
 
-    /* "fastavro/_read.pyx":380
+    /* "fastavro/_read.pyx":378
  *                 ))
  *         else:
  *             for i in range(block_count):             # <<<<<<<<<<<<<<
  *                 read_items.append(_read_data(
  *                     fo,
  */
     /*else*/ {
       __pyx_t_2 = __pyx_v_block_count;
       __pyx_t_4 = __pyx_t_2;
       for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
         __pyx_v_i = __pyx_t_5;
 
-        /* "fastavro/_read.pyx":383
+        /* "fastavro/_read.pyx":381
  *                 read_items.append(_read_data(
  *                     fo,
  *                     writer_schema["items"],             # <<<<<<<<<<<<<<
  *                     named_schemas,
  *                     None,
  */
-        __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_items); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 383, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_items); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 381, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
 
-        /* "fastavro/_read.pyx":381
+        /* "fastavro/_read.pyx":379
  *         else:
  *             for i in range(block_count):
  *                 read_items.append(_read_data(             # <<<<<<<<<<<<<<
  *                     fo,
  *                     writer_schema["items"],
  */
-        __pyx_t_8.__pyx_n = 3;
+        __pyx_t_8.__pyx_n = 2;
         __pyx_t_8.reader_schema = Py_None;
-        __pyx_t_8.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_8.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_6 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_7, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 381, __pyx_L1_error)
+        __pyx_t_8.options = __pyx_v_options;
+        __pyx_t_6 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_7, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_read_items, __pyx_t_6); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 381, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_read_items, __pyx_t_6); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 379, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
     }
     __pyx_L6:;
 
-    /* "fastavro/_read.pyx":389
- *                     return_record_name_override,
+    /* "fastavro/_read.pyx":386
+ *                     options,
  *                 ))
  *         block_count = read_long(fo)             # <<<<<<<<<<<<<<
  * 
  *     return read_items
  */
-    __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 389, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L1_error)
     __pyx_v_block_count = __pyx_t_2;
   }
 
-  /* "fastavro/_read.pyx":391
+  /* "fastavro/_read.pyx":388
  *         block_count = read_long(fo)
  * 
  *     return read_items             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
@@ -7419,58 +7481,38 @@
 static PyObject *__pyx_pw_8fastavro_5_read_43read_array(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_8fastavro_5_read_42read_array[] = "Arrays are encoded as a series of blocks.\n\n    Each block consists of a long count value, followed by that many array\n    items.  A block with count zero indicates the end of the array.  Each item\n    is encoded per the array's item schema.\n\n    If a block's count is negative, then the count is followed immediately by a\n    long block size, indicating the number of bytes in the block.  The actual\n    count in this case is the absolute value of the count written.\n    ";
 static PyObject *__pyx_pw_8fastavro_5_read_43read_array(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_writer_schema = 0;
   PyObject *__pyx_v_named_schemas = 0;
   PyObject *__pyx_v_reader_schema = 0;
-  PyObject *__pyx_v_return_record_name = 0;
-  PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_options = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_array (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_options,0};
+    PyObject* values[5] = {0,0,0,0,0};
 
     /* "fastavro/_read.pyx":341
  *     writer_schema,
  *     named_schemas,
  *     reader_schema=None,             # <<<<<<<<<<<<<<
- *     return_record_name=False,
- *     return_record_name_override=False,
- */
-    values[3] = ((PyObject *)Py_None);
-
-    /* "fastavro/_read.pyx":342
- *     named_schemas,
- *     reader_schema=None,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
+ *     options={},
  * ):
  */
-    values[4] = ((PyObject *)Py_False);
-
-    /* "fastavro/_read.pyx":343
- *     reader_schema=None,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
- * ):
- *     """Arrays are encoded as a series of blocks.
- */
-    values[5] = ((PyObject *)Py_False);
+    values[3] = ((PyObject *)Py_None);
+    values[4] = __pyx_k__2;
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -7485,48 +7527,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_array", 0, 3, 6, 1); __PYX_ERR(0, 337, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_array", 0, 3, 5, 1); __PYX_ERR(0, 337, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_array", 0, 3, 6, 2); __PYX_ERR(0, 337, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_array", 0, 3, 5, 2); __PYX_ERR(0, 337, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema);
           if (value) { values[3] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name);
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options);
           if (value) { values[4] = value; kw_args--; }
         }
-        CYTHON_FALLTHROUGH;
-        case  5:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
-          if (value) { values[5] = value; kw_args--; }
-        }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_array") < 0)) __PYX_ERR(0, 337, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -7534,54 +7568,52 @@
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_named_schemas = values[2];
     __pyx_v_reader_schema = values[3];
-    __pyx_v_return_record_name = values[4];
-    __pyx_v_return_record_name_override = values[5];
+    __pyx_v_options = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_array", 0, 3, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 337, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_array", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 337, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.read_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_42read_array(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
+  __pyx_r = __pyx_pf_8fastavro_5_read_42read_array(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_options);
 
   /* "fastavro/_read.pyx":337
  * 
  * 
  * cpdef read_array(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_42read_array(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_42read_array(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_8fastavro_5_read_read_array __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_array", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2.__pyx_n = 3;
+  __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.reader_schema = __pyx_v_reader_schema;
-  __pyx_t_2.return_record_name = __pyx_v_return_record_name;
-  __pyx_t_2.return_record_name_override = __pyx_v_return_record_name_override;
+  __pyx_t_2.options = __pyx_v_options;
   __pyx_t_1 = __pyx_f_8fastavro_5_read_read_array(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
@@ -7591,15 +7623,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":394
+/* "fastavro/_read.pyx":391
  * 
  * 
  * cpdef skip_array(fo, writer_schema, named_schemas):             # <<<<<<<<<<<<<<
  *     """Arrays are encoded as a series of blocks.
  * 
  */
 
@@ -7619,136 +7651,136 @@
   __pyx_t_8fastavro_5_read_long64 __pyx_t_7;
   __pyx_t_8fastavro_5_read_long64 __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("skip_array", 0);
 
-  /* "fastavro/_read.pyx":408
+  /* "fastavro/_read.pyx":405
  *     cdef long64 i
  * 
  *     block_count = read_long(fo)             # <<<<<<<<<<<<<<
  * 
  *     while block_count != 0:
  */
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 405, __pyx_L1_error)
   __pyx_v_block_count = __pyx_t_1;
 
-  /* "fastavro/_read.pyx":410
+  /* "fastavro/_read.pyx":407
  *     block_count = read_long(fo)
  * 
  *     while block_count != 0:             # <<<<<<<<<<<<<<
  *         if block_count < 0:
  *             block_size = read_long(fo)
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_block_count != 0) != 0);
     if (!__pyx_t_2) break;
 
-    /* "fastavro/_read.pyx":411
+    /* "fastavro/_read.pyx":408
  * 
  *     while block_count != 0:
  *         if block_count < 0:             # <<<<<<<<<<<<<<
  *             block_size = read_long(fo)
  *             fo.read(block_size)
  */
     __pyx_t_2 = ((__pyx_v_block_count < 0) != 0);
     if (__pyx_t_2) {
 
-      /* "fastavro/_read.pyx":412
+      /* "fastavro/_read.pyx":409
  *     while block_count != 0:
  *         if block_count < 0:
  *             block_size = read_long(fo)             # <<<<<<<<<<<<<<
  *             fo.read(block_size)
  *         else:
  */
-      __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 412, __pyx_L1_error)
+      __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 409, __pyx_L1_error)
       __pyx_v_block_size = __pyx_t_1;
 
-      /* "fastavro/_read.pyx":413
+      /* "fastavro/_read.pyx":410
  *         if block_count < 0:
  *             block_size = read_long(fo)
  *             fo.read(block_size)             # <<<<<<<<<<<<<<
  *         else:
  *             for i in range(block_count):
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_block_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_block_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "fastavro/_read.pyx":411
+      /* "fastavro/_read.pyx":408
  * 
  *     while block_count != 0:
  *         if block_count < 0:             # <<<<<<<<<<<<<<
  *             block_size = read_long(fo)
  *             fo.read(block_size)
  */
       goto __pyx_L5;
     }
 
-    /* "fastavro/_read.pyx":415
+    /* "fastavro/_read.pyx":412
  *             fo.read(block_size)
  *         else:
  *             for i in range(block_count):             # <<<<<<<<<<<<<<
  *                 _skip_data(fo, writer_schema["items"], named_schemas)
  * 
  */
     /*else*/ {
       __pyx_t_1 = __pyx_v_block_count;
       __pyx_t_7 = __pyx_t_1;
       for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
         __pyx_v_i = __pyx_t_8;
 
-        /* "fastavro/_read.pyx":416
+        /* "fastavro/_read.pyx":413
  *         else:
  *             for i in range(block_count):
  *                 _skip_data(fo, writer_schema["items"], named_schemas)             # <<<<<<<<<<<<<<
  * 
  *         block_count = read_long(fo)
  */
-        __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_3, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 416, __pyx_L1_error)
+        __pyx_t_4 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_3, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
     }
     __pyx_L5:;
 
-    /* "fastavro/_read.pyx":418
+    /* "fastavro/_read.pyx":415
  *                 _skip_data(fo, writer_schema["items"], named_schemas)
  * 
  *         block_count = read_long(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
     __pyx_v_block_count = __pyx_t_1;
   }
 
-  /* "fastavro/_read.pyx":394
+  /* "fastavro/_read.pyx":391
  * 
  * 
  * cpdef skip_array(fo, writer_schema, named_schemas):             # <<<<<<<<<<<<<<
  *     """Arrays are encoded as a series of blocks.
  * 
  */
 
@@ -7802,40 +7834,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("skip_array", 1, 3, 3, 1); __PYX_ERR(0, 394, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("skip_array", 1, 3, 3, 1); __PYX_ERR(0, 391, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("skip_array", 1, 3, 3, 2); __PYX_ERR(0, 394, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("skip_array", 1, 3, 3, 2); __PYX_ERR(0, 391, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "skip_array") < 0)) __PYX_ERR(0, 394, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "skip_array") < 0)) __PYX_ERR(0, 391, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_named_schemas = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("skip_array", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 394, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("skip_array", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 391, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.skip_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8fastavro_5_read_44skip_array(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas);
 
@@ -7849,15 +7881,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("skip_array", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_array(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 394, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_array(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 391, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7866,325 +7898,320 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":421
+/* "fastavro/_read.pyx":418
  * 
  * 
  * cpdef read_map(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
 static PyObject *__pyx_pw_8fastavro_5_read_47read_map(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_read_map(PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_8fastavro_5_read_read_map *__pyx_optional_args) {
 
-  /* "fastavro/_read.pyx":425
+  /* "fastavro/_read.pyx":422
  *     writer_schema,
  *     named_schemas,
  *     reader_schema=None,             # <<<<<<<<<<<<<<
- *     return_record_name=False,
- *     return_record_name_override=False,
- */
-  PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
-
-  /* "fastavro/_read.pyx":426
- *     named_schemas,
- *     reader_schema=None,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
- * ):
- */
-  PyObject *__pyx_v_return_record_name = ((PyObject *)Py_False);
-
-  /* "fastavro/_read.pyx":427
- *     reader_schema=None,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
+ *     options={},
  * ):
- *     """Maps are encoded as a series of blocks.
  */
-  PyObject *__pyx_v_return_record_name_override = ((PyObject *)Py_False);
+  PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
+  PyObject *__pyx_v_options = __pyx_k__3;
   PyObject *__pyx_v_read_items = 0;
   __pyx_t_8fastavro_5_read_long64 __pyx_v_block_count;
   CYTHON_UNUSED __pyx_t_8fastavro_5_read_long64 __pyx_v_i;
   PyObject *__pyx_v_key = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __pyx_t_8fastavro_5_read_long64 __pyx_t_2;
   int __pyx_t_3;
   __pyx_t_8fastavro_5_read_long64 __pyx_t_4;
   __pyx_t_8fastavro_5_read_long64 __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  struct __pyx_opt_args_8fastavro_5_read__read_data __pyx_t_8;
+  struct __pyx_opt_args_8fastavro_5_read_read_utf8 __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  struct __pyx_opt_args_8fastavro_5_read__read_data __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_map", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_reader_schema = __pyx_optional_args->reader_schema;
       if (__pyx_optional_args->__pyx_n > 1) {
-        __pyx_v_return_record_name = __pyx_optional_args->return_record_name;
-        if (__pyx_optional_args->__pyx_n > 2) {
-          __pyx_v_return_record_name_override = __pyx_optional_args->return_record_name_override;
-        }
+        __pyx_v_options = __pyx_optional_args->options;
       }
     }
   }
 
-  /* "fastavro/_read.pyx":444
+  /* "fastavro/_read.pyx":440
  *     cdef unicode key
  * 
  *     read_items = {}             # <<<<<<<<<<<<<<
  *     block_count = read_long(fo)
  *     while block_count != 0:
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_read_items = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":445
+  /* "fastavro/_read.pyx":441
  * 
  *     read_items = {}
  *     block_count = read_long(fo)             # <<<<<<<<<<<<<<
  *     while block_count != 0:
  *         if block_count < 0:
  */
-  __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 445, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L1_error)
   __pyx_v_block_count = __pyx_t_2;
 
-  /* "fastavro/_read.pyx":446
+  /* "fastavro/_read.pyx":442
  *     read_items = {}
  *     block_count = read_long(fo)
  *     while block_count != 0:             # <<<<<<<<<<<<<<
  *         if block_count < 0:
  *             block_count = -block_count
  */
   while (1) {
     __pyx_t_3 = ((__pyx_v_block_count != 0) != 0);
     if (!__pyx_t_3) break;
 
-    /* "fastavro/_read.pyx":447
+    /* "fastavro/_read.pyx":443
  *     block_count = read_long(fo)
  *     while block_count != 0:
  *         if block_count < 0:             # <<<<<<<<<<<<<<
  *             block_count = -block_count
  *             # Read block size, unused
  */
     __pyx_t_3 = ((__pyx_v_block_count < 0) != 0);
     if (__pyx_t_3) {
 
-      /* "fastavro/_read.pyx":448
+      /* "fastavro/_read.pyx":444
  *     while block_count != 0:
  *         if block_count < 0:
  *             block_count = -block_count             # <<<<<<<<<<<<<<
  *             # Read block size, unused
  *             read_long(fo)
  */
       __pyx_v_block_count = (-__pyx_v_block_count);
 
-      /* "fastavro/_read.pyx":450
+      /* "fastavro/_read.pyx":446
  *             block_count = -block_count
  *             # Read block size, unused
  *             read_long(fo)             # <<<<<<<<<<<<<<
  * 
  *         if reader_schema:
  */
-      __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 450, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 446, __pyx_L1_error)
 
-      /* "fastavro/_read.pyx":447
+      /* "fastavro/_read.pyx":443
  *     block_count = read_long(fo)
  *     while block_count != 0:
  *         if block_count < 0:             # <<<<<<<<<<<<<<
  *             block_count = -block_count
  *             # Read block size, unused
  */
     }
 
-    /* "fastavro/_read.pyx":452
+    /* "fastavro/_read.pyx":448
  *             read_long(fo)
  * 
  *         if reader_schema:             # <<<<<<<<<<<<<<
  *             for i in range(block_count):
- *                 key = read_utf8(fo)
+ *                 key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  */
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 452, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 448, __pyx_L1_error)
     if (__pyx_t_3) {
 
-      /* "fastavro/_read.pyx":453
+      /* "fastavro/_read.pyx":449
  * 
  *         if reader_schema:
  *             for i in range(block_count):             # <<<<<<<<<<<<<<
- *                 key = read_utf8(fo)
+ *                 key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  *                 read_items[key] = _read_data(
  */
       __pyx_t_2 = __pyx_v_block_count;
       __pyx_t_4 = __pyx_t_2;
       for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
         __pyx_v_i = __pyx_t_5;
 
-        /* "fastavro/_read.pyx":454
+        /* "fastavro/_read.pyx":450
  *         if reader_schema:
  *             for i in range(block_count):
- *                 key = read_utf8(fo)             # <<<<<<<<<<<<<<
+ *                 key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))             # <<<<<<<<<<<<<<
  *                 read_items[key] = _read_data(
  *                     fo,
  */
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_utf8(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_options, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 450, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_7.__pyx_n = 1;
+        __pyx_t_7.handle_unicode_errors = __pyx_t_6;
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_utf8(__pyx_v_fo, 0, &__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_XDECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_1));
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":457
+        /* "fastavro/_read.pyx":453
  *                 read_items[key] = _read_data(
  *                     fo,
  *                     writer_schema["values"],             # <<<<<<<<<<<<<<
  *                     named_schemas,
  *                     reader_schema["values"],
  */
-        __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 453, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
 
-        /* "fastavro/_read.pyx":459
+        /* "fastavro/_read.pyx":455
  *                     writer_schema["values"],
  *                     named_schemas,
  *                     reader_schema["values"],             # <<<<<<<<<<<<<<
- *                     return_record_name,
- *                     return_record_name_override,
+ *                     options,
+ *                 )
  */
-        __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_reader_schema, __pyx_n_u_values); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 459, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_reader_schema, __pyx_n_u_values); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 455, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "fastavro/_read.pyx":455
+        /* "fastavro/_read.pyx":451
  *             for i in range(block_count):
- *                 key = read_utf8(fo)
+ *                 key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  *                 read_items[key] = _read_data(             # <<<<<<<<<<<<<<
  *                     fo,
  *                     writer_schema["values"],
  */
-        __pyx_t_8.__pyx_n = 3;
-        __pyx_t_8.reader_schema = __pyx_t_6;
-        __pyx_t_8.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_8.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_7 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_1, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 455, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_9.__pyx_n = 2;
+        __pyx_t_9.reader_schema = __pyx_t_6;
+        __pyx_t_9.options = __pyx_v_options;
+        __pyx_t_8 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_1, __pyx_v_named_schemas, 0, &__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 451, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(PyDict_SetItem(__pyx_v_read_items, __pyx_v_key, __pyx_t_7) < 0)) __PYX_ERR(0, 455, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        if (unlikely(PyDict_SetItem(__pyx_v_read_items, __pyx_v_key, __pyx_t_8) < 0)) __PYX_ERR(0, 451, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
 
-      /* "fastavro/_read.pyx":452
+      /* "fastavro/_read.pyx":448
  *             read_long(fo)
  * 
  *         if reader_schema:             # <<<<<<<<<<<<<<
  *             for i in range(block_count):
- *                 key = read_utf8(fo)
+ *                 key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  */
       goto __pyx_L6;
     }
 
-    /* "fastavro/_read.pyx":464
+    /* "fastavro/_read.pyx":459
  *                 )
  *         else:
  *             for i in range(block_count):             # <<<<<<<<<<<<<<
- *                 key = read_utf8(fo)
+ *                 key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  *                 read_items[key] = _read_data(
  */
     /*else*/ {
       __pyx_t_2 = __pyx_v_block_count;
       __pyx_t_4 = __pyx_t_2;
       for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
         __pyx_v_i = __pyx_t_5;
 
-        /* "fastavro/_read.pyx":465
+        /* "fastavro/_read.pyx":460
  *         else:
  *             for i in range(block_count):
- *                 key = read_utf8(fo)             # <<<<<<<<<<<<<<
+ *                 key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))             # <<<<<<<<<<<<<<
  *                 read_items[key] = _read_data(
  *                     fo,
  */
-        __pyx_t_7 = __pyx_f_8fastavro_5_read_read_utf8(__pyx_v_fo, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 465, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __Pyx_XDECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_7));
-        __pyx_t_7 = 0;
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_options, __pyx_n_s_get); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 460, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 460, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_7.__pyx_n = 1;
+        __pyx_t_7.handle_unicode_errors = __pyx_t_6;
+        __pyx_t_8 = __pyx_f_8fastavro_5_read_read_utf8(__pyx_v_fo, 0, &__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 460, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_8));
+        __pyx_t_8 = 0;
 
-        /* "fastavro/_read.pyx":468
+        /* "fastavro/_read.pyx":463
  *                 read_items[key] = _read_data(
  *                     fo,
  *                     writer_schema["values"],             # <<<<<<<<<<<<<<
  *                     named_schemas,
  *                     None,
  */
-        __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_values); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 468, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_values); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 463, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
 
-        /* "fastavro/_read.pyx":466
+        /* "fastavro/_read.pyx":461
  *             for i in range(block_count):
- *                 key = read_utf8(fo)
+ *                 key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  *                 read_items[key] = _read_data(             # <<<<<<<<<<<<<<
  *                     fo,
  *                     writer_schema["values"],
  */
-        __pyx_t_8.__pyx_n = 3;
-        __pyx_t_8.reader_schema = Py_None;
-        __pyx_t_8.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_8.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_6 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_7, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 466, __pyx_L1_error)
+        __pyx_t_9.__pyx_n = 2;
+        __pyx_t_9.reader_schema = Py_None;
+        __pyx_t_9.options = __pyx_v_options;
+        __pyx_t_6 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_8, __pyx_v_named_schemas, 0, &__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 461, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(PyDict_SetItem(__pyx_v_read_items, __pyx_v_key, __pyx_t_6) < 0)) __PYX_ERR(0, 466, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        if (unlikely(PyDict_SetItem(__pyx_v_read_items, __pyx_v_key, __pyx_t_6) < 0)) __PYX_ERR(0, 461, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
     }
     __pyx_L6:;
 
-    /* "fastavro/_read.pyx":474
- *                     return_record_name_override,
+    /* "fastavro/_read.pyx":468
+ *                     options,
  *                 )
  *         block_count = read_long(fo)             # <<<<<<<<<<<<<<
  * 
  *     return read_items
  */
-    __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 474, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_2 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 468, __pyx_L1_error)
     __pyx_v_block_count = __pyx_t_2;
   }
 
-  /* "fastavro/_read.pyx":476
+  /* "fastavro/_read.pyx":470
  *         block_count = read_long(fo)
  * 
  *     return read_items             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_read_items);
   __pyx_r = __pyx_v_read_items;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":421
+  /* "fastavro/_read.pyx":418
  * 
  * 
  * cpdef read_map(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("fastavro._read.read_map", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_read_items);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -8195,58 +8222,38 @@
 static PyObject *__pyx_pw_8fastavro_5_read_47read_map(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_8fastavro_5_read_46read_map[] = "Maps are encoded as a series of blocks.\n\n    Each block consists of a long count value, followed by that many key/value\n    pairs.  A block with count zero indicates the end of the map.  Each item is\n    encoded per the map's value schema.\n\n    If a block's count is negative, then the count is followed immediately by a\n    long block size, indicating the number of bytes in the block.  The actual\n    count in this case is the absolute value of the count written.\n    ";
 static PyObject *__pyx_pw_8fastavro_5_read_47read_map(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_writer_schema = 0;
   PyObject *__pyx_v_named_schemas = 0;
   PyObject *__pyx_v_reader_schema = 0;
-  PyObject *__pyx_v_return_record_name = 0;
-  PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_options = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_map (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_options,0};
+    PyObject* values[5] = {0,0,0,0,0};
 
-    /* "fastavro/_read.pyx":425
+    /* "fastavro/_read.pyx":422
  *     writer_schema,
  *     named_schemas,
  *     reader_schema=None,             # <<<<<<<<<<<<<<
- *     return_record_name=False,
- *     return_record_name_override=False,
- */
-    values[3] = ((PyObject *)Py_None);
-
-    /* "fastavro/_read.pyx":426
- *     named_schemas,
- *     reader_schema=None,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
+ *     options={},
  * ):
  */
-    values[4] = ((PyObject *)Py_False);
-
-    /* "fastavro/_read.pyx":427
- *     reader_schema=None,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
- * ):
- *     """Maps are encoded as a series of blocks.
- */
-    values[5] = ((PyObject *)Py_False);
+    values[3] = ((PyObject *)Py_None);
+    values[4] = __pyx_k__3;
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -8261,48 +8268,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_map", 0, 3, 6, 1); __PYX_ERR(0, 421, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_map", 0, 3, 5, 1); __PYX_ERR(0, 418, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_map", 0, 3, 6, 2); __PYX_ERR(0, 421, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_map", 0, 3, 5, 2); __PYX_ERR(0, 418, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema);
           if (value) { values[3] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name);
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options);
           if (value) { values[4] = value; kw_args--; }
         }
-        CYTHON_FALLTHROUGH;
-        case  5:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
-          if (value) { values[5] = value; kw_args--; }
-        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_map") < 0)) __PYX_ERR(0, 421, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_map") < 0)) __PYX_ERR(0, 418, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -8310,55 +8309,53 @@
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_named_schemas = values[2];
     __pyx_v_reader_schema = values[3];
-    __pyx_v_return_record_name = values[4];
-    __pyx_v_return_record_name_override = values[5];
+    __pyx_v_options = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_map", 0, 3, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 421, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_map", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 418, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.read_map", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_46read_map(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
+  __pyx_r = __pyx_pf_8fastavro_5_read_46read_map(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_options);
 
-  /* "fastavro/_read.pyx":421
+  /* "fastavro/_read.pyx":418
  * 
  * 
  * cpdef read_map(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_46read_map(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_46read_map(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_8fastavro_5_read_read_map __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_map", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2.__pyx_n = 3;
+  __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.reader_schema = __pyx_v_reader_schema;
-  __pyx_t_2.return_record_name = __pyx_v_return_record_name;
-  __pyx_t_2.return_record_name_override = __pyx_v_return_record_name_override;
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_map(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_2.options = __pyx_v_options;
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_map(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8367,15 +8364,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":479
+/* "fastavro/_read.pyx":473
  * 
  * 
  * cpdef skip_map(fo, writer_schema, named_schemas):             # <<<<<<<<<<<<<<
  *     """Maps are encoded as a series of blocks.
  * 
  */
 
@@ -8395,147 +8392,147 @@
   __pyx_t_8fastavro_5_read_long64 __pyx_t_7;
   __pyx_t_8fastavro_5_read_long64 __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("skip_map", 0);
 
-  /* "fastavro/_read.pyx":493
+  /* "fastavro/_read.pyx":487
  *     cdef long64 i
  * 
  *     block_count = read_long(fo)             # <<<<<<<<<<<<<<
  *     while block_count != 0:
  *         if block_count < 0:
  */
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 487, __pyx_L1_error)
   __pyx_v_block_count = __pyx_t_1;
 
-  /* "fastavro/_read.pyx":494
+  /* "fastavro/_read.pyx":488
  * 
  *     block_count = read_long(fo)
  *     while block_count != 0:             # <<<<<<<<<<<<<<
  *         if block_count < 0:
  *             block_size = read_long(fo)
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_block_count != 0) != 0);
     if (!__pyx_t_2) break;
 
-    /* "fastavro/_read.pyx":495
+    /* "fastavro/_read.pyx":489
  *     block_count = read_long(fo)
  *     while block_count != 0:
  *         if block_count < 0:             # <<<<<<<<<<<<<<
  *             block_size = read_long(fo)
  *             fo.read(block_size)
  */
     __pyx_t_2 = ((__pyx_v_block_count < 0) != 0);
     if (__pyx_t_2) {
 
-      /* "fastavro/_read.pyx":496
+      /* "fastavro/_read.pyx":490
  *     while block_count != 0:
  *         if block_count < 0:
  *             block_size = read_long(fo)             # <<<<<<<<<<<<<<
  *             fo.read(block_size)
  *         else:
  */
-      __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 496, __pyx_L1_error)
+      __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 490, __pyx_L1_error)
       __pyx_v_block_size = __pyx_t_1;
 
-      /* "fastavro/_read.pyx":497
+      /* "fastavro/_read.pyx":491
  *         if block_count < 0:
  *             block_size = read_long(fo)
  *             fo.read(block_size)             # <<<<<<<<<<<<<<
  *         else:
  *             for i in range(block_count):
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 497, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_block_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 497, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_block_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 491, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "fastavro/_read.pyx":495
+      /* "fastavro/_read.pyx":489
  *     block_count = read_long(fo)
  *     while block_count != 0:
  *         if block_count < 0:             # <<<<<<<<<<<<<<
  *             block_size = read_long(fo)
  *             fo.read(block_size)
  */
       goto __pyx_L5;
     }
 
-    /* "fastavro/_read.pyx":499
+    /* "fastavro/_read.pyx":493
  *             fo.read(block_size)
  *         else:
  *             for i in range(block_count):             # <<<<<<<<<<<<<<
  *                 skip_utf8(fo)
  *                 _skip_data(fo, writer_schema["values"], named_schemas)
  */
     /*else*/ {
       __pyx_t_1 = __pyx_v_block_count;
       __pyx_t_7 = __pyx_t_1;
       for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
         __pyx_v_i = __pyx_t_8;
 
-        /* "fastavro/_read.pyx":500
+        /* "fastavro/_read.pyx":494
  *         else:
  *             for i in range(block_count):
  *                 skip_utf8(fo)             # <<<<<<<<<<<<<<
  *                 _skip_data(fo, writer_schema["values"], named_schemas)
  * 
  */
-        __pyx_t_3 = __pyx_f_8fastavro_5_read_skip_utf8(__pyx_v_fo, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 500, __pyx_L1_error)
+        __pyx_t_3 = __pyx_f_8fastavro_5_read_skip_utf8(__pyx_v_fo, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "fastavro/_read.pyx":501
+        /* "fastavro/_read.pyx":495
  *             for i in range(block_count):
  *                 skip_utf8(fo)
  *                 _skip_data(fo, writer_schema["values"], named_schemas)             # <<<<<<<<<<<<<<
  * 
  *         block_count = read_long(fo)
  */
-        __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 501, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 495, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_3, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 501, __pyx_L1_error)
+        __pyx_t_4 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_3, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 495, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
     }
     __pyx_L5:;
 
-    /* "fastavro/_read.pyx":503
+    /* "fastavro/_read.pyx":497
  *                 _skip_data(fo, writer_schema["values"], named_schemas)
  * 
  *         block_count = read_long(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 503, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 497, __pyx_L1_error)
     __pyx_v_block_count = __pyx_t_1;
   }
 
-  /* "fastavro/_read.pyx":479
+  /* "fastavro/_read.pyx":473
  * 
  * 
  * cpdef skip_map(fo, writer_schema, named_schemas):             # <<<<<<<<<<<<<<
  *     """Maps are encoded as a series of blocks.
  * 
  */
 
@@ -8589,40 +8586,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("skip_map", 1, 3, 3, 1); __PYX_ERR(0, 479, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("skip_map", 1, 3, 3, 1); __PYX_ERR(0, 473, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("skip_map", 1, 3, 3, 2); __PYX_ERR(0, 479, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("skip_map", 1, 3, 3, 2); __PYX_ERR(0, 473, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "skip_map") < 0)) __PYX_ERR(0, 479, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "skip_map") < 0)) __PYX_ERR(0, 473, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_named_schemas = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("skip_map", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 479, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("skip_map", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 473, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.skip_map", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8fastavro_5_read_48skip_map(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas);
 
@@ -8636,15 +8633,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("skip_map", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_map(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 479, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_map(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 473, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8653,55 +8650,40 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":506
+/* "fastavro/_read.pyx":500
  * 
  * 
  * cpdef read_union(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
 static PyObject *__pyx_pw_8fastavro_5_read_51read_union(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_read_union(PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_8fastavro_5_read_read_union *__pyx_optional_args) {
 
-  /* "fastavro/_read.pyx":510
+  /* "fastavro/_read.pyx":504
  *     writer_schema,
  *     named_schemas,
  *     reader_schema=None,             # <<<<<<<<<<<<<<
- *     return_record_name=False,
- *     return_record_name_override=False,
- */
-  PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
-
-  /* "fastavro/_read.pyx":511
- *     named_schemas,
- *     reader_schema=None,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
- * ):
- */
-  PyObject *__pyx_v_return_record_name = ((PyObject *)Py_False);
-
-  /* "fastavro/_read.pyx":512
- *     reader_schema=None,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
+ *     options={}
  * ):
- *     """A union is encoded by first writing a long value indicating the
  */
-  PyObject *__pyx_v_return_record_name_override = ((PyObject *)Py_False);
+  PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
+  PyObject *__pyx_v_options = __pyx_k__5;
   __pyx_t_8fastavro_5_read_long64 __pyx_v_index;
   PyObject *__pyx_v_idx_schema = NULL;
   PyObject *__pyx_v_schema = NULL;
   PyObject *__pyx_v_msg = NULL;
+  PyObject *__pyx_v_return_record_name_override = NULL;
+  PyObject *__pyx_v_return_record_name = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __pyx_t_8fastavro_5_read_long64 __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   struct __pyx_opt_args_8fastavro_5_read__read_data __pyx_t_5;
@@ -8715,616 +8697,645 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_union", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_reader_schema = __pyx_optional_args->reader_schema;
       if (__pyx_optional_args->__pyx_n > 1) {
-        __pyx_v_return_record_name = __pyx_optional_args->return_record_name;
-        if (__pyx_optional_args->__pyx_n > 2) {
-          __pyx_v_return_record_name_override = __pyx_optional_args->return_record_name_override;
-        }
+        __pyx_v_options = __pyx_optional_args->options;
       }
     }
   }
 
-  /* "fastavro/_read.pyx":520
+  /* "fastavro/_read.pyx":513
  *     """
  *     # schema resolution
  *     index = read_long(fo)             # <<<<<<<<<<<<<<
  *     idx_schema = writer_schema[index]
  * 
  */
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 513, __pyx_L1_error)
   __pyx_v_index = __pyx_t_1;
 
-  /* "fastavro/_read.pyx":521
+  /* "fastavro/_read.pyx":514
  *     # schema resolution
  *     index = read_long(fo)
  *     idx_schema = writer_schema[index]             # <<<<<<<<<<<<<<
  * 
  *     if reader_schema:
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_writer_schema, __pyx_v_index, __pyx_t_8fastavro_5_read_long64, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_writer_schema, __pyx_v_index, __pyx_t_8fastavro_5_read_long64, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_idx_schema = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":523
+  /* "fastavro/_read.pyx":516
  *     idx_schema = writer_schema[index]
  * 
  *     if reader_schema:             # <<<<<<<<<<<<<<
  *         # Handle case where the reader schema is just a single type (not union)
  *         if not isinstance(reader_schema, list):
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 516, __pyx_L1_error)
   if (__pyx_t_3) {
 
-    /* "fastavro/_read.pyx":525
+    /* "fastavro/_read.pyx":518
  *     if reader_schema:
  *         # Handle case where the reader schema is just a single type (not union)
  *         if not isinstance(reader_schema, list):             # <<<<<<<<<<<<<<
  *             if match_types(idx_schema, reader_schema):
  *                 return _read_data(
  */
     __pyx_t_3 = PyList_Check(__pyx_v_reader_schema); 
     __pyx_t_4 = ((!(__pyx_t_3 != 0)) != 0);
     if (__pyx_t_4) {
 
-      /* "fastavro/_read.pyx":526
+      /* "fastavro/_read.pyx":519
  *         # Handle case where the reader schema is just a single type (not union)
  *         if not isinstance(reader_schema, list):
  *             if match_types(idx_schema, reader_schema):             # <<<<<<<<<<<<<<
  *                 return _read_data(
  *                     fo,
  */
-      __pyx_t_2 = __pyx_f_8fastavro_5_read_match_types(__pyx_v_idx_schema, __pyx_v_reader_schema, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_8fastavro_5_read_match_types(__pyx_v_idx_schema, __pyx_v_reader_schema, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 519, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":527
+        /* "fastavro/_read.pyx":520
  *         if not isinstance(reader_schema, list):
  *             if match_types(idx_schema, reader_schema):
  *                 return _read_data(             # <<<<<<<<<<<<<<
  *                     fo,
  *                     idx_schema,
  */
         __Pyx_XDECREF(__pyx_r);
 
-        /* "fastavro/_read.pyx":533
+        /* "fastavro/_read.pyx":525
+ *                     named_schemas,
  *                     reader_schema,
- *                     return_record_name,
- *                     return_record_name_override,             # <<<<<<<<<<<<<<
+ *                     options,             # <<<<<<<<<<<<<<
  *                 )
  *         else:
  */
-        __pyx_t_5.__pyx_n = 3;
+        __pyx_t_5.__pyx_n = 2;
         __pyx_t_5.reader_schema = __pyx_v_reader_schema;
-        __pyx_t_5.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_5.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_2 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 527, __pyx_L1_error)
+        __pyx_t_5.options = __pyx_v_options;
+        __pyx_t_2 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         goto __pyx_L0;
 
-        /* "fastavro/_read.pyx":526
+        /* "fastavro/_read.pyx":519
  *         # Handle case where the reader schema is just a single type (not union)
  *         if not isinstance(reader_schema, list):
  *             if match_types(idx_schema, reader_schema):             # <<<<<<<<<<<<<<
  *                 return _read_data(
  *                     fo,
  */
       }
 
-      /* "fastavro/_read.pyx":525
+      /* "fastavro/_read.pyx":518
  *     if reader_schema:
  *         # Handle case where the reader schema is just a single type (not union)
  *         if not isinstance(reader_schema, list):             # <<<<<<<<<<<<<<
  *             if match_types(idx_schema, reader_schema):
  *                 return _read_data(
  */
       goto __pyx_L4;
     }
 
-    /* "fastavro/_read.pyx":536
+    /* "fastavro/_read.pyx":528
  *                 )
  *         else:
  *             for schema in reader_schema:             # <<<<<<<<<<<<<<
  *                 if match_types(idx_schema, schema):
  *                     return _read_data(
  */
     /*else*/ {
       if (likely(PyList_CheckExact(__pyx_v_reader_schema)) || PyTuple_CheckExact(__pyx_v_reader_schema)) {
         __pyx_t_2 = __pyx_v_reader_schema; __Pyx_INCREF(__pyx_t_2); __pyx_t_6 = 0;
         __pyx_t_7 = NULL;
       } else {
-        __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_reader_schema); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 536, __pyx_L1_error)
+        __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_reader_schema); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 528, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 536, __pyx_L1_error)
+        __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 528, __pyx_L1_error)
       }
       for (;;) {
         if (likely(!__pyx_t_7)) {
           if (likely(PyList_CheckExact(__pyx_t_2))) {
             if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_2)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_8 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 536, __pyx_L1_error)
+            __pyx_t_8 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 528, __pyx_L1_error)
             #else
-            __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 536, __pyx_L1_error)
+            __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 528, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_8);
             #endif
           } else {
             if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 536, __pyx_L1_error)
+            __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 528, __pyx_L1_error)
             #else
-            __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 536, __pyx_L1_error)
+            __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 528, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_8);
             #endif
           }
         } else {
           __pyx_t_8 = __pyx_t_7(__pyx_t_2);
           if (unlikely(!__pyx_t_8)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 536, __pyx_L1_error)
+              else __PYX_ERR(0, 528, __pyx_L1_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_8);
         }
         __Pyx_XDECREF_SET(__pyx_v_schema, __pyx_t_8);
         __pyx_t_8 = 0;
 
-        /* "fastavro/_read.pyx":537
+        /* "fastavro/_read.pyx":529
  *         else:
  *             for schema in reader_schema:
  *                 if match_types(idx_schema, schema):             # <<<<<<<<<<<<<<
  *                     return _read_data(
  *                         fo,
  */
-        __pyx_t_8 = __pyx_f_8fastavro_5_read_match_types(__pyx_v_idx_schema, __pyx_v_schema, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 537, __pyx_L1_error)
+        __pyx_t_8 = __pyx_f_8fastavro_5_read_match_types(__pyx_v_idx_schema, __pyx_v_schema, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 529, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 537, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 529, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         if (__pyx_t_4) {
 
-          /* "fastavro/_read.pyx":538
+          /* "fastavro/_read.pyx":530
  *             for schema in reader_schema:
  *                 if match_types(idx_schema, schema):
  *                     return _read_data(             # <<<<<<<<<<<<<<
  *                         fo,
  *                         idx_schema,
  */
           __Pyx_XDECREF(__pyx_r);
 
-          /* "fastavro/_read.pyx":544
+          /* "fastavro/_read.pyx":535
+ *                         named_schemas,
  *                         schema,
- *                         return_record_name,
- *                         return_record_name_override,             # <<<<<<<<<<<<<<
+ *                         options,             # <<<<<<<<<<<<<<
  *                     )
  *         msg = f"schema mismatch: {writer_schema} not found in {reader_schema}"
  */
-          __pyx_t_5.__pyx_n = 3;
+          __pyx_t_5.__pyx_n = 2;
           __pyx_t_5.reader_schema = __pyx_v_schema;
-          __pyx_t_5.return_record_name = __pyx_v_return_record_name;
-          __pyx_t_5.return_record_name_override = __pyx_v_return_record_name_override;
-          __pyx_t_8 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 538, __pyx_L1_error)
+          __pyx_t_5.options = __pyx_v_options;
+          __pyx_t_8 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 530, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __pyx_r = __pyx_t_8;
           __pyx_t_8 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           goto __pyx_L0;
 
-          /* "fastavro/_read.pyx":537
+          /* "fastavro/_read.pyx":529
  *         else:
  *             for schema in reader_schema:
  *                 if match_types(idx_schema, schema):             # <<<<<<<<<<<<<<
  *                     return _read_data(
  *                         fo,
  */
         }
 
-        /* "fastavro/_read.pyx":536
+        /* "fastavro/_read.pyx":528
  *                 )
  *         else:
  *             for schema in reader_schema:             # <<<<<<<<<<<<<<
  *                 if match_types(idx_schema, schema):
  *                     return _read_data(
  */
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L4:;
 
-    /* "fastavro/_read.pyx":546
- *                         return_record_name_override,
+    /* "fastavro/_read.pyx":537
+ *                         options,
  *                     )
  *         msg = f"schema mismatch: {writer_schema} not found in {reader_schema}"             # <<<<<<<<<<<<<<
  *         raise SchemaResolutionError(msg)
  *     else:
  */
-    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 537, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = 0;
     __pyx_t_9 = 127;
     __Pyx_INCREF(__pyx_kp_u_schema_mismatch);
     __pyx_t_6 += 17;
     __Pyx_GIVEREF(__pyx_kp_u_schema_mismatch);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u_schema_mismatch);
-    __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_writer_schema, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 546, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_writer_schema, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 537, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_9) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_9;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_8);
     __pyx_t_8 = 0;
     __Pyx_INCREF(__pyx_kp_u_not_found_in);
     __pyx_t_6 += 14;
     __Pyx_GIVEREF(__pyx_kp_u_not_found_in);
     PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u_not_found_in);
-    __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_reader_schema, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 546, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_reader_schema, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 537, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_9) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_9;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_8);
     __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_2, 4, __pyx_t_6, __pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 546, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_2, 4, __pyx_t_6, __pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 537, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_msg = ((PyObject*)__pyx_t_8);
     __pyx_t_8 = 0;
 
-    /* "fastavro/_read.pyx":547
+    /* "fastavro/_read.pyx":538
  *                     )
  *         msg = f"schema mismatch: {writer_schema} not found in {reader_schema}"
  *         raise SchemaResolutionError(msg)             # <<<<<<<<<<<<<<
  *     else:
- *         if return_record_name_override and is_nullable_union(writer_schema):
+ *         return_record_name_override = options.get("return_record_name_override")
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SchemaResolutionError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SchemaResolutionError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 538, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_10 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_10, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 547, __pyx_L1_error)
+    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 538, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_8, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __PYX_ERR(0, 547, __pyx_L1_error)
+    __PYX_ERR(0, 538, __pyx_L1_error)
 
-    /* "fastavro/_read.pyx":523
+    /* "fastavro/_read.pyx":516
  *     idx_schema = writer_schema[index]
  * 
  *     if reader_schema:             # <<<<<<<<<<<<<<
  *         # Handle case where the reader schema is just a single type (not union)
  *         if not isinstance(reader_schema, list):
  */
   }
 
-  /* "fastavro/_read.pyx":549
+  /* "fastavro/_read.pyx":540
  *         raise SchemaResolutionError(msg)
  *     else:
- *         if return_record_name_override and is_nullable_union(writer_schema):             # <<<<<<<<<<<<<<
- *             return _read_data(
- *                 fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
+ *         return_record_name_override = options.get("return_record_name_override")             # <<<<<<<<<<<<<<
+ *         return_record_name = options.get("return_record_name")
+ *         if return_record_name_override and is_nullable_union(writer_schema):
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_return_record_name_override); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 549, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_options, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 540, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_10 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_10)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_10);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
+      }
+    }
+    __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_10, __pyx_n_u_return_record_name_override) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_u_return_record_name_override);
+    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 540, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_v_return_record_name_override = __pyx_t_8;
+    __pyx_t_8 = 0;
+
+    /* "fastavro/_read.pyx":541
+ *     else:
+ *         return_record_name_override = options.get("return_record_name_override")
+ *         return_record_name = options.get("return_record_name")             # <<<<<<<<<<<<<<
+ *         if return_record_name_override and is_nullable_union(writer_schema):
+ *             return _read_data(fo, idx_schema, named_schemas, None, options)
+ */
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_options, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 541, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_10 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_10)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_10);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
+      }
+    }
+    __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_10, __pyx_n_u_return_record_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_u_return_record_name);
+    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 541, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_v_return_record_name = __pyx_t_8;
+    __pyx_t_8 = 0;
+
+    /* "fastavro/_read.pyx":542
+ *         return_record_name_override = options.get("return_record_name_override")
+ *         return_record_name = options.get("return_record_name")
+ *         if return_record_name_override and is_nullable_union(writer_schema):             # <<<<<<<<<<<<<<
+ *             return _read_data(fo, idx_schema, named_schemas, None, options)
+ *         elif return_record_name and extract_record_type(idx_schema) == "record":
+ */
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_return_record_name_override); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 542, __pyx_L1_error)
     if (__pyx_t_3) {
     } else {
       __pyx_t_4 = __pyx_t_3;
       goto __pyx_L10_bool_binop_done;
     }
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_is_nullable_union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 549, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_is_nullable_union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_10 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_10, __pyx_v_writer_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_writer_schema);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 549, __pyx_L1_error)
+    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 549, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_4 = __pyx_t_3;
     __pyx_L10_bool_binop_done:;
     if (__pyx_t_4) {
 
-      /* "fastavro/_read.pyx":550
- *     else:
- *         if return_record_name_override and is_nullable_union(writer_schema):
- *             return _read_data(             # <<<<<<<<<<<<<<
- *                 fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
- *             )
- */
-      __Pyx_XDECREF(__pyx_r);
-
-      /* "fastavro/_read.pyx":551
+      /* "fastavro/_read.pyx":543
+ *         return_record_name = options.get("return_record_name")
  *         if return_record_name_override and is_nullable_union(writer_schema):
- *             return _read_data(
- *                 fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override             # <<<<<<<<<<<<<<
- *             )
+ *             return _read_data(fo, idx_schema, named_schemas, None, options)             # <<<<<<<<<<<<<<
  *         elif return_record_name and extract_record_type(idx_schema) == "record":
+ *             return (
  */
-      __pyx_t_5.__pyx_n = 3;
+      __Pyx_XDECREF(__pyx_r);
+      __pyx_t_5.__pyx_n = 2;
       __pyx_t_5.reader_schema = Py_None;
-      __pyx_t_5.return_record_name = __pyx_v_return_record_name;
-      __pyx_t_5.return_record_name_override = __pyx_v_return_record_name_override;
-      __pyx_t_8 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 550, __pyx_L1_error)
+      __pyx_t_5.options = __pyx_v_options;
+      __pyx_t_8 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 543, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_r = __pyx_t_8;
       __pyx_t_8 = 0;
       goto __pyx_L0;
 
-      /* "fastavro/_read.pyx":549
- *         raise SchemaResolutionError(msg)
- *     else:
+      /* "fastavro/_read.pyx":542
+ *         return_record_name_override = options.get("return_record_name_override")
+ *         return_record_name = options.get("return_record_name")
  *         if return_record_name_override and is_nullable_union(writer_schema):             # <<<<<<<<<<<<<<
- *             return _read_data(
- *                 fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
+ *             return _read_data(fo, idx_schema, named_schemas, None, options)
+ *         elif return_record_name and extract_record_type(idx_schema) == "record":
  */
     }
 
-    /* "fastavro/_read.pyx":553
- *                 fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
- *             )
+    /* "fastavro/_read.pyx":544
+ *         if return_record_name_override and is_nullable_union(writer_schema):
+ *             return _read_data(fo, idx_schema, named_schemas, None, options)
  *         elif return_record_name and extract_record_type(idx_schema) == "record":             # <<<<<<<<<<<<<<
  *             return (
  *                 idx_schema["name"],
  */
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_return_record_name); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_return_record_name); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 544, __pyx_L1_error)
     if (__pyx_t_3) {
     } else {
       __pyx_t_4 = __pyx_t_3;
       goto __pyx_L12_bool_binop_done;
     }
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_extract_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_extract_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 544, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_10 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_10, __pyx_v_idx_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_idx_schema);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 553, __pyx_L1_error)
+    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 544, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_8, __pyx_n_u_record, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_8, __pyx_n_u_record, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 544, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_4 = __pyx_t_3;
     __pyx_L12_bool_binop_done:;
     if (__pyx_t_4) {
 
-      /* "fastavro/_read.pyx":554
- *             )
+      /* "fastavro/_read.pyx":545
+ *             return _read_data(fo, idx_schema, named_schemas, None, options)
  *         elif return_record_name and extract_record_type(idx_schema) == "record":
  *             return (             # <<<<<<<<<<<<<<
  *                 idx_schema["name"],
  *                 _read_data(
  */
       __Pyx_XDECREF(__pyx_r);
 
-      /* "fastavro/_read.pyx":555
+      /* "fastavro/_read.pyx":546
  *         elif return_record_name and extract_record_type(idx_schema) == "record":
  *             return (
  *                 idx_schema["name"],             # <<<<<<<<<<<<<<
  *                 _read_data(
  *                     fo,
  */
-      __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_idx_schema, __pyx_n_u_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 555, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_idx_schema, __pyx_n_u_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 546, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
 
-      /* "fastavro/_read.pyx":556
+      /* "fastavro/_read.pyx":547
  *             return (
  *                 idx_schema["name"],
  *                 _read_data(             # <<<<<<<<<<<<<<
  *                     fo,
  *                     idx_schema,
  */
-      __pyx_t_5.__pyx_n = 3;
+      __pyx_t_5.__pyx_n = 2;
       __pyx_t_5.reader_schema = Py_None;
-      __pyx_t_5.return_record_name = __pyx_v_return_record_name;
-      __pyx_t_5.return_record_name_override = __pyx_v_return_record_name_override;
-      __pyx_t_2 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 556, __pyx_L1_error)
+      __pyx_t_5.options = __pyx_v_options;
+      __pyx_t_2 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
 
-      /* "fastavro/_read.pyx":555
+      /* "fastavro/_read.pyx":546
  *         elif return_record_name and extract_record_type(idx_schema) == "record":
  *             return (
  *                 idx_schema["name"],             # <<<<<<<<<<<<<<
  *                 _read_data(
  *                     fo,
  */
-      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 555, __pyx_L1_error)
+      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 546, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_2);
       __pyx_t_8 = 0;
       __pyx_t_2 = 0;
       __pyx_r = __pyx_t_10;
       __pyx_t_10 = 0;
       goto __pyx_L0;
 
-      /* "fastavro/_read.pyx":553
- *                 fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
- *             )
+      /* "fastavro/_read.pyx":544
+ *         if return_record_name_override and is_nullable_union(writer_schema):
+ *             return _read_data(fo, idx_schema, named_schemas, None, options)
  *         elif return_record_name and extract_record_type(idx_schema) == "record":             # <<<<<<<<<<<<<<
  *             return (
  *                 idx_schema["name"],
  */
     }
 
-    /* "fastavro/_read.pyx":565
+    /* "fastavro/_read.pyx":555
  *                 )
  *             )
  *         elif return_record_name and extract_record_type(idx_schema) not in AVRO_TYPES:             # <<<<<<<<<<<<<<
  *             # idx_schema is a named type
  *             return (
  */
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_return_record_name); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 565, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_return_record_name); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 555, __pyx_L1_error)
     if (__pyx_t_3) {
     } else {
       __pyx_t_4 = __pyx_t_3;
       goto __pyx_L14_bool_binop_done;
     }
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_extract_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 565, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_extract_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 555, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_10 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_8, __pyx_v_idx_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_idx_schema);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 565, __pyx_L1_error)
+    if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 555, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_AVRO_TYPES); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 565, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_AVRO_TYPES); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 555, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_t_10, __pyx_t_2, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 565, __pyx_L1_error)
+    __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_t_10, __pyx_t_2, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 555, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_11 = (__pyx_t_3 != 0);
     __pyx_t_4 = __pyx_t_11;
     __pyx_L14_bool_binop_done:;
     if (__pyx_t_4) {
 
-      /* "fastavro/_read.pyx":567
+      /* "fastavro/_read.pyx":557
  *         elif return_record_name and extract_record_type(idx_schema) not in AVRO_TYPES:
  *             # idx_schema is a named type
  *             return (             # <<<<<<<<<<<<<<
  *                 named_schemas["writer"][idx_schema]["name"],
- *                 _read_data(
+ *                 _read_data(fo, idx_schema, named_schemas, None, options)
  */
       __Pyx_XDECREF(__pyx_r);
 
-      /* "fastavro/_read.pyx":568
+      /* "fastavro/_read.pyx":558
  *             # idx_schema is a named type
  *             return (
  *                 named_schemas["writer"][idx_schema]["name"],             # <<<<<<<<<<<<<<
- *                 _read_data(
- *                     fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
+ *                 _read_data(fo, idx_schema, named_schemas, None, options)
+ *             )
  */
-      __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_named_schemas, __pyx_n_u_writer); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 568, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_named_schemas, __pyx_n_u_writer); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_idx_schema); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 568, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_idx_schema); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_10, __pyx_n_u_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 568, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_10, __pyx_n_u_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-      /* "fastavro/_read.pyx":569
+      /* "fastavro/_read.pyx":559
  *             return (
  *                 named_schemas["writer"][idx_schema]["name"],
- *                 _read_data(             # <<<<<<<<<<<<<<
- *                     fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
- *                 )
+ *                 _read_data(fo, idx_schema, named_schemas, None, options)             # <<<<<<<<<<<<<<
+ *             )
+ * 
  */
-      __pyx_t_5.__pyx_n = 3;
+      __pyx_t_5.__pyx_n = 2;
       __pyx_t_5.reader_schema = Py_None;
-      __pyx_t_5.return_record_name = __pyx_v_return_record_name;
-      __pyx_t_5.return_record_name_override = __pyx_v_return_record_name_override;
-      __pyx_t_10 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 569, __pyx_L1_error)
+      __pyx_t_5.options = __pyx_v_options;
+      __pyx_t_10 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 559, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
 
-      /* "fastavro/_read.pyx":568
+      /* "fastavro/_read.pyx":558
  *             # idx_schema is a named type
  *             return (
  *                 named_schemas["writer"][idx_schema]["name"],             # <<<<<<<<<<<<<<
- *                 _read_data(
- *                     fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
+ *                 _read_data(fo, idx_schema, named_schemas, None, options)
+ *             )
  */
-      __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 568, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_10);
       PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_10);
       __pyx_t_2 = 0;
       __pyx_t_10 = 0;
       __pyx_r = __pyx_t_8;
       __pyx_t_8 = 0;
       goto __pyx_L0;
 
-      /* "fastavro/_read.pyx":565
+      /* "fastavro/_read.pyx":555
  *                 )
  *             )
  *         elif return_record_name and extract_record_type(idx_schema) not in AVRO_TYPES:             # <<<<<<<<<<<<<<
  *             # idx_schema is a named type
  *             return (
  */
     }
 
-    /* "fastavro/_read.pyx":575
+    /* "fastavro/_read.pyx":563
  * 
  *         else:
- *             return _read_data(             # <<<<<<<<<<<<<<
- *                 fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
- *             )
+ *             return _read_data(fo, idx_schema, named_schemas, None, options)             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
-
-      /* "fastavro/_read.pyx":576
- *         else:
- *             return _read_data(
- *                 fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override             # <<<<<<<<<<<<<<
- *             )
- * 
- */
-      __pyx_t_5.__pyx_n = 3;
+      __pyx_t_5.__pyx_n = 2;
       __pyx_t_5.reader_schema = Py_None;
-      __pyx_t_5.return_record_name = __pyx_v_return_record_name;
-      __pyx_t_5.return_record_name_override = __pyx_v_return_record_name_override;
-      __pyx_t_8 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 575, __pyx_L1_error)
+      __pyx_t_5.options = __pyx_v_options;
+      __pyx_t_8 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_idx_schema, __pyx_v_named_schemas, 0, &__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 563, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_r = __pyx_t_8;
       __pyx_t_8 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "fastavro/_read.pyx":506
+  /* "fastavro/_read.pyx":500
  * 
  * 
  * cpdef read_union(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
@@ -9335,71 +9346,53 @@
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("fastavro._read.read_union", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_idx_schema);
   __Pyx_XDECREF(__pyx_v_schema);
   __Pyx_XDECREF(__pyx_v_msg);
+  __Pyx_XDECREF(__pyx_v_return_record_name_override);
+  __Pyx_XDECREF(__pyx_v_return_record_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8fastavro_5_read_51read_union(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_8fastavro_5_read_50read_union[] = "A union is encoded by first writing a long value indicating the\n    zero-based position within the union of the schema of its value.\n\n    The value is then encoded per the indicated schema within the union.\n    ";
 static PyObject *__pyx_pw_8fastavro_5_read_51read_union(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_writer_schema = 0;
   PyObject *__pyx_v_named_schemas = 0;
   PyObject *__pyx_v_reader_schema = 0;
-  PyObject *__pyx_v_return_record_name = 0;
-  PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_options = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_union (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_options,0};
+    PyObject* values[5] = {0,0,0,0,0};
 
-    /* "fastavro/_read.pyx":510
+    /* "fastavro/_read.pyx":504
  *     writer_schema,
  *     named_schemas,
  *     reader_schema=None,             # <<<<<<<<<<<<<<
- *     return_record_name=False,
- *     return_record_name_override=False,
- */
-    values[3] = ((PyObject *)Py_None);
-
-    /* "fastavro/_read.pyx":511
- *     named_schemas,
- *     reader_schema=None,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
- * ):
- */
-    values[4] = ((PyObject *)Py_False);
-
-    /* "fastavro/_read.pyx":512
- *     reader_schema=None,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
+ *     options={}
  * ):
- *     """A union is encoded by first writing a long value indicating the
  */
-    values[5] = ((PyObject *)Py_False);
+    values[3] = ((PyObject *)Py_None);
+    values[4] = __pyx_k__5;
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -9414,48 +9407,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_union", 0, 3, 6, 1); __PYX_ERR(0, 506, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_union", 0, 3, 5, 1); __PYX_ERR(0, 500, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_union", 0, 3, 6, 2); __PYX_ERR(0, 506, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_union", 0, 3, 5, 2); __PYX_ERR(0, 500, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema);
           if (value) { values[3] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name);
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options);
           if (value) { values[4] = value; kw_args--; }
         }
-        CYTHON_FALLTHROUGH;
-        case  5:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
-          if (value) { values[5] = value; kw_args--; }
-        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_union") < 0)) __PYX_ERR(0, 506, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_union") < 0)) __PYX_ERR(0, 500, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -9463,55 +9448,53 @@
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_named_schemas = values[2];
     __pyx_v_reader_schema = values[3];
-    __pyx_v_return_record_name = values[4];
-    __pyx_v_return_record_name_override = values[5];
+    __pyx_v_options = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_union", 0, 3, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 506, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_union", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 500, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.read_union", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_50read_union(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
+  __pyx_r = __pyx_pf_8fastavro_5_read_50read_union(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_options);
 
-  /* "fastavro/_read.pyx":506
+  /* "fastavro/_read.pyx":500
  * 
  * 
  * cpdef read_union(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_50read_union(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_50read_union(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_8fastavro_5_read_read_union __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_union", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2.__pyx_n = 3;
+  __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.reader_schema = __pyx_v_reader_schema;
-  __pyx_t_2.return_record_name = __pyx_v_return_record_name;
-  __pyx_t_2.return_record_name_override = __pyx_v_return_record_name_override;
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_union(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_2.options = __pyx_v_options;
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_union(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9520,15 +9503,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":580
+/* "fastavro/_read.pyx":566
  * 
  * 
  * cpdef skip_union(fo, writer_schema, named_schemas):             # <<<<<<<<<<<<<<
  *     """A union is encoded by first writing a long value indicating the
  *     zero-based position within the union of the schema of its value.
  */
 
@@ -9541,39 +9524,39 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("skip_union", 0);
 
-  /* "fastavro/_read.pyx":587
+  /* "fastavro/_read.pyx":573
  *     """
  *     # schema resolution
  *     index = read_long(fo)             # <<<<<<<<<<<<<<
  *     _skip_data(fo, writer_schema[index], named_schemas)
  * 
  */
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 587, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 573, __pyx_L1_error)
   __pyx_v_index = __pyx_t_1;
 
-  /* "fastavro/_read.pyx":588
+  /* "fastavro/_read.pyx":574
  *     # schema resolution
  *     index = read_long(fo)
  *     _skip_data(fo, writer_schema[index], named_schemas)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_writer_schema, __pyx_v_index, __pyx_t_8fastavro_5_read_long64, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_writer_schema, __pyx_v_index, __pyx_t_8fastavro_5_read_long64, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_2, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_2, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "fastavro/_read.pyx":580
+  /* "fastavro/_read.pyx":566
  * 
  * 
  * cpdef skip_union(fo, writer_schema, named_schemas):             # <<<<<<<<<<<<<<
  *     """A union is encoded by first writing a long value indicating the
  *     zero-based position within the union of the schema of its value.
  */
 
@@ -9625,40 +9608,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("skip_union", 1, 3, 3, 1); __PYX_ERR(0, 580, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("skip_union", 1, 3, 3, 1); __PYX_ERR(0, 566, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("skip_union", 1, 3, 3, 2); __PYX_ERR(0, 580, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("skip_union", 1, 3, 3, 2); __PYX_ERR(0, 566, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "skip_union") < 0)) __PYX_ERR(0, 580, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "skip_union") < 0)) __PYX_ERR(0, 566, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_named_schemas = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("skip_union", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 580, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("skip_union", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 566, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.skip_union", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8fastavro_5_read_52skip_union(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas);
 
@@ -9672,15 +9655,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("skip_union", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_union(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_union(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9689,51 +9672,34 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":591
+/* "fastavro/_read.pyx":577
  * 
  * 
  * cpdef read_record(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
 static PyObject *__pyx_pw_8fastavro_5_read_55read_record(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_read_record(PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_8fastavro_5_read_read_record *__pyx_optional_args) {
 
-  /* "fastavro/_read.pyx":595
+  /* "fastavro/_read.pyx":581
  *     writer_schema,
  *     named_schemas,
  *     reader_schema=None,             # <<<<<<<<<<<<<<
- *     return_record_name=False,
- *     return_record_name_override=False,
- */
-  PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
-
-  /* "fastavro/_read.pyx":596
- *     named_schemas,
- *     reader_schema=None,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
- * ):
- */
-  PyObject *__pyx_v_return_record_name = ((PyObject *)Py_False);
-
-  /* "fastavro/_read.pyx":597
- *     reader_schema=None,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
+ *     options={},
  * ):
- *     """A record is encoded by encoding the values of its fields in the order
  */
-  PyObject *__pyx_v_return_record_name_override = ((PyObject *)Py_False);
+  PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
+  PyObject *__pyx_v_options = __pyx_k__6;
   PyObject *__pyx_v_record = NULL;
   PyObject *__pyx_v_field = NULL;
   PyObject *__pyx_v_readers_field_dict = NULL;
   PyObject *__pyx_v_aliases_field_dict = NULL;
   PyObject *__pyx_v_f = NULL;
   PyObject *__pyx_v_alias = NULL;
   PyObject *__pyx_v_readers_field = NULL;
@@ -9763,246 +9729,242 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_record", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_reader_schema = __pyx_optional_args->reader_schema;
       if (__pyx_optional_args->__pyx_n > 1) {
-        __pyx_v_return_record_name = __pyx_optional_args->return_record_name;
-        if (__pyx_optional_args->__pyx_n > 2) {
-          __pyx_v_return_record_name_override = __pyx_optional_args->return_record_name_override;
-        }
+        __pyx_v_options = __pyx_optional_args->options;
       }
     }
   }
 
-  /* "fastavro/_read.pyx":617
+  /* "fastavro/_read.pyx":602
  *          field's value is unset.
  *     """
  *     record = {}             # <<<<<<<<<<<<<<
  *     if reader_schema is None:
  *         for field in writer_schema["fields"]:
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 617, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_record = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":618
+  /* "fastavro/_read.pyx":603
  *     """
  *     record = {}
  *     if reader_schema is None:             # <<<<<<<<<<<<<<
  *         for field in writer_schema["fields"]:
  *             record[field["name"]] = _read_data(
  */
   __pyx_t_2 = (__pyx_v_reader_schema == Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "fastavro/_read.pyx":619
+    /* "fastavro/_read.pyx":604
  *     record = {}
  *     if reader_schema is None:
  *         for field in writer_schema["fields"]:             # <<<<<<<<<<<<<<
  *             record[field["name"]] = _read_data(
  *                 fo,
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_fields); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_fields); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 604, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
       __pyx_t_4 = __pyx_t_1; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 619, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 604, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 619, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 604, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_1 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 619, __pyx_L1_error)
+          __pyx_t_1 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 604, __pyx_L1_error)
           #else
-          __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+          __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 604, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 619, __pyx_L1_error)
+          __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 604, __pyx_L1_error)
           #else
-          __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+          __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 604, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           #endif
         }
       } else {
         __pyx_t_1 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_1)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 619, __pyx_L1_error)
+            else __PYX_ERR(0, 604, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_1);
       }
       __Pyx_XDECREF_SET(__pyx_v_field, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "fastavro/_read.pyx":622
+      /* "fastavro/_read.pyx":607
  *             record[field["name"]] = _read_data(
  *                 fo,
  *                 field["type"],             # <<<<<<<<<<<<<<
  *                 named_schemas,
  *                 None,
  */
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 622, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "fastavro/_read.pyx":620
+      /* "fastavro/_read.pyx":605
  *     if reader_schema is None:
  *         for field in writer_schema["fields"]:
  *             record[field["name"]] = _read_data(             # <<<<<<<<<<<<<<
  *                 fo,
  *                 field["type"],
  */
-      __pyx_t_8.__pyx_n = 3;
+      __pyx_t_8.__pyx_n = 2;
       __pyx_t_8.reader_schema = Py_None;
-      __pyx_t_8.return_record_name = __pyx_v_return_record_name;
-      __pyx_t_8.return_record_name_override = __pyx_v_return_record_name_override;
-      __pyx_t_7 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_1, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 620, __pyx_L1_error)
+      __pyx_t_8.options = __pyx_v_options;
+      __pyx_t_7 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_1, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 605, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (unlikely(PyDict_SetItem(__pyx_v_record, __pyx_t_1, __pyx_t_7) < 0)) __PYX_ERR(0, 620, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_v_record, __pyx_t_1, __pyx_t_7) < 0)) __PYX_ERR(0, 605, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "fastavro/_read.pyx":619
+      /* "fastavro/_read.pyx":604
  *     record = {}
  *     if reader_schema is None:
  *         for field in writer_schema["fields"]:             # <<<<<<<<<<<<<<
  *             record[field["name"]] = _read_data(
  *                 fo,
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "fastavro/_read.pyx":618
+    /* "fastavro/_read.pyx":603
  *     """
  *     record = {}
  *     if reader_schema is None:             # <<<<<<<<<<<<<<
  *         for field in writer_schema["fields"]:
  *             record[field["name"]] = _read_data(
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":629
+  /* "fastavro/_read.pyx":613
  *             )
  *     else:
  *         readers_field_dict = {}             # <<<<<<<<<<<<<<
  *         aliases_field_dict = {}
  *         for f in reader_schema["fields"]:
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 629, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 613, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_v_readers_field_dict = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "fastavro/_read.pyx":630
+    /* "fastavro/_read.pyx":614
  *     else:
  *         readers_field_dict = {}
  *         aliases_field_dict = {}             # <<<<<<<<<<<<<<
  *         for f in reader_schema["fields"]:
  *             readers_field_dict[f["name"]] = f
  */
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 630, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 614, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_v_aliases_field_dict = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "fastavro/_read.pyx":631
+    /* "fastavro/_read.pyx":615
  *         readers_field_dict = {}
  *         aliases_field_dict = {}
  *         for f in reader_schema["fields"]:             # <<<<<<<<<<<<<<
  *             readers_field_dict[f["name"]] = f
  *             for alias in f.get("aliases", []):
  */
-    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_reader_schema, __pyx_n_u_fields); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 631, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_reader_schema, __pyx_n_u_fields); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 615, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
       __pyx_t_7 = __pyx_t_4; __Pyx_INCREF(__pyx_t_7); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 631, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 615, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_6 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 631, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 615, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_7))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_7)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_5); __Pyx_INCREF(__pyx_t_4); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 631, __pyx_L1_error)
+          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_5); __Pyx_INCREF(__pyx_t_4); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 615, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_7, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 631, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_7, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 615, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_7)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_5); __Pyx_INCREF(__pyx_t_4); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 631, __pyx_L1_error)
+          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_5); __Pyx_INCREF(__pyx_t_4); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 615, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_7, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 631, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_7, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 615, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_6(__pyx_t_7);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 631, __pyx_L1_error)
+            else __PYX_ERR(0, 615, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       __Pyx_XDECREF_SET(__pyx_v_f, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "fastavro/_read.pyx":632
+      /* "fastavro/_read.pyx":616
  *         aliases_field_dict = {}
  *         for f in reader_schema["fields"]:
  *             readers_field_dict[f["name"]] = f             # <<<<<<<<<<<<<<
  *             for alias in f.get("aliases", []):
  *                 aliases_field_dict[alias] = f
  */
-      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_f, __pyx_n_u_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 632, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_f, __pyx_n_u_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 616, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely(PyDict_SetItem(__pyx_v_readers_field_dict, __pyx_t_4, __pyx_v_f) < 0)) __PYX_ERR(0, 632, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_v_readers_field_dict, __pyx_t_4, __pyx_v_f) < 0)) __PYX_ERR(0, 616, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "fastavro/_read.pyx":633
+      /* "fastavro/_read.pyx":617
  *         for f in reader_schema["fields"]:
  *             readers_field_dict[f["name"]] = f
  *             for alias in f.get("aliases", []):             # <<<<<<<<<<<<<<
  *                 aliases_field_dict[alias] = f
  * 
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 617, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 633, __pyx_L1_error)
+      __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 617, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_10 = NULL;
       __pyx_t_11 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -10011,541 +9973,540 @@
           __Pyx_DECREF_SET(__pyx_t_1, function);
           __pyx_t_11 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_1)) {
         PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_n_u_aliases, __pyx_t_9};
-        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 617, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
         PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_n_u_aliases, __pyx_t_9};
-        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 617, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else
       #endif
       {
-        __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 617, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         if (__pyx_t_10) {
           __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
         }
         __Pyx_INCREF(__pyx_n_u_aliases);
         __Pyx_GIVEREF(__pyx_n_u_aliases);
         PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_n_u_aliases);
         __Pyx_GIVEREF(__pyx_t_9);
         PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_t_9);
         __pyx_t_9 = 0;
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_12, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_12, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 617, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
         __pyx_t_1 = __pyx_t_4; __Pyx_INCREF(__pyx_t_1); __pyx_t_13 = 0;
         __pyx_t_14 = NULL;
       } else {
-        __pyx_t_13 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_13 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 617, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_14 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_14 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 617, __pyx_L1_error)
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       for (;;) {
         if (likely(!__pyx_t_14)) {
           if (likely(PyList_CheckExact(__pyx_t_1))) {
             if (__pyx_t_13 >= PyList_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_13); __Pyx_INCREF(__pyx_t_4); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 633, __pyx_L1_error)
+            __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_13); __Pyx_INCREF(__pyx_t_4); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 617, __pyx_L1_error)
             #else
-            __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
+            __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 617, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_4);
             #endif
           } else {
             if (__pyx_t_13 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_13); __Pyx_INCREF(__pyx_t_4); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 633, __pyx_L1_error)
+            __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_13); __Pyx_INCREF(__pyx_t_4); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 617, __pyx_L1_error)
             #else
-            __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
+            __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 617, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_4);
             #endif
           }
         } else {
           __pyx_t_4 = __pyx_t_14(__pyx_t_1);
           if (unlikely(!__pyx_t_4)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 633, __pyx_L1_error)
+              else __PYX_ERR(0, 617, __pyx_L1_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_4);
         }
         __Pyx_XDECREF_SET(__pyx_v_alias, __pyx_t_4);
         __pyx_t_4 = 0;
 
-        /* "fastavro/_read.pyx":634
+        /* "fastavro/_read.pyx":618
  *             readers_field_dict[f["name"]] = f
  *             for alias in f.get("aliases", []):
  *                 aliases_field_dict[alias] = f             # <<<<<<<<<<<<<<
  * 
  *         for field in writer_schema["fields"]:
  */
-        if (unlikely(PyDict_SetItem(__pyx_v_aliases_field_dict, __pyx_v_alias, __pyx_v_f) < 0)) __PYX_ERR(0, 634, __pyx_L1_error)
+        if (unlikely(PyDict_SetItem(__pyx_v_aliases_field_dict, __pyx_v_alias, __pyx_v_f) < 0)) __PYX_ERR(0, 618, __pyx_L1_error)
 
-        /* "fastavro/_read.pyx":633
+        /* "fastavro/_read.pyx":617
  *         for f in reader_schema["fields"]:
  *             readers_field_dict[f["name"]] = f
  *             for alias in f.get("aliases", []):             # <<<<<<<<<<<<<<
  *                 aliases_field_dict[alias] = f
  * 
  */
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "fastavro/_read.pyx":631
+      /* "fastavro/_read.pyx":615
  *         readers_field_dict = {}
  *         aliases_field_dict = {}
  *         for f in reader_schema["fields"]:             # <<<<<<<<<<<<<<
  *             readers_field_dict[f["name"]] = f
  *             for alias in f.get("aliases", []):
  */
     }
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "fastavro/_read.pyx":636
+    /* "fastavro/_read.pyx":620
  *                 aliases_field_dict[alias] = f
  * 
  *         for field in writer_schema["fields"]:             # <<<<<<<<<<<<<<
  *             readers_field = readers_field_dict.get(
  *                 field["name"],
  */
-    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_fields); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 636, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_fields); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 620, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (likely(PyList_CheckExact(__pyx_t_7)) || PyTuple_CheckExact(__pyx_t_7)) {
       __pyx_t_1 = __pyx_t_7; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 636, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 636, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 620, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 636, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 620, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 636, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 620, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 636, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 620, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 636, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 620, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_1);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 636, __pyx_L1_error)
+            else __PYX_ERR(0, 620, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_field, __pyx_t_7);
       __pyx_t_7 = 0;
 
-      /* "fastavro/_read.pyx":638
+      /* "fastavro/_read.pyx":622
  *         for field in writer_schema["fields"]:
  *             readers_field = readers_field_dict.get(
  *                 field["name"],             # <<<<<<<<<<<<<<
  *                 aliases_field_dict.get(field["name"]),
  *             )
  */
-      __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 638, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 622, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "fastavro/_read.pyx":639
+      /* "fastavro/_read.pyx":623
  *             readers_field = readers_field_dict.get(
  *                 field["name"],
  *                 aliases_field_dict.get(field["name"]),             # <<<<<<<<<<<<<<
  *             )
  *             if readers_field:
  */
-      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 639, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 623, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_12 = __Pyx_PyDict_GetItemDefault(__pyx_v_aliases_field_dict, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 639, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyDict_GetItemDefault(__pyx_v_aliases_field_dict, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 623, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "fastavro/_read.pyx":637
+      /* "fastavro/_read.pyx":621
  * 
  *         for field in writer_schema["fields"]:
  *             readers_field = readers_field_dict.get(             # <<<<<<<<<<<<<<
  *                 field["name"],
  *                 aliases_field_dict.get(field["name"]),
  */
-      __pyx_t_4 = __Pyx_PyDict_GetItemDefault(__pyx_v_readers_field_dict, __pyx_t_7, __pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 637, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_GetItemDefault(__pyx_v_readers_field_dict, __pyx_t_7, __pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_XDECREF_SET(__pyx_v_readers_field, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "fastavro/_read.pyx":641
+      /* "fastavro/_read.pyx":625
  *                 aliases_field_dict.get(field["name"]),
  *             )
  *             if readers_field:             # <<<<<<<<<<<<<<
  *                 record[readers_field["name"]] = _read_data(
  *                     fo,
  */
-      __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_readers_field); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 641, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_readers_field); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 625, __pyx_L1_error)
       if (__pyx_t_3) {
 
-        /* "fastavro/_read.pyx":644
+        /* "fastavro/_read.pyx":628
  *                 record[readers_field["name"]] = _read_data(
  *                     fo,
  *                     field["type"],             # <<<<<<<<<<<<<<
  *                     named_schemas,
  *                     readers_field["type"],
  */
-        __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 644, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 628, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
 
-        /* "fastavro/_read.pyx":646
+        /* "fastavro/_read.pyx":630
  *                     field["type"],
  *                     named_schemas,
  *                     readers_field["type"],             # <<<<<<<<<<<<<<
- *                     return_record_name,
- *                     return_record_name_override,
+ *                     options,
+ *                 )
  */
-        __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_readers_field, __pyx_n_u_type); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 646, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_readers_field, __pyx_n_u_type); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 630, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
 
-        /* "fastavro/_read.pyx":642
+        /* "fastavro/_read.pyx":626
  *             )
  *             if readers_field:
  *                 record[readers_field["name"]] = _read_data(             # <<<<<<<<<<<<<<
  *                     fo,
  *                     field["type"],
  */
-        __pyx_t_8.__pyx_n = 3;
+        __pyx_t_8.__pyx_n = 2;
         __pyx_t_8.reader_schema = __pyx_t_12;
-        __pyx_t_8.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_8.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_7 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_4, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 642, __pyx_L1_error)
+        __pyx_t_8.options = __pyx_v_options;
+        __pyx_t_7 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_4, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 626, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_readers_field, __pyx_n_u_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 642, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_readers_field, __pyx_n_u_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 626, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
-        if (unlikely(PyDict_SetItem(__pyx_v_record, __pyx_t_12, __pyx_t_7) < 0)) __PYX_ERR(0, 642, __pyx_L1_error)
+        if (unlikely(PyDict_SetItem(__pyx_v_record, __pyx_t_12, __pyx_t_7) < 0)) __PYX_ERR(0, 626, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "fastavro/_read.pyx":641
+        /* "fastavro/_read.pyx":625
  *                 aliases_field_dict.get(field["name"]),
  *             )
  *             if readers_field:             # <<<<<<<<<<<<<<
  *                 record[readers_field["name"]] = _read_data(
  *                     fo,
  */
         goto __pyx_L12;
       }
 
-      /* "fastavro/_read.pyx":651
+      /* "fastavro/_read.pyx":634
  *                 )
  *             else:
  *                 _skip_data(fo, field["type"], named_schemas)             # <<<<<<<<<<<<<<
  * 
  *         # fill in default values
  */
       /*else*/ {
-        __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_type); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 651, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_type); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 634, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_12 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_7, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 651, __pyx_L1_error)
+        __pyx_t_12 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_7, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 634, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       }
       __pyx_L12:;
 
-      /* "fastavro/_read.pyx":636
+      /* "fastavro/_read.pyx":620
  *                 aliases_field_dict[alias] = f
  * 
  *         for field in writer_schema["fields"]:             # <<<<<<<<<<<<<<
  *             readers_field = readers_field_dict.get(
  *                 field["name"],
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":654
+    /* "fastavro/_read.pyx":637
  * 
  *         # fill in default values
  *         if len(readers_field_dict) > len(record):             # <<<<<<<<<<<<<<
  *             writer_fields = [f["name"] for f in writer_schema["fields"]]
  *             for f_name, field in readers_field_dict.items():
  */
-    __pyx_t_5 = PyDict_Size(__pyx_v_readers_field_dict); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 654, __pyx_L1_error)
-    __pyx_t_13 = PyDict_Size(__pyx_v_record); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 654, __pyx_L1_error)
+    __pyx_t_5 = PyDict_Size(__pyx_v_readers_field_dict); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 637, __pyx_L1_error)
+    __pyx_t_13 = PyDict_Size(__pyx_v_record); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 637, __pyx_L1_error)
     __pyx_t_3 = ((__pyx_t_5 > __pyx_t_13) != 0);
     if (__pyx_t_3) {
 
-      /* "fastavro/_read.pyx":655
+      /* "fastavro/_read.pyx":638
  *         # fill in default values
  *         if len(readers_field_dict) > len(record):
  *             writer_fields = [f["name"] for f in writer_schema["fields"]]             # <<<<<<<<<<<<<<
  *             for f_name, field in readers_field_dict.items():
  *                 if f_name not in writer_fields and f_name not in record:
  */
       { /* enter inner scope */
-        __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 655, __pyx_L16_error)
+        __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 638, __pyx_L16_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_fields); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 655, __pyx_L16_error)
+        __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_fields); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 638, __pyx_L16_error)
         __Pyx_GOTREF(__pyx_t_12);
         if (likely(PyList_CheckExact(__pyx_t_12)) || PyTuple_CheckExact(__pyx_t_12)) {
           __pyx_t_7 = __pyx_t_12; __Pyx_INCREF(__pyx_t_7); __pyx_t_13 = 0;
           __pyx_t_6 = NULL;
         } else {
-          __pyx_t_13 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 655, __pyx_L16_error)
+          __pyx_t_13 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 638, __pyx_L16_error)
           __Pyx_GOTREF(__pyx_t_7);
-          __pyx_t_6 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 655, __pyx_L16_error)
+          __pyx_t_6 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 638, __pyx_L16_error)
         }
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         for (;;) {
           if (likely(!__pyx_t_6)) {
             if (likely(PyList_CheckExact(__pyx_t_7))) {
               if (__pyx_t_13 >= PyList_GET_SIZE(__pyx_t_7)) break;
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_12 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_13); __Pyx_INCREF(__pyx_t_12); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 655, __pyx_L16_error)
+              __pyx_t_12 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_13); __Pyx_INCREF(__pyx_t_12); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 638, __pyx_L16_error)
               #else
-              __pyx_t_12 = PySequence_ITEM(__pyx_t_7, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 655, __pyx_L16_error)
+              __pyx_t_12 = PySequence_ITEM(__pyx_t_7, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 638, __pyx_L16_error)
               __Pyx_GOTREF(__pyx_t_12);
               #endif
             } else {
               if (__pyx_t_13 >= PyTuple_GET_SIZE(__pyx_t_7)) break;
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_12 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_13); __Pyx_INCREF(__pyx_t_12); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 655, __pyx_L16_error)
+              __pyx_t_12 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_13); __Pyx_INCREF(__pyx_t_12); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 638, __pyx_L16_error)
               #else
-              __pyx_t_12 = PySequence_ITEM(__pyx_t_7, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 655, __pyx_L16_error)
+              __pyx_t_12 = PySequence_ITEM(__pyx_t_7, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 638, __pyx_L16_error)
               __Pyx_GOTREF(__pyx_t_12);
               #endif
             }
           } else {
             __pyx_t_12 = __pyx_t_6(__pyx_t_7);
             if (unlikely(!__pyx_t_12)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                else __PYX_ERR(0, 655, __pyx_L16_error)
+                else __PYX_ERR(0, 638, __pyx_L16_error)
               }
               break;
             }
             __Pyx_GOTREF(__pyx_t_12);
           }
           __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_f, __pyx_t_12);
           __pyx_t_12 = 0;
-          __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_7genexpr__pyx_v_f, __pyx_n_u_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 655, __pyx_L16_error)
+          __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_7genexpr__pyx_v_f, __pyx_n_u_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 638, __pyx_L16_error)
           __Pyx_GOTREF(__pyx_t_12);
-          if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_12))) __PYX_ERR(0, 655, __pyx_L16_error)
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_12))) __PYX_ERR(0, 638, __pyx_L16_error)
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         }
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_XDECREF(__pyx_7genexpr__pyx_v_f); __pyx_7genexpr__pyx_v_f = 0;
         goto __pyx_L19_exit_scope;
         __pyx_L16_error:;
         __Pyx_XDECREF(__pyx_7genexpr__pyx_v_f); __pyx_7genexpr__pyx_v_f = 0;
         goto __pyx_L1_error;
         __pyx_L19_exit_scope:;
       } /* exit inner scope */
       __pyx_v_writer_fields = ((PyObject*)__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "fastavro/_read.pyx":656
+      /* "fastavro/_read.pyx":639
  *         if len(readers_field_dict) > len(record):
  *             writer_fields = [f["name"] for f in writer_schema["fields"]]
  *             for f_name, field in readers_field_dict.items():             # <<<<<<<<<<<<<<
  *                 if f_name not in writer_fields and f_name not in record:
  *                     if "default" in field:
  */
       __pyx_t_13 = 0;
-      __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_readers_field_dict, 1, __pyx_n_s_items, (&__pyx_t_5), (&__pyx_t_11)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 656, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_readers_field_dict, 1, __pyx_n_s_items, (&__pyx_t_5), (&__pyx_t_11)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 639, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_1);
       __pyx_t_1 = __pyx_t_7;
       __pyx_t_7 = 0;
       while (1) {
         __pyx_t_15 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_5, &__pyx_t_13, &__pyx_t_7, &__pyx_t_12, NULL, __pyx_t_11);
         if (unlikely(__pyx_t_15 == 0)) break;
-        if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 656, __pyx_L1_error)
+        if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 639, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_XDECREF_SET(__pyx_v_f_name, __pyx_t_7);
         __pyx_t_7 = 0;
         __Pyx_XDECREF_SET(__pyx_v_field, __pyx_t_12);
         __pyx_t_12 = 0;
 
-        /* "fastavro/_read.pyx":657
+        /* "fastavro/_read.pyx":640
  *             writer_fields = [f["name"] for f in writer_schema["fields"]]
  *             for f_name, field in readers_field_dict.items():
  *                 if f_name not in writer_fields and f_name not in record:             # <<<<<<<<<<<<<<
  *                     if "default" in field:
  *                         record[field["name"]] = field["default"]
  */
-        __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_v_f_name, __pyx_v_writer_fields, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 657, __pyx_L1_error)
+        __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_v_f_name, __pyx_v_writer_fields, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 640, __pyx_L1_error)
         __pyx_t_16 = (__pyx_t_2 != 0);
         if (__pyx_t_16) {
         } else {
           __pyx_t_3 = __pyx_t_16;
           goto __pyx_L23_bool_binop_done;
         }
-        __pyx_t_16 = (__Pyx_PyDict_ContainsTF(__pyx_v_f_name, __pyx_v_record, Py_NE)); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 657, __pyx_L1_error)
+        __pyx_t_16 = (__Pyx_PyDict_ContainsTF(__pyx_v_f_name, __pyx_v_record, Py_NE)); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 640, __pyx_L1_error)
         __pyx_t_2 = (__pyx_t_16 != 0);
         __pyx_t_3 = __pyx_t_2;
         __pyx_L23_bool_binop_done:;
         if (__pyx_t_3) {
 
-          /* "fastavro/_read.pyx":658
+          /* "fastavro/_read.pyx":641
  *             for f_name, field in readers_field_dict.items():
  *                 if f_name not in writer_fields and f_name not in record:
  *                     if "default" in field:             # <<<<<<<<<<<<<<
  *                         record[field["name"]] = field["default"]
  *                     else:
  */
-          __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_default, __pyx_v_field, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 658, __pyx_L1_error)
+          __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_default, __pyx_v_field, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 641, __pyx_L1_error)
           __pyx_t_2 = (__pyx_t_3 != 0);
           if (likely(__pyx_t_2)) {
 
-            /* "fastavro/_read.pyx":659
+            /* "fastavro/_read.pyx":642
  *                 if f_name not in writer_fields and f_name not in record:
  *                     if "default" in field:
  *                         record[field["name"]] = field["default"]             # <<<<<<<<<<<<<<
  *                     else:
  *                         msg = f"No default value for {field['name']}"
  */
-            __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_default); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 659, __pyx_L1_error)
+            __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_default); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 642, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_12);
-            __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 659, __pyx_L1_error)
+            __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 642, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_7);
-            if (unlikely(PyDict_SetItem(__pyx_v_record, __pyx_t_7, __pyx_t_12) < 0)) __PYX_ERR(0, 659, __pyx_L1_error)
+            if (unlikely(PyDict_SetItem(__pyx_v_record, __pyx_t_7, __pyx_t_12) < 0)) __PYX_ERR(0, 642, __pyx_L1_error)
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-            /* "fastavro/_read.pyx":658
+            /* "fastavro/_read.pyx":641
  *             for f_name, field in readers_field_dict.items():
  *                 if f_name not in writer_fields and f_name not in record:
  *                     if "default" in field:             # <<<<<<<<<<<<<<
  *                         record[field["name"]] = field["default"]
  *                     else:
  */
             goto __pyx_L25;
           }
 
-          /* "fastavro/_read.pyx":661
+          /* "fastavro/_read.pyx":644
  *                         record[field["name"]] = field["default"]
  *                     else:
  *                         msg = f"No default value for {field['name']}"             # <<<<<<<<<<<<<<
  *                         raise SchemaResolutionError(msg)
  * 
  */
           /*else*/ {
-            __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 661, __pyx_L1_error)
+            __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 644, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_12);
-            __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_12, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 661, __pyx_L1_error)
+            __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_12, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 644, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-            __pyx_t_12 = __Pyx_PyUnicode_Concat(__pyx_kp_u_No_default_value_for, __pyx_t_7); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 661, __pyx_L1_error)
+            __pyx_t_12 = __Pyx_PyUnicode_Concat(__pyx_kp_u_No_default_value_for, __pyx_t_7); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 644, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_12);
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
             __pyx_v_msg = ((PyObject*)__pyx_t_12);
             __pyx_t_12 = 0;
 
-            /* "fastavro/_read.pyx":662
+            /* "fastavro/_read.pyx":645
  *                     else:
  *                         msg = f"No default value for {field['name']}"
  *                         raise SchemaResolutionError(msg)             # <<<<<<<<<<<<<<
  * 
  *     return record
  */
-            __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_SchemaResolutionError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 662, __pyx_L1_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_SchemaResolutionError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 645, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_7);
             __pyx_t_4 = NULL;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
               __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
               if (likely(__pyx_t_4)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
                 __Pyx_INCREF(__pyx_t_4);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_7, function);
               }
             }
             __pyx_t_12 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_msg);
             __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-            if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 662, __pyx_L1_error)
+            if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 645, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_12);
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
             __Pyx_Raise(__pyx_t_12, 0, 0, 0);
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-            __PYX_ERR(0, 662, __pyx_L1_error)
+            __PYX_ERR(0, 645, __pyx_L1_error)
           }
           __pyx_L25:;
 
-          /* "fastavro/_read.pyx":657
+          /* "fastavro/_read.pyx":640
  *             writer_fields = [f["name"] for f in writer_schema["fields"]]
  *             for f_name, field in readers_field_dict.items():
  *                 if f_name not in writer_fields and f_name not in record:             # <<<<<<<<<<<<<<
  *                     if "default" in field:
  *                         record[field["name"]] = field["default"]
  */
         }
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "fastavro/_read.pyx":654
+      /* "fastavro/_read.pyx":637
  * 
  *         # fill in default values
  *         if len(readers_field_dict) > len(record):             # <<<<<<<<<<<<<<
  *             writer_fields = [f["name"] for f in writer_schema["fields"]]
  *             for f_name, field in readers_field_dict.items():
  */
     }
   }
   __pyx_L3:;
 
-  /* "fastavro/_read.pyx":664
+  /* "fastavro/_read.pyx":647
  *                         raise SchemaResolutionError(msg)
  * 
  *     return record             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_record);
   __pyx_r = __pyx_v_record;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":591
+  /* "fastavro/_read.pyx":577
  * 
  * 
  * cpdef read_record(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
@@ -10580,58 +10541,38 @@
 static PyObject *__pyx_pw_8fastavro_5_read_55read_record(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_8fastavro_5_read_54read_record[] = "A record is encoded by encoding the values of its fields in the order\n    that they are declared. In other words, a record is encoded as just the\n    concatenation of the encodings of its fields.  Field values are encoded per\n    their schema.\n\n    Schema Resolution:\n     * the ordering of fields may be different: fields are matched by name.\n     * schemas for fields with the same name in both records are resolved\n         recursively.\n     * if the writer's record contains a field with a name not present in the\n         reader's record, the writer's value for that field is ignored.\n     * if the reader's record schema has a field that contains a default value,\n         and writer's schema does not have a field with the same name, then the\n         reader should use the default value from its field.\n     * if the reader's record schema has a field with no default value, and\n         writer's schema does not have a field with the same name, then the\n         field's value is unset.\n    ";
 static PyObject *__pyx_pw_8fastavro_5_read_55read_record(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_writer_schema = 0;
   PyObject *__pyx_v_named_schemas = 0;
   PyObject *__pyx_v_reader_schema = 0;
-  PyObject *__pyx_v_return_record_name = 0;
-  PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_options = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_record (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_options,0};
+    PyObject* values[5] = {0,0,0,0,0};
 
-    /* "fastavro/_read.pyx":595
+    /* "fastavro/_read.pyx":581
  *     writer_schema,
  *     named_schemas,
  *     reader_schema=None,             # <<<<<<<<<<<<<<
- *     return_record_name=False,
- *     return_record_name_override=False,
- */
-    values[3] = ((PyObject *)Py_None);
-
-    /* "fastavro/_read.pyx":596
- *     named_schemas,
- *     reader_schema=None,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
+ *     options={},
  * ):
  */
-    values[4] = ((PyObject *)Py_False);
-
-    /* "fastavro/_read.pyx":597
- *     reader_schema=None,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
- * ):
- *     """A record is encoded by encoding the values of its fields in the order
- */
-    values[5] = ((PyObject *)Py_False);
+    values[3] = ((PyObject *)Py_None);
+    values[4] = __pyx_k__6;
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -10646,48 +10587,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_record", 0, 3, 6, 1); __PYX_ERR(0, 591, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_record", 0, 3, 5, 1); __PYX_ERR(0, 577, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_record", 0, 3, 6, 2); __PYX_ERR(0, 591, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_record", 0, 3, 5, 2); __PYX_ERR(0, 577, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema);
           if (value) { values[3] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name);
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options);
           if (value) { values[4] = value; kw_args--; }
         }
-        CYTHON_FALLTHROUGH;
-        case  5:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
-          if (value) { values[5] = value; kw_args--; }
-        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_record") < 0)) __PYX_ERR(0, 591, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_record") < 0)) __PYX_ERR(0, 577, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -10695,55 +10628,53 @@
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_named_schemas = values[2];
     __pyx_v_reader_schema = values[3];
-    __pyx_v_return_record_name = values[4];
-    __pyx_v_return_record_name_override = values[5];
+    __pyx_v_options = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_record", 0, 3, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 591, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_record", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 577, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.read_record", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_54read_record(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
+  __pyx_r = __pyx_pf_8fastavro_5_read_54read_record(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_options);
 
-  /* "fastavro/_read.pyx":591
+  /* "fastavro/_read.pyx":577
  * 
  * 
  * cpdef read_record(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_54read_record(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_54read_record(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_8fastavro_5_read_read_record __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_record", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2.__pyx_n = 3;
+  __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.reader_schema = __pyx_v_reader_schema;
-  __pyx_t_2.return_record_name = __pyx_v_return_record_name;
-  __pyx_t_2.return_record_name_override = __pyx_v_return_record_name_override;
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_record(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_2.options = __pyx_v_options;
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_record(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -10752,15 +10683,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":667
+/* "fastavro/_read.pyx":650
  * 
  * 
  * cpdef skip_record(fo, writer_schema, named_schemas):             # <<<<<<<<<<<<<<
  *     for field in writer_schema["fields"]:
  *         _skip_data(fo, field["type"], named_schemas)
  */
 
@@ -10775,91 +10706,91 @@
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("skip_record", 0);
 
-  /* "fastavro/_read.pyx":668
+  /* "fastavro/_read.pyx":651
  * 
  * cpdef skip_record(fo, writer_schema, named_schemas):
  *     for field in writer_schema["fields"]:             # <<<<<<<<<<<<<<
  *         _skip_data(fo, field["type"], named_schemas)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_fields); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 668, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_writer_schema, __pyx_n_u_fields); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 668, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 651, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 668, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 651, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 668, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 651, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 668, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 651, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 668, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 651, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 668, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 651, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 668, __pyx_L1_error)
+          else __PYX_ERR(0, 651, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_field, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":669
+    /* "fastavro/_read.pyx":652
  * cpdef skip_record(fo, writer_schema, named_schemas):
  *     for field in writer_schema["fields"]:
  *         _skip_data(fo, field["type"], named_schemas)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 669, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_field, __pyx_n_u_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_1, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 669, __pyx_L1_error)
+    __pyx_t_5 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_1, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "fastavro/_read.pyx":668
+    /* "fastavro/_read.pyx":651
  * 
  * cpdef skip_record(fo, writer_schema, named_schemas):
  *     for field in writer_schema["fields"]:             # <<<<<<<<<<<<<<
  *         _skip_data(fo, field["type"], named_schemas)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":667
+  /* "fastavro/_read.pyx":650
  * 
  * 
  * cpdef skip_record(fo, writer_schema, named_schemas):             # <<<<<<<<<<<<<<
  *     for field in writer_schema["fields"]:
  *         _skip_data(fo, field["type"], named_schemas)
  */
 
@@ -10912,40 +10843,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("skip_record", 1, 3, 3, 1); __PYX_ERR(0, 667, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("skip_record", 1, 3, 3, 1); __PYX_ERR(0, 650, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("skip_record", 1, 3, 3, 2); __PYX_ERR(0, 667, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("skip_record", 1, 3, 3, 2); __PYX_ERR(0, 650, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "skip_record") < 0)) __PYX_ERR(0, 667, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "skip_record") < 0)) __PYX_ERR(0, 650, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_named_schemas = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("skip_record", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 667, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("skip_record", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 650, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.skip_record", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8fastavro_5_read_56skip_record(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas);
 
@@ -10959,15 +10890,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("skip_record", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_record(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 667, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_record(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -10976,15 +10907,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":672
+/* "fastavro/_read.pyx":655
  * 
  * 
  * cpdef maybe_promote(data, writer_type, reader_type):             # <<<<<<<<<<<<<<
  *     if writer_type == "int":
  *         # No need to promote to long since they are the same type in Python
  */
 
@@ -10998,259 +10929,259 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("maybe_promote", 0);
 
-  /* "fastavro/_read.pyx":673
+  /* "fastavro/_read.pyx":656
  * 
  * cpdef maybe_promote(data, writer_type, reader_type):
  *     if writer_type == "int":             # <<<<<<<<<<<<<<
  *         # No need to promote to long since they are the same type in Python
  *         if reader_type == "float" or reader_type == "double":
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_writer_type, __pyx_n_u_int, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 673, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_writer_type, __pyx_n_u_int, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 656, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "fastavro/_read.pyx":675
+    /* "fastavro/_read.pyx":658
  *     if writer_type == "int":
  *         # No need to promote to long since they are the same type in Python
  *         if reader_type == "float" or reader_type == "double":             # <<<<<<<<<<<<<<
  *             return float(data)
  *     if writer_type == "long":
  */
-    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_float, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 675, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_float, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 658, __pyx_L1_error)
     if (!__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L5_bool_binop_done;
     }
-    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_double, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 675, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_double, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 658, __pyx_L1_error)
     __pyx_t_1 = __pyx_t_2;
     __pyx_L5_bool_binop_done:;
     if (__pyx_t_1) {
 
-      /* "fastavro/_read.pyx":676
+      /* "fastavro/_read.pyx":659
  *         # No need to promote to long since they are the same type in Python
  *         if reader_type == "float" or reader_type == "double":
  *             return float(data)             # <<<<<<<<<<<<<<
  *     if writer_type == "long":
  *         if reader_type == "float" or reader_type == "double":
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_3 = __Pyx_PyNumber_Float(__pyx_v_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 676, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyNumber_Float(__pyx_v_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 659, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "fastavro/_read.pyx":675
+      /* "fastavro/_read.pyx":658
  *     if writer_type == "int":
  *         # No need to promote to long since they are the same type in Python
  *         if reader_type == "float" or reader_type == "double":             # <<<<<<<<<<<<<<
  *             return float(data)
  *     if writer_type == "long":
  */
     }
 
-    /* "fastavro/_read.pyx":673
+    /* "fastavro/_read.pyx":656
  * 
  * cpdef maybe_promote(data, writer_type, reader_type):
  *     if writer_type == "int":             # <<<<<<<<<<<<<<
  *         # No need to promote to long since they are the same type in Python
  *         if reader_type == "float" or reader_type == "double":
  */
   }
 
-  /* "fastavro/_read.pyx":677
+  /* "fastavro/_read.pyx":660
  *         if reader_type == "float" or reader_type == "double":
  *             return float(data)
  *     if writer_type == "long":             # <<<<<<<<<<<<<<
  *         if reader_type == "float" or reader_type == "double":
  *             return float(data)
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_writer_type, __pyx_n_u_long, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 677, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_writer_type, __pyx_n_u_long, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 660, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "fastavro/_read.pyx":678
+    /* "fastavro/_read.pyx":661
  *             return float(data)
  *     if writer_type == "long":
  *         if reader_type == "float" or reader_type == "double":             # <<<<<<<<<<<<<<
  *             return float(data)
  *     if writer_type == "string" and reader_type == "bytes":
  */
-    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_float, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 678, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_float, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 661, __pyx_L1_error)
     if (!__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L9_bool_binop_done;
     }
-    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_double, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 678, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_double, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 661, __pyx_L1_error)
     __pyx_t_1 = __pyx_t_2;
     __pyx_L9_bool_binop_done:;
     if (__pyx_t_1) {
 
-      /* "fastavro/_read.pyx":679
+      /* "fastavro/_read.pyx":662
  *     if writer_type == "long":
  *         if reader_type == "float" or reader_type == "double":
  *             return float(data)             # <<<<<<<<<<<<<<
  *     if writer_type == "string" and reader_type == "bytes":
  *         return data.encode()
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_3 = __Pyx_PyNumber_Float(__pyx_v_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 679, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyNumber_Float(__pyx_v_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 662, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "fastavro/_read.pyx":678
+      /* "fastavro/_read.pyx":661
  *             return float(data)
  *     if writer_type == "long":
  *         if reader_type == "float" or reader_type == "double":             # <<<<<<<<<<<<<<
  *             return float(data)
  *     if writer_type == "string" and reader_type == "bytes":
  */
     }
 
-    /* "fastavro/_read.pyx":677
+    /* "fastavro/_read.pyx":660
  *         if reader_type == "float" or reader_type == "double":
  *             return float(data)
  *     if writer_type == "long":             # <<<<<<<<<<<<<<
  *         if reader_type == "float" or reader_type == "double":
  *             return float(data)
  */
   }
 
-  /* "fastavro/_read.pyx":680
+  /* "fastavro/_read.pyx":663
  *         if reader_type == "float" or reader_type == "double":
  *             return float(data)
  *     if writer_type == "string" and reader_type == "bytes":             # <<<<<<<<<<<<<<
  *         return data.encode()
  *     if writer_type == "bytes" and reader_type == "string":
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_writer_type, __pyx_n_u_string, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_writer_type, __pyx_n_u_string, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 663, __pyx_L1_error)
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L12_bool_binop_done;
   }
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_bytes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_bytes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 663, __pyx_L1_error)
   __pyx_t_1 = __pyx_t_2;
   __pyx_L12_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "fastavro/_read.pyx":681
+    /* "fastavro/_read.pyx":664
  *             return float(data)
  *     if writer_type == "string" and reader_type == "bytes":
  *         return data.encode()             # <<<<<<<<<<<<<<
  *     if writer_type == "bytes" and reader_type == "string":
  *         return data.decode()
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 681, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 681, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "fastavro/_read.pyx":680
+    /* "fastavro/_read.pyx":663
  *         if reader_type == "float" or reader_type == "double":
  *             return float(data)
  *     if writer_type == "string" and reader_type == "bytes":             # <<<<<<<<<<<<<<
  *         return data.encode()
  *     if writer_type == "bytes" and reader_type == "string":
  */
   }
 
-  /* "fastavro/_read.pyx":682
+  /* "fastavro/_read.pyx":665
  *     if writer_type == "string" and reader_type == "bytes":
  *         return data.encode()
  *     if writer_type == "bytes" and reader_type == "string":             # <<<<<<<<<<<<<<
  *         return data.decode()
  *     return data
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_writer_type, __pyx_n_u_bytes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_writer_type, __pyx_n_u_bytes, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 665, __pyx_L1_error)
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L15_bool_binop_done;
   }
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_string, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_reader_type, __pyx_n_u_string, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 665, __pyx_L1_error)
   __pyx_t_1 = __pyx_t_2;
   __pyx_L15_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "fastavro/_read.pyx":683
+    /* "fastavro/_read.pyx":666
  *         return data.encode()
  *     if writer_type == "bytes" and reader_type == "string":
  *         return data.decode()             # <<<<<<<<<<<<<<
  *     return data
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 683, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 666, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 683, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 666, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "fastavro/_read.pyx":682
+    /* "fastavro/_read.pyx":665
  *     if writer_type == "string" and reader_type == "bytes":
  *         return data.encode()
  *     if writer_type == "bytes" and reader_type == "string":             # <<<<<<<<<<<<<<
  *         return data.decode()
  *     return data
  */
   }
 
-  /* "fastavro/_read.pyx":684
+  /* "fastavro/_read.pyx":667
  *     if writer_type == "bytes" and reader_type == "string":
  *         return data.decode()
  *     return data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":672
+  /* "fastavro/_read.pyx":655
  * 
  * 
  * cpdef maybe_promote(data, writer_type, reader_type):             # <<<<<<<<<<<<<<
  *     if writer_type == "int":
  *         # No need to promote to long since they are the same type in Python
  */
 
@@ -11300,40 +11231,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_type)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("maybe_promote", 1, 3, 3, 1); __PYX_ERR(0, 672, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("maybe_promote", 1, 3, 3, 1); __PYX_ERR(0, 655, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_type)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("maybe_promote", 1, 3, 3, 2); __PYX_ERR(0, 672, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("maybe_promote", 1, 3, 3, 2); __PYX_ERR(0, 655, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "maybe_promote") < 0)) __PYX_ERR(0, 672, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "maybe_promote") < 0)) __PYX_ERR(0, 655, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_data = values[0];
     __pyx_v_writer_type = values[1];
     __pyx_v_reader_type = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("maybe_promote", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 672, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("maybe_promote", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 655, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.maybe_promote", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8fastavro_5_read_58maybe_promote(__pyx_self, __pyx_v_data, __pyx_v_writer_type, __pyx_v_reader_type);
 
@@ -11347,15 +11278,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("maybe_promote", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_maybe_promote(__pyx_v_data, __pyx_v_writer_type, __pyx_v_reader_type, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 672, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_maybe_promote(__pyx_v_data, __pyx_v_writer_type, __pyx_v_reader_type, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 655, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -11364,152 +11295,133 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":687
+/* "fastavro/_read.pyx":670
  * 
  * 
  * cpdef _read_data(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
 static PyObject *__pyx_pw_8fastavro_5_read_61_read_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read__read_data(PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_8fastavro_5_read__read_data *__pyx_optional_args) {
 
-  /* "fastavro/_read.pyx":691
+  /* "fastavro/_read.pyx":674
  *     writer_schema,
  *     named_schemas,
  *     reader_schema=None,             # <<<<<<<<<<<<<<
- *     return_record_name=False,
- *     return_record_name_override=False,
- */
-  PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
-
-  /* "fastavro/_read.pyx":692
- *     named_schemas,
- *     reader_schema=None,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
+ *     options={},
  * ):
  */
-  PyObject *__pyx_v_return_record_name = ((PyObject *)Py_False);
-
-  /* "fastavro/_read.pyx":693
- *     reader_schema=None,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
- * ):
- *     """Read data from file object according to schema."""
- */
-  PyObject *__pyx_v_return_record_name_override = ((PyObject *)Py_False);
+  PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
+  PyObject *__pyx_v_options = __pyx_k__7;
   PyObject *__pyx_v_record_type = NULL;
   PyObject *__pyx_v_data = NULL;
   PyObject *__pyx_v_logical_type = NULL;
   PyObject *__pyx_v_fn = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  __pyx_t_8fastavro_5_read_long64 __pyx_t_9;
-  struct __pyx_opt_args_8fastavro_5_read_read_array __pyx_t_10;
-  struct __pyx_opt_args_8fastavro_5_read_read_map __pyx_t_11;
-  struct __pyx_opt_args_8fastavro_5_read_read_union __pyx_t_12;
-  struct __pyx_opt_args_8fastavro_5_read_read_record __pyx_t_13;
-  PyObject *__pyx_t_14 = NULL;
-  struct __pyx_opt_args_8fastavro_5_read__read_data __pyx_t_15;
-  int __pyx_t_16;
-  Py_ssize_t __pyx_t_17;
-  Py_UCS4 __pyx_t_18;
-  PyObject *__pyx_t_19 = NULL;
+  struct __pyx_opt_args_8fastavro_5_read_read_utf8 __pyx_t_8;
+  int __pyx_t_9;
+  __pyx_t_8fastavro_5_read_long64 __pyx_t_10;
+  struct __pyx_opt_args_8fastavro_5_read_read_array __pyx_t_11;
+  struct __pyx_opt_args_8fastavro_5_read_read_map __pyx_t_12;
+  struct __pyx_opt_args_8fastavro_5_read_read_union __pyx_t_13;
+  struct __pyx_opt_args_8fastavro_5_read_read_record __pyx_t_14;
+  PyObject *__pyx_t_15 = NULL;
+  struct __pyx_opt_args_8fastavro_5_read__read_data __pyx_t_16;
+  int __pyx_t_17;
+  Py_ssize_t __pyx_t_18;
+  Py_UCS4 __pyx_t_19;
+  PyObject *__pyx_t_20 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_read_data", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_reader_schema = __pyx_optional_args->reader_schema;
       if (__pyx_optional_args->__pyx_n > 1) {
-        __pyx_v_return_record_name = __pyx_optional_args->return_record_name;
-        if (__pyx_optional_args->__pyx_n > 2) {
-          __pyx_v_return_record_name_override = __pyx_optional_args->return_record_name_override;
-        }
+        __pyx_v_options = __pyx_optional_args->options;
       }
     }
   }
   __Pyx_INCREF(__pyx_v_reader_schema);
 
-  /* "fastavro/_read.pyx":697
+  /* "fastavro/_read.pyx":679
  *     """Read data from file object according to schema."""
  * 
  *     record_type = extract_record_type(writer_schema)             # <<<<<<<<<<<<<<
  * 
  *     if reader_schema:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_extract_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 697, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_extract_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_writer_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_writer_schema);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 697, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_record_type = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":699
+  /* "fastavro/_read.pyx":681
  *     record_type = extract_record_type(writer_schema)
  * 
  *     if reader_schema:             # <<<<<<<<<<<<<<
  *         reader_schema = match_schemas(writer_schema, reader_schema)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 699, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 681, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":700
+    /* "fastavro/_read.pyx":682
  * 
  *     if reader_schema:
  *         reader_schema = match_schemas(writer_schema, reader_schema)             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_match_schemas(__pyx_v_writer_schema, __pyx_v_reader_schema, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 700, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_match_schemas(__pyx_v_writer_schema, __pyx_v_reader_schema, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 682, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_reader_schema, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":699
+    /* "fastavro/_read.pyx":681
  *     record_type = extract_record_type(writer_schema)
  * 
  *     if reader_schema:             # <<<<<<<<<<<<<<
  *         reader_schema = match_schemas(writer_schema, reader_schema)
  * 
  */
   }
 
-  /* "fastavro/_read.pyx":702
+  /* "fastavro/_read.pyx":684
  *         reader_schema = match_schemas(writer_schema, reader_schema)
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         if record_type == "null":
  *             data = read_null(fo)
  */
   {
@@ -11517,629 +11429,632 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
     __Pyx_XGOTREF(__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_6);
     __Pyx_XGOTREF(__pyx_t_7);
     /*try:*/ {
 
-      /* "fastavro/_read.pyx":703
+      /* "fastavro/_read.pyx":685
  * 
  *     try:
  *         if record_type == "null":             # <<<<<<<<<<<<<<
  *             data = read_null(fo)
  *         elif record_type == "string":
  */
-      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_null, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 703, __pyx_L4_error)
+      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_null, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 685, __pyx_L4_error)
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":704
+        /* "fastavro/_read.pyx":686
  *     try:
  *         if record_type == "null":
  *             data = read_null(fo)             # <<<<<<<<<<<<<<
  *         elif record_type == "string":
- *             data = read_utf8(fo)
+ *             data = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  */
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_null(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 704, __pyx_L4_error)
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_null(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 686, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":703
+        /* "fastavro/_read.pyx":685
  * 
  *     try:
  *         if record_type == "null":             # <<<<<<<<<<<<<<
  *             data = read_null(fo)
  *         elif record_type == "string":
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":705
+      /* "fastavro/_read.pyx":687
  *         if record_type == "null":
  *             data = read_null(fo)
  *         elif record_type == "string":             # <<<<<<<<<<<<<<
- *             data = read_utf8(fo)
+ *             data = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  *         elif record_type == "int" or record_type == "long":
  */
-      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_string, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 705, __pyx_L4_error)
+      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_string, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 687, __pyx_L4_error)
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":706
+        /* "fastavro/_read.pyx":688
  *             data = read_null(fo)
  *         elif record_type == "string":
- *             data = read_utf8(fo)             # <<<<<<<<<<<<<<
+ *             data = read_utf8(fo, options.get("handle_unicode_errors", "strict"))             # <<<<<<<<<<<<<<
  *         elif record_type == "int" or record_type == "long":
  *             data = read_long(fo)
  */
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_utf8(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 706, __pyx_L4_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_options, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 688, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 688, __pyx_L4_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_8.__pyx_n = 1;
+        __pyx_t_8.handle_unicode_errors = __pyx_t_2;
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_utf8(__pyx_v_fo, 0, &__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 688, __pyx_L4_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":705
+        /* "fastavro/_read.pyx":687
  *         if record_type == "null":
  *             data = read_null(fo)
  *         elif record_type == "string":             # <<<<<<<<<<<<<<
- *             data = read_utf8(fo)
+ *             data = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  *         elif record_type == "int" or record_type == "long":
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":707
+      /* "fastavro/_read.pyx":689
  *         elif record_type == "string":
- *             data = read_utf8(fo)
+ *             data = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  *         elif record_type == "int" or record_type == "long":             # <<<<<<<<<<<<<<
  *             data = read_long(fo)
  *         elif record_type == "float":
  */
-      __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_int, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 707, __pyx_L4_error)
-      if (!__pyx_t_8) {
+      __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_int, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 689, __pyx_L4_error)
+      if (!__pyx_t_9) {
       } else {
-        __pyx_t_4 = __pyx_t_8;
+        __pyx_t_4 = __pyx_t_9;
         goto __pyx_L11_bool_binop_done;
       }
-      __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_long, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 707, __pyx_L4_error)
-      __pyx_t_4 = __pyx_t_8;
+      __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_long, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 689, __pyx_L4_error)
+      __pyx_t_4 = __pyx_t_9;
       __pyx_L11_bool_binop_done:;
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":708
- *             data = read_utf8(fo)
+        /* "fastavro/_read.pyx":690
+ *             data = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  *         elif record_type == "int" or record_type == "long":
  *             data = read_long(fo)             # <<<<<<<<<<<<<<
  *         elif record_type == "float":
  *             data = read_float(fo)
  */
-        __pyx_t_9 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_9 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 708, __pyx_L4_error)
-        __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 708, __pyx_L4_error)
+        __pyx_t_10 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_10 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 690, __pyx_L4_error)
+        __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 690, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":707
+        /* "fastavro/_read.pyx":689
  *         elif record_type == "string":
- *             data = read_utf8(fo)
+ *             data = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
  *         elif record_type == "int" or record_type == "long":             # <<<<<<<<<<<<<<
  *             data = read_long(fo)
  *         elif record_type == "float":
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":709
+      /* "fastavro/_read.pyx":691
  *         elif record_type == "int" or record_type == "long":
  *             data = read_long(fo)
  *         elif record_type == "float":             # <<<<<<<<<<<<<<
  *             data = read_float(fo)
  *         elif record_type == "double":
  */
-      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_float, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 709, __pyx_L4_error)
+      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_float, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 691, __pyx_L4_error)
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":710
+        /* "fastavro/_read.pyx":692
  *             data = read_long(fo)
  *         elif record_type == "float":
  *             data = read_float(fo)             # <<<<<<<<<<<<<<
  *         elif record_type == "double":
  *             data = read_double(fo)
  */
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_float(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 710, __pyx_L4_error)
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_float(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 692, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":709
+        /* "fastavro/_read.pyx":691
  *         elif record_type == "int" or record_type == "long":
  *             data = read_long(fo)
  *         elif record_type == "float":             # <<<<<<<<<<<<<<
  *             data = read_float(fo)
  *         elif record_type == "double":
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":711
+      /* "fastavro/_read.pyx":693
  *         elif record_type == "float":
  *             data = read_float(fo)
  *         elif record_type == "double":             # <<<<<<<<<<<<<<
  *             data = read_double(fo)
  *         elif record_type == "boolean":
  */
-      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_double, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 711, __pyx_L4_error)
+      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_double, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 693, __pyx_L4_error)
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":712
+        /* "fastavro/_read.pyx":694
  *             data = read_float(fo)
  *         elif record_type == "double":
  *             data = read_double(fo)             # <<<<<<<<<<<<<<
  *         elif record_type == "boolean":
  *             data = read_boolean(fo)
  */
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_double(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L4_error)
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_double(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 694, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":711
+        /* "fastavro/_read.pyx":693
  *         elif record_type == "float":
  *             data = read_float(fo)
  *         elif record_type == "double":             # <<<<<<<<<<<<<<
  *             data = read_double(fo)
  *         elif record_type == "boolean":
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":713
+      /* "fastavro/_read.pyx":695
  *         elif record_type == "double":
  *             data = read_double(fo)
  *         elif record_type == "boolean":             # <<<<<<<<<<<<<<
  *             data = read_boolean(fo)
  *         elif record_type == "bytes":
  */
-      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_boolean, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 713, __pyx_L4_error)
+      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_boolean, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 695, __pyx_L4_error)
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":714
+        /* "fastavro/_read.pyx":696
  *             data = read_double(fo)
  *         elif record_type == "boolean":
  *             data = read_boolean(fo)             # <<<<<<<<<<<<<<
  *         elif record_type == "bytes":
  *             data = read_bytes(fo)
  */
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_boolean(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 714, __pyx_L4_error)
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_boolean(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 696, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":713
+        /* "fastavro/_read.pyx":695
  *         elif record_type == "double":
  *             data = read_double(fo)
  *         elif record_type == "boolean":             # <<<<<<<<<<<<<<
  *             data = read_boolean(fo)
  *         elif record_type == "bytes":
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":715
+      /* "fastavro/_read.pyx":697
  *         elif record_type == "boolean":
  *             data = read_boolean(fo)
  *         elif record_type == "bytes":             # <<<<<<<<<<<<<<
  *             data = read_bytes(fo)
  *         elif record_type == "fixed":
  */
-      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_bytes, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 715, __pyx_L4_error)
+      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_bytes, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 697, __pyx_L4_error)
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":716
+        /* "fastavro/_read.pyx":698
  *             data = read_boolean(fo)
  *         elif record_type == "bytes":
  *             data = read_bytes(fo)             # <<<<<<<<<<<<<<
  *         elif record_type == "fixed":
  *             data = read_fixed(fo, writer_schema)
  */
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 716, __pyx_L4_error)
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 698, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":715
+        /* "fastavro/_read.pyx":697
  *         elif record_type == "boolean":
  *             data = read_boolean(fo)
  *         elif record_type == "bytes":             # <<<<<<<<<<<<<<
  *             data = read_bytes(fo)
  *         elif record_type == "fixed":
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":717
+      /* "fastavro/_read.pyx":699
  *         elif record_type == "bytes":
  *             data = read_bytes(fo)
  *         elif record_type == "fixed":             # <<<<<<<<<<<<<<
  *             data = read_fixed(fo, writer_schema)
  *         elif record_type == "enum":
  */
-      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_fixed, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 717, __pyx_L4_error)
+      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_fixed, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 699, __pyx_L4_error)
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":718
+        /* "fastavro/_read.pyx":700
  *             data = read_bytes(fo)
  *         elif record_type == "fixed":
  *             data = read_fixed(fo, writer_schema)             # <<<<<<<<<<<<<<
  *         elif record_type == "enum":
  *             data = read_enum(fo, writer_schema, reader_schema)
  */
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_fixed(__pyx_v_fo, __pyx_v_writer_schema, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 718, __pyx_L4_error)
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_fixed(__pyx_v_fo, __pyx_v_writer_schema, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 700, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":717
+        /* "fastavro/_read.pyx":699
  *         elif record_type == "bytes":
  *             data = read_bytes(fo)
  *         elif record_type == "fixed":             # <<<<<<<<<<<<<<
  *             data = read_fixed(fo, writer_schema)
  *         elif record_type == "enum":
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":719
+      /* "fastavro/_read.pyx":701
  *         elif record_type == "fixed":
  *             data = read_fixed(fo, writer_schema)
  *         elif record_type == "enum":             # <<<<<<<<<<<<<<
  *             data = read_enum(fo, writer_schema, reader_schema)
  *         elif record_type == "array":
  */
-      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_enum, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 719, __pyx_L4_error)
+      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_enum, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 701, __pyx_L4_error)
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":720
+        /* "fastavro/_read.pyx":702
  *             data = read_fixed(fo, writer_schema)
  *         elif record_type == "enum":
  *             data = read_enum(fo, writer_schema, reader_schema)             # <<<<<<<<<<<<<<
  *         elif record_type == "array":
  *             data = read_array(
  */
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_enum(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_reader_schema, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L4_error)
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_enum(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_reader_schema, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 702, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":719
+        /* "fastavro/_read.pyx":701
  *         elif record_type == "fixed":
  *             data = read_fixed(fo, writer_schema)
  *         elif record_type == "enum":             # <<<<<<<<<<<<<<
  *             data = read_enum(fo, writer_schema, reader_schema)
  *         elif record_type == "array":
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":721
+      /* "fastavro/_read.pyx":703
  *         elif record_type == "enum":
  *             data = read_enum(fo, writer_schema, reader_schema)
  *         elif record_type == "array":             # <<<<<<<<<<<<<<
  *             data = read_array(
  *                 fo,
  */
-      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_array, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 721, __pyx_L4_error)
+      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_array, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 703, __pyx_L4_error)
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":722
+        /* "fastavro/_read.pyx":704
  *             data = read_enum(fo, writer_schema, reader_schema)
  *         elif record_type == "array":
  *             data = read_array(             # <<<<<<<<<<<<<<
  *                 fo,
  *                 writer_schema,
  */
-        __pyx_t_10.__pyx_n = 3;
-        __pyx_t_10.reader_schema = __pyx_v_reader_schema;
-        __pyx_t_10.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_10.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_array(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 722, __pyx_L4_error)
+        __pyx_t_11.__pyx_n = 2;
+        __pyx_t_11.reader_schema = __pyx_v_reader_schema;
+        __pyx_t_11.options = __pyx_v_options;
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_array(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 704, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":721
+        /* "fastavro/_read.pyx":703
  *         elif record_type == "enum":
  *             data = read_enum(fo, writer_schema, reader_schema)
  *         elif record_type == "array":             # <<<<<<<<<<<<<<
  *             data = read_array(
  *                 fo,
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":730
- *                 return_record_name_override,
+      /* "fastavro/_read.pyx":711
+ *                 options,
  *             )
  *         elif record_type == "map":             # <<<<<<<<<<<<<<
  *             data = read_map(
  *                 fo,
  */
-      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_map, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 730, __pyx_L4_error)
+      __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_map, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 711, __pyx_L4_error)
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":731
+        /* "fastavro/_read.pyx":712
  *             )
  *         elif record_type == "map":
  *             data = read_map(             # <<<<<<<<<<<<<<
  *                 fo,
  *                 writer_schema,
  */
-        __pyx_t_11.__pyx_n = 3;
-        __pyx_t_11.reader_schema = __pyx_v_reader_schema;
-        __pyx_t_11.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_11.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_map(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 731, __pyx_L4_error)
+        __pyx_t_12.__pyx_n = 2;
+        __pyx_t_12.reader_schema = __pyx_v_reader_schema;
+        __pyx_t_12.options = __pyx_v_options;
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_map(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":730
- *                 return_record_name_override,
+        /* "fastavro/_read.pyx":711
+ *                 options,
  *             )
  *         elif record_type == "map":             # <<<<<<<<<<<<<<
  *             data = read_map(
  *                 fo,
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":739
- *                 return_record_name_override,
+      /* "fastavro/_read.pyx":719
+ *                 options,
  *             )
  *         elif record_type == "union" or record_type == "error_union":             # <<<<<<<<<<<<<<
  *             data = read_union(
  *                 fo,
  */
-      __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_union, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 739, __pyx_L4_error)
-      if (!__pyx_t_8) {
+      __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_union, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 719, __pyx_L4_error)
+      if (!__pyx_t_9) {
       } else {
-        __pyx_t_4 = __pyx_t_8;
+        __pyx_t_4 = __pyx_t_9;
         goto __pyx_L13_bool_binop_done;
       }
-      __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_error_union, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 739, __pyx_L4_error)
-      __pyx_t_4 = __pyx_t_8;
+      __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_error_union, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 719, __pyx_L4_error)
+      __pyx_t_4 = __pyx_t_9;
       __pyx_L13_bool_binop_done:;
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":740
+        /* "fastavro/_read.pyx":720
  *             )
  *         elif record_type == "union" or record_type == "error_union":
  *             data = read_union(             # <<<<<<<<<<<<<<
  *                 fo,
  *                 writer_schema,
  */
-        __pyx_t_12.__pyx_n = 3;
-        __pyx_t_12.reader_schema = __pyx_v_reader_schema;
-        __pyx_t_12.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_12.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_union(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 740, __pyx_L4_error)
+        __pyx_t_13.__pyx_n = 2;
+        __pyx_t_13.reader_schema = __pyx_v_reader_schema;
+        __pyx_t_13.options = __pyx_v_options;
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_union(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":739
- *                 return_record_name_override,
+        /* "fastavro/_read.pyx":719
+ *                 options,
  *             )
  *         elif record_type == "union" or record_type == "error_union":             # <<<<<<<<<<<<<<
  *             data = read_union(
  *                 fo,
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":748
- *                 return_record_name_override,
+      /* "fastavro/_read.pyx":727
+ *                 options,
  *             )
  *         elif record_type == "record" or record_type == "error":             # <<<<<<<<<<<<<<
  *             data = read_record(
  *                 fo,
  */
-      __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_record, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 748, __pyx_L4_error)
-      if (!__pyx_t_8) {
+      __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_record, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 727, __pyx_L4_error)
+      if (!__pyx_t_9) {
       } else {
-        __pyx_t_4 = __pyx_t_8;
+        __pyx_t_4 = __pyx_t_9;
         goto __pyx_L15_bool_binop_done;
       }
-      __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_error, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 748, __pyx_L4_error)
-      __pyx_t_4 = __pyx_t_8;
+      __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_error, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 727, __pyx_L4_error)
+      __pyx_t_4 = __pyx_t_9;
       __pyx_L15_bool_binop_done:;
       if (__pyx_t_4) {
 
-        /* "fastavro/_read.pyx":749
+        /* "fastavro/_read.pyx":728
  *             )
  *         elif record_type == "record" or record_type == "error":
  *             data = read_record(             # <<<<<<<<<<<<<<
  *                 fo,
  *                 writer_schema,
  */
-        __pyx_t_13.__pyx_n = 3;
-        __pyx_t_13.reader_schema = __pyx_v_reader_schema;
-        __pyx_t_13.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_13.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_record(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 749, __pyx_L4_error)
+        __pyx_t_14.__pyx_n = 2;
+        __pyx_t_14.reader_schema = __pyx_v_reader_schema;
+        __pyx_t_14.options = __pyx_v_options;
+        __pyx_t_1 = __pyx_f_8fastavro_5_read_read_record(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_14); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 728, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":748
- *                 return_record_name_override,
+        /* "fastavro/_read.pyx":727
+ *                 options,
  *             )
  *         elif record_type == "record" or record_type == "error":             # <<<<<<<<<<<<<<
  *             data = read_record(
  *                 fo,
  */
         goto __pyx_L10;
       }
 
-      /* "fastavro/_read.pyx":758
+      /* "fastavro/_read.pyx":736
  *             )
  *         else:
  *             return _read_data(             # <<<<<<<<<<<<<<
  *                 fo,
  *                 named_schemas["writer"][record_type],
  */
       /*else*/ {
         __Pyx_XDECREF(__pyx_r);
 
-        /* "fastavro/_read.pyx":760
+        /* "fastavro/_read.pyx":738
  *             return _read_data(
  *                 fo,
  *                 named_schemas["writer"][record_type],             # <<<<<<<<<<<<<<
  *                 named_schemas,
  *                 named_schemas["reader"].get(reader_schema),
  */
-        __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_named_schemas, __pyx_n_u_writer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 760, __pyx_L4_error)
+        __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_named_schemas, __pyx_n_u_writer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 738, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 760, __pyx_L4_error)
+        __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 738, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "fastavro/_read.pyx":762
+        /* "fastavro/_read.pyx":740
  *                 named_schemas["writer"][record_type],
  *                 named_schemas,
  *                 named_schemas["reader"].get(reader_schema),             # <<<<<<<<<<<<<<
- *                 return_record_name,
- *                 return_record_name_override,
+ *                 options,
+ *             )
  */
-        __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_named_schemas, __pyx_n_u_reader); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 762, __pyx_L4_error)
+        __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_named_schemas, __pyx_n_u_reader); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 740, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 762, __pyx_L4_error)
-        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 740, __pyx_L4_error)
+        __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_3 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
-          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_14);
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_15))) {
+          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_15);
           if (likely(__pyx_t_3)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_14, function);
+            __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
-        __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_3, __pyx_v_reader_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_v_reader_schema);
+        __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_3, __pyx_v_reader_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_v_reader_schema);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 762, __pyx_L4_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 740, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
 
-        /* "fastavro/_read.pyx":758
+        /* "fastavro/_read.pyx":736
  *             )
  *         else:
  *             return _read_data(             # <<<<<<<<<<<<<<
  *                 fo,
  *                 named_schemas["writer"][record_type],
  */
-        __pyx_t_15.__pyx_n = 3;
-        __pyx_t_15.reader_schema = __pyx_t_1;
-        __pyx_t_15.return_record_name = __pyx_v_return_record_name;
-        __pyx_t_15.return_record_name_override = __pyx_v_return_record_name_override;
-        __pyx_t_14 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_2, __pyx_v_named_schemas, 0, &__pyx_t_15); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 758, __pyx_L4_error)
-        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_16.__pyx_n = 2;
+        __pyx_t_16.reader_schema = __pyx_t_1;
+        __pyx_t_16.options = __pyx_v_options;
+        __pyx_t_15 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_t_2, __pyx_v_named_schemas, 0, &__pyx_t_16); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 736, __pyx_L4_error)
+        __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_r = __pyx_t_14;
-        __pyx_t_14 = 0;
+        __pyx_r = __pyx_t_15;
+        __pyx_t_15 = 0;
         goto __pyx_L8_try_return;
       }
       __pyx_L10:;
 
-      /* "fastavro/_read.pyx":702
+      /* "fastavro/_read.pyx":684
  *         reader_schema = match_schemas(writer_schema, reader_schema)
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         if record_type == "null":
  *             data = read_null(fo)
  */
     }
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     goto __pyx_L9_try_end;
     __pyx_L4_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+    __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "fastavro/_read.pyx":766
- *                 return_record_name_override,
+    /* "fastavro/_read.pyx":743
+ *                 options,
  *             )
  *     except ReadError:             # <<<<<<<<<<<<<<
  *         raise EOFError(f"cannot read {record_type} from {fo}")
  * 
  */
-    __Pyx_ErrFetch(&__pyx_t_14, &__pyx_t_1, &__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ReadError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 766, __pyx_L6_except_error)
+    __Pyx_ErrFetch(&__pyx_t_15, &__pyx_t_1, &__pyx_t_2);
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ReadError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 743, __pyx_L6_except_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_16 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_14, __pyx_t_3);
+    __pyx_t_17 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_15, __pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_ErrRestore(__pyx_t_14, __pyx_t_1, __pyx_t_2);
-    __pyx_t_14 = 0; __pyx_t_1 = 0; __pyx_t_2 = 0;
-    if (__pyx_t_16) {
+    __Pyx_ErrRestore(__pyx_t_15, __pyx_t_1, __pyx_t_2);
+    __pyx_t_15 = 0; __pyx_t_1 = 0; __pyx_t_2 = 0;
+    if (__pyx_t_17) {
       __Pyx_AddTraceback("fastavro._read._read_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_14) < 0) __PYX_ERR(0, 766, __pyx_L6_except_error)
+      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_15) < 0) __PYX_ERR(0, 743, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_14);
+      __Pyx_GOTREF(__pyx_t_15);
 
-      /* "fastavro/_read.pyx":767
+      /* "fastavro/_read.pyx":744
  *             )
  *     except ReadError:
  *         raise EOFError(f"cannot read {record_type} from {fo}")             # <<<<<<<<<<<<<<
  * 
  *     if "logicalType" in writer_schema:
  */
-      __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 767, __pyx_L6_except_error)
+      __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 744, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_17 = 0;
-      __pyx_t_18 = 127;
+      __pyx_t_18 = 0;
+      __pyx_t_19 = 127;
       __Pyx_INCREF(__pyx_kp_u_cannot_read);
-      __pyx_t_17 += 12;
+      __pyx_t_18 += 12;
       __Pyx_GIVEREF(__pyx_kp_u_cannot_read);
       PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_cannot_read);
-      __pyx_t_19 = __Pyx_PyObject_FormatSimple(__pyx_v_record_type, __pyx_empty_unicode); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 767, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_19);
-      __pyx_t_18 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) > __pyx_t_18) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) : __pyx_t_18;
-      __pyx_t_17 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_19);
-      __Pyx_GIVEREF(__pyx_t_19);
-      PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_19);
-      __pyx_t_19 = 0;
+      __pyx_t_20 = __Pyx_PyObject_FormatSimple(__pyx_v_record_type, __pyx_empty_unicode); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 744, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_20);
+      __pyx_t_19 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_20) > __pyx_t_19) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_20) : __pyx_t_19;
+      __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_20);
+      __Pyx_GIVEREF(__pyx_t_20);
+      PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_20);
+      __pyx_t_20 = 0;
       __Pyx_INCREF(__pyx_kp_u_from);
-      __pyx_t_17 += 6;
+      __pyx_t_18 += 6;
       __Pyx_GIVEREF(__pyx_kp_u_from);
       PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_from);
-      __pyx_t_19 = __Pyx_PyObject_FormatSimple(__pyx_v_fo, __pyx_empty_unicode); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 767, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_19);
-      __pyx_t_18 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) > __pyx_t_18) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) : __pyx_t_18;
-      __pyx_t_17 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_19);
-      __Pyx_GIVEREF(__pyx_t_19);
-      PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_t_19);
-      __pyx_t_19 = 0;
-      __pyx_t_19 = __Pyx_PyUnicode_Join(__pyx_t_3, 4, __pyx_t_17, __pyx_t_18); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 767, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_19);
+      __pyx_t_20 = __Pyx_PyObject_FormatSimple(__pyx_v_fo, __pyx_empty_unicode); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 744, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_20);
+      __pyx_t_19 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_20) > __pyx_t_19) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_20) : __pyx_t_19;
+      __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_20);
+      __Pyx_GIVEREF(__pyx_t_20);
+      PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_t_20);
+      __pyx_t_20 = 0;
+      __pyx_t_20 = __Pyx_PyUnicode_Join(__pyx_t_3, 4, __pyx_t_18, __pyx_t_19); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 744, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_20);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_EOFError, __pyx_t_19); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 767, __pyx_L6_except_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_EOFError, __pyx_t_20); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 744, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+      __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 767, __pyx_L6_except_error)
+      __PYX_ERR(0, 744, __pyx_L6_except_error)
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
-    /* "fastavro/_read.pyx":702
+    /* "fastavro/_read.pyx":684
  *         reader_schema = match_schemas(writer_schema, reader_schema)
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         if record_type == "null":
  *             data = read_null(fo)
  */
     __Pyx_XGIVEREF(__pyx_t_5);
@@ -12152,268 +12067,268 @@
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_XGIVEREF(__pyx_t_7);
     __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_6, __pyx_t_7);
     goto __pyx_L0;
     __pyx_L9_try_end:;
   }
 
-  /* "fastavro/_read.pyx":769
+  /* "fastavro/_read.pyx":746
  *         raise EOFError(f"cannot read {record_type} from {fo}")
  * 
  *     if "logicalType" in writer_schema:             # <<<<<<<<<<<<<<
  *         logical_type = extract_logical_type(writer_schema)
  *         fn = LOGICAL_READERS.get(logical_type)
  */
-  __pyx_t_4 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_logicalType, __pyx_v_writer_schema, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 769, __pyx_L1_error)
-  __pyx_t_8 = (__pyx_t_4 != 0);
-  if (__pyx_t_8) {
+  __pyx_t_4 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_logicalType, __pyx_v_writer_schema, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 746, __pyx_L1_error)
+  __pyx_t_9 = (__pyx_t_4 != 0);
+  if (__pyx_t_9) {
 
-    /* "fastavro/_read.pyx":770
+    /* "fastavro/_read.pyx":747
  * 
  *     if "logicalType" in writer_schema:
  *         logical_type = extract_logical_type(writer_schema)             # <<<<<<<<<<<<<<
  *         fn = LOGICAL_READERS.get(logical_type)
  *         if fn:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_extract_logical_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 770, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_extract_logical_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 747, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_14 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_v_writer_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_writer_schema);
+    __pyx_t_15 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_v_writer_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_writer_schema);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 770, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_14);
+    if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 747, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_15);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_v_logical_type = __pyx_t_14;
-    __pyx_t_14 = 0;
+    __pyx_v_logical_type = __pyx_t_15;
+    __pyx_t_15 = 0;
 
-    /* "fastavro/_read.pyx":771
+    /* "fastavro/_read.pyx":748
  *     if "logicalType" in writer_schema:
  *         logical_type = extract_logical_type(writer_schema)
  *         fn = LOGICAL_READERS.get(logical_type)             # <<<<<<<<<<<<<<
  *         if fn:
  *             return fn(data, writer_schema, reader_schema)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_LOGICAL_READERS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 771, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_LOGICAL_READERS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 771, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_14 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_v_logical_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_logical_type);
+    __pyx_t_15 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_v_logical_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_logical_type);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 771, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_14);
+    if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 748, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_15);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_v_fn = __pyx_t_14;
-    __pyx_t_14 = 0;
+    __pyx_v_fn = __pyx_t_15;
+    __pyx_t_15 = 0;
 
-    /* "fastavro/_read.pyx":772
+    /* "fastavro/_read.pyx":749
  *         logical_type = extract_logical_type(writer_schema)
  *         fn = LOGICAL_READERS.get(logical_type)
  *         if fn:             # <<<<<<<<<<<<<<
  *             return fn(data, writer_schema, reader_schema)
  * 
  */
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_fn); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 772, __pyx_L1_error)
-    if (__pyx_t_8) {
+    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_fn); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 749, __pyx_L1_error)
+    if (__pyx_t_9) {
 
-      /* "fastavro/_read.pyx":773
+      /* "fastavro/_read.pyx":750
  *         fn = LOGICAL_READERS.get(logical_type)
  *         if fn:
  *             return fn(data, writer_schema, reader_schema)             # <<<<<<<<<<<<<<
  * 
  *     if reader_schema is not None:
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_fn);
       __pyx_t_2 = __pyx_v_fn; __pyx_t_1 = NULL;
-      __pyx_t_16 = 0;
+      __pyx_t_17 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
-          __pyx_t_16 = 1;
+          __pyx_t_17 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_2)) {
         PyObject *__pyx_temp[4] = {__pyx_t_1, __pyx_v_data, __pyx_v_writer_schema, __pyx_v_reader_schema};
-        __pyx_t_14 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 773, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_17, 3+__pyx_t_17); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 750, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_GOTREF(__pyx_t_15);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
         PyObject *__pyx_temp[4] = {__pyx_t_1, __pyx_v_data, __pyx_v_writer_schema, __pyx_v_reader_schema};
-        __pyx_t_14 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 773, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_17, 3+__pyx_t_17); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 750, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_GOTREF(__pyx_t_15);
       } else
       #endif
       {
-        __pyx_t_3 = PyTuple_New(3+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 773, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_New(3+__pyx_t_17); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 750, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         if (__pyx_t_1) {
           __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1); __pyx_t_1 = NULL;
         }
         __Pyx_INCREF(__pyx_v_data);
         __Pyx_GIVEREF(__pyx_v_data);
-        PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_16, __pyx_v_data);
+        PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_17, __pyx_v_data);
         __Pyx_INCREF(__pyx_v_writer_schema);
         __Pyx_GIVEREF(__pyx_v_writer_schema);
-        PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_16, __pyx_v_writer_schema);
+        PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_17, __pyx_v_writer_schema);
         __Pyx_INCREF(__pyx_v_reader_schema);
         __Pyx_GIVEREF(__pyx_v_reader_schema);
-        PyTuple_SET_ITEM(__pyx_t_3, 2+__pyx_t_16, __pyx_v_reader_schema);
-        __pyx_t_14 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 773, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_14);
+        PyTuple_SET_ITEM(__pyx_t_3, 2+__pyx_t_17, __pyx_v_reader_schema);
+        __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 750, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_r = __pyx_t_14;
-      __pyx_t_14 = 0;
+      __pyx_r = __pyx_t_15;
+      __pyx_t_15 = 0;
       goto __pyx_L0;
 
-      /* "fastavro/_read.pyx":772
+      /* "fastavro/_read.pyx":749
  *         logical_type = extract_logical_type(writer_schema)
  *         fn = LOGICAL_READERS.get(logical_type)
  *         if fn:             # <<<<<<<<<<<<<<
  *             return fn(data, writer_schema, reader_schema)
  * 
  */
     }
 
-    /* "fastavro/_read.pyx":769
+    /* "fastavro/_read.pyx":746
  *         raise EOFError(f"cannot read {record_type} from {fo}")
  * 
  *     if "logicalType" in writer_schema:             # <<<<<<<<<<<<<<
  *         logical_type = extract_logical_type(writer_schema)
  *         fn = LOGICAL_READERS.get(logical_type)
  */
   }
 
-  /* "fastavro/_read.pyx":775
+  /* "fastavro/_read.pyx":752
  *             return fn(data, writer_schema, reader_schema)
  * 
  *     if reader_schema is not None:             # <<<<<<<<<<<<<<
  *         return maybe_promote(
  *             data,
  */
-  __pyx_t_8 = (__pyx_v_reader_schema != Py_None);
-  __pyx_t_4 = (__pyx_t_8 != 0);
+  __pyx_t_9 = (__pyx_v_reader_schema != Py_None);
+  __pyx_t_4 = (__pyx_t_9 != 0);
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":776
+    /* "fastavro/_read.pyx":753
  * 
  *     if reader_schema is not None:
  *         return maybe_promote(             # <<<<<<<<<<<<<<
  *             data,
  *             record_type,
  */
     __Pyx_XDECREF(__pyx_r);
 
-    /* "fastavro/_read.pyx":779
+    /* "fastavro/_read.pyx":756
  *             data,
  *             record_type,
  *             extract_record_type(reader_schema)             # <<<<<<<<<<<<<<
  *         )
  *     else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_extract_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_extract_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 756, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_14 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_reader_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_reader_schema);
+    __pyx_t_15 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_reader_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_reader_schema);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 779, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_14);
+    if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 756, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_15);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "fastavro/_read.pyx":776
+    /* "fastavro/_read.pyx":753
  * 
  *     if reader_schema is not None:
  *         return maybe_promote(             # <<<<<<<<<<<<<<
  *             data,
  *             record_type,
  */
-    __pyx_t_2 = __pyx_f_8fastavro_5_read_maybe_promote(__pyx_v_data, __pyx_v_record_type, __pyx_t_14, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8fastavro_5_read_maybe_promote(__pyx_v_data, __pyx_v_record_type, __pyx_t_15, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 753, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+    __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "fastavro/_read.pyx":775
+    /* "fastavro/_read.pyx":752
  *             return fn(data, writer_schema, reader_schema)
  * 
  *     if reader_schema is not None:             # <<<<<<<<<<<<<<
  *         return maybe_promote(
  *             data,
  */
   }
 
-  /* "fastavro/_read.pyx":782
+  /* "fastavro/_read.pyx":759
  *         )
  *     else:
  *         return data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_data);
     __pyx_r = __pyx_v_data;
     goto __pyx_L0;
   }
 
-  /* "fastavro/_read.pyx":687
+  /* "fastavro/_read.pyx":670
  * 
  * 
  * cpdef _read_data(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_14);
-  __Pyx_XDECREF(__pyx_t_19);
+  __Pyx_XDECREF(__pyx_t_15);
+  __Pyx_XDECREF(__pyx_t_20);
   __Pyx_AddTraceback("fastavro._read._read_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_record_type);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XDECREF(__pyx_v_logical_type);
   __Pyx_XDECREF(__pyx_v_fn);
@@ -12427,58 +12342,38 @@
 static PyObject *__pyx_pw_8fastavro_5_read_61_read_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_8fastavro_5_read_60_read_data[] = "Read data from file object according to schema.";
 static PyObject *__pyx_pw_8fastavro_5_read_61_read_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_writer_schema = 0;
   PyObject *__pyx_v_named_schemas = 0;
   PyObject *__pyx_v_reader_schema = 0;
-  PyObject *__pyx_v_return_record_name = 0;
-  PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_options = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_read_data (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_options,0};
+    PyObject* values[5] = {0,0,0,0,0};
 
-    /* "fastavro/_read.pyx":691
+    /* "fastavro/_read.pyx":674
  *     writer_schema,
  *     named_schemas,
  *     reader_schema=None,             # <<<<<<<<<<<<<<
- *     return_record_name=False,
- *     return_record_name_override=False,
- */
-    values[3] = ((PyObject *)Py_None);
-
-    /* "fastavro/_read.pyx":692
- *     named_schemas,
- *     reader_schema=None,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
- * ):
- */
-    values[4] = ((PyObject *)Py_False);
-
-    /* "fastavro/_read.pyx":693
- *     reader_schema=None,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
+ *     options={},
  * ):
- *     """Read data from file object according to schema."""
  */
-    values[5] = ((PyObject *)Py_False);
+    values[3] = ((PyObject *)Py_None);
+    values[4] = __pyx_k__7;
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -12493,48 +12388,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_read_data", 0, 3, 6, 1); __PYX_ERR(0, 687, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_read_data", 0, 3, 5, 1); __PYX_ERR(0, 670, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_read_data", 0, 3, 6, 2); __PYX_ERR(0, 687, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_read_data", 0, 3, 5, 2); __PYX_ERR(0, 670, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema);
           if (value) { values[3] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name);
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options);
           if (value) { values[4] = value; kw_args--; }
         }
-        CYTHON_FALLTHROUGH;
-        case  5:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
-          if (value) { values[5] = value; kw_args--; }
-        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_read_data") < 0)) __PYX_ERR(0, 687, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_read_data") < 0)) __PYX_ERR(0, 670, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -12542,55 +12429,53 @@
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_named_schemas = values[2];
     __pyx_v_reader_schema = values[3];
-    __pyx_v_return_record_name = values[4];
-    __pyx_v_return_record_name_override = values[5];
+    __pyx_v_options = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_read_data", 0, 3, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 687, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_read_data", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 670, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read._read_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_60_read_data(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
+  __pyx_r = __pyx_pf_8fastavro_5_read_60_read_data(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_options);
 
-  /* "fastavro/_read.pyx":687
+  /* "fastavro/_read.pyx":670
  * 
  * 
  * cpdef _read_data(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_60_read_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_60_read_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_8fastavro_5_read__read_data __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_read_data", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2.__pyx_n = 3;
+  __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.reader_schema = __pyx_v_reader_schema;
-  __pyx_t_2.return_record_name = __pyx_v_return_record_name;
-  __pyx_t_2.return_record_name_override = __pyx_v_return_record_name_override;
-  __pyx_t_1 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 687, __pyx_L1_error)
+  __pyx_t_2.options = __pyx_v_options;
+  __pyx_t_1 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12599,15 +12484,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":785
+/* "fastavro/_read.pyx":762
  * 
  * 
  * cpdef _skip_data(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
@@ -12622,489 +12507,489 @@
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_skip_data", 0);
 
-  /* "fastavro/_read.pyx":790
+  /* "fastavro/_read.pyx":767
  *     named_schemas,
  * ):
  *     record_type = extract_record_type(writer_schema)             # <<<<<<<<<<<<<<
  * 
  *     if record_type == "null":
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_extract_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 790, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_extract_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 767, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_writer_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_writer_schema);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 790, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 767, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_record_type = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":792
+  /* "fastavro/_read.pyx":769
  *     record_type = extract_record_type(writer_schema)
  * 
  *     if record_type == "null":             # <<<<<<<<<<<<<<
  *         skip_null(fo)
  *     elif record_type == "string":
  */
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_null, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 792, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_null, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 769, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":793
+    /* "fastavro/_read.pyx":770
  * 
  *     if record_type == "null":
  *         skip_null(fo)             # <<<<<<<<<<<<<<
  *     elif record_type == "string":
  *         skip_utf8(fo)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_null(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 793, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_null(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 770, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":792
+    /* "fastavro/_read.pyx":769
  *     record_type = extract_record_type(writer_schema)
  * 
  *     if record_type == "null":             # <<<<<<<<<<<<<<
  *         skip_null(fo)
  *     elif record_type == "string":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":794
+  /* "fastavro/_read.pyx":771
  *     if record_type == "null":
  *         skip_null(fo)
  *     elif record_type == "string":             # <<<<<<<<<<<<<<
  *         skip_utf8(fo)
  *     elif record_type == "int" or record_type == "long":
  */
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_string, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 794, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_string, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 771, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":795
+    /* "fastavro/_read.pyx":772
  *         skip_null(fo)
  *     elif record_type == "string":
  *         skip_utf8(fo)             # <<<<<<<<<<<<<<
  *     elif record_type == "int" or record_type == "long":
  *         skip_long(fo)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_utf8(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 795, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_utf8(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 772, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":794
+    /* "fastavro/_read.pyx":771
  *     if record_type == "null":
  *         skip_null(fo)
  *     elif record_type == "string":             # <<<<<<<<<<<<<<
  *         skip_utf8(fo)
  *     elif record_type == "int" or record_type == "long":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":796
+  /* "fastavro/_read.pyx":773
  *     elif record_type == "string":
  *         skip_utf8(fo)
  *     elif record_type == "int" or record_type == "long":             # <<<<<<<<<<<<<<
  *         skip_long(fo)
  *     elif record_type == "float":
  */
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_int, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_int, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 773, __pyx_L1_error)
   if (!__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_long, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_long, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 773, __pyx_L1_error)
   __pyx_t_4 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":797
+    /* "fastavro/_read.pyx":774
  *         skip_utf8(fo)
  *     elif record_type == "int" or record_type == "long":
  *         skip_long(fo)             # <<<<<<<<<<<<<<
  *     elif record_type == "float":
  *         skip_float(fo)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_long(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 797, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_long(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 774, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":796
+    /* "fastavro/_read.pyx":773
  *     elif record_type == "string":
  *         skip_utf8(fo)
  *     elif record_type == "int" or record_type == "long":             # <<<<<<<<<<<<<<
  *         skip_long(fo)
  *     elif record_type == "float":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":798
+  /* "fastavro/_read.pyx":775
  *     elif record_type == "int" or record_type == "long":
  *         skip_long(fo)
  *     elif record_type == "float":             # <<<<<<<<<<<<<<
  *         skip_float(fo)
  *     elif record_type == "double":
  */
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_float, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_float, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 775, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":799
+    /* "fastavro/_read.pyx":776
  *         skip_long(fo)
  *     elif record_type == "float":
  *         skip_float(fo)             # <<<<<<<<<<<<<<
  *     elif record_type == "double":
  *         skip_double(fo)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_float(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 799, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_float(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":798
+    /* "fastavro/_read.pyx":775
  *     elif record_type == "int" or record_type == "long":
  *         skip_long(fo)
  *     elif record_type == "float":             # <<<<<<<<<<<<<<
  *         skip_float(fo)
  *     elif record_type == "double":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":800
+  /* "fastavro/_read.pyx":777
  *     elif record_type == "float":
  *         skip_float(fo)
  *     elif record_type == "double":             # <<<<<<<<<<<<<<
  *         skip_double(fo)
  *     elif record_type == "boolean":
  */
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_double, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_double, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 777, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":801
+    /* "fastavro/_read.pyx":778
  *         skip_float(fo)
  *     elif record_type == "double":
  *         skip_double(fo)             # <<<<<<<<<<<<<<
  *     elif record_type == "boolean":
  *         skip_boolean(fo)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_double(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 801, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_double(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":800
+    /* "fastavro/_read.pyx":777
  *     elif record_type == "float":
  *         skip_float(fo)
  *     elif record_type == "double":             # <<<<<<<<<<<<<<
  *         skip_double(fo)
  *     elif record_type == "boolean":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":802
+  /* "fastavro/_read.pyx":779
  *     elif record_type == "double":
  *         skip_double(fo)
  *     elif record_type == "boolean":             # <<<<<<<<<<<<<<
  *         skip_boolean(fo)
  *     elif record_type == "bytes":
  */
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_boolean, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 802, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_boolean, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 779, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":803
+    /* "fastavro/_read.pyx":780
  *         skip_double(fo)
  *     elif record_type == "boolean":
  *         skip_boolean(fo)             # <<<<<<<<<<<<<<
  *     elif record_type == "bytes":
  *         skip_bytes(fo)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_boolean(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 803, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_boolean(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 780, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":802
+    /* "fastavro/_read.pyx":779
  *     elif record_type == "double":
  *         skip_double(fo)
  *     elif record_type == "boolean":             # <<<<<<<<<<<<<<
  *         skip_boolean(fo)
  *     elif record_type == "bytes":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":804
+  /* "fastavro/_read.pyx":781
  *     elif record_type == "boolean":
  *         skip_boolean(fo)
  *     elif record_type == "bytes":             # <<<<<<<<<<<<<<
  *         skip_bytes(fo)
  *     elif record_type == "fixed":
  */
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_bytes, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 804, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_bytes, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 781, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":805
+    /* "fastavro/_read.pyx":782
  *         skip_boolean(fo)
  *     elif record_type == "bytes":
  *         skip_bytes(fo)             # <<<<<<<<<<<<<<
  *     elif record_type == "fixed":
  *         skip_fixed(fo, writer_schema)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 805, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 782, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":804
+    /* "fastavro/_read.pyx":781
  *     elif record_type == "boolean":
  *         skip_boolean(fo)
  *     elif record_type == "bytes":             # <<<<<<<<<<<<<<
  *         skip_bytes(fo)
  *     elif record_type == "fixed":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":806
+  /* "fastavro/_read.pyx":783
  *     elif record_type == "bytes":
  *         skip_bytes(fo)
  *     elif record_type == "fixed":             # <<<<<<<<<<<<<<
  *         skip_fixed(fo, writer_schema)
  *     elif record_type == "enum":
  */
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_fixed, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 806, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_fixed, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 783, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":807
+    /* "fastavro/_read.pyx":784
  *         skip_bytes(fo)
  *     elif record_type == "fixed":
  *         skip_fixed(fo, writer_schema)             # <<<<<<<<<<<<<<
  *     elif record_type == "enum":
  *         skip_enum(fo)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_fixed(__pyx_v_fo, __pyx_v_writer_schema, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 807, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_fixed(__pyx_v_fo, __pyx_v_writer_schema, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 784, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":806
+    /* "fastavro/_read.pyx":783
  *     elif record_type == "bytes":
  *         skip_bytes(fo)
  *     elif record_type == "fixed":             # <<<<<<<<<<<<<<
  *         skip_fixed(fo, writer_schema)
  *     elif record_type == "enum":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":808
+  /* "fastavro/_read.pyx":785
  *     elif record_type == "fixed":
  *         skip_fixed(fo, writer_schema)
  *     elif record_type == "enum":             # <<<<<<<<<<<<<<
  *         skip_enum(fo)
  *     elif record_type == "array":
  */
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_enum, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 808, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_enum, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 785, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":809
+    /* "fastavro/_read.pyx":786
  *         skip_fixed(fo, writer_schema)
  *     elif record_type == "enum":
  *         skip_enum(fo)             # <<<<<<<<<<<<<<
  *     elif record_type == "array":
  *         skip_array(fo, writer_schema, named_schemas)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_enum(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_enum(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 786, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":808
+    /* "fastavro/_read.pyx":785
  *     elif record_type == "fixed":
  *         skip_fixed(fo, writer_schema)
  *     elif record_type == "enum":             # <<<<<<<<<<<<<<
  *         skip_enum(fo)
  *     elif record_type == "array":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":810
+  /* "fastavro/_read.pyx":787
  *     elif record_type == "enum":
  *         skip_enum(fo)
  *     elif record_type == "array":             # <<<<<<<<<<<<<<
  *         skip_array(fo, writer_schema, named_schemas)
  *     elif record_type == "map":
  */
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_array, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 810, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_array, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 787, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":811
+    /* "fastavro/_read.pyx":788
  *         skip_enum(fo)
  *     elif record_type == "array":
  *         skip_array(fo, writer_schema, named_schemas)             # <<<<<<<<<<<<<<
  *     elif record_type == "map":
  *         skip_map(fo, writer_schema, named_schemas)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_array(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 811, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_array(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 788, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":810
+    /* "fastavro/_read.pyx":787
  *     elif record_type == "enum":
  *         skip_enum(fo)
  *     elif record_type == "array":             # <<<<<<<<<<<<<<
  *         skip_array(fo, writer_schema, named_schemas)
  *     elif record_type == "map":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":812
+  /* "fastavro/_read.pyx":789
  *     elif record_type == "array":
  *         skip_array(fo, writer_schema, named_schemas)
  *     elif record_type == "map":             # <<<<<<<<<<<<<<
  *         skip_map(fo, writer_schema, named_schemas)
  *     elif record_type == "union" or record_type == "error_union":
  */
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_map, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 812, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_map, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 789, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":813
+    /* "fastavro/_read.pyx":790
  *         skip_array(fo, writer_schema, named_schemas)
  *     elif record_type == "map":
  *         skip_map(fo, writer_schema, named_schemas)             # <<<<<<<<<<<<<<
  *     elif record_type == "union" or record_type == "error_union":
  *         skip_union(fo, writer_schema, named_schemas)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_map(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 813, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_map(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 790, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":812
+    /* "fastavro/_read.pyx":789
  *     elif record_type == "array":
  *         skip_array(fo, writer_schema, named_schemas)
  *     elif record_type == "map":             # <<<<<<<<<<<<<<
  *         skip_map(fo, writer_schema, named_schemas)
  *     elif record_type == "union" or record_type == "error_union":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":814
+  /* "fastavro/_read.pyx":791
  *     elif record_type == "map":
  *         skip_map(fo, writer_schema, named_schemas)
  *     elif record_type == "union" or record_type == "error_union":             # <<<<<<<<<<<<<<
  *         skip_union(fo, writer_schema, named_schemas)
  *     elif record_type == "record" or record_type == "error":
  */
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_union, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_union, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 791, __pyx_L1_error)
   if (!__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L6_bool_binop_done;
   }
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_error_union, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_error_union, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 791, __pyx_L1_error)
   __pyx_t_4 = __pyx_t_5;
   __pyx_L6_bool_binop_done:;
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":815
+    /* "fastavro/_read.pyx":792
  *         skip_map(fo, writer_schema, named_schemas)
  *     elif record_type == "union" or record_type == "error_union":
  *         skip_union(fo, writer_schema, named_schemas)             # <<<<<<<<<<<<<<
  *     elif record_type == "record" or record_type == "error":
  *         skip_record(fo, writer_schema, named_schemas)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_union(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 815, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_union(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":814
+    /* "fastavro/_read.pyx":791
  *     elif record_type == "map":
  *         skip_map(fo, writer_schema, named_schemas)
  *     elif record_type == "union" or record_type == "error_union":             # <<<<<<<<<<<<<<
  *         skip_union(fo, writer_schema, named_schemas)
  *     elif record_type == "record" or record_type == "error":
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":816
+  /* "fastavro/_read.pyx":793
  *     elif record_type == "union" or record_type == "error_union":
  *         skip_union(fo, writer_schema, named_schemas)
  *     elif record_type == "record" or record_type == "error":             # <<<<<<<<<<<<<<
  *         skip_record(fo, writer_schema, named_schemas)
  *     else:
  */
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_record, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 816, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_record, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 793, __pyx_L1_error)
   if (!__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L8_bool_binop_done;
   }
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_error, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 816, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_record_type, __pyx_n_u_error, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 793, __pyx_L1_error)
   __pyx_t_4 = __pyx_t_5;
   __pyx_L8_bool_binop_done:;
   if (__pyx_t_4) {
 
-    /* "fastavro/_read.pyx":817
+    /* "fastavro/_read.pyx":794
  *         skip_union(fo, writer_schema, named_schemas)
  *     elif record_type == "record" or record_type == "error":
  *         skip_record(fo, writer_schema, named_schemas)             # <<<<<<<<<<<<<<
  *     else:
  *         _skip_data(fo, named_schemas["writer"][record_type], named_schemas)
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_record(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 817, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_record(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":816
+    /* "fastavro/_read.pyx":793
  *     elif record_type == "union" or record_type == "error_union":
  *         skip_union(fo, writer_schema, named_schemas)
  *     elif record_type == "record" or record_type == "error":             # <<<<<<<<<<<<<<
  *         skip_record(fo, writer_schema, named_schemas)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":819
+  /* "fastavro/_read.pyx":796
  *         skip_record(fo, writer_schema, named_schemas)
  *     else:
  *         _skip_data(fo, named_schemas["writer"][record_type], named_schemas)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_named_schemas, __pyx_n_u_writer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 819, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_named_schemas, __pyx_n_u_writer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 796, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 819, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_record_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 796, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_2, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 819, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_t_2, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 796, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "fastavro/_read.pyx":785
+  /* "fastavro/_read.pyx":762
  * 
  * 
  * cpdef _skip_data(             # <<<<<<<<<<<<<<
  *     fo,
  *     writer_schema,
  */
 
@@ -13157,40 +13042,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_skip_data", 1, 3, 3, 1); __PYX_ERR(0, 785, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_skip_data", 1, 3, 3, 1); __PYX_ERR(0, 762, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_skip_data", 1, 3, 3, 2); __PYX_ERR(0, 785, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_skip_data", 1, 3, 3, 2); __PYX_ERR(0, 762, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_skip_data") < 0)) __PYX_ERR(0, 785, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_skip_data") < 0)) __PYX_ERR(0, 762, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_named_schemas = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_skip_data", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 785, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_skip_data", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 762, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read._skip_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8fastavro_5_read_62_skip_data(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas);
 
@@ -13204,15 +13089,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_skip_data", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 785, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read__skip_data(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 762, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13221,15 +13106,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":822
+/* "fastavro/_read.pyx":799
  * 
  * 
  * cpdef skip_sync(fo, sync_marker):             # <<<<<<<<<<<<<<
  *     """Skip an expected sync marker, complaining if it doesn't match"""
  *     if fo.read(SYNC_SIZE) != sync_marker:
  */
 
@@ -13243,70 +13128,70 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("skip_sync", 0);
 
-  /* "fastavro/_read.pyx":824
+  /* "fastavro/_read.pyx":801
  * cpdef skip_sync(fo, sync_marker):
  *     """Skip an expected sync marker, complaining if it doesn't match"""
  *     if fo.read(SYNC_SIZE) != sync_marker:             # <<<<<<<<<<<<<<
  *         raise ValueError("expected sync marker not found")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 824, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 801, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SYNC_SIZE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 824, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SYNC_SIZE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 801, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 824, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 801, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_v_sync_marker, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 824, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_v_sync_marker, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 801, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 824, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 801, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_5)) {
 
-    /* "fastavro/_read.pyx":825
+    /* "fastavro/_read.pyx":802
  *     """Skip an expected sync marker, complaining if it doesn't match"""
  *     if fo.read(SYNC_SIZE) != sync_marker:
  *         raise ValueError("expected sync marker not found")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 825, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 802, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 825, __pyx_L1_error)
+    __PYX_ERR(0, 802, __pyx_L1_error)
 
-    /* "fastavro/_read.pyx":824
+    /* "fastavro/_read.pyx":801
  * cpdef skip_sync(fo, sync_marker):
  *     """Skip an expected sync marker, complaining if it doesn't match"""
  *     if fo.read(SYNC_SIZE) != sync_marker:             # <<<<<<<<<<<<<<
  *         raise ValueError("expected sync marker not found")
  * 
  */
   }
 
-  /* "fastavro/_read.pyx":822
+  /* "fastavro/_read.pyx":799
  * 
  * 
  * cpdef skip_sync(fo, sync_marker):             # <<<<<<<<<<<<<<
  *     """Skip an expected sync marker, complaining if it doesn't match"""
  *     if fo.read(SYNC_SIZE) != sync_marker:
  */
 
@@ -13357,32 +13242,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sync_marker)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("skip_sync", 1, 2, 2, 1); __PYX_ERR(0, 822, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("skip_sync", 1, 2, 2, 1); __PYX_ERR(0, 799, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "skip_sync") < 0)) __PYX_ERR(0, 822, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "skip_sync") < 0)) __PYX_ERR(0, 799, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_fo = values[0];
     __pyx_v_sync_marker = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("skip_sync", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 822, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("skip_sync", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 799, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.skip_sync", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8fastavro_5_read_64skip_sync(__pyx_self, __pyx_v_fo, __pyx_v_sync_marker);
 
@@ -13396,15 +13281,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("skip_sync", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_sync(__pyx_v_fo, __pyx_v_sync_marker, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 822, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_sync(__pyx_v_fo, __pyx_v_sync_marker, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 799, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13413,15 +13298,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":828
+/* "fastavro/_read.pyx":805
  * 
  * 
  * cpdef null_read_block(fo):             # <<<<<<<<<<<<<<
  *     """Read block in "null" codec."""
  *     return BytesIO(read_bytes(fo))
  */
 
@@ -13434,47 +13319,47 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("null_read_block", 0);
 
-  /* "fastavro/_read.pyx":830
+  /* "fastavro/_read.pyx":807
  * cpdef null_read_block(fo):
  *     """Read block in "null" codec."""
  *     return BytesIO(read_bytes(fo))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 830, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 807, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __pyx_f_8fastavro_5_read_read_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 830, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_8fastavro_5_read_read_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 807, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 830, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 807, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":828
+  /* "fastavro/_read.pyx":805
  * 
  * 
  * cpdef null_read_block(fo):             # <<<<<<<<<<<<<<
  *     """Read block in "null" codec."""
  *     return BytesIO(read_bytes(fo))
  */
 
@@ -13511,15 +13396,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("null_read_block", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_null_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 828, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_null_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 805, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13528,15 +13413,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":833
+/* "fastavro/_read.pyx":810
  * 
  * 
  * cpdef deflate_read_block(fo):             # <<<<<<<<<<<<<<
  *     """Read block in "deflate" codec."""
  *     data = read_bytes(fo)
  */
 
@@ -13552,72 +13437,72 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("deflate_read_block", 0);
 
-  /* "fastavro/_read.pyx":835
+  /* "fastavro/_read.pyx":812
  * cpdef deflate_read_block(fo):
  *     """Read block in "deflate" codec."""
  *     data = read_bytes(fo)             # <<<<<<<<<<<<<<
  *     # -15 is the log of the window size; negative indicates "raw" (no
  *     # zlib headers) decompression.  See zlib.h.
  */
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 835, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 812, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":838
+  /* "fastavro/_read.pyx":815
  *     # -15 is the log of the window size; negative indicates "raw" (no
  *     # zlib headers) decompression.  See zlib.h.
  *     return BytesIO(zlib.decompressobj(-15).decompress(data))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 838, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 815, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_zlib); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 838, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_zlib); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 815, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_decompressobj); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 838, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_decompressobj); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 815, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_int_neg_15) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_int_neg_15);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 838, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 815, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_decompress); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 838, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_decompress); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 815, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_4, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_data);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 838, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 815, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -13625,22 +13510,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 838, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 815, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":833
+  /* "fastavro/_read.pyx":810
  * 
  * 
  * cpdef deflate_read_block(fo):             # <<<<<<<<<<<<<<
  *     """Read block in "deflate" codec."""
  *     data = read_bytes(fo)
  */
 
@@ -13680,15 +13565,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("deflate_read_block", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_deflate_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 833, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_deflate_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 810, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13697,15 +13582,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":841
+/* "fastavro/_read.pyx":818
  * 
  * 
  * cpdef bzip2_read_block(fo):             # <<<<<<<<<<<<<<
  *     """Read block in "bzip2" codec."""
  *     data = read_bytes(fo)
  */
 
@@ -13720,54 +13605,54 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("bzip2_read_block", 0);
 
-  /* "fastavro/_read.pyx":843
+  /* "fastavro/_read.pyx":820
  * cpdef bzip2_read_block(fo):
  *     """Read block in "bzip2" codec."""
  *     data = read_bytes(fo)             # <<<<<<<<<<<<<<
  *     return BytesIO(bz2.decompress(data))
  * 
  */
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 843, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_bytes(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 820, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":844
+  /* "fastavro/_read.pyx":821
  *     """Read block in "bzip2" codec."""
  *     data = read_bytes(fo)
  *     return BytesIO(bz2.decompress(data))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 844, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 821, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_bz2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 844, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_bz2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 821, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_decompress); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 844, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_decompress); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 821, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_data);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 844, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 821, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -13775,22 +13660,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 844, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 821, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":841
+  /* "fastavro/_read.pyx":818
  * 
  * 
  * cpdef bzip2_read_block(fo):             # <<<<<<<<<<<<<<
  *     """Read block in "bzip2" codec."""
  *     data = read_bytes(fo)
  */
 
@@ -13829,15 +13714,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("bzip2_read_block", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_bzip2_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 841, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_bzip2_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 818, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13846,15 +13731,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":847
+/* "fastavro/_read.pyx":824
  * 
  * 
  * cpdef xz_read_block(fo):             # <<<<<<<<<<<<<<
  *     length = read_long(fo)
  *     data = fo.read(length)
  */
 
@@ -13871,82 +13756,82 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("xz_read_block", 0);
 
-  /* "fastavro/_read.pyx":848
+  /* "fastavro/_read.pyx":825
  * 
  * cpdef xz_read_block(fo):
  *     length = read_long(fo)             # <<<<<<<<<<<<<<
  *     data = fo.read(length)
  *     return BytesIO(lzma.decompress(data))
  */
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 848, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 825, __pyx_L1_error)
   __pyx_v_length = __pyx_t_1;
 
-  /* "fastavro/_read.pyx":849
+  /* "fastavro/_read.pyx":826
  * cpdef xz_read_block(fo):
  *     length = read_long(fo)
  *     data = fo.read(length)             # <<<<<<<<<<<<<<
  *     return BytesIO(lzma.decompress(data))
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 849, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 849, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 849, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":850
+  /* "fastavro/_read.pyx":827
  *     length = read_long(fo)
  *     data = fo.read(length)
  *     return BytesIO(lzma.decompress(data))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 850, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_lzma); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 850, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_lzma); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_decompress); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 850, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_decompress); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_data);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 850, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -13954,22 +13839,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 850, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":847
+  /* "fastavro/_read.pyx":824
  * 
  * 
  * cpdef xz_read_block(fo):             # <<<<<<<<<<<<<<
  *     length = read_long(fo)
  *     data = fo.read(length)
  */
 
@@ -14007,15 +13892,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("xz_read_block", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_xz_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 847, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_xz_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 824, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14024,15 +13909,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":861
+/* "fastavro/_read.pyx":838
  * 
  * 
  * cpdef snappy_read_block(fo):             # <<<<<<<<<<<<<<
  *     length = read_long(fo)
  *     data = fo.read(length - 4)
  */
 
@@ -14049,111 +13934,111 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("snappy_read_block", 0);
 
-  /* "fastavro/_read.pyx":862
+  /* "fastavro/_read.pyx":839
  * 
  * cpdef snappy_read_block(fo):
  *     length = read_long(fo)             # <<<<<<<<<<<<<<
  *     data = fo.read(length - 4)
  *     fo.read(4)  # CRC
  */
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 862, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 862, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 839, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 839, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_length = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":863
+  /* "fastavro/_read.pyx":840
  * cpdef snappy_read_block(fo):
  *     length = read_long(fo)
  *     data = fo.read(length - 4)             # <<<<<<<<<<<<<<
  *     fo.read(4)  # CRC
  *     return BytesIO(snappy.decompress(data))
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 863, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 840, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_length, __pyx_int_4, 4, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 863, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_length, __pyx_int_4, 4, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 840, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 863, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 840, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":864
+  /* "fastavro/_read.pyx":841
  *     length = read_long(fo)
  *     data = fo.read(length - 4)
  *     fo.read(4)  # CRC             # <<<<<<<<<<<<<<
  *     return BytesIO(snappy.decompress(data))
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 864, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 841, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_int_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_int_4);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 864, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 841, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":865
+  /* "fastavro/_read.pyx":842
  *     data = fo.read(length - 4)
  *     fo.read(4)  # CRC
  *     return BytesIO(snappy.decompress(data))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 865, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 842, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_snappy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 865, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_snappy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 842, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_decompress); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 865, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_decompress); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 842, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_data);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 865, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 842, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -14161,22 +14046,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 865, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 842, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":861
+  /* "fastavro/_read.pyx":838
  * 
  * 
  * cpdef snappy_read_block(fo):             # <<<<<<<<<<<<<<
  *     length = read_long(fo)
  *     data = fo.read(length - 4)
  */
 
@@ -14215,15 +14100,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("snappy_read_block", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_snappy_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 861, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_snappy_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 838, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14232,15 +14117,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":876
+/* "fastavro/_read.pyx":853
  * 
  * 
  * cpdef zstandard_read_block(fo):             # <<<<<<<<<<<<<<
  *     length = read_long(fo)
  *     data = fo.read(length)
  */
 
@@ -14259,118 +14144,118 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("zstandard_read_block", 0);
 
-  /* "fastavro/_read.pyx":877
+  /* "fastavro/_read.pyx":854
  * 
  * cpdef zstandard_read_block(fo):
  *     length = read_long(fo)             # <<<<<<<<<<<<<<
  *     data = fo.read(length)
  *     return BytesIO(zstd.ZstdDecompressor().decompressobj().decompress(data))
  */
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 877, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 854, __pyx_L1_error)
   __pyx_v_length = __pyx_t_1;
 
-  /* "fastavro/_read.pyx":878
+  /* "fastavro/_read.pyx":855
  * cpdef zstandard_read_block(fo):
  *     length = read_long(fo)
  *     data = fo.read(length)             # <<<<<<<<<<<<<<
  *     return BytesIO(zstd.ZstdDecompressor().decompressobj().decompress(data))
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 878, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 855, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 878, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 855, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 878, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 855, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":879
+  /* "fastavro/_read.pyx":856
  *     length = read_long(fo)
  *     data = fo.read(length)
  *     return BytesIO(zstd.ZstdDecompressor().decompressobj().decompress(data))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 879, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_zstd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 879, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_zstd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_ZstdDecompressor); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 879, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_ZstdDecompressor); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 879, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decompressobj); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 879, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decompressobj); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 879, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_decompress); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 879, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_decompress); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_5, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_data);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 879, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -14378,22 +14263,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 879, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":876
+  /* "fastavro/_read.pyx":853
  * 
  * 
  * cpdef zstandard_read_block(fo):             # <<<<<<<<<<<<<<
  *     length = read_long(fo)
  *     data = fo.read(length)
  */
 
@@ -14433,15 +14318,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("zstandard_read_block", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_zstandard_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 876, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_zstandard_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 853, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14450,15 +14335,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":890
+/* "fastavro/_read.pyx":867
  * 
  * 
  * cpdef lz4_read_block(fo):             # <<<<<<<<<<<<<<
  *     length = read_long(fo)
  *     data = fo.read(length)
  */
 
@@ -14475,85 +14360,85 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lz4_read_block", 0);
 
-  /* "fastavro/_read.pyx":891
+  /* "fastavro/_read.pyx":868
  * 
  * cpdef lz4_read_block(fo):
  *     length = read_long(fo)             # <<<<<<<<<<<<<<
  *     data = fo.read(length)
  *     return BytesIO(lz4.block.decompress(data))
  */
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 891, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_read_long(__pyx_v_fo, 0); if (unlikely(__pyx_t_1 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 868, __pyx_L1_error)
   __pyx_v_length = __pyx_t_1;
 
-  /* "fastavro/_read.pyx":892
+  /* "fastavro/_read.pyx":869
  * cpdef lz4_read_block(fo):
  *     length = read_long(fo)
  *     data = fo.read(length)             # <<<<<<<<<<<<<<
  *     return BytesIO(lz4.block.decompress(data))
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 892, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 869, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 892, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 869, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 892, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 869, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":893
+  /* "fastavro/_read.pyx":870
  *     length = read_long(fo)
  *     data = fo.read(length)
  *     return BytesIO(lz4.block.decompress(data))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 893, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 870, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_lz4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 893, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_lz4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 870, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_block); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 893, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_block); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 870, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decompress); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 893, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decompress); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 870, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_data);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 893, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 870, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -14561,22 +14446,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 893, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 870, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":890
+  /* "fastavro/_read.pyx":867
  * 
  * 
  * cpdef lz4_read_block(fo):             # <<<<<<<<<<<<<<
  *     length = read_long(fo)
  *     data = fo.read(length)
  */
 
@@ -14614,15 +14499,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lz4_read_block", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_lz4_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 890, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_lz4_read_block(__pyx_v_fo, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 867, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14632,15 +14517,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_8fastavro_5_read_82generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "fastavro/_read.pyx":904
+/* "fastavro/_read.pyx":881
  * 
  * 
  * def _iter_avro_records(             # <<<<<<<<<<<<<<
  *     fo,
  *     header,
  */
 
@@ -14650,49 +14535,28 @@
 static PyObject *__pyx_pw_8fastavro_5_read_81_iter_avro_records(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_header = 0;
   PyObject *__pyx_v_codec = 0;
   PyObject *__pyx_v_writer_schema = 0;
   PyObject *__pyx_v_named_schemas = 0;
   PyObject *__pyx_v_reader_schema = 0;
-  PyObject *__pyx_v_return_record_name = 0;
-  PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_options = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_iter_avro_records (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_header,&__pyx_n_s_codec,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[8] = {0,0,0,0,0,0,0,0};
-
-    /* "fastavro/_read.pyx":911
- *     named_schemas,
- *     reader_schema,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
- * ):
- */
-    values[6] = ((PyObject *)Py_False);
-
-    /* "fastavro/_read.pyx":912
- *     reader_schema,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
- * ):
- *     cdef int32 i
- */
-    values[7] = ((PyObject *)Py_False);
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_header,&__pyx_n_s_codec,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_options,0};
+    PyObject* values[7] = {0,0,0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
-        CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
@@ -14711,117 +14575,97 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_header)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 0, 6, 8, 1); __PYX_ERR(0, 904, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 1, 7, 7, 1); __PYX_ERR(0, 881, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_codec)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 0, 6, 8, 2); __PYX_ERR(0, 904, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 1, 7, 7, 2); __PYX_ERR(0, 881, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 0, 6, 8, 3); __PYX_ERR(0, 904, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 1, 7, 7, 3); __PYX_ERR(0, 881, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 0, 6, 8, 4); __PYX_ERR(0, 904, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 1, 7, 7, 4); __PYX_ERR(0, 881, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 0, 6, 8, 5); __PYX_ERR(0, 904, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 1, 7, 7, 5); __PYX_ERR(0, 881, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name);
-          if (value) { values[6] = value; kw_args--; }
-        }
-        CYTHON_FALLTHROUGH;
-        case  7:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
-          if (value) { values[7] = value; kw_args--; }
+        if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 1, 7, 7, 6); __PYX_ERR(0, 881, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_iter_avro_records") < 0)) __PYX_ERR(0, 904, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_iter_avro_records") < 0)) __PYX_ERR(0, 881, __pyx_L3_error)
       }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 7) {
+      goto __pyx_L5_argtuple_error;
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
-        CYTHON_FALLTHROUGH;
-        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
-        CYTHON_FALLTHROUGH;
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+      values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
     __pyx_v_fo = values[0];
     __pyx_v_header = values[1];
     __pyx_v_codec = values[2];
     __pyx_v_writer_schema = values[3];
     __pyx_v_named_schemas = values[4];
     __pyx_v_reader_schema = values[5];
-    __pyx_v_return_record_name = values[6];
-    __pyx_v_return_record_name_override = values[7];
+    __pyx_v_options = values[6];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 0, 6, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 904, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_iter_avro_records", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 881, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read._iter_avro_records", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_80_iter_avro_records(__pyx_self, __pyx_v_fo, __pyx_v_header, __pyx_v_codec, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
-
-  /* "fastavro/_read.pyx":904
- * 
- * 
- * def _iter_avro_records(             # <<<<<<<<<<<<<<
- *     fo,
- *     header,
- */
+  __pyx_r = __pyx_pf_8fastavro_5_read_80_iter_avro_records(__pyx_self, __pyx_v_fo, __pyx_v_header, __pyx_v_codec, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_options);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_80_iter_avro_records(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_header, PyObject *__pyx_v_codec, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_80_iter_avro_records(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_header, PyObject *__pyx_v_codec, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options) {
   struct __pyx_obj_8fastavro_5_read___pyx_scope_struct___iter_avro_records *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_iter_avro_records", 0);
   __pyx_cur_scope = (struct __pyx_obj_8fastavro_5_read___pyx_scope_struct___iter_avro_records *)__pyx_tp_new_8fastavro_5_read___pyx_scope_struct___iter_avro_records(__pyx_ptype_8fastavro_5_read___pyx_scope_struct___iter_avro_records, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8fastavro_5_read___pyx_scope_struct___iter_avro_records *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 904, __pyx_L1_error)
+    __PYX_ERR(0, 881, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_fo = __pyx_v_fo;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_fo);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_fo);
   __pyx_cur_scope->__pyx_v_header = __pyx_v_header;
@@ -14835,22 +14679,19 @@
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_writer_schema);
   __pyx_cur_scope->__pyx_v_named_schemas = __pyx_v_named_schemas;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_named_schemas);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_named_schemas);
   __pyx_cur_scope->__pyx_v_reader_schema = __pyx_v_reader_schema;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_reader_schema);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_reader_schema);
-  __pyx_cur_scope->__pyx_v_return_record_name = __pyx_v_return_record_name;
-  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_return_record_name);
-  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_return_record_name);
-  __pyx_cur_scope->__pyx_v_return_record_name_override = __pyx_v_return_record_name_override;
-  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_return_record_name_override);
-  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_return_record_name_override);
+  __pyx_cur_scope->__pyx_v_options = __pyx_v_options;
+  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_options);
+  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_options);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8fastavro_5_read_82generator, __pyx_codeobj__3, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter_avro_records, __pyx_n_s_iter_avro_records, __pyx_n_s_fastavro__read); if (unlikely(!gen)) __PYX_ERR(0, 904, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8fastavro_5_read_82generator, __pyx_codeobj__9, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter_avro_records, __pyx_n_s_iter_avro_records, __pyx_n_s_fastavro__read); if (unlikely(!gen)) __PYX_ERR(0, 881, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14884,128 +14725,128 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L9_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 904, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 881, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":916
+  /* "fastavro/_read.pyx":892
  *     cdef int32 i
  * 
  *     sync_marker = header["sync"]             # <<<<<<<<<<<<<<
  * 
  *     read_block = BLOCK_READERS.get(codec)
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_cur_scope->__pyx_v_header, __pyx_n_u_sync); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 916, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_cur_scope->__pyx_v_header, __pyx_n_u_sync); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 892, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_sync_marker = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":918
+  /* "fastavro/_read.pyx":894
  *     sync_marker = header["sync"]
  * 
  *     read_block = BLOCK_READERS.get(codec)             # <<<<<<<<<<<<<<
  *     if not read_block:
  *         raise ValueError(f"Unrecognized codec: {codec}")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 918, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 894, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 918, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 894, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_cur_scope->__pyx_v_codec) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_cur_scope->__pyx_v_codec);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 918, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 894, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_read_block = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":919
+  /* "fastavro/_read.pyx":895
  * 
  *     read_block = BLOCK_READERS.get(codec)
  *     if not read_block:             # <<<<<<<<<<<<<<
  *         raise ValueError(f"Unrecognized codec: {codec}")
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_read_block); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 919, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_read_block); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 895, __pyx_L1_error)
   __pyx_t_5 = ((!__pyx_t_4) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "fastavro/_read.pyx":920
+    /* "fastavro/_read.pyx":896
  *     read_block = BLOCK_READERS.get(codec)
  *     if not read_block:
  *         raise ValueError(f"Unrecognized codec: {codec}")             # <<<<<<<<<<<<<<
  * 
  *     block_count = 0
  */
-    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_cur_scope->__pyx_v_codec, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 920, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_cur_scope->__pyx_v_codec, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 896, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unrecognized_codec, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 920, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unrecognized_codec, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 896, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 920, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 896, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 920, __pyx_L1_error)
+    __PYX_ERR(0, 896, __pyx_L1_error)
 
-    /* "fastavro/_read.pyx":919
+    /* "fastavro/_read.pyx":895
  * 
  *     read_block = BLOCK_READERS.get(codec)
  *     if not read_block:             # <<<<<<<<<<<<<<
  *         raise ValueError(f"Unrecognized codec: {codec}")
  * 
  */
   }
 
-  /* "fastavro/_read.pyx":922
+  /* "fastavro/_read.pyx":898
  *         raise ValueError(f"Unrecognized codec: {codec}")
  * 
  *     block_count = 0             # <<<<<<<<<<<<<<
  *     while True:
  *         block_count = read_long(fo)
  */
   __pyx_cur_scope->__pyx_v_block_count = 0;
 
-  /* "fastavro/_read.pyx":923
+  /* "fastavro/_read.pyx":899
  * 
  *     block_count = 0
  *     while True:             # <<<<<<<<<<<<<<
  *         block_count = read_long(fo)
  *         block_fo = read_block(fo)
  */
   while (1) {
 
-    /* "fastavro/_read.pyx":924
+    /* "fastavro/_read.pyx":900
  *     block_count = 0
  *     while True:
  *         block_count = read_long(fo)             # <<<<<<<<<<<<<<
  *         block_fo = read_block(fo)
  * 
  */
-    __pyx_t_6 = __pyx_f_8fastavro_5_read_read_long(__pyx_cur_scope->__pyx_v_fo, 0); if (unlikely(__pyx_t_6 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 924, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_8fastavro_5_read_read_long(__pyx_cur_scope->__pyx_v_fo, 0); if (unlikely(__pyx_t_6 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 900, __pyx_L1_error)
     __pyx_cur_scope->__pyx_v_block_count = __pyx_t_6;
 
-    /* "fastavro/_read.pyx":925
+    /* "fastavro/_read.pyx":901
  *     while True:
  *         block_count = read_long(fo)
  *         block_fo = read_block(fo)             # <<<<<<<<<<<<<<
  * 
  *         for i in range(block_count):
  */
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_read_block);
@@ -15017,46 +14858,45 @@
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_cur_scope->__pyx_v_fo) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_cur_scope->__pyx_v_fo);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 925, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 901, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_block_fo);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_block_fo, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":927
+    /* "fastavro/_read.pyx":903
  *         block_fo = read_block(fo)
  * 
  *         for i in range(block_count):             # <<<<<<<<<<<<<<
  *             yield _read_data(
  *                 block_fo,
  */
     __pyx_t_6 = __pyx_cur_scope->__pyx_v_block_count;
     __pyx_t_7 = __pyx_t_6;
     for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
       __pyx_cur_scope->__pyx_v_i = __pyx_t_8;
 
-      /* "fastavro/_read.pyx":928
+      /* "fastavro/_read.pyx":904
  * 
  *         for i in range(block_count):
  *             yield _read_data(             # <<<<<<<<<<<<<<
  *                 block_fo,
  *                 writer_schema,
  */
-      __pyx_t_9.__pyx_n = 3;
+      __pyx_t_9.__pyx_n = 2;
       __pyx_t_9.reader_schema = __pyx_cur_scope->__pyx_v_reader_schema;
-      __pyx_t_9.return_record_name = __pyx_cur_scope->__pyx_v_return_record_name;
-      __pyx_t_9.return_record_name_override = __pyx_cur_scope->__pyx_v_return_record_name_override;
-      __pyx_t_1 = __pyx_f_8fastavro_5_read__read_data(__pyx_cur_scope->__pyx_v_block_fo, __pyx_cur_scope->__pyx_v_writer_schema, __pyx_cur_scope->__pyx_v_named_schemas, 0, &__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 928, __pyx_L1_error)
+      __pyx_t_9.options = __pyx_cur_scope->__pyx_v_options;
+      __pyx_t_1 = __pyx_f_8fastavro_5_read__read_data(__pyx_cur_scope->__pyx_v_block_fo, __pyx_cur_scope->__pyx_v_writer_schema, __pyx_cur_scope->__pyx_v_named_schemas, 0, &__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 904, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_r = __pyx_t_1;
       __pyx_t_1 = 0;
       __pyx_cur_scope->__pyx_t_0 = __pyx_t_6;
       __pyx_cur_scope->__pyx_t_1 = __pyx_t_7;
       __pyx_cur_scope->__pyx_t_2 = __pyx_t_8;
       __Pyx_XGIVEREF(__pyx_r);
@@ -15065,31 +14905,31 @@
       /* return from generator, yielding value */
       __pyx_generator->resume_label = 1;
       return __pyx_r;
       __pyx_L9_resume_from_yield:;
       __pyx_t_6 = __pyx_cur_scope->__pyx_t_0;
       __pyx_t_7 = __pyx_cur_scope->__pyx_t_1;
       __pyx_t_8 = __pyx_cur_scope->__pyx_t_2;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 928, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 904, __pyx_L1_error)
     }
 
-    /* "fastavro/_read.pyx":937
+    /* "fastavro/_read.pyx":912
  *             )
  * 
  *         skip_sync(fo, sync_marker)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_sync(__pyx_cur_scope->__pyx_v_fo, __pyx_cur_scope->__pyx_v_sync_marker, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 937, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8fastavro_5_read_skip_sync(__pyx_cur_scope->__pyx_v_fo, __pyx_cur_scope->__pyx_v_sync_marker, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 912, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "fastavro/_read.pyx":904
+  /* "fastavro/_read.pyx":881
  * 
  * 
  * def _iter_avro_records(             # <<<<<<<<<<<<<<
  *     fo,
  *     header,
  */
 
@@ -15109,15 +14949,15 @@
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_8fastavro_5_read_85generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "fastavro/_read.pyx":940
+/* "fastavro/_read.pyx":915
  * 
  * 
  * def _iter_avro_blocks(             # <<<<<<<<<<<<<<
  *     fo,
  *     header,
  */
 
@@ -15127,49 +14967,28 @@
 static PyObject *__pyx_pw_8fastavro_5_read_84_iter_avro_blocks(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_header = 0;
   PyObject *__pyx_v_codec = 0;
   PyObject *__pyx_v_writer_schema = 0;
   PyObject *__pyx_v_named_schemas = 0;
   PyObject *__pyx_v_reader_schema = 0;
-  PyObject *__pyx_v_return_record_name = 0;
-  PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_options = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_iter_avro_blocks (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_header,&__pyx_n_s_codec,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[8] = {0,0,0,0,0,0,0,0};
-
-    /* "fastavro/_read.pyx":947
- *     named_schemas,
- *     reader_schema,
- *     return_record_name=False,             # <<<<<<<<<<<<<<
- *     return_record_name_override=False,
- * ):
- */
-    values[6] = ((PyObject *)Py_False);
-
-    /* "fastavro/_read.pyx":948
- *     reader_schema,
- *     return_record_name=False,
- *     return_record_name_override=False,             # <<<<<<<<<<<<<<
- * ):
- *     sync_marker = header["sync"]
- */
-    values[7] = ((PyObject *)Py_False);
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_header,&__pyx_n_s_codec,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_reader_schema,&__pyx_n_s_options,0};
+    PyObject* values[7] = {0,0,0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
-        CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
@@ -15188,117 +15007,97 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_header)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 0, 6, 8, 1); __PYX_ERR(0, 940, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 1, 7, 7, 1); __PYX_ERR(0, 915, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_codec)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 0, 6, 8, 2); __PYX_ERR(0, 940, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 1, 7, 7, 2); __PYX_ERR(0, 915, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 0, 6, 8, 3); __PYX_ERR(0, 940, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 1, 7, 7, 3); __PYX_ERR(0, 915, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 0, 6, 8, 4); __PYX_ERR(0, 940, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 1, 7, 7, 4); __PYX_ERR(0, 915, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 0, 6, 8, 5); __PYX_ERR(0, 940, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 1, 7, 7, 5); __PYX_ERR(0, 915, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name);
-          if (value) { values[6] = value; kw_args--; }
-        }
-        CYTHON_FALLTHROUGH;
-        case  7:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
-          if (value) { values[7] = value; kw_args--; }
+        if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 1, 7, 7, 6); __PYX_ERR(0, 915, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_iter_avro_blocks") < 0)) __PYX_ERR(0, 940, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_iter_avro_blocks") < 0)) __PYX_ERR(0, 915, __pyx_L3_error)
       }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 7) {
+      goto __pyx_L5_argtuple_error;
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
-        CYTHON_FALLTHROUGH;
-        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
-        CYTHON_FALLTHROUGH;
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+      values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
     __pyx_v_fo = values[0];
     __pyx_v_header = values[1];
     __pyx_v_codec = values[2];
     __pyx_v_writer_schema = values[3];
     __pyx_v_named_schemas = values[4];
     __pyx_v_reader_schema = values[5];
-    __pyx_v_return_record_name = values[6];
-    __pyx_v_return_record_name_override = values[7];
+    __pyx_v_options = values[6];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 0, 6, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 940, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_iter_avro_blocks", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 915, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read._iter_avro_blocks", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_83_iter_avro_blocks(__pyx_self, __pyx_v_fo, __pyx_v_header, __pyx_v_codec, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
-
-  /* "fastavro/_read.pyx":940
- * 
- * 
- * def _iter_avro_blocks(             # <<<<<<<<<<<<<<
- *     fo,
- *     header,
- */
+  __pyx_r = __pyx_pf_8fastavro_5_read_83_iter_avro_blocks(__pyx_self, __pyx_v_fo, __pyx_v_header, __pyx_v_codec, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_reader_schema, __pyx_v_options);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_83_iter_avro_blocks(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_header, PyObject *__pyx_v_codec, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_83_iter_avro_blocks(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_header, PyObject *__pyx_v_codec, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options) {
   struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_iter_avro_blocks", 0);
   __pyx_cur_scope = (struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks *)__pyx_tp_new_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks(__pyx_ptype_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 940, __pyx_L1_error)
+    __PYX_ERR(0, 915, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_fo = __pyx_v_fo;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_fo);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_fo);
   __pyx_cur_scope->__pyx_v_header = __pyx_v_header;
@@ -15312,22 +15111,19 @@
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_writer_schema);
   __pyx_cur_scope->__pyx_v_named_schemas = __pyx_v_named_schemas;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_named_schemas);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_named_schemas);
   __pyx_cur_scope->__pyx_v_reader_schema = __pyx_v_reader_schema;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_reader_schema);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_reader_schema);
-  __pyx_cur_scope->__pyx_v_return_record_name = __pyx_v_return_record_name;
-  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_return_record_name);
-  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_return_record_name);
-  __pyx_cur_scope->__pyx_v_return_record_name_override = __pyx_v_return_record_name_override;
-  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_return_record_name_override);
-  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_return_record_name_override);
+  __pyx_cur_scope->__pyx_v_options = __pyx_v_options;
+  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_options);
+  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_options);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8fastavro_5_read_85generator1, __pyx_codeobj__4, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter_avro_blocks, __pyx_n_s_iter_avro_blocks, __pyx_n_s_fastavro__read); if (unlikely(!gen)) __PYX_ERR(0, 940, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8fastavro_5_read_85generator1, __pyx_codeobj__10, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter_avro_blocks, __pyx_n_s_iter_avro_blocks, __pyx_n_s_fastavro__read); if (unlikely(!gen)) __PYX_ERR(0, 915, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15364,162 +15160,162 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L17_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 940, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 915, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":950
- *     return_record_name_override=False,
+  /* "fastavro/_read.pyx":924
+ *     options,
  * ):
  *     sync_marker = header["sync"]             # <<<<<<<<<<<<<<
  * 
  *     read_block = BLOCK_READERS.get(codec)
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_cur_scope->__pyx_v_header, __pyx_n_u_sync); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 950, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_cur_scope->__pyx_v_header, __pyx_n_u_sync); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 924, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_sync_marker = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":952
+  /* "fastavro/_read.pyx":926
  *     sync_marker = header["sync"]
  * 
  *     read_block = BLOCK_READERS.get(codec)             # <<<<<<<<<<<<<<
  *     if not read_block:
  *         raise ValueError(f"Unrecognized codec: {codec}")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 952, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 926, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 952, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 926, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_cur_scope->__pyx_v_codec) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_cur_scope->__pyx_v_codec);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 952, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 926, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_read_block = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":953
+  /* "fastavro/_read.pyx":927
  * 
  *     read_block = BLOCK_READERS.get(codec)
  *     if not read_block:             # <<<<<<<<<<<<<<
  *         raise ValueError(f"Unrecognized codec: {codec}")
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_read_block); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 953, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_read_block); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 927, __pyx_L1_error)
   __pyx_t_5 = ((!__pyx_t_4) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "fastavro/_read.pyx":954
+    /* "fastavro/_read.pyx":928
  *     read_block = BLOCK_READERS.get(codec)
  *     if not read_block:
  *         raise ValueError(f"Unrecognized codec: {codec}")             # <<<<<<<<<<<<<<
  * 
  *     while True:
  */
-    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_cur_scope->__pyx_v_codec, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 954, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_cur_scope->__pyx_v_codec, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 928, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unrecognized_codec, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 954, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unrecognized_codec, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 928, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 954, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 928, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 954, __pyx_L1_error)
+    __PYX_ERR(0, 928, __pyx_L1_error)
 
-    /* "fastavro/_read.pyx":953
+    /* "fastavro/_read.pyx":927
  * 
  *     read_block = BLOCK_READERS.get(codec)
  *     if not read_block:             # <<<<<<<<<<<<<<
  *         raise ValueError(f"Unrecognized codec: {codec}")
  * 
  */
   }
 
-  /* "fastavro/_read.pyx":956
+  /* "fastavro/_read.pyx":930
  *         raise ValueError(f"Unrecognized codec: {codec}")
  * 
  *     while True:             # <<<<<<<<<<<<<<
  *         offset = fo.tell()
  *         try:
  */
   while (1) {
 
-    /* "fastavro/_read.pyx":957
+    /* "fastavro/_read.pyx":931
  * 
  *     while True:
  *         offset = fo.tell()             # <<<<<<<<<<<<<<
  *         try:
  *             num_block_records = read_long(fo)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_fo, __pyx_n_s_tell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 957, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_fo, __pyx_n_s_tell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 931, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 957, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 931, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_offset);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_offset, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":958
+    /* "fastavro/_read.pyx":932
  *     while True:
  *         offset = fo.tell()
  *         try:             # <<<<<<<<<<<<<<
  *             num_block_records = read_long(fo)
  *         except StopIteration:
  */
     {
       __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_8);
       /*try:*/ {
 
-        /* "fastavro/_read.pyx":959
+        /* "fastavro/_read.pyx":933
  *         offset = fo.tell()
  *         try:
  *             num_block_records = read_long(fo)             # <<<<<<<<<<<<<<
  *         except StopIteration:
  *             return
  */
-        __pyx_t_9 = __pyx_f_8fastavro_5_read_read_long(__pyx_cur_scope->__pyx_v_fo, 0); if (unlikely(__pyx_t_9 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 959, __pyx_L7_error)
+        __pyx_t_9 = __pyx_f_8fastavro_5_read_read_long(__pyx_cur_scope->__pyx_v_fo, 0); if (unlikely(__pyx_t_9 == ((__pyx_t_8fastavro_5_read_long64)-1LL) && PyErr_Occurred())) __PYX_ERR(0, 933, __pyx_L7_error)
         __pyx_cur_scope->__pyx_v_num_block_records = __pyx_t_9;
 
-        /* "fastavro/_read.pyx":958
+        /* "fastavro/_read.pyx":932
  *     while True:
  *         offset = fo.tell()
  *         try:             # <<<<<<<<<<<<<<
  *             num_block_records = read_long(fo)
  *         except StopIteration:
  */
       }
@@ -15528,30 +15324,30 @@
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       goto __pyx_L14_try_end;
       __pyx_L7_error:;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "fastavro/_read.pyx":960
+      /* "fastavro/_read.pyx":934
  *         try:
  *             num_block_records = read_long(fo)
  *         except StopIteration:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
       __pyx_t_10 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_StopIteration);
       if (__pyx_t_10) {
         __Pyx_AddTraceback("fastavro._read._iter_avro_blocks", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 960, __pyx_L9_except_error)
+        if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 934, __pyx_L9_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_t_2);
 
-        /* "fastavro/_read.pyx":961
+        /* "fastavro/_read.pyx":935
  *             num_block_records = read_long(fo)
  *         except StopIteration:
  *             return             # <<<<<<<<<<<<<<
  * 
  *         block_bytes = read_block(fo)
  */
         __Pyx_XDECREF(__pyx_r);
@@ -15560,15 +15356,15 @@
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         goto __pyx_L10_except_return;
       }
       goto __pyx_L9_except_error;
       __pyx_L9_except_error:;
 
-      /* "fastavro/_read.pyx":958
+      /* "fastavro/_read.pyx":932
  *     while True:
  *         offset = fo.tell()
  *         try:             # <<<<<<<<<<<<<<
  *             num_block_records = read_long(fo)
  *         except StopIteration:
  */
       __Pyx_XGIVEREF(__pyx_t_6);
@@ -15581,15 +15377,15 @@
       __Pyx_XGIVEREF(__pyx_t_7);
       __Pyx_XGIVEREF(__pyx_t_8);
       __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
       goto __pyx_L0;
       __pyx_L14_try_end:;
     }
 
-    /* "fastavro/_read.pyx":963
+    /* "fastavro/_read.pyx":937
  *             return
  * 
  *         block_bytes = read_block(fo)             # <<<<<<<<<<<<<<
  * 
  *         skip_sync(fo, sync_marker)
  */
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_read_block);
@@ -15601,89 +15397,89 @@
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_cur_scope->__pyx_v_fo) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_cur_scope->__pyx_v_fo);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 963, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 937, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_block_bytes);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_block_bytes, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "fastavro/_read.pyx":965
+    /* "fastavro/_read.pyx":939
  *         block_bytes = read_block(fo)
  * 
  *         skip_sync(fo, sync_marker)             # <<<<<<<<<<<<<<
  * 
  *         size = fo.tell() - offset
  */
-    __pyx_t_2 = __pyx_f_8fastavro_5_read_skip_sync(__pyx_cur_scope->__pyx_v_fo, __pyx_cur_scope->__pyx_v_sync_marker, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 965, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8fastavro_5_read_skip_sync(__pyx_cur_scope->__pyx_v_fo, __pyx_cur_scope->__pyx_v_sync_marker, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 939, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "fastavro/_read.pyx":967
+    /* "fastavro/_read.pyx":941
  *         skip_sync(fo, sync_marker)
  * 
  *         size = fo.tell() - offset             # <<<<<<<<<<<<<<
  * 
  *         yield Block(
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_fo, __pyx_n_s_tell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 967, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_fo, __pyx_n_s_tell); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 941, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 967, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 941, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_cur_scope->__pyx_v_offset); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 967, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_cur_scope->__pyx_v_offset); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 941, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_size);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_size, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "fastavro/_read.pyx":969
+    /* "fastavro/_read.pyx":943
  *         size = fo.tell() - offset
  * 
  *         yield Block(             # <<<<<<<<<<<<<<
  *             block_bytes, num_block_records, codec, reader_schema,
- *             writer_schema, named_schemas, offset, size, return_record_name, return_record_name_override
+ *             writer_schema, named_schemas, offset, size, options,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 969, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 943, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "fastavro/_read.pyx":970
+    /* "fastavro/_read.pyx":944
  * 
  *         yield Block(
  *             block_bytes, num_block_records, codec, reader_schema,             # <<<<<<<<<<<<<<
- *             writer_schema, named_schemas, offset, size, return_record_name, return_record_name_override
+ *             writer_schema, named_schemas, offset, size, options,
  *         )
  */
-    __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_cur_scope->__pyx_v_num_block_records); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 970, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_cur_scope->__pyx_v_num_block_records); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 944, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "fastavro/_read.pyx":971
+    /* "fastavro/_read.pyx":945
  *         yield Block(
  *             block_bytes, num_block_records, codec, reader_schema,
- *             writer_schema, named_schemas, offset, size, return_record_name, return_record_name_override             # <<<<<<<<<<<<<<
+ *             writer_schema, named_schemas, offset, size, options,             # <<<<<<<<<<<<<<
  *         )
  * 
  */
     __pyx_t_11 = NULL;
     __pyx_t_10 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
@@ -15693,32 +15489,32 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_10 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
-      PyObject *__pyx_temp[11] = {__pyx_t_11, __pyx_cur_scope->__pyx_v_block_bytes, __pyx_t_1, __pyx_cur_scope->__pyx_v_codec, __pyx_cur_scope->__pyx_v_reader_schema, __pyx_cur_scope->__pyx_v_writer_schema, __pyx_cur_scope->__pyx_v_named_schemas, __pyx_cur_scope->__pyx_v_offset, __pyx_cur_scope->__pyx_v_size, __pyx_cur_scope->__pyx_v_return_record_name, __pyx_cur_scope->__pyx_v_return_record_name_override};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 10+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 969, __pyx_L1_error)
+      PyObject *__pyx_temp[10] = {__pyx_t_11, __pyx_cur_scope->__pyx_v_block_bytes, __pyx_t_1, __pyx_cur_scope->__pyx_v_codec, __pyx_cur_scope->__pyx_v_reader_schema, __pyx_cur_scope->__pyx_v_writer_schema, __pyx_cur_scope->__pyx_v_named_schemas, __pyx_cur_scope->__pyx_v_offset, __pyx_cur_scope->__pyx_v_size, __pyx_cur_scope->__pyx_v_options};
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 9+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 943, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-      PyObject *__pyx_temp[11] = {__pyx_t_11, __pyx_cur_scope->__pyx_v_block_bytes, __pyx_t_1, __pyx_cur_scope->__pyx_v_codec, __pyx_cur_scope->__pyx_v_reader_schema, __pyx_cur_scope->__pyx_v_writer_schema, __pyx_cur_scope->__pyx_v_named_schemas, __pyx_cur_scope->__pyx_v_offset, __pyx_cur_scope->__pyx_v_size, __pyx_cur_scope->__pyx_v_return_record_name, __pyx_cur_scope->__pyx_v_return_record_name_override};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 10+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 969, __pyx_L1_error)
+      PyObject *__pyx_temp[10] = {__pyx_t_11, __pyx_cur_scope->__pyx_v_block_bytes, __pyx_t_1, __pyx_cur_scope->__pyx_v_codec, __pyx_cur_scope->__pyx_v_reader_schema, __pyx_cur_scope->__pyx_v_writer_schema, __pyx_cur_scope->__pyx_v_named_schemas, __pyx_cur_scope->__pyx_v_offset, __pyx_cur_scope->__pyx_v_size, __pyx_cur_scope->__pyx_v_options};
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 9+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 943, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     {
-      __pyx_t_12 = PyTuple_New(10+__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 969, __pyx_L1_error)
+      __pyx_t_12 = PyTuple_New(9+__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 943, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       if (__pyx_t_11) {
         __Pyx_GIVEREF(__pyx_t_11); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_11); __pyx_t_11 = NULL;
       }
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_block_bytes);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_block_bytes);
       PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_10, __pyx_cur_scope->__pyx_v_block_bytes);
@@ -15738,40 +15534,37 @@
       PyTuple_SET_ITEM(__pyx_t_12, 5+__pyx_t_10, __pyx_cur_scope->__pyx_v_named_schemas);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_offset);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_offset);
       PyTuple_SET_ITEM(__pyx_t_12, 6+__pyx_t_10, __pyx_cur_scope->__pyx_v_offset);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_size);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_size);
       PyTuple_SET_ITEM(__pyx_t_12, 7+__pyx_t_10, __pyx_cur_scope->__pyx_v_size);
-      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_return_record_name);
-      __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_return_record_name);
-      PyTuple_SET_ITEM(__pyx_t_12, 8+__pyx_t_10, __pyx_cur_scope->__pyx_v_return_record_name);
-      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_return_record_name_override);
-      __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_return_record_name_override);
-      PyTuple_SET_ITEM(__pyx_t_12, 9+__pyx_t_10, __pyx_cur_scope->__pyx_v_return_record_name_override);
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_options);
+      __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_options);
+      PyTuple_SET_ITEM(__pyx_t_12, 8+__pyx_t_10, __pyx_cur_scope->__pyx_v_options);
       __pyx_t_1 = 0;
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 969, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 943, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
     /* return from generator, yielding value */
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L17_resume_from_yield:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 969, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 943, __pyx_L1_error)
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "fastavro/_read.pyx":940
+  /* "fastavro/_read.pyx":915
  * 
  * 
  * def _iter_avro_blocks(             # <<<<<<<<<<<<<<
  *     fo,
  *     header,
  */
 
@@ -15792,20 +15585,20 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":976
+/* "fastavro/_read.pyx":950
  * 
  * class Block:
  *     def __init__(             # <<<<<<<<<<<<<<
- *             self,
- *             bytes_,
+ *         self,
+ *         bytes_,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8fastavro_5_read_5Block_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_8fastavro_5_read_5Block_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_5Block_1__init__, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_8fastavro_5_read_5Block_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
@@ -15813,49 +15606,28 @@
   PyObject *__pyx_v_num_records = 0;
   PyObject *__pyx_v_codec = 0;
   PyObject *__pyx_v_reader_schema = 0;
   PyObject *__pyx_v_writer_schema = 0;
   PyObject *__pyx_v_named_schemas = 0;
   PyObject *__pyx_v_offset = 0;
   PyObject *__pyx_v_size = 0;
-  PyObject *__pyx_v_return_record_name = 0;
-  PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_options = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_bytes_2,&__pyx_n_s_num_records,&__pyx_n_s_codec,&__pyx_n_s_reader_schema,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_offset,&__pyx_n_s_size,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[11] = {0,0,0,0,0,0,0,0,0,0,0};
-
-    /* "fastavro/_read.pyx":986
- *             offset,
- *             size,
- *             return_record_name=False,             # <<<<<<<<<<<<<<
- *             return_record_name_override=False):
- *         self.bytes_ = bytes_
- */
-    values[9] = ((PyObject *)((PyObject *)Py_False));
-
-    /* "fastavro/_read.pyx":987
- *             size,
- *             return_record_name=False,
- *             return_record_name_override=False):             # <<<<<<<<<<<<<<
- *         self.bytes_ = bytes_
- *         self.num_records = num_records
- */
-    values[10] = ((PyObject *)((PyObject *)Py_False));
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_bytes_2,&__pyx_n_s_num_records,&__pyx_n_s_codec,&__pyx_n_s_reader_schema,&__pyx_n_s_writer_schema,&__pyx_n_s_named_schemas,&__pyx_n_s_offset,&__pyx_n_s_size,&__pyx_n_s_options,0};
+    PyObject* values[10] = {0,0,0,0,0,0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
-        CYTHON_FALLTHROUGH;
         case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -15880,232 +15652,203 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bytes_2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 9, 11, 1); __PYX_ERR(0, 976, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 10, 10, 1); __PYX_ERR(0, 950, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_num_records)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 9, 11, 2); __PYX_ERR(0, 976, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 10, 10, 2); __PYX_ERR(0, 950, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_codec)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 9, 11, 3); __PYX_ERR(0, 976, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 10, 10, 3); __PYX_ERR(0, 950, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 9, 11, 4); __PYX_ERR(0, 976, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 10, 10, 4); __PYX_ERR(0, 950, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 9, 11, 5); __PYX_ERR(0, 976, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 10, 10, 5); __PYX_ERR(0, 950, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_named_schemas)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 9, 11, 6); __PYX_ERR(0, 976, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 10, 10, 6); __PYX_ERR(0, 950, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_offset)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 9, 11, 7); __PYX_ERR(0, 976, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 10, 10, 7); __PYX_ERR(0, 950, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (likely((values[8] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_size)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 9, 11, 8); __PYX_ERR(0, 976, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 10, 10, 8); __PYX_ERR(0, 950, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name);
-          if (value) { values[9] = value; kw_args--; }
-        }
-        CYTHON_FALLTHROUGH;
-        case 10:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
-          if (value) { values[10] = value; kw_args--; }
+        if (likely((values[9] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 10, 10, 9); __PYX_ERR(0, 950, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 976, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 950, __pyx_L3_error)
       }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 10) {
+      goto __pyx_L5_argtuple_error;
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
-        CYTHON_FALLTHROUGH;
-        case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
-        CYTHON_FALLTHROUGH;
-        case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
-        values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
-        values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
-        values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
-        values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+      values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+      values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+      values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
+      values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
     }
     __pyx_v_self = values[0];
     __pyx_v_bytes_ = values[1];
     __pyx_v_num_records = values[2];
     __pyx_v_codec = values[3];
     __pyx_v_reader_schema = values[4];
     __pyx_v_writer_schema = values[5];
     __pyx_v_named_schemas = values[6];
     __pyx_v_offset = values[7];
     __pyx_v_size = values[8];
-    __pyx_v_return_record_name = values[9];
-    __pyx_v_return_record_name_override = values[10];
+    __pyx_v_options = values[9];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 9, 11, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 976, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 10, 10, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 950, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.Block.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_5Block___init__(__pyx_self, __pyx_v_self, __pyx_v_bytes_, __pyx_v_num_records, __pyx_v_codec, __pyx_v_reader_schema, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_offset, __pyx_v_size, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
-
-  /* "fastavro/_read.pyx":976
- * 
- * class Block:
- *     def __init__(             # <<<<<<<<<<<<<<
- *             self,
- *             bytes_,
- */
+  __pyx_r = __pyx_pf_8fastavro_5_read_5Block___init__(__pyx_self, __pyx_v_self, __pyx_v_bytes_, __pyx_v_num_records, __pyx_v_codec, __pyx_v_reader_schema, __pyx_v_writer_schema, __pyx_v_named_schemas, __pyx_v_offset, __pyx_v_size, __pyx_v_options);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_5Block___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_bytes_, PyObject *__pyx_v_num_records, PyObject *__pyx_v_codec, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_offset, PyObject *__pyx_v_size, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_5Block___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_bytes_, PyObject *__pyx_v_num_records, PyObject *__pyx_v_codec, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_named_schemas, PyObject *__pyx_v_offset, PyObject *__pyx_v_size, PyObject *__pyx_v_options) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "fastavro/_read.pyx":988
- *             return_record_name=False,
- *             return_record_name_override=False):
+  /* "fastavro/_read.pyx":962
+ *         options,
+ *     ):
  *         self.bytes_ = bytes_             # <<<<<<<<<<<<<<
  *         self.num_records = num_records
  *         self.codec = codec
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_bytes_2, __pyx_v_bytes_) < 0) __PYX_ERR(0, 988, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_bytes_2, __pyx_v_bytes_) < 0) __PYX_ERR(0, 962, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":989
- *             return_record_name_override=False):
+  /* "fastavro/_read.pyx":963
+ *     ):
  *         self.bytes_ = bytes_
  *         self.num_records = num_records             # <<<<<<<<<<<<<<
  *         self.codec = codec
  *         self.reader_schema = reader_schema
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_num_records, __pyx_v_num_records) < 0) __PYX_ERR(0, 989, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_num_records, __pyx_v_num_records) < 0) __PYX_ERR(0, 963, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":990
+  /* "fastavro/_read.pyx":964
  *         self.bytes_ = bytes_
  *         self.num_records = num_records
  *         self.codec = codec             # <<<<<<<<<<<<<<
  *         self.reader_schema = reader_schema
  *         self.writer_schema = writer_schema
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_codec, __pyx_v_codec) < 0) __PYX_ERR(0, 990, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_codec, __pyx_v_codec) < 0) __PYX_ERR(0, 964, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":991
+  /* "fastavro/_read.pyx":965
  *         self.num_records = num_records
  *         self.codec = codec
  *         self.reader_schema = reader_schema             # <<<<<<<<<<<<<<
  *         self.writer_schema = writer_schema
  *         self._named_schemas = named_schemas
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_reader_schema, __pyx_v_reader_schema) < 0) __PYX_ERR(0, 991, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_reader_schema, __pyx_v_reader_schema) < 0) __PYX_ERR(0, 965, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":992
+  /* "fastavro/_read.pyx":966
  *         self.codec = codec
  *         self.reader_schema = reader_schema
  *         self.writer_schema = writer_schema             # <<<<<<<<<<<<<<
  *         self._named_schemas = named_schemas
  *         self.offset = offset
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_writer_schema, __pyx_v_writer_schema) < 0) __PYX_ERR(0, 992, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_writer_schema, __pyx_v_writer_schema) < 0) __PYX_ERR(0, 966, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":993
+  /* "fastavro/_read.pyx":967
  *         self.reader_schema = reader_schema
  *         self.writer_schema = writer_schema
  *         self._named_schemas = named_schemas             # <<<<<<<<<<<<<<
  *         self.offset = offset
  *         self.size = size
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2, __pyx_v_named_schemas) < 0) __PYX_ERR(0, 993, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2, __pyx_v_named_schemas) < 0) __PYX_ERR(0, 967, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":994
+  /* "fastavro/_read.pyx":968
  *         self.writer_schema = writer_schema
  *         self._named_schemas = named_schemas
  *         self.offset = offset             # <<<<<<<<<<<<<<
  *         self.size = size
- *         self.return_record_name = return_record_name
+ *         self.options = options
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_offset, __pyx_v_offset) < 0) __PYX_ERR(0, 994, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_offset, __pyx_v_offset) < 0) __PYX_ERR(0, 968, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":995
+  /* "fastavro/_read.pyx":969
  *         self._named_schemas = named_schemas
  *         self.offset = offset
  *         self.size = size             # <<<<<<<<<<<<<<
- *         self.return_record_name = return_record_name
- *         self.return_record_name_override = return_record_name_override
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_size, __pyx_v_size) < 0) __PYX_ERR(0, 995, __pyx_L1_error)
-
-  /* "fastavro/_read.pyx":996
- *         self.offset = offset
- *         self.size = size
- *         self.return_record_name = return_record_name             # <<<<<<<<<<<<<<
- *         self.return_record_name_override = return_record_name_override
+ *         self.options = options
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_return_record_name, __pyx_v_return_record_name) < 0) __PYX_ERR(0, 996, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_size, __pyx_v_size) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":997
+  /* "fastavro/_read.pyx":970
+ *         self.offset = offset
  *         self.size = size
- *         self.return_record_name = return_record_name
- *         self.return_record_name_override = return_record_name_override             # <<<<<<<<<<<<<<
+ *         self.options = options             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_return_record_name_override, __pyx_v_return_record_name_override) < 0) __PYX_ERR(0, 997, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_options, __pyx_v_options) < 0) __PYX_ERR(0, 970, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":976
+  /* "fastavro/_read.pyx":950
  * 
  * class Block:
  *     def __init__(             # <<<<<<<<<<<<<<
- *             self,
- *             bytes_,
+ *         self,
+ *         bytes_,
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("fastavro._read.Block.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -16113,16 +15856,16 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_8fastavro_5_read_5Block_4generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "fastavro/_read.pyx":999
- *         self.return_record_name_override = return_record_name_override
+/* "fastavro/_read.pyx":972
+ *         self.options = options
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         for i in range(self.num_records):
  *             yield _read_data(
  */
 
 /* Python wrapper */
@@ -16147,23 +15890,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
   __pyx_cur_scope = (struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_2___iter__ *)__pyx_tp_new_8fastavro_5_read___pyx_scope_struct_2___iter__(__pyx_ptype_8fastavro_5_read___pyx_scope_struct_2___iter__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_2___iter__ *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 999, __pyx_L1_error)
+    __PYX_ERR(0, 972, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8fastavro_5_read_5Block_4generator2, __pyx_codeobj__5, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter, __pyx_n_s_Block___iter, __pyx_n_s_fastavro__read); if (unlikely(!gen)) __PYX_ERR(0, 999, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8fastavro_5_read_5Block_4generator2, __pyx_codeobj__11, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter, __pyx_n_s_Block___iter, __pyx_n_s_fastavro__read); if (unlikely(!gen)) __PYX_ERR(0, 972, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16184,169 +15927,156 @@
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
-  PyObject *__pyx_t_10 = NULL;
-  struct __pyx_opt_args_8fastavro_5_read__read_data __pyx_t_11;
+  struct __pyx_opt_args_8fastavro_5_read__read_data __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 999, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 972, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1000
+  /* "fastavro/_read.pyx":973
  * 
  *     def __iter__(self):
  *         for i in range(self.num_records):             # <<<<<<<<<<<<<<
  *             yield _read_data(
  *                 self.bytes_,
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_num_records); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1000, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_num_records); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 973, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1000, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 973, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
     __pyx_t_1 = __pyx_t_2; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1000, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 973, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1000, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 973, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 1000, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 973, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1000, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 973, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 1000, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 973, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1000, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 973, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_4(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 1000, __pyx_L1_error)
+          else __PYX_ERR(0, 973, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_i);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_i, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "fastavro/_read.pyx":1002
+    /* "fastavro/_read.pyx":975
  *         for i in range(self.num_records):
  *             yield _read_data(
  *                 self.bytes_,             # <<<<<<<<<<<<<<
  *                 self.writer_schema,
  *                 self._named_schemas,
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_bytes_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1002, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_bytes_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 975, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "fastavro/_read.pyx":1003
+    /* "fastavro/_read.pyx":976
  *             yield _read_data(
  *                 self.bytes_,
  *                 self.writer_schema,             # <<<<<<<<<<<<<<
  *                 self._named_schemas,
  *                 self.reader_schema,
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_writer_schema); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1003, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_writer_schema); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 976, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
 
-    /* "fastavro/_read.pyx":1004
+    /* "fastavro/_read.pyx":977
  *                 self.bytes_,
  *                 self.writer_schema,
  *                 self._named_schemas,             # <<<<<<<<<<<<<<
  *                 self.reader_schema,
- *                 self.return_record_name,
+ *                 self.options,
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_named_schemas_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1004, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_named_schemas_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 977, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "fastavro/_read.pyx":1005
+    /* "fastavro/_read.pyx":978
  *                 self.writer_schema,
  *                 self._named_schemas,
  *                 self.reader_schema,             # <<<<<<<<<<<<<<
- *                 self.return_record_name,
- *                 self.return_record_name_override
+ *                 self.options,
+ *             )
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_reader_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1005, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_reader_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 978, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
 
-    /* "fastavro/_read.pyx":1006
+    /* "fastavro/_read.pyx":979
  *                 self._named_schemas,
  *                 self.reader_schema,
- *                 self.return_record_name,             # <<<<<<<<<<<<<<
- *                 self.return_record_name_override
- *             )
- */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_return_record_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1006, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-
-    /* "fastavro/_read.pyx":1007
- *                 self.reader_schema,
- *                 self.return_record_name,
- *                 self.return_record_name_override             # <<<<<<<<<<<<<<
+ *                 self.options,             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_return_record_name_override); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1007, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_options); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 979, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
 
-    /* "fastavro/_read.pyx":1001
+    /* "fastavro/_read.pyx":974
  *     def __iter__(self):
  *         for i in range(self.num_records):
  *             yield _read_data(             # <<<<<<<<<<<<<<
  *                 self.bytes_,
  *                 self.writer_schema,
  */
-    __pyx_t_11.__pyx_n = 3;
-    __pyx_t_11.reader_schema = __pyx_t_7;
-    __pyx_t_11.return_record_name = __pyx_t_8;
-    __pyx_t_11.return_record_name_override = __pyx_t_9;
-    __pyx_t_10 = __pyx_f_8fastavro_5_read__read_data(__pyx_t_2, __pyx_t_5, __pyx_t_6, 0, &__pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1001, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_10.__pyx_n = 2;
+    __pyx_t_10.reader_schema = __pyx_t_7;
+    __pyx_t_10.options = __pyx_t_8;
+    __pyx_t_9 = __pyx_f_8fastavro_5_read__read_data(__pyx_t_2, __pyx_t_5, __pyx_t_6, 0, &__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 974, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_r = __pyx_t_10;
-    __pyx_t_10 = 0;
+    __pyx_r = __pyx_t_9;
+    __pyx_t_9 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_3;
     __pyx_cur_scope->__pyx_t_2 = __pyx_t_4;
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
@@ -16355,29 +16085,29 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_4 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 1001, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 974, __pyx_L1_error)
 
-    /* "fastavro/_read.pyx":1000
+    /* "fastavro/_read.pyx":973
  * 
  *     def __iter__(self):
  *         for i in range(self.num_records):             # <<<<<<<<<<<<<<
  *             yield _read_data(
  *                 self.bytes_,
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "fastavro/_read.pyx":999
- *         self.return_record_name_override = return_record_name_override
+  /* "fastavro/_read.pyx":972
+ *         self.options = options
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         for i in range(self.num_records):
  *             yield _read_data(
  */
 
   /* function exit code */
@@ -16387,28 +16117,27 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("__iter__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
   #if !CYTHON_USE_EXC_INFO_STACK
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":1010
+/* "fastavro/_read.pyx":982
  *             )
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return (
  *             f"Avro block: {len(self.bytes_)} bytes, {self.num_records} records, "
  */
 
@@ -16437,135 +16166,135 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "fastavro/_read.pyx":1011
+  /* "fastavro/_read.pyx":983
  * 
  *     def __str__(self):
  *         return (             # <<<<<<<<<<<<<<
  *             f"Avro block: {len(self.bytes_)} bytes, {self.num_records} records, "
  *             + f"codec: {self.codec}, position {self.offset}+{self.size}"
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "fastavro/_read.pyx":1012
+  /* "fastavro/_read.pyx":984
  *     def __str__(self):
  *         return (
  *             f"Avro block: {len(self.bytes_)} bytes, {self.num_records} records, "             # <<<<<<<<<<<<<<
  *             + f"codec: {self.codec}, position {self.offset}+{self.size}"
  *         )
  */
-  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1012, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_3 = 127;
   __Pyx_INCREF(__pyx_kp_u_Avro_block);
   __pyx_t_2 += 12;
   __Pyx_GIVEREF(__pyx_kp_u_Avro_block);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Avro_block);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_bytes_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1012, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_bytes_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyObject_Length(__pyx_t_4); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1012, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_t_4); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1012, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u_bytes_3);
   __pyx_t_2 += 8;
   __Pyx_GIVEREF(__pyx_kp_u_bytes_3);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_bytes_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_num_records); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1012, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_num_records); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1012, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_6);
   __pyx_t_6 = 0;
   __Pyx_INCREF(__pyx_kp_u_records);
   __pyx_t_2 += 10;
   __Pyx_GIVEREF(__pyx_kp_u_records);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u_records);
-  __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1012, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":1013
+  /* "fastavro/_read.pyx":985
  *         return (
  *             f"Avro block: {len(self.bytes_)} bytes, {self.num_records} records, "
  *             + f"codec: {self.codec}, position {self.offset}+{self.size}"             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_1 = PyTuple_New(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_3 = 127;
   __Pyx_INCREF(__pyx_kp_u_codec_2);
   __pyx_t_2 += 7;
   __Pyx_GIVEREF(__pyx_kp_u_codec_2);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_codec_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_codec); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_codec); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_7);
   __pyx_t_7 = 0;
   __Pyx_INCREF(__pyx_kp_u_position);
   __pyx_t_2 += 11;
   __Pyx_GIVEREF(__pyx_kp_u_position);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_position);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_offset); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_offset); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_INCREF(__pyx_kp_u__6);
+  __Pyx_INCREF(__pyx_kp_u__12);
   __pyx_t_2 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__6);
-  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_kp_u__12);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__12);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_1, 6, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_1, 6, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":1010
+  /* "fastavro/_read.pyx":982
  *             )
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return (
  *             f"Avro block: {len(self.bytes_)} bytes, {self.num_records} records, "
  */
 
@@ -16579,49 +16308,88 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":1018
+/* "fastavro/_read.pyx":990
  * 
  * class file_reader:
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
+ *     def __init__(self, fo, reader_schema=None, options={}):             # <<<<<<<<<<<<<<
  *         self.fo = fo
- *         self.return_record_name = return_record_name
+ *         self.options = options
  */
 
+static PyObject *__pyx_pf_8fastavro_5_read_90__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__defaults__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 990, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(((PyObject *)Py_None));
+  __Pyx_GIVEREF(((PyObject *)Py_None));
+  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_None));
+  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_options);
+  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_options);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_options);
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 990, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
+  __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("fastavro._read.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* Python wrapper */
 static PyObject *__pyx_pw_8fastavro_5_read_11file_reader_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_8fastavro_5_read_11file_reader_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_11file_reader_1__init__, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_8fastavro_5_read_11file_reader_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_reader_schema = 0;
-  PyObject *__pyx_v_return_record_name = 0;
-  PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_options = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_fo,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[5] = {0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_fo,&__pyx_n_s_reader_schema,&__pyx_n_s_options,0};
+    PyObject* values[4] = {0,0,0,0};
+    __pyx_defaults *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self);
     values[2] = ((PyObject *)((PyObject *)Py_None));
-    values[3] = ((PyObject *)((PyObject *)Py_False));
-    values[4] = ((PyObject *)((PyObject *)Py_False));
+    values[3] = __pyx_dynamic_args->__pyx_arg_options;
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -16634,653 +16402,622 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, 1); __PYX_ERR(0, 1018, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, 1); __PYX_ERR(0, 990, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema);
           if (value) { values[2] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name);
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options);
           if (value) { values[3] = value; kw_args--; }
         }
-        CYTHON_FALLTHROUGH;
-        case  4:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
-          if (value) { values[4] = value; kw_args--; }
-        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1018, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 990, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_self = values[0];
     __pyx_v_fo = values[1];
     __pyx_v_reader_schema = values[2];
-    __pyx_v_return_record_name = values[3];
-    __pyx_v_return_record_name_override = values[4];
+    __pyx_v_options = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1018, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 990, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.file_reader.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_11file_reader___init__(__pyx_self, __pyx_v_self, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
+  __pyx_r = __pyx_pf_8fastavro_5_read_11file_reader___init__(__pyx_self, __pyx_v_self, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_options);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_11file_reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_11file_reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_options) {
   int __pyx_v_ignore_default_error;
   PyObject *__pyx_8genexpr1__pyx_v_k = NULL;
   PyObject *__pyx_8genexpr1__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  struct __pyx_opt_args_8fastavro_5_read__read_data __pyx_t_8;
-  int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
+  PyObject *__pyx_t_8 = NULL;
+  struct __pyx_opt_args_8fastavro_5_read__read_data __pyx_t_9;
+  int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
-  int __pyx_t_12;
-  PyObject *__pyx_t_13 = NULL;
+  Py_ssize_t __pyx_t_12;
+  int __pyx_t_13;
   int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "fastavro/_read.pyx":1019
+  /* "fastavro/_read.pyx":991
  * class file_reader:
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
+ *     def __init__(self, fo, reader_schema=None, options={}):
  *         self.fo = fo             # <<<<<<<<<<<<<<
- *         self.return_record_name = return_record_name
- *         self.return_record_name_override= return_record_name_override
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_fo, __pyx_v_fo) < 0) __PYX_ERR(0, 1019, __pyx_L1_error)
-
-  /* "fastavro/_read.pyx":1020
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
- *         self.fo = fo
- *         self.return_record_name = return_record_name             # <<<<<<<<<<<<<<
- *         self.return_record_name_override= return_record_name_override
+ *         self.options = options
  *         try:
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_return_record_name, __pyx_v_return_record_name) < 0) __PYX_ERR(0, 1020, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_fo, __pyx_v_fo) < 0) __PYX_ERR(0, 991, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1021
+  /* "fastavro/_read.pyx":992
+ *     def __init__(self, fo, reader_schema=None, options={}):
  *         self.fo = fo
- *         self.return_record_name = return_record_name
- *         self.return_record_name_override= return_record_name_override             # <<<<<<<<<<<<<<
+ *         self.options = options             # <<<<<<<<<<<<<<
  *         try:
- *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None,
+ *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None, self.options)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_return_record_name_override, __pyx_v_return_record_name_override) < 0) __PYX_ERR(0, 1021, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_options, __pyx_v_options) < 0) __PYX_ERR(0, 992, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1022
- *         self.return_record_name = return_record_name
- *         self.return_record_name_override= return_record_name_override
+  /* "fastavro/_read.pyx":993
+ *         self.fo = fo
+ *         self.options = options
  *         try:             # <<<<<<<<<<<<<<
- *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None,
- *                                       return_record_name, return_record_name_override)
+ *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None, self.options)
+ *         except (StopIteration, EOFError):
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "fastavro/_read.pyx":1023
- *         self.return_record_name_override= return_record_name_override
+      /* "fastavro/_read.pyx":994
+ *         self.options = options
  *         try:
- *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None,             # <<<<<<<<<<<<<<
- *                                       return_record_name, return_record_name_override)
+ *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None, self.options)             # <<<<<<<<<<<<<<
  *         except (StopIteration, EOFError):
+ *             raise ValueError("cannot read header - is it an avro file?")
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fo); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1023, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fo); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 994, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_HEADER_SCHEMA); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1023, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_HEADER_SCHEMA); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 994, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1023, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 994, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
-
-      /* "fastavro/_read.pyx":1024
- *         try:
- *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None,
- *                                       return_record_name, return_record_name_override)             # <<<<<<<<<<<<<<
- *         except (StopIteration, EOFError):
- *             raise ValueError("cannot read header - is it an avro file?")
- */
-      __pyx_t_8.__pyx_n = 3;
-      __pyx_t_8.reader_schema = Py_None;
-      __pyx_t_8.return_record_name = __pyx_v_return_record_name;
-      __pyx_t_8.return_record_name_override = __pyx_v_return_record_name_override;
-      __pyx_t_7 = __pyx_f_8fastavro_5_read__read_data(__pyx_t_4, __pyx_t_5, __pyx_t_6, 0, &__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1023, __pyx_L3_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_options); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 994, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_9.__pyx_n = 2;
+      __pyx_t_9.reader_schema = Py_None;
+      __pyx_t_9.options = __pyx_t_7;
+      __pyx_t_8 = __pyx_f_8fastavro_5_read__read_data(__pyx_t_4, __pyx_t_5, __pyx_t_6, 0, &__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 994, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-
-      /* "fastavro/_read.pyx":1023
- *         self.return_record_name_override= return_record_name_override
- *         try:
- *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None,             # <<<<<<<<<<<<<<
- *                                       return_record_name, return_record_name_override)
- *         except (StopIteration, EOFError):
- */
-      if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_header_2, __pyx_t_7) < 0) __PYX_ERR(0, 1023, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_header_2, __pyx_t_8) < 0) __PYX_ERR(0, 994, __pyx_L3_error)
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "fastavro/_read.pyx":1022
- *         self.return_record_name = return_record_name
- *         self.return_record_name_override= return_record_name_override
+      /* "fastavro/_read.pyx":993
+ *         self.fo = fo
+ *         self.options = options
  *         try:             # <<<<<<<<<<<<<<
- *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None,
- *                                       return_record_name, return_record_name_override)
+ *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None, self.options)
+ *         except (StopIteration, EOFError):
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "fastavro/_read.pyx":1025
- *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None,
- *                                       return_record_name, return_record_name_override)
+    /* "fastavro/_read.pyx":995
+ *         try:
+ *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None, self.options)
  *         except (StopIteration, EOFError):             # <<<<<<<<<<<<<<
  *             raise ValueError("cannot read header - is it an avro file?")
  * 
  */
-    __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_StopIteration) || __Pyx_PyErr_ExceptionMatches(__pyx_builtin_EOFError);
-    if (__pyx_t_9) {
+    __pyx_t_10 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_StopIteration) || __Pyx_PyErr_ExceptionMatches(__pyx_builtin_EOFError);
+    if (__pyx_t_10) {
       __Pyx_AddTraceback("fastavro._read.file_reader.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_6, &__pyx_t_5) < 0) __PYX_ERR(0, 1025, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_7, &__pyx_t_6) < 0) __PYX_ERR(0, 995, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_5);
 
-      /* "fastavro/_read.pyx":1026
- *                                       return_record_name, return_record_name_override)
+      /* "fastavro/_read.pyx":996
+ *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None, self.options)
  *         except (StopIteration, EOFError):
  *             raise ValueError("cannot read header - is it an avro file?")             # <<<<<<<<<<<<<<
  * 
  *         # `meta` values are bytes. So, the actual decoding has to be external.
  */
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1026, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 1026, __pyx_L5_except_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 996, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_Raise(__pyx_t_5, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __PYX_ERR(0, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "fastavro/_read.pyx":1022
- *         self.return_record_name = return_record_name
- *         self.return_record_name_override= return_record_name_override
+    /* "fastavro/_read.pyx":993
+ *         self.fo = fo
+ *         self.options = options
  *         try:             # <<<<<<<<<<<<<<
- *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None,
- *                                       return_record_name, return_record_name_override)
+ *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None, self.options)
+ *         except (StopIteration, EOFError):
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "fastavro/_read.pyx":1029
+  /* "fastavro/_read.pyx":999
  * 
  *         # `meta` values are bytes. So, the actual decoding has to be external.
  *         self.metadata = {             # <<<<<<<<<<<<<<
  *             k: v.decode() for k, v in self._header["meta"].items()
  *         }
  */
   { /* enter inner scope */
-    __pyx_t_5 = PyDict_New(); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1029, __pyx_L13_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = PyDict_New(); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 999, __pyx_L13_error)
+    __Pyx_GOTREF(__pyx_t_6);
 
-    /* "fastavro/_read.pyx":1030
+    /* "fastavro/_read.pyx":1000
  *         # `meta` values are bytes. So, the actual decoding has to be external.
  *         self.metadata = {
  *             k: v.decode() for k, v in self._header["meta"].items()             # <<<<<<<<<<<<<<
  *         }
  * 
  */
-    __pyx_t_10 = 0;
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_header_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1030, __pyx_L13_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_meta); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1030, __pyx_L13_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(__pyx_t_4 == Py_None)) {
+    __pyx_t_11 = 0;
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_header_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1000, __pyx_L13_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_8, __pyx_n_u_meta); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1000, __pyx_L13_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(__pyx_t_5 == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 1030, __pyx_L13_error)
+      __PYX_ERR(0, 1000, __pyx_L13_error)
     }
-    __pyx_t_7 = __Pyx_dict_iterator(__pyx_t_4, 0, __pyx_n_s_items, (&__pyx_t_11), (&__pyx_t_9)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1030, __pyx_L13_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_XDECREF(__pyx_t_6);
-    __pyx_t_6 = __pyx_t_7;
-    __pyx_t_7 = 0;
+    __pyx_t_8 = __Pyx_dict_iterator(__pyx_t_5, 0, __pyx_n_s_items, (&__pyx_t_12), (&__pyx_t_10)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1000, __pyx_L13_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF(__pyx_t_7);
+    __pyx_t_7 = __pyx_t_8;
+    __pyx_t_8 = 0;
     while (1) {
-      __pyx_t_12 = __Pyx_dict_iter_next(__pyx_t_6, __pyx_t_11, &__pyx_t_10, &__pyx_t_7, &__pyx_t_4, NULL, __pyx_t_9);
-      if (unlikely(__pyx_t_12 == 0)) break;
-      if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 1030, __pyx_L13_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_k, __pyx_t_7);
-      __pyx_t_7 = 0;
-      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_v, __pyx_t_4);
-      __pyx_t_4 = 0;
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_v, __pyx_n_s_decode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1030, __pyx_L13_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_13 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-        __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_7);
-        if (likely(__pyx_t_13)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-          __Pyx_INCREF(__pyx_t_13);
+      __pyx_t_13 = __Pyx_dict_iter_next(__pyx_t_7, __pyx_t_12, &__pyx_t_11, &__pyx_t_8, &__pyx_t_5, NULL, __pyx_t_10);
+      if (unlikely(__pyx_t_13 == 0)) break;
+      if (unlikely(__pyx_t_13 == -1)) __PYX_ERR(0, 1000, __pyx_L13_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_k, __pyx_t_8);
+      __pyx_t_8 = 0;
+      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_v, __pyx_t_5);
+      __pyx_t_5 = 0;
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_v, __pyx_n_s_decode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1000, __pyx_L13_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_4 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_8);
+        if (likely(__pyx_t_4)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+          __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_7, function);
+          __Pyx_DECREF_SET(__pyx_t_8, function);
         }
       }
-      __pyx_t_4 = (__pyx_t_13) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_13) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
-      __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1030, __pyx_L13_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(PyDict_SetItem(__pyx_t_5, (PyObject*)__pyx_8genexpr1__pyx_v_k, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 1030, __pyx_L13_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1000, __pyx_L13_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      if (unlikely(PyDict_SetItem(__pyx_t_6, (PyObject*)__pyx_8genexpr1__pyx_v_k, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 1000, __pyx_L13_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_k); __pyx_8genexpr1__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
     goto __pyx_L16_exit_scope;
     __pyx_L13_error:;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_k); __pyx_8genexpr1__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L16_exit_scope:;
   } /* exit inner scope */
 
-  /* "fastavro/_read.pyx":1029
+  /* "fastavro/_read.pyx":999
  * 
  *         # `meta` values are bytes. So, the actual decoding has to be external.
  *         self.metadata = {             # <<<<<<<<<<<<<<
  *             k: v.decode() for k, v in self._header["meta"].items()
  *         }
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_metadata, __pyx_t_5) < 0) __PYX_ERR(0, 1029, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_metadata, __pyx_t_6) < 0) __PYX_ERR(0, 999, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "fastavro/_read.pyx":1033
+  /* "fastavro/_read.pyx":1003
  *         }
  * 
  *         self._schema = json.loads(self.metadata["avro.schema"])             # <<<<<<<<<<<<<<
  *         self.codec = self.metadata.get("avro.codec", "null")
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_json); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1033, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_loads); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1033, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_metadata); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1033, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_6, __pyx_kp_u_avro_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1033, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_json); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1003, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_6);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_loads); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1003, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_metadata); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1003, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_kp_u_avro_schema); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1003, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_7)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1033, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_schema, __pyx_t_5) < 0) __PYX_ERR(0, 1033, __pyx_L1_error)
+  __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1003, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_schema, __pyx_t_6) < 0) __PYX_ERR(0, 1003, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "fastavro/_read.pyx":1034
+  /* "fastavro/_read.pyx":1004
  * 
  *         self._schema = json.loads(self.metadata["avro.schema"])
  *         self.codec = self.metadata.get("avro.codec", "null")             # <<<<<<<<<<<<<<
  * 
  *         self._named_schemas = {"writer": {}, "reader": {}}
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_metadata); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1034, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1034, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1034, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_metadata); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1004, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1004, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_codec, __pyx_t_5) < 0) __PYX_ERR(0, 1034, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1004, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_codec, __pyx_t_6) < 0) __PYX_ERR(0, 1004, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "fastavro/_read.pyx":1036
+  /* "fastavro/_read.pyx":1006
  *         self.codec = self.metadata.get("avro.codec", "null")
  * 
  *         self._named_schemas = {"writer": {}, "reader": {}}             # <<<<<<<<<<<<<<
  *         if reader_schema:
  *             self.reader_schema = parse_schema(
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1036, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1006, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1006, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1036, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_writer, __pyx_t_4) < 0) __PYX_ERR(0, 1036, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1036, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_reader, __pyx_t_4) < 0) __PYX_ERR(0, 1036, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2, __pyx_t_5) < 0) __PYX_ERR(0, 1036, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_writer, __pyx_t_5) < 0) __PYX_ERR(0, 1006, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1006, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_reader, __pyx_t_5) < 0) __PYX_ERR(0, 1006, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2, __pyx_t_6) < 0) __PYX_ERR(0, 1006, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "fastavro/_read.pyx":1037
+  /* "fastavro/_read.pyx":1007
  * 
  *         self._named_schemas = {"writer": {}, "reader": {}}
  *         if reader_schema:             # <<<<<<<<<<<<<<
  *             self.reader_schema = parse_schema(
  *                 reader_schema, self._named_schemas["reader"], _write_hint=False
  */
-  __pyx_t_14 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_14 < 0)) __PYX_ERR(0, 1037, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_14 < 0)) __PYX_ERR(0, 1007, __pyx_L1_error)
   if (__pyx_t_14) {
 
-    /* "fastavro/_read.pyx":1038
+    /* "fastavro/_read.pyx":1008
  *         self._named_schemas = {"writer": {}, "reader": {}}
  *         if reader_schema:
  *             self.reader_schema = parse_schema(             # <<<<<<<<<<<<<<
  *                 reader_schema, self._named_schemas["reader"], _write_hint=False
  *             )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_parse_schema); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1038, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_parse_schema); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1008, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
 
-    /* "fastavro/_read.pyx":1039
+    /* "fastavro/_read.pyx":1009
  *         if reader_schema:
  *             self.reader_schema = parse_schema(
  *                 reader_schema, self._named_schemas["reader"], _write_hint=False             # <<<<<<<<<<<<<<
  *             )
  *             # Older avro files created before we were more strict about
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1039, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_reader); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1039, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1009, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_reader); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1009, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "fastavro/_read.pyx":1038
+    /* "fastavro/_read.pyx":1008
  *         self._named_schemas = {"writer": {}, "reader": {}}
  *         if reader_schema:
  *             self.reader_schema = parse_schema(             # <<<<<<<<<<<<<<
  *                 reader_schema, self._named_schemas["reader"], _write_hint=False
  *             )
  */
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1038, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1008, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_reader_schema);
     __Pyx_GIVEREF(__pyx_v_reader_schema);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_reader_schema);
-    __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
-    __pyx_t_7 = 0;
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_reader_schema);
+    __Pyx_GIVEREF(__pyx_t_8);
+    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_8);
+    __pyx_t_8 = 0;
 
-    /* "fastavro/_read.pyx":1039
+    /* "fastavro/_read.pyx":1009
  *         if reader_schema:
  *             self.reader_schema = parse_schema(
  *                 reader_schema, self._named_schemas["reader"], _write_hint=False             # <<<<<<<<<<<<<<
  *             )
  *             # Older avro files created before we were more strict about
  */
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1039, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_write_hint, Py_False) < 0) __PYX_ERR(0, 1039, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1009, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_write_hint, Py_False) < 0) __PYX_ERR(0, 1009, __pyx_L1_error)
 
-    /* "fastavro/_read.pyx":1038
+    /* "fastavro/_read.pyx":1008
  *         self._named_schemas = {"writer": {}, "reader": {}}
  *         if reader_schema:
  *             self.reader_schema = parse_schema(             # <<<<<<<<<<<<<<
  *                 reader_schema, self._named_schemas["reader"], _write_hint=False
  *             )
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1038, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1008, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_reader_schema, __pyx_t_7) < 0) __PYX_ERR(0, 1008, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_reader_schema, __pyx_t_6) < 0) __PYX_ERR(0, 1038, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "fastavro/_read.pyx":1046
+    /* "fastavro/_read.pyx":1016
  *             # provides a reader schema that passes parsing, we will ignore those
  *             # default errors
  *             ignore_default_error = True             # <<<<<<<<<<<<<<
  *         else:
  *             self.reader_schema = None
  */
     __pyx_v_ignore_default_error = 1;
 
-    /* "fastavro/_read.pyx":1037
+    /* "fastavro/_read.pyx":1007
  * 
  *         self._named_schemas = {"writer": {}, "reader": {}}
  *         if reader_schema:             # <<<<<<<<<<<<<<
  *             self.reader_schema = parse_schema(
  *                 reader_schema, self._named_schemas["reader"], _write_hint=False
  */
     goto __pyx_L17;
   }
 
-  /* "fastavro/_read.pyx":1048
+  /* "fastavro/_read.pyx":1018
  *             ignore_default_error = True
  *         else:
  *             self.reader_schema = None             # <<<<<<<<<<<<<<
  *             ignore_default_error = False
  * 
  */
   /*else*/ {
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_reader_schema, Py_None) < 0) __PYX_ERR(0, 1048, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_reader_schema, Py_None) < 0) __PYX_ERR(0, 1018, __pyx_L1_error)
 
-    /* "fastavro/_read.pyx":1049
+    /* "fastavro/_read.pyx":1019
  *         else:
  *             self.reader_schema = None
  *             ignore_default_error = False             # <<<<<<<<<<<<<<
  * 
  *         self.writer_schema = parse_schema(
  */
     __pyx_v_ignore_default_error = 0;
   }
   __pyx_L17:;
 
-  /* "fastavro/_read.pyx":1051
+  /* "fastavro/_read.pyx":1021
  *             ignore_default_error = False
  * 
  *         self.writer_schema = parse_schema(             # <<<<<<<<<<<<<<
  *             self._schema,
  *             self._named_schemas["writer"],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_parse_schema); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1051, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_parse_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1021, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
 
-  /* "fastavro/_read.pyx":1052
+  /* "fastavro/_read.pyx":1022
  * 
  *         self.writer_schema = parse_schema(
  *             self._schema,             # <<<<<<<<<<<<<<
  *             self._named_schemas["writer"],
  *             _write_hint=False,
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1052, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_schema); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1022, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
 
-  /* "fastavro/_read.pyx":1053
+  /* "fastavro/_read.pyx":1023
  *         self.writer_schema = parse_schema(
  *             self._schema,
  *             self._named_schemas["writer"],             # <<<<<<<<<<<<<<
  *             _write_hint=False,
  *             _force=True,
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1053, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_writer); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1053, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1023, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_writer); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1023, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "fastavro/_read.pyx":1051
+  /* "fastavro/_read.pyx":1021
  *             ignore_default_error = False
  * 
  *         self.writer_schema = parse_schema(             # <<<<<<<<<<<<<<
  *             self._schema,
  *             self._named_schemas["writer"],
  */
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1051, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5);
-  __pyx_t_7 = 0;
-  __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1021, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_6);
+  __pyx_t_8 = 0;
+  __pyx_t_6 = 0;
 
-  /* "fastavro/_read.pyx":1054
+  /* "fastavro/_read.pyx":1024
  *             self._schema,
  *             self._named_schemas["writer"],
  *             _write_hint=False,             # <<<<<<<<<<<<<<
  *             _force=True,
  *             _ignore_default_error=ignore_default_error,
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1054, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_write_hint, Py_False) < 0) __PYX_ERR(0, 1054, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1024, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_write_hint, Py_False) < 0) __PYX_ERR(0, 1024, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1055
+  /* "fastavro/_read.pyx":1025
  *             self._named_schemas["writer"],
  *             _write_hint=False,
  *             _force=True,             # <<<<<<<<<<<<<<
  *             _ignore_default_error=ignore_default_error,
  *         )
  */
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 1054, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 1024, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1056
+  /* "fastavro/_read.pyx":1026
  *             _write_hint=False,
  *             _force=True,
  *             _ignore_default_error=ignore_default_error,             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_ignore_default_error); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1056, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_ignore_default_error, __pyx_t_7) < 0) __PYX_ERR(0, 1054, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_8 = __Pyx_PyBool_FromLong(__pyx_v_ignore_default_error); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1026, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_ignore_default_error, __pyx_t_8) < 0) __PYX_ERR(0, 1024, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "fastavro/_read.pyx":1051
+  /* "fastavro/_read.pyx":1021
  *             ignore_default_error = False
  * 
  *         self.writer_schema = parse_schema(             # <<<<<<<<<<<<<<
  *             self._schema,
  *             self._named_schemas["writer"],
  */
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1051, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_writer_schema, __pyx_t_7) < 0) __PYX_ERR(0, 1051, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1021, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_writer_schema, __pyx_t_8) < 0) __PYX_ERR(0, 1021, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "fastavro/_read.pyx":1059
+  /* "fastavro/_read.pyx":1029
  *         )
  * 
  *         self._elems = None             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_elems, Py_None) < 0) __PYX_ERR(0, 1059, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_elems, Py_None) < 0) __PYX_ERR(0, 1029, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1018
+  /* "fastavro/_read.pyx":990
  * 
  * class file_reader:
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
+ *     def __init__(self, fo, reader_schema=None, options={}):             # <<<<<<<<<<<<<<
  *         self.fo = fo
- *         self.return_record_name = return_record_name
+ *         self.options = options
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_13);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("fastavro._read.file_reader.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_k);
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":1062
+/* "fastavro/_read.pyx":1032
  * 
  *     @property
  *     def schema(self):             # <<<<<<<<<<<<<<
  *         import warnings
  *         warnings.warn(
  */
 
@@ -17305,63 +17042,63 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("schema", 0);
 
-  /* "fastavro/_read.pyx":1063
+  /* "fastavro/_read.pyx":1033
  *     @property
  *     def schema(self):
  *         import warnings             # <<<<<<<<<<<<<<
  *         warnings.warn(
  *             "The 'schema' attribute is deprecated. Please use 'writer_schema'",
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_warnings, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1063, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_warnings, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1033, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_warnings = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":1064
+  /* "fastavro/_read.pyx":1034
  *     def schema(self):
  *         import warnings
  *         warnings.warn(             # <<<<<<<<<<<<<<
  *             "The 'schema' attribute is deprecated. Please use 'writer_schema'",
  *             DeprecationWarning,
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_warnings, __pyx_n_s_warn); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1064, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_warnings, __pyx_n_s_warn); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1034, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "fastavro/_read.pyx":1066
+  /* "fastavro/_read.pyx":1036
  *         warnings.warn(
  *             "The 'schema' attribute is deprecated. Please use 'writer_schema'",
  *             DeprecationWarning,             # <<<<<<<<<<<<<<
  *         )
  *         return self._schema
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1064, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1034, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":1068
+  /* "fastavro/_read.pyx":1038
  *             DeprecationWarning,
  *         )
  *         return self._schema             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_schema); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1068, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_schema); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1038, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":1062
+  /* "fastavro/_read.pyx":1032
  * 
  *     @property
  *     def schema(self):             # <<<<<<<<<<<<<<
  *         import warnings
  *         warnings.warn(
  */
 
@@ -17374,15 +17111,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_warnings);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":1070
+/* "fastavro/_read.pyx":1040
  *         return self._schema
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         if not self._elems:
  *             raise NotImplementedError
  */
 
@@ -17407,62 +17144,62 @@
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "fastavro/_read.pyx":1071
+  /* "fastavro/_read.pyx":1041
  * 
  *     def __iter__(self):
  *         if not self._elems:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError
  *         return self._elems
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_elems); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1071, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_elems); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1041, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1071, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1041, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = ((!__pyx_t_2) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "fastavro/_read.pyx":1072
+    /* "fastavro/_read.pyx":1042
  *     def __iter__(self):
  *         if not self._elems:
  *             raise NotImplementedError             # <<<<<<<<<<<<<<
  *         return self._elems
  * 
  */
     __Pyx_Raise(__pyx_builtin_NotImplementedError, 0, 0, 0);
-    __PYX_ERR(0, 1072, __pyx_L1_error)
+    __PYX_ERR(0, 1042, __pyx_L1_error)
 
-    /* "fastavro/_read.pyx":1071
+    /* "fastavro/_read.pyx":1041
  * 
  *     def __iter__(self):
  *         if not self._elems:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError
  *         return self._elems
  */
   }
 
-  /* "fastavro/_read.pyx":1073
+  /* "fastavro/_read.pyx":1043
  *         if not self._elems:
  *             raise NotImplementedError
  *         return self._elems             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_elems); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1073, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_elems); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1043, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":1070
+  /* "fastavro/_read.pyx":1040
  *         return self._schema
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         if not self._elems:
  *             raise NotImplementedError
  */
 
@@ -17473,15 +17210,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":1075
+/* "fastavro/_read.pyx":1045
  *         return self._elems
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         return next(self._elems)
  * 
  */
 
@@ -17505,32 +17242,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__next__", 0);
 
-  /* "fastavro/_read.pyx":1076
+  /* "fastavro/_read.pyx":1046
  * 
  *     def __next__(self):
  *         return next(self._elems)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_elems); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1076, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_elems); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1046, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyIter_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1076, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyIter_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1046, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":1075
+  /* "fastavro/_read.pyx":1045
  *         return self._elems
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         return next(self._elems)
  * 
  */
 
@@ -17542,47 +17279,75 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":1080
+/* "fastavro/_read.pyx":1050
  * 
  * class reader(file_reader):
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
- * 
+ *     def __init__(             # <<<<<<<<<<<<<<
+ *         self,
+ *         fo,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8fastavro_5_read_6reader_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_8fastavro_5_read_6reader_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_6reader_1__init__, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_8fastavro_5_read_6reader_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_reader_schema = 0;
   PyObject *__pyx_v_return_record_name = 0;
   PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_handle_unicode_errors = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_fo,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[5] = {0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_fo,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,&__pyx_n_s_handle_unicode_errors,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
+
+    /* "fastavro/_read.pyx":1053
+ *         self,
+ *         fo,
+ *         reader_schema=None,             # <<<<<<<<<<<<<<
+ *         return_record_name=False,
+ *         return_record_name_override=False,
+ */
     values[2] = ((PyObject *)((PyObject *)Py_None));
+
+    /* "fastavro/_read.pyx":1054
+ *         fo,
+ *         reader_schema=None,
+ *         return_record_name=False,             # <<<<<<<<<<<<<<
+ *         return_record_name_override=False,
+ *         handle_unicode_errors="strict",
+ */
     values[3] = ((PyObject *)((PyObject *)Py_False));
+
+    /* "fastavro/_read.pyx":1055
+ *         reader_schema=None,
+ *         return_record_name=False,
+ *         return_record_name_override=False,             # <<<<<<<<<<<<<<
+ *         handle_unicode_errors="strict",
+ *     ):
+ */
     values[4] = ((PyObject *)((PyObject *)Py_False));
+    values[5] = ((PyObject *)((PyObject*)__pyx_n_u_strict));
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -17597,15 +17362,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, 1); __PYX_ERR(0, 1080, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 6, 1); __PYX_ERR(0, 1050, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -17617,20 +17382,28 @@
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
           if (value) { values[4] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_handle_unicode_errors);
+          if (value) { values[5] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1080, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1050, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -17640,73 +17413,113 @@
       }
     }
     __pyx_v_self = values[0];
     __pyx_v_fo = values[1];
     __pyx_v_reader_schema = values[2];
     __pyx_v_return_record_name = values[3];
     __pyx_v_return_record_name_override = values[4];
+    __pyx_v_handle_unicode_errors = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1080, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1050, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.reader.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_6reader___init__(__pyx_self, __pyx_v_self, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
+  __pyx_r = __pyx_pf_8fastavro_5_read_6reader___init__(__pyx_self, __pyx_v_self, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override, __pyx_v_handle_unicode_errors);
+
+  /* "fastavro/_read.pyx":1050
+ * 
+ * class reader(file_reader):
+ *     def __init__(             # <<<<<<<<<<<<<<
+ *         self,
+ *         fo,
+ */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_6reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_6reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override, PyObject *__pyx_v_handle_unicode_errors) {
+  PyObject *__pyx_v_options = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
-  PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "fastavro/_read.pyx":1081
- * class reader(file_reader):
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)             # <<<<<<<<<<<<<<
+  /* "fastavro/_read.pyx":1059
+ *     ):
+ *         options = {
+ *             "return_record_name": return_record_name,             # <<<<<<<<<<<<<<
+ *             "return_record_name_override": return_record_name_override,
+ *             "handle_unicode_errors": handle_unicode_errors,
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1059, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_return_record_name, __pyx_v_return_record_name) < 0) __PYX_ERR(0, 1059, __pyx_L1_error)
+
+  /* "fastavro/_read.pyx":1060
+ *         options = {
+ *             "return_record_name": return_record_name,
+ *             "return_record_name_override": return_record_name_override,             # <<<<<<<<<<<<<<
+ *             "handle_unicode_errors": handle_unicode_errors,
+ *         }
+ */
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_return_record_name_override, __pyx_v_return_record_name_override) < 0) __PYX_ERR(0, 1059, __pyx_L1_error)
+
+  /* "fastavro/_read.pyx":1061
+ *             "return_record_name": return_record_name,
+ *             "return_record_name_override": return_record_name_override,
+ *             "handle_unicode_errors": handle_unicode_errors,             # <<<<<<<<<<<<<<
+ *         }
+ *         super().__init__(fo, reader_schema, options)
+ */
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_handle_unicode_errors, __pyx_v_handle_unicode_errors) < 0) __PYX_ERR(0, 1059, __pyx_L1_error)
+  __pyx_v_options = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "fastavro/_read.pyx":1063
+ *             "handle_unicode_errors": handle_unicode_errors,
+ *         }
+ *         super().__init__(fo, reader_schema, options)             # <<<<<<<<<<<<<<
  * 
  *         self._elems = _iter_avro_records(self.fo,
  */
   __pyx_t_2 = __Pyx_CyFunction_GetClassObj(__pyx_self);
-  if (!__pyx_t_2) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 1081, __pyx_L1_error) }
+  if (!__pyx_t_2) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 1063, __pyx_L1_error) }
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1081, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1063, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_INCREF(__pyx_v_self);
   __Pyx_GIVEREF(__pyx_v_self);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_self);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1081, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1063, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1081, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1063, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -17715,230 +17528,212 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_2, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 4+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1081, __pyx_L1_error)
+    PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_options};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1063, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_2, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 4+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1081, __pyx_L1_error)
+    PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_options};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1063, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(4+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1081, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1063, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_v_fo);
     __Pyx_GIVEREF(__pyx_v_fo);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_fo);
     __Pyx_INCREF(__pyx_v_reader_schema);
     __Pyx_GIVEREF(__pyx_v_reader_schema);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_reader_schema);
-    __Pyx_INCREF(__pyx_v_return_record_name);
-    __Pyx_GIVEREF(__pyx_v_return_record_name);
-    PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_4, __pyx_v_return_record_name);
-    __Pyx_INCREF(__pyx_v_return_record_name_override);
-    __Pyx_GIVEREF(__pyx_v_return_record_name_override);
-    PyTuple_SET_ITEM(__pyx_t_5, 3+__pyx_t_4, __pyx_v_return_record_name_override);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1081, __pyx_L1_error)
+    __Pyx_INCREF(__pyx_v_options);
+    __Pyx_GIVEREF(__pyx_v_options);
+    PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_4, __pyx_v_options);
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1063, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":1083
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
+  /* "fastavro/_read.pyx":1065
+ *         super().__init__(fo, reader_schema, options)
  * 
  *         self._elems = _iter_avro_records(self.fo,             # <<<<<<<<<<<<<<
  *                                          self._header,
  *                                          self.codec,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_iter_avro_records); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1083, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_iter_avro_records); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1065, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fo); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1083, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fo); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1065, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "fastavro/_read.pyx":1084
+  /* "fastavro/_read.pyx":1066
  * 
  *         self._elems = _iter_avro_records(self.fo,
  *                                          self._header,             # <<<<<<<<<<<<<<
  *                                          self.codec,
  *                                          self.writer_schema,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_header_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1084, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_header_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1066, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "fastavro/_read.pyx":1085
+  /* "fastavro/_read.pyx":1067
  *         self._elems = _iter_avro_records(self.fo,
  *                                          self._header,
  *                                          self.codec,             # <<<<<<<<<<<<<<
  *                                          self.writer_schema,
  *                                          self._named_schemas,
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_codec); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1085, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_codec); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1067, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "fastavro/_read.pyx":1086
+  /* "fastavro/_read.pyx":1068
  *                                          self._header,
  *                                          self.codec,
  *                                          self.writer_schema,             # <<<<<<<<<<<<<<
  *                                          self._named_schemas,
  *                                          self.reader_schema,
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_writer_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1086, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_writer_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1068, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
 
-  /* "fastavro/_read.pyx":1087
+  /* "fastavro/_read.pyx":1069
  *                                          self.codec,
  *                                          self.writer_schema,
  *                                          self._named_schemas,             # <<<<<<<<<<<<<<
  *                                          self.reader_schema,
- *                                          self.return_record_name,
+ *                                          self.options)
  */
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1087, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1069, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
 
-  /* "fastavro/_read.pyx":1088
+  /* "fastavro/_read.pyx":1070
  *                                          self.writer_schema,
  *                                          self._named_schemas,
  *                                          self.reader_schema,             # <<<<<<<<<<<<<<
- *                                          self.return_record_name,
- *                                          self.return_record_name_override)
+ *                                          self.options)
+ * 
  */
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_reader_schema); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1088, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_reader_schema); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1070, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
 
-  /* "fastavro/_read.pyx":1089
+  /* "fastavro/_read.pyx":1071
  *                                          self._named_schemas,
  *                                          self.reader_schema,
- *                                          self.return_record_name,             # <<<<<<<<<<<<<<
- *                                          self.return_record_name_override)
- * 
- */
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_return_record_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1089, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-
-  /* "fastavro/_read.pyx":1090
- *                                          self.reader_schema,
- *                                          self.return_record_name,
- *                                          self.return_record_name_override)             # <<<<<<<<<<<<<<
+ *                                          self.options)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_return_record_name_override); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1090, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_12 = NULL;
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_options); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1071, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_11 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_12)) {
+    __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_12);
+      __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[9] = {__pyx_t_12, __pyx_t_5, __pyx_t_2, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 8+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1083, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+    PyObject *__pyx_temp[8] = {__pyx_t_11, __pyx_t_5, __pyx_t_2, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 7+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1065, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[9] = {__pyx_t_12, __pyx_t_5, __pyx_t_2, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 8+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1083, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+    PyObject *__pyx_temp[8] = {__pyx_t_11, __pyx_t_5, __pyx_t_2, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 7+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1065, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   {
-    __pyx_t_13 = PyTuple_New(8+__pyx_t_4); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1083, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_13);
-    if (__pyx_t_12) {
-      __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_12); __pyx_t_12 = NULL;
+    __pyx_t_12 = PyTuple_New(7+__pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1065, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    if (__pyx_t_11) {
+      __Pyx_GIVEREF(__pyx_t_11); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_11); __pyx_t_11 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_4, __pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_4, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_13, 1+__pyx_t_4, __pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_4, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_13, 2+__pyx_t_4, __pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_4, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_13, 3+__pyx_t_4, __pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_12, 3+__pyx_t_4, __pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_13, 4+__pyx_t_4, __pyx_t_8);
+    PyTuple_SET_ITEM(__pyx_t_12, 4+__pyx_t_4, __pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_9);
-    PyTuple_SET_ITEM(__pyx_t_13, 5+__pyx_t_4, __pyx_t_9);
+    PyTuple_SET_ITEM(__pyx_t_12, 5+__pyx_t_4, __pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_13, 6+__pyx_t_4, __pyx_t_10);
-    __Pyx_GIVEREF(__pyx_t_11);
-    PyTuple_SET_ITEM(__pyx_t_13, 7+__pyx_t_4, __pyx_t_11);
+    PyTuple_SET_ITEM(__pyx_t_12, 6+__pyx_t_4, __pyx_t_10);
     __pyx_t_5 = 0;
     __pyx_t_2 = 0;
     __pyx_t_6 = 0;
     __pyx_t_7 = 0;
     __pyx_t_8 = 0;
     __pyx_t_9 = 0;
     __pyx_t_10 = 0;
-    __pyx_t_11 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1083, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1065, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "fastavro/_read.pyx":1083
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
+  /* "fastavro/_read.pyx":1065
+ *         super().__init__(fo, reader_schema, options)
  * 
  *         self._elems = _iter_avro_records(self.fo,             # <<<<<<<<<<<<<<
  *                                          self._header,
  *                                          self.codec,
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_elems, __pyx_t_1) < 0) __PYX_ERR(0, 1083, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_elems, __pyx_t_1) < 0) __PYX_ERR(0, 1065, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":1080
+  /* "fastavro/_read.pyx":1050
  * 
  * class reader(file_reader):
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
- * 
+ *     def __init__(             # <<<<<<<<<<<<<<
+ *         self,
+ *         fo,
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -17948,56 +17743,84 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_XDECREF(__pyx_t_13);
   __Pyx_AddTraceback("fastavro._read.reader.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_options);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":1094
+/* "fastavro/_read.pyx":1075
  * 
  * class block_reader(file_reader):
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
- * 
+ *     def __init__(             # <<<<<<<<<<<<<<
+ *         self,
+ *         fo,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8fastavro_5_read_12block_reader_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_8fastavro_5_read_12block_reader_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_12block_reader_1__init__, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_8fastavro_5_read_12block_reader_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_reader_schema = 0;
   PyObject *__pyx_v_return_record_name = 0;
   PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_handle_unicode_errors = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_fo,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[5] = {0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_fo,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,&__pyx_n_s_handle_unicode_errors,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
+
+    /* "fastavro/_read.pyx":1078
+ *         self,
+ *         fo,
+ *         reader_schema=None,             # <<<<<<<<<<<<<<
+ *         return_record_name=False,
+ *         return_record_name_override=False,
+ */
     values[2] = ((PyObject *)((PyObject *)Py_None));
+
+    /* "fastavro/_read.pyx":1079
+ *         fo,
+ *         reader_schema=None,
+ *         return_record_name=False,             # <<<<<<<<<<<<<<
+ *         return_record_name_override=False,
+ *         handle_unicode_errors="strict",
+ */
     values[3] = ((PyObject *)((PyObject *)Py_False));
+
+    /* "fastavro/_read.pyx":1080
+ *         reader_schema=None,
+ *         return_record_name=False,
+ *         return_record_name_override=False,             # <<<<<<<<<<<<<<
+ *         handle_unicode_errors="strict",
+ *     ):
+ */
     values[4] = ((PyObject *)((PyObject *)Py_False));
+    values[5] = ((PyObject *)((PyObject*)__pyx_n_u_strict));
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -18012,15 +17835,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, 1); __PYX_ERR(0, 1094, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 6, 1); __PYX_ERR(0, 1075, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -18032,20 +17855,28 @@
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
           if (value) { values[4] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_handle_unicode_errors);
+          if (value) { values[5] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1094, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1075, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -18055,73 +17886,113 @@
       }
     }
     __pyx_v_self = values[0];
     __pyx_v_fo = values[1];
     __pyx_v_reader_schema = values[2];
     __pyx_v_return_record_name = values[3];
     __pyx_v_return_record_name_override = values[4];
+    __pyx_v_handle_unicode_errors = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1094, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1075, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.block_reader.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_12block_reader___init__(__pyx_self, __pyx_v_self, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
+  __pyx_r = __pyx_pf_8fastavro_5_read_12block_reader___init__(__pyx_self, __pyx_v_self, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override, __pyx_v_handle_unicode_errors);
+
+  /* "fastavro/_read.pyx":1075
+ * 
+ * class block_reader(file_reader):
+ *     def __init__(             # <<<<<<<<<<<<<<
+ *         self,
+ *         fo,
+ */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_12block_reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_12block_reader___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override, PyObject *__pyx_v_handle_unicode_errors) {
+  PyObject *__pyx_v_options = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
-  PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "fastavro/_read.pyx":1095
- * class block_reader(file_reader):
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)             # <<<<<<<<<<<<<<
+  /* "fastavro/_read.pyx":1084
+ *     ):
+ *         options = {
+ *             "return_record_name": return_record_name,             # <<<<<<<<<<<<<<
+ *             "return_record_name_override": return_record_name_override,
+ *             "handle_unicode_errors": handle_unicode_errors,
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1084, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_return_record_name, __pyx_v_return_record_name) < 0) __PYX_ERR(0, 1084, __pyx_L1_error)
+
+  /* "fastavro/_read.pyx":1085
+ *         options = {
+ *             "return_record_name": return_record_name,
+ *             "return_record_name_override": return_record_name_override,             # <<<<<<<<<<<<<<
+ *             "handle_unicode_errors": handle_unicode_errors,
+ *         }
+ */
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_return_record_name_override, __pyx_v_return_record_name_override) < 0) __PYX_ERR(0, 1084, __pyx_L1_error)
+
+  /* "fastavro/_read.pyx":1086
+ *             "return_record_name": return_record_name,
+ *             "return_record_name_override": return_record_name_override,
+ *             "handle_unicode_errors": handle_unicode_errors,             # <<<<<<<<<<<<<<
+ *         }
+ *         super().__init__(fo, reader_schema, options)
+ */
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_handle_unicode_errors, __pyx_v_handle_unicode_errors) < 0) __PYX_ERR(0, 1084, __pyx_L1_error)
+  __pyx_v_options = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "fastavro/_read.pyx":1088
+ *             "handle_unicode_errors": handle_unicode_errors,
+ *         }
+ *         super().__init__(fo, reader_schema, options)             # <<<<<<<<<<<<<<
  * 
  *         self._elems = _iter_avro_blocks(self.fo,
  */
   __pyx_t_2 = __Pyx_CyFunction_GetClassObj(__pyx_self);
-  if (!__pyx_t_2) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 1095, __pyx_L1_error) }
+  if (!__pyx_t_2) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 1088, __pyx_L1_error) }
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1095, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1088, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_INCREF(__pyx_v_self);
   __Pyx_GIVEREF(__pyx_v_self);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_self);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1095, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1088, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1095, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1088, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -18130,230 +18001,212 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_2, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 4+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1095, __pyx_L1_error)
+    PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_options};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1088, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_2, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 4+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1095, __pyx_L1_error)
+    PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_v_fo, __pyx_v_reader_schema, __pyx_v_options};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1088, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(4+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1095, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1088, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_v_fo);
     __Pyx_GIVEREF(__pyx_v_fo);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_fo);
     __Pyx_INCREF(__pyx_v_reader_schema);
     __Pyx_GIVEREF(__pyx_v_reader_schema);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_reader_schema);
-    __Pyx_INCREF(__pyx_v_return_record_name);
-    __Pyx_GIVEREF(__pyx_v_return_record_name);
-    PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_4, __pyx_v_return_record_name);
-    __Pyx_INCREF(__pyx_v_return_record_name_override);
-    __Pyx_GIVEREF(__pyx_v_return_record_name_override);
-    PyTuple_SET_ITEM(__pyx_t_5, 3+__pyx_t_4, __pyx_v_return_record_name_override);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1095, __pyx_L1_error)
+    __Pyx_INCREF(__pyx_v_options);
+    __Pyx_GIVEREF(__pyx_v_options);
+    PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_4, __pyx_v_options);
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1088, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":1097
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
+  /* "fastavro/_read.pyx":1090
+ *         super().__init__(fo, reader_schema, options)
  * 
  *         self._elems = _iter_avro_blocks(self.fo,             # <<<<<<<<<<<<<<
  *                                         self._header,
  *                                         self.codec,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_iter_avro_blocks); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1097, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_iter_avro_blocks); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1090, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fo); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1097, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fo); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1090, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "fastavro/_read.pyx":1098
+  /* "fastavro/_read.pyx":1091
  * 
  *         self._elems = _iter_avro_blocks(self.fo,
  *                                         self._header,             # <<<<<<<<<<<<<<
  *                                         self.codec,
  *                                         self.writer_schema,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_header_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1098, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_header_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "fastavro/_read.pyx":1099
+  /* "fastavro/_read.pyx":1092
  *         self._elems = _iter_avro_blocks(self.fo,
  *                                         self._header,
  *                                         self.codec,             # <<<<<<<<<<<<<<
  *                                         self.writer_schema,
  *                                         self._named_schemas,
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_codec); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1099, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_codec); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1092, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "fastavro/_read.pyx":1100
+  /* "fastavro/_read.pyx":1093
  *                                         self._header,
  *                                         self.codec,
  *                                         self.writer_schema,             # <<<<<<<<<<<<<<
  *                                         self._named_schemas,
  *                                         self.reader_schema,
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_writer_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1100, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_writer_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1093, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
 
-  /* "fastavro/_read.pyx":1101
+  /* "fastavro/_read.pyx":1094
  *                                         self.codec,
  *                                         self.writer_schema,
  *                                         self._named_schemas,             # <<<<<<<<<<<<<<
  *                                         self.reader_schema,
- *                                         self.return_record_name,
+ *                                         self.options)
  */
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1101, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_named_schemas_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
 
-  /* "fastavro/_read.pyx":1102
+  /* "fastavro/_read.pyx":1095
  *                                         self.writer_schema,
  *                                         self._named_schemas,
  *                                         self.reader_schema,             # <<<<<<<<<<<<<<
- *                                         self.return_record_name,
- *                                         self.return_record_name_override)
+ *                                         self.options)
+ * 
  */
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_reader_schema); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1102, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_reader_schema); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1095, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
 
-  /* "fastavro/_read.pyx":1103
+  /* "fastavro/_read.pyx":1096
  *                                         self._named_schemas,
  *                                         self.reader_schema,
- *                                         self.return_record_name,             # <<<<<<<<<<<<<<
- *                                         self.return_record_name_override)
- * 
- */
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_return_record_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-
-  /* "fastavro/_read.pyx":1104
- *                                         self.reader_schema,
- *                                         self.return_record_name,
- *                                         self.return_record_name_override)             # <<<<<<<<<<<<<<
+ *                                         self.options)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_return_record_name_override); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1104, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_12 = NULL;
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_options); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1096, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_11 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_12)) {
+    __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_12);
+      __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[9] = {__pyx_t_12, __pyx_t_5, __pyx_t_2, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 8+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1097, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+    PyObject *__pyx_temp[8] = {__pyx_t_11, __pyx_t_5, __pyx_t_2, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 7+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1090, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[9] = {__pyx_t_12, __pyx_t_5, __pyx_t_2, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 8+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1097, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+    PyObject *__pyx_temp[8] = {__pyx_t_11, __pyx_t_5, __pyx_t_2, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 7+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1090, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   {
-    __pyx_t_13 = PyTuple_New(8+__pyx_t_4); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1097, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_13);
-    if (__pyx_t_12) {
-      __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_12); __pyx_t_12 = NULL;
+    __pyx_t_12 = PyTuple_New(7+__pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1090, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    if (__pyx_t_11) {
+      __Pyx_GIVEREF(__pyx_t_11); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_11); __pyx_t_11 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_4, __pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_4, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_13, 1+__pyx_t_4, __pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_4, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_13, 2+__pyx_t_4, __pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_4, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_13, 3+__pyx_t_4, __pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_12, 3+__pyx_t_4, __pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_13, 4+__pyx_t_4, __pyx_t_8);
+    PyTuple_SET_ITEM(__pyx_t_12, 4+__pyx_t_4, __pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_9);
-    PyTuple_SET_ITEM(__pyx_t_13, 5+__pyx_t_4, __pyx_t_9);
+    PyTuple_SET_ITEM(__pyx_t_12, 5+__pyx_t_4, __pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_13, 6+__pyx_t_4, __pyx_t_10);
-    __Pyx_GIVEREF(__pyx_t_11);
-    PyTuple_SET_ITEM(__pyx_t_13, 7+__pyx_t_4, __pyx_t_11);
+    PyTuple_SET_ITEM(__pyx_t_12, 6+__pyx_t_4, __pyx_t_10);
     __pyx_t_5 = 0;
     __pyx_t_2 = 0;
     __pyx_t_6 = 0;
     __pyx_t_7 = 0;
     __pyx_t_8 = 0;
     __pyx_t_9 = 0;
     __pyx_t_10 = 0;
-    __pyx_t_11 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1097, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "fastavro/_read.pyx":1097
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
+  /* "fastavro/_read.pyx":1090
+ *         super().__init__(fo, reader_schema, options)
  * 
  *         self._elems = _iter_avro_blocks(self.fo,             # <<<<<<<<<<<<<<
  *                                         self._header,
  *                                         self.codec,
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_elems, __pyx_t_1) < 0) __PYX_ERR(0, 1097, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_elems, __pyx_t_1) < 0) __PYX_ERR(0, 1090, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":1094
+  /* "fastavro/_read.pyx":1075
  * 
  * class block_reader(file_reader):
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
- * 
+ *     def __init__(             # <<<<<<<<<<<<<<
+ *         self,
+ *         fo,
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -18363,53 +18216,63 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_XDECREF(__pyx_t_13);
   __Pyx_AddTraceback("fastavro._read.block_reader.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_options);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":1107
+/* "fastavro/_read.pyx":1099
  * 
  * 
- * cpdef schemaless_reader(fo, writer_schema, reader_schema=None,             # <<<<<<<<<<<<<<
- *                         return_record_name=False,
- *                         return_record_name_override=False):
+ * cpdef schemaless_reader(             # <<<<<<<<<<<<<<
+ *     fo,
+ *     writer_schema,
  */
 
 static PyObject *__pyx_pw_8fastavro_5_read_87schemaless_reader(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_8fastavro_5_read_schemaless_reader(PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_8fastavro_5_read_schemaless_reader *__pyx_optional_args) {
+
+  /* "fastavro/_read.pyx":1102
+ *     fo,
+ *     writer_schema,
+ *     reader_schema=None,             # <<<<<<<<<<<<<<
+ *     return_record_name=False,
+ *     return_record_name_override=False,
+ */
   PyObject *__pyx_v_reader_schema = ((PyObject *)Py_None);
 
-  /* "fastavro/_read.pyx":1108
- * 
- * cpdef schemaless_reader(fo, writer_schema, reader_schema=None,
- *                         return_record_name=False,             # <<<<<<<<<<<<<<
- *                         return_record_name_override=False):
- *     if writer_schema == reader_schema:
+  /* "fastavro/_read.pyx":1103
+ *     writer_schema,
+ *     reader_schema=None,
+ *     return_record_name=False,             # <<<<<<<<<<<<<<
+ *     return_record_name_override=False,
+ *     handle_unicode_errors="strict",
  */
   PyObject *__pyx_v_return_record_name = ((PyObject *)Py_False);
 
-  /* "fastavro/_read.pyx":1109
- * cpdef schemaless_reader(fo, writer_schema, reader_schema=None,
- *                         return_record_name=False,
- *                         return_record_name_override=False):             # <<<<<<<<<<<<<<
- *     if writer_schema == reader_schema:
- *         # No need for the reader schema if they are the same
+  /* "fastavro/_read.pyx":1104
+ *     reader_schema=None,
+ *     return_record_name=False,
+ *     return_record_name_override=False,             # <<<<<<<<<<<<<<
+ *     handle_unicode_errors="strict",
+ * ):
  */
   PyObject *__pyx_v_return_record_name_override = ((PyObject *)Py_False);
+  PyObject *__pyx_v_handle_unicode_errors = ((PyObject *)__pyx_n_u_strict);
   PyObject *__pyx_v_named_schemas = NULL;
+  PyObject *__pyx_v_options = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -18423,82 +18286,85 @@
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_reader_schema = __pyx_optional_args->reader_schema;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_return_record_name = __pyx_optional_args->return_record_name;
         if (__pyx_optional_args->__pyx_n > 2) {
           __pyx_v_return_record_name_override = __pyx_optional_args->return_record_name_override;
+          if (__pyx_optional_args->__pyx_n > 3) {
+            __pyx_v_handle_unicode_errors = __pyx_optional_args->handle_unicode_errors;
+          }
         }
       }
     }
   }
   __Pyx_INCREF(__pyx_v_writer_schema);
   __Pyx_INCREF(__pyx_v_reader_schema);
 
-  /* "fastavro/_read.pyx":1110
- *                         return_record_name=False,
- *                         return_record_name_override=False):
+  /* "fastavro/_read.pyx":1107
+ *     handle_unicode_errors="strict",
+ * ):
  *     if writer_schema == reader_schema:             # <<<<<<<<<<<<<<
  *         # No need for the reader schema if they are the same
  *         reader_schema = None
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_writer_schema, __pyx_v_reader_schema, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1110, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1110, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_writer_schema, __pyx_v_reader_schema, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1107, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1107, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "fastavro/_read.pyx":1112
+    /* "fastavro/_read.pyx":1109
  *     if writer_schema == reader_schema:
  *         # No need for the reader schema if they are the same
  *         reader_schema = None             # <<<<<<<<<<<<<<
  * 
  *     named_schemas = {"writer": {}, "reader": {}}
  */
     __Pyx_INCREF(Py_None);
     __Pyx_DECREF_SET(__pyx_v_reader_schema, Py_None);
 
-    /* "fastavro/_read.pyx":1110
- *                         return_record_name=False,
- *                         return_record_name_override=False):
+    /* "fastavro/_read.pyx":1107
+ *     handle_unicode_errors="strict",
+ * ):
  *     if writer_schema == reader_schema:             # <<<<<<<<<<<<<<
  *         # No need for the reader schema if they are the same
  *         reader_schema = None
  */
   }
 
-  /* "fastavro/_read.pyx":1114
+  /* "fastavro/_read.pyx":1111
  *         reader_schema = None
  * 
  *     named_schemas = {"writer": {}, "reader": {}}             # <<<<<<<<<<<<<<
  *     writer_schema = parse_schema(writer_schema, named_schemas["writer"])
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1114, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1114, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_writer, __pyx_t_3) < 0) __PYX_ERR(0, 1114, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_writer, __pyx_t_3) < 0) __PYX_ERR(0, 1111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1114, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_reader, __pyx_t_3) < 0) __PYX_ERR(0, 1114, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_reader, __pyx_t_3) < 0) __PYX_ERR(0, 1111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_named_schemas = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":1115
+  /* "fastavro/_read.pyx":1112
  * 
  *     named_schemas = {"writer": {}, "reader": {}}
  *     writer_schema = parse_schema(writer_schema, named_schemas["writer"])             # <<<<<<<<<<<<<<
  * 
  *     if reader_schema:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parse_schema); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1115, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parse_schema); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_named_schemas, __pyx_n_u_writer); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1115, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_named_schemas, __pyx_n_u_writer); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -18507,69 +18373,69 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_writer_schema, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1115, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1112, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_writer_schema, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1115, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1112, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1115, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_v_writer_schema);
     __Pyx_GIVEREF(__pyx_v_writer_schema);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_writer_schema);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1115, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_writer_schema, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":1117
+  /* "fastavro/_read.pyx":1114
  *     writer_schema = parse_schema(writer_schema, named_schemas["writer"])
  * 
  *     if reader_schema:             # <<<<<<<<<<<<<<
  *         reader_schema = parse_schema(reader_schema, named_schemas["reader"])
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1117, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_reader_schema); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1114, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "fastavro/_read.pyx":1118
+    /* "fastavro/_read.pyx":1115
  * 
  *     if reader_schema:
  *         reader_schema = parse_schema(reader_schema, named_schemas["reader"])             # <<<<<<<<<<<<<<
  * 
- *     return _read_data(
+ *     options = {
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parse_schema); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1118, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parse_schema); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_named_schemas, __pyx_n_u_reader); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1118, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_named_schemas, __pyx_n_u_reader); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_4 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -18578,103 +18444,134 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_reader_schema, __pyx_t_7};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1118, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1115, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_reader_schema, __pyx_t_7};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1118, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1115, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1118, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1115, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_INCREF(__pyx_v_reader_schema);
       __Pyx_GIVEREF(__pyx_v_reader_schema);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_6, __pyx_v_reader_schema);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_6, __pyx_t_7);
       __pyx_t_7 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1118, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1115, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_reader_schema, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "fastavro/_read.pyx":1117
+    /* "fastavro/_read.pyx":1114
  *     writer_schema = parse_schema(writer_schema, named_schemas["writer"])
  * 
  *     if reader_schema:             # <<<<<<<<<<<<<<
  *         reader_schema = parse_schema(reader_schema, named_schemas["reader"])
  * 
  */
   }
 
-  /* "fastavro/_read.pyx":1120
- *         reader_schema = parse_schema(reader_schema, named_schemas["reader"])
+  /* "fastavro/_read.pyx":1118
  * 
+ *     options = {
+ *         "return_record_name": return_record_name,             # <<<<<<<<<<<<<<
+ *         "return_record_name_override": return_record_name_override,
+ *         "handle_unicode_errors": handle_unicode_errors,
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1118, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_return_record_name, __pyx_v_return_record_name) < 0) __PYX_ERR(0, 1118, __pyx_L1_error)
+
+  /* "fastavro/_read.pyx":1119
+ *     options = {
+ *         "return_record_name": return_record_name,
+ *         "return_record_name_override": return_record_name_override,             # <<<<<<<<<<<<<<
+ *         "handle_unicode_errors": handle_unicode_errors,
+ *     }
+ */
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_return_record_name_override, __pyx_v_return_record_name_override) < 0) __PYX_ERR(0, 1118, __pyx_L1_error)
+
+  /* "fastavro/_read.pyx":1120
+ *         "return_record_name": return_record_name,
+ *         "return_record_name_override": return_record_name_override,
+ *         "handle_unicode_errors": handle_unicode_errors,             # <<<<<<<<<<<<<<
+ *     }
+ *     return _read_data(
+ */
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_handle_unicode_errors, __pyx_v_handle_unicode_errors) < 0) __PYX_ERR(0, 1118, __pyx_L1_error)
+  __pyx_v_options = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "fastavro/_read.pyx":1122
+ *         "handle_unicode_errors": handle_unicode_errors,
+ *     }
  *     return _read_data(             # <<<<<<<<<<<<<<
  *         fo,
  *         writer_schema,
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "fastavro/_read.pyx":1126
+  /* "fastavro/_read.pyx":1127
+ *         named_schemas,
  *         reader_schema,
- *         return_record_name,
- *         return_record_name_override,             # <<<<<<<<<<<<<<
+ *         options,             # <<<<<<<<<<<<<<
  *     )
  * 
  */
-  __pyx_t_8.__pyx_n = 3;
+  __pyx_t_8.__pyx_n = 2;
   __pyx_t_8.reader_schema = __pyx_v_reader_schema;
-  __pyx_t_8.return_record_name = __pyx_v_return_record_name;
-  __pyx_t_8.return_record_name_override = __pyx_v_return_record_name_override;
-  __pyx_t_1 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1120, __pyx_L1_error)
+  __pyx_t_8.options = __pyx_v_options;
+  __pyx_t_1 = __pyx_f_8fastavro_5_read__read_data(__pyx_v_fo, __pyx_v_writer_schema, __pyx_v_named_schemas, 0, &__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "fastavro/_read.pyx":1107
+  /* "fastavro/_read.pyx":1099
  * 
  * 
- * cpdef schemaless_reader(fo, writer_schema, reader_schema=None,             # <<<<<<<<<<<<<<
- *                         return_record_name=False,
- *                         return_record_name_override=False):
+ * cpdef schemaless_reader(             # <<<<<<<<<<<<<<
+ *     fo,
+ *     writer_schema,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("fastavro._read.schemaless_reader", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_named_schemas);
+  __Pyx_XDECREF(__pyx_v_options);
   __Pyx_XDECREF(__pyx_v_writer_schema);
   __Pyx_XDECREF(__pyx_v_reader_schema);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -18682,46 +18579,58 @@
 static PyObject *__pyx_pw_8fastavro_5_read_87schemaless_reader(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_8fastavro_5_read_87schemaless_reader(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_fo = 0;
   PyObject *__pyx_v_writer_schema = 0;
   PyObject *__pyx_v_reader_schema = 0;
   PyObject *__pyx_v_return_record_name = 0;
   PyObject *__pyx_v_return_record_name_override = 0;
+  PyObject *__pyx_v_handle_unicode_errors = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("schemaless_reader (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,0};
-    PyObject* values[5] = {0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fo,&__pyx_n_s_writer_schema,&__pyx_n_s_reader_schema,&__pyx_n_s_return_record_name,&__pyx_n_s_return_record_name_override,&__pyx_n_s_handle_unicode_errors,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
+
+    /* "fastavro/_read.pyx":1102
+ *     fo,
+ *     writer_schema,
+ *     reader_schema=None,             # <<<<<<<<<<<<<<
+ *     return_record_name=False,
+ *     return_record_name_override=False,
+ */
     values[2] = ((PyObject *)Py_None);
 
-    /* "fastavro/_read.pyx":1108
- * 
- * cpdef schemaless_reader(fo, writer_schema, reader_schema=None,
- *                         return_record_name=False,             # <<<<<<<<<<<<<<
- *                         return_record_name_override=False):
- *     if writer_schema == reader_schema:
+    /* "fastavro/_read.pyx":1103
+ *     writer_schema,
+ *     reader_schema=None,
+ *     return_record_name=False,             # <<<<<<<<<<<<<<
+ *     return_record_name_override=False,
+ *     handle_unicode_errors="strict",
  */
     values[3] = ((PyObject *)Py_False);
 
-    /* "fastavro/_read.pyx":1109
- * cpdef schemaless_reader(fo, writer_schema, reader_schema=None,
- *                         return_record_name=False,
- *                         return_record_name_override=False):             # <<<<<<<<<<<<<<
- *     if writer_schema == reader_schema:
- *         # No need for the reader schema if they are the same
+    /* "fastavro/_read.pyx":1104
+ *     reader_schema=None,
+ *     return_record_name=False,
+ *     return_record_name_override=False,             # <<<<<<<<<<<<<<
+ *     handle_unicode_errors="strict",
+ * ):
  */
     values[4] = ((PyObject *)Py_False);
+    values[5] = ((PyObject *)__pyx_n_u_strict);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -18736,15 +18645,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fo)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_writer_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("schemaless_reader", 0, 2, 5, 1); __PYX_ERR(0, 1107, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("schemaless_reader", 0, 2, 6, 1); __PYX_ERR(0, 1099, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader_schema);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -18756,20 +18665,28 @@
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_return_record_name_override);
           if (value) { values[4] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_handle_unicode_errors);
+          if (value) { values[5] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "schemaless_reader") < 0)) __PYX_ERR(0, 1107, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "schemaless_reader") < 0)) __PYX_ERR(0, 1099, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -18779,53 +18696,55 @@
       }
     }
     __pyx_v_fo = values[0];
     __pyx_v_writer_schema = values[1];
     __pyx_v_reader_schema = values[2];
     __pyx_v_return_record_name = values[3];
     __pyx_v_return_record_name_override = values[4];
+    __pyx_v_handle_unicode_errors = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("schemaless_reader", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1107, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("schemaless_reader", 0, 2, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1099, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastavro._read.schemaless_reader", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8fastavro_5_read_86schemaless_reader(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override);
+  __pyx_r = __pyx_pf_8fastavro_5_read_86schemaless_reader(__pyx_self, __pyx_v_fo, __pyx_v_writer_schema, __pyx_v_reader_schema, __pyx_v_return_record_name, __pyx_v_return_record_name_override, __pyx_v_handle_unicode_errors);
 
-  /* "fastavro/_read.pyx":1107
+  /* "fastavro/_read.pyx":1099
  * 
  * 
- * cpdef schemaless_reader(fo, writer_schema, reader_schema=None,             # <<<<<<<<<<<<<<
- *                         return_record_name=False,
- *                         return_record_name_override=False):
+ * cpdef schemaless_reader(             # <<<<<<<<<<<<<<
+ *     fo,
+ *     writer_schema,
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8fastavro_5_read_86schemaless_reader(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override) {
+static PyObject *__pyx_pf_8fastavro_5_read_86schemaless_reader(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fo, PyObject *__pyx_v_writer_schema, PyObject *__pyx_v_reader_schema, PyObject *__pyx_v_return_record_name, PyObject *__pyx_v_return_record_name_override, PyObject *__pyx_v_handle_unicode_errors) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_8fastavro_5_read_schemaless_reader __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("schemaless_reader", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2.__pyx_n = 3;
+  __pyx_t_2.__pyx_n = 4;
   __pyx_t_2.reader_schema = __pyx_v_reader_schema;
   __pyx_t_2.return_record_name = __pyx_v_return_record_name;
   __pyx_t_2.return_record_name_override = __pyx_v_return_record_name_override;
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_schemaless_reader(__pyx_v_fo, __pyx_v_writer_schema, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1107, __pyx_L1_error)
+  __pyx_t_2.handle_unicode_errors = __pyx_v_handle_unicode_errors;
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_schemaless_reader(__pyx_v_fo, __pyx_v_writer_schema, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1099, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -18834,15 +18753,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastavro/_read.pyx":1130
+/* "fastavro/_read.pyx":1131
  * 
  * 
  * cpdef is_avro(path_or_buffer):             # <<<<<<<<<<<<<<
  *     if isinstance(path_or_buffer, str):
  *         fp = open(path_or_buffer, "rb")
  */
 
@@ -18870,148 +18789,148 @@
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_avro", 0);
 
-  /* "fastavro/_read.pyx":1131
+  /* "fastavro/_read.pyx":1132
  * 
  * cpdef is_avro(path_or_buffer):
  *     if isinstance(path_or_buffer, str):             # <<<<<<<<<<<<<<
  *         fp = open(path_or_buffer, "rb")
  *         close = True
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_path_or_buffer); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "fastavro/_read.pyx":1132
+    /* "fastavro/_read.pyx":1133
  * cpdef is_avro(path_or_buffer):
  *     if isinstance(path_or_buffer, str):
  *         fp = open(path_or_buffer, "rb")             # <<<<<<<<<<<<<<
  *         close = True
  *     else:
  */
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1132, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_path_or_buffer);
     __Pyx_GIVEREF(__pyx_v_path_or_buffer);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_path_or_buffer);
     __Pyx_INCREF(__pyx_n_u_rb);
     __Pyx_GIVEREF(__pyx_n_u_rb);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_n_u_rb);
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1132, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_fp = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "fastavro/_read.pyx":1133
+    /* "fastavro/_read.pyx":1134
  *     if isinstance(path_or_buffer, str):
  *         fp = open(path_or_buffer, "rb")
  *         close = True             # <<<<<<<<<<<<<<
  *     else:
  *         fp = path_or_buffer
  */
     __pyx_v_close = 1;
 
-    /* "fastavro/_read.pyx":1131
+    /* "fastavro/_read.pyx":1132
  * 
  * cpdef is_avro(path_or_buffer):
  *     if isinstance(path_or_buffer, str):             # <<<<<<<<<<<<<<
  *         fp = open(path_or_buffer, "rb")
  *         close = True
  */
     goto __pyx_L3;
   }
 
-  /* "fastavro/_read.pyx":1135
+  /* "fastavro/_read.pyx":1136
  *         close = True
  *     else:
  *         fp = path_or_buffer             # <<<<<<<<<<<<<<
  *         close = False
  * 
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_path_or_buffer);
     __pyx_v_fp = __pyx_v_path_or_buffer;
 
-    /* "fastavro/_read.pyx":1136
+    /* "fastavro/_read.pyx":1137
  *     else:
  *         fp = path_or_buffer
  *         close = False             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
     __pyx_v_close = 0;
   }
   __pyx_L3:;
 
-  /* "fastavro/_read.pyx":1138
+  /* "fastavro/_read.pyx":1139
  *         close = False
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         header = fp.read(len(MAGIC))
  *         return header == MAGIC
  */
   /*try:*/ {
 
-    /* "fastavro/_read.pyx":1139
+    /* "fastavro/_read.pyx":1140
  * 
  *     try:
  *         header = fp.read(len(MAGIC))             # <<<<<<<<<<<<<<
  *         return header == MAGIC
  *     finally:
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1139, __pyx_L5_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1140, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_MAGIC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1139, __pyx_L5_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_MAGIC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1140, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1139, __pyx_L5_error)
+    __pyx_t_6 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1140, __pyx_L5_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1139, __pyx_L5_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1140, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_7, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1139, __pyx_L5_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1140, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_header = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "fastavro/_read.pyx":1140
+    /* "fastavro/_read.pyx":1141
  *     try:
  *         header = fp.read(len(MAGIC))
  *         return header == MAGIC             # <<<<<<<<<<<<<<
  *     finally:
  *         if close:
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MAGIC); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1140, __pyx_L5_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MAGIC); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1141, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyObject_RichCompare(__pyx_v_header, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1140, __pyx_L5_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_v_header, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1141, __pyx_L5_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L4_return;
   }
 
-  /* "fastavro/_read.pyx":1142
+  /* "fastavro/_read.pyx":1143
  *         return header == MAGIC
  *     finally:
  *         if close:             # <<<<<<<<<<<<<<
  *             fp.close()
  */
   /*finally:*/ {
     __pyx_L5_error:;
@@ -19032,39 +18951,39 @@
       __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_XGOTREF(__pyx_t_16);
       __pyx_t_8 = __pyx_lineno; __pyx_t_9 = __pyx_clineno; __pyx_t_10 = __pyx_filename;
       {
         __pyx_t_2 = (__pyx_v_close != 0);
         if (__pyx_t_2) {
 
-          /* "fastavro/_read.pyx":1143
+          /* "fastavro/_read.pyx":1144
  *     finally:
  *         if close:
  *             fp.close()             # <<<<<<<<<<<<<<
  */
-          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_close); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1143, __pyx_L8_error)
+          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_close); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1144, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_4);
           __pyx_t_5 = NULL;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
             __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
             if (likely(__pyx_t_5)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
               __Pyx_INCREF(__pyx_t_5);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_4, function);
             }
           }
           __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1143, __pyx_L8_error)
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1144, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          /* "fastavro/_read.pyx":1142
+          /* "fastavro/_read.pyx":1143
  *         return header == MAGIC
  *     finally:
  *         if close:             # <<<<<<<<<<<<<<
  *             fp.close()
  */
         }
       }
@@ -19096,52 +19015,52 @@
     }
     __pyx_L4_return: {
       __pyx_t_16 = __pyx_r;
       __pyx_r = 0;
       __pyx_t_2 = (__pyx_v_close != 0);
       if (__pyx_t_2) {
 
-        /* "fastavro/_read.pyx":1143
+        /* "fastavro/_read.pyx":1144
  *     finally:
  *         if close:
  *             fp.close()             # <<<<<<<<<<<<<<
  */
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_close); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1143, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_close); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1144, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
             __Pyx_INCREF(__pyx_t_5);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
         __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1143, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1144, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "fastavro/_read.pyx":1142
+        /* "fastavro/_read.pyx":1143
  *         return header == MAGIC
  *     finally:
  *         if close:             # <<<<<<<<<<<<<<
  *             fp.close()
  */
       }
       __pyx_r = __pyx_t_16;
       __pyx_t_16 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "fastavro/_read.pyx":1130
+  /* "fastavro/_read.pyx":1131
  * 
  * 
  * cpdef is_avro(path_or_buffer):             # <<<<<<<<<<<<<<
  *     if isinstance(path_or_buffer, str):
  *         fp = open(path_or_buffer, "rb")
  */
 
@@ -19179,15 +19098,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_avro", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8fastavro_5_read_is_avro(__pyx_v_path_or_buffer, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1130, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8fastavro_5_read_is_avro(__pyx_v_path_or_buffer, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -19221,18 +19140,17 @@
   struct __pyx_obj_8fastavro_5_read___pyx_scope_struct___iter_avro_records *p = (struct __pyx_obj_8fastavro_5_read___pyx_scope_struct___iter_avro_records *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_block_fo);
   Py_CLEAR(p->__pyx_v_codec);
   Py_CLEAR(p->__pyx_v_fo);
   Py_CLEAR(p->__pyx_v_header);
   Py_CLEAR(p->__pyx_v_named_schemas);
+  Py_CLEAR(p->__pyx_v_options);
   Py_CLEAR(p->__pyx_v_read_block);
   Py_CLEAR(p->__pyx_v_reader_schema);
-  Py_CLEAR(p->__pyx_v_return_record_name);
-  Py_CLEAR(p->__pyx_v_return_record_name_override);
   Py_CLEAR(p->__pyx_v_sync_marker);
   Py_CLEAR(p->__pyx_v_writer_schema);
   if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_8fastavro_5_read___pyx_scope_struct___iter_avro_records < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8fastavro_5_read___pyx_scope_struct___iter_avro_records)))) {
     __pyx_freelist_8fastavro_5_read___pyx_scope_struct___iter_avro_records[__pyx_freecount_8fastavro_5_read___pyx_scope_struct___iter_avro_records++] = ((struct __pyx_obj_8fastavro_5_read___pyx_scope_struct___iter_avro_records *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
@@ -19252,26 +19170,23 @@
   }
   if (p->__pyx_v_header) {
     e = (*v)(p->__pyx_v_header, a); if (e) return e;
   }
   if (p->__pyx_v_named_schemas) {
     e = (*v)(p->__pyx_v_named_schemas, a); if (e) return e;
   }
+  if (p->__pyx_v_options) {
+    e = (*v)(p->__pyx_v_options, a); if (e) return e;
+  }
   if (p->__pyx_v_read_block) {
     e = (*v)(p->__pyx_v_read_block, a); if (e) return e;
   }
   if (p->__pyx_v_reader_schema) {
     e = (*v)(p->__pyx_v_reader_schema, a); if (e) return e;
   }
-  if (p->__pyx_v_return_record_name) {
-    e = (*v)(p->__pyx_v_return_record_name, a); if (e) return e;
-  }
-  if (p->__pyx_v_return_record_name_override) {
-    e = (*v)(p->__pyx_v_return_record_name_override, a); if (e) return e;
-  }
   if (p->__pyx_v_sync_marker) {
     e = (*v)(p->__pyx_v_sync_marker, a); if (e) return e;
   }
   if (p->__pyx_v_writer_schema) {
     e = (*v)(p->__pyx_v_writer_schema, a); if (e) return e;
   }
   return 0;
@@ -19371,18 +19286,17 @@
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_block_bytes);
   Py_CLEAR(p->__pyx_v_codec);
   Py_CLEAR(p->__pyx_v_fo);
   Py_CLEAR(p->__pyx_v_header);
   Py_CLEAR(p->__pyx_v_named_schemas);
   Py_CLEAR(p->__pyx_v_offset);
+  Py_CLEAR(p->__pyx_v_options);
   Py_CLEAR(p->__pyx_v_read_block);
   Py_CLEAR(p->__pyx_v_reader_schema);
-  Py_CLEAR(p->__pyx_v_return_record_name);
-  Py_CLEAR(p->__pyx_v_return_record_name_override);
   Py_CLEAR(p->__pyx_v_size);
   Py_CLEAR(p->__pyx_v_sync_marker);
   Py_CLEAR(p->__pyx_v_writer_schema);
   if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks)))) {
     __pyx_freelist_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks[__pyx_freecount_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks++] = ((struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
@@ -19406,26 +19320,23 @@
   }
   if (p->__pyx_v_named_schemas) {
     e = (*v)(p->__pyx_v_named_schemas, a); if (e) return e;
   }
   if (p->__pyx_v_offset) {
     e = (*v)(p->__pyx_v_offset, a); if (e) return e;
   }
+  if (p->__pyx_v_options) {
+    e = (*v)(p->__pyx_v_options, a); if (e) return e;
+  }
   if (p->__pyx_v_read_block) {
     e = (*v)(p->__pyx_v_read_block, a); if (e) return e;
   }
   if (p->__pyx_v_reader_schema) {
     e = (*v)(p->__pyx_v_reader_schema, a); if (e) return e;
   }
-  if (p->__pyx_v_return_record_name) {
-    e = (*v)(p->__pyx_v_return_record_name, a); if (e) return e;
-  }
-  if (p->__pyx_v_return_record_name_override) {
-    e = (*v)(p->__pyx_v_return_record_name_override, a); if (e) return e;
-  }
   if (p->__pyx_v_size) {
     e = (*v)(p->__pyx_v_size, a); if (e) return e;
   }
   if (p->__pyx_v_sync_marker) {
     e = (*v)(p->__pyx_v_sync_marker, a); if (e) return e;
   }
   if (p->__pyx_v_writer_schema) {
@@ -19635,15 +19546,15 @@
   {"skip_int", (PyCFunction)__pyx_pw_8fastavro_5_read_17skip_int, METH_O, 0},
   {"read_float", (PyCFunction)__pyx_pw_8fastavro_5_read_19read_float, METH_O, __pyx_doc_8fastavro_5_read_18read_float},
   {"skip_float", (PyCFunction)__pyx_pw_8fastavro_5_read_21skip_float, METH_O, __pyx_doc_8fastavro_5_read_20skip_float},
   {"read_double", (PyCFunction)__pyx_pw_8fastavro_5_read_23read_double, METH_O, __pyx_doc_8fastavro_5_read_22read_double},
   {"skip_double", (PyCFunction)__pyx_pw_8fastavro_5_read_25skip_double, METH_O, __pyx_doc_8fastavro_5_read_24skip_double},
   {"read_bytes", (PyCFunction)__pyx_pw_8fastavro_5_read_27read_bytes, METH_O, __pyx_doc_8fastavro_5_read_26read_bytes},
   {"skip_bytes", (PyCFunction)__pyx_pw_8fastavro_5_read_29skip_bytes, METH_O, __pyx_doc_8fastavro_5_read_28skip_bytes},
-  {"read_utf8", (PyCFunction)__pyx_pw_8fastavro_5_read_31read_utf8, METH_O, __pyx_doc_8fastavro_5_read_30read_utf8},
+  {"read_utf8", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_31read_utf8, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8fastavro_5_read_30read_utf8},
   {"skip_utf8", (PyCFunction)__pyx_pw_8fastavro_5_read_33skip_utf8, METH_O, __pyx_doc_8fastavro_5_read_32skip_utf8},
   {"read_fixed", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_35read_fixed, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8fastavro_5_read_34read_fixed},
   {"skip_fixed", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_37skip_fixed, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8fastavro_5_read_36skip_fixed},
   {"read_enum", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_39read_enum, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8fastavro_5_read_38read_enum},
   {"skip_enum", (PyCFunction)__pyx_pw_8fastavro_5_read_41skip_enum, METH_O, __pyx_doc_8fastavro_5_read_40skip_enum},
   {"read_array", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_43read_array, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8fastavro_5_read_42read_array},
   {"skip_array", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_45skip_array, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8fastavro_5_read_44skip_array},
@@ -19737,15 +19648,15 @@
   {&__pyx_n_s_SchemaResolutionError, __pyx_k_SchemaResolutionError, sizeof(__pyx_k_SchemaResolutionError), 0, 0, 1, 1},
   {&__pyx_kp_u_Schema_mismatch, __pyx_k_Schema_mismatch, sizeof(__pyx_k_Schema_mismatch), 0, 1, 0, 0},
   {&__pyx_n_s_StopIteration, __pyx_k_StopIteration, sizeof(__pyx_k_StopIteration), 0, 0, 1, 1},
   {&__pyx_kp_u_The_schema_attribute_is_deprecat, __pyx_k_The_schema_attribute_is_deprecat, sizeof(__pyx_k_The_schema_attribute_is_deprecat), 0, 1, 0, 0},
   {&__pyx_kp_u_Unrecognized_codec, __pyx_k_Unrecognized_codec, sizeof(__pyx_k_Unrecognized_codec), 0, 1, 0, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_ZstdDecompressor, __pyx_k_ZstdDecompressor, sizeof(__pyx_k_ZstdDecompressor), 0, 0, 1, 1},
-  {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
+  {&__pyx_kp_u__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 1, 0, 0},
   {&__pyx_n_u_aliases, __pyx_k_aliases, sizeof(__pyx_k_aliases), 0, 1, 0, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_u_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 1, 0, 1},
   {&__pyx_kp_u_avro_codec, __pyx_k_avro_codec, sizeof(__pyx_k_avro_codec), 0, 1, 0, 0},
   {&__pyx_kp_u_avro_schema, __pyx_k_avro_schema, sizeof(__pyx_k_avro_schema), 0, 1, 0, 0},
   {&__pyx_n_s_block, __pyx_k_block, sizeof(__pyx_k_block), 0, 0, 1, 1},
   {&__pyx_n_s_block_bytes, __pyx_k_block_bytes, sizeof(__pyx_k_block_bytes), 0, 0, 1, 1},
@@ -19783,14 +19694,15 @@
   {&__pyx_n_s_elems, __pyx_k_elems, sizeof(__pyx_k_elems), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_u_enum, __pyx_k_enum, sizeof(__pyx_k_enum), 0, 1, 0, 1},
   {&__pyx_n_s_epoch, __pyx_k_epoch, sizeof(__pyx_k_epoch), 0, 0, 1, 1},
   {&__pyx_n_s_epoch_naive, __pyx_k_epoch_naive, sizeof(__pyx_k_epoch_naive), 0, 0, 1, 1},
   {&__pyx_n_u_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 1, 0, 1},
   {&__pyx_n_u_error_union, __pyx_k_error_union, sizeof(__pyx_k_error_union), 0, 1, 0, 1},
+  {&__pyx_n_s_errors, __pyx_k_errors, sizeof(__pyx_k_errors), 0, 0, 1, 1},
   {&__pyx_kp_u_expected_sync_marker_not_found, __pyx_k_expected_sync_marker_not_found, sizeof(__pyx_k_expected_sync_marker_not_found), 0, 1, 0, 0},
   {&__pyx_n_s_extract_logical_type, __pyx_k_extract_logical_type, sizeof(__pyx_k_extract_logical_type), 0, 0, 1, 1},
   {&__pyx_n_s_extract_record_type, __pyx_k_extract_record_type, sizeof(__pyx_k_extract_record_type), 0, 0, 1, 1},
   {&__pyx_n_s_fastavro__read, __pyx_k_fastavro__read, sizeof(__pyx_k_fastavro__read), 0, 0, 1, 1},
   {&__pyx_kp_s_fastavro__read_pyx, __pyx_k_fastavro__read_pyx, sizeof(__pyx_k_fastavro__read_pyx), 0, 0, 1, 0},
   {&__pyx_n_u_fields, __pyx_k_fields, sizeof(__pyx_k_fields), 0, 1, 0, 1},
   {&__pyx_n_s_file_reader, __pyx_k_file_reader, sizeof(__pyx_k_file_reader), 0, 0, 1, 1},
@@ -19800,14 +19712,16 @@
   {&__pyx_n_s_file_reader_schema, __pyx_k_file_reader_schema, sizeof(__pyx_k_file_reader_schema), 0, 0, 1, 1},
   {&__pyx_n_u_fixed, __pyx_k_fixed, sizeof(__pyx_k_fixed), 0, 1, 0, 1},
   {&__pyx_n_u_float, __pyx_k_float, sizeof(__pyx_k_float), 0, 1, 0, 1},
   {&__pyx_n_s_fo, __pyx_k_fo, sizeof(__pyx_k_fo), 0, 0, 1, 1},
   {&__pyx_n_s_force, __pyx_k_force, sizeof(__pyx_k_force), 0, 0, 1, 1},
   {&__pyx_kp_u_from, __pyx_k_from, sizeof(__pyx_k_from), 0, 1, 0, 0},
   {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
+  {&__pyx_n_s_handle_unicode_errors, __pyx_k_handle_unicode_errors, sizeof(__pyx_k_handle_unicode_errors), 0, 0, 1, 1},
+  {&__pyx_n_u_handle_unicode_errors, __pyx_k_handle_unicode_errors, sizeof(__pyx_k_handle_unicode_errors), 0, 1, 0, 1},
   {&__pyx_n_s_header, __pyx_k_header, sizeof(__pyx_k_header), 0, 0, 1, 1},
   {&__pyx_n_s_header_2, __pyx_k_header_2, sizeof(__pyx_k_header_2), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_ignore_default_error, __pyx_k_ignore_default_error, sizeof(__pyx_k_ignore_default_error), 0, 0, 1, 1},
   {&__pyx_n_s_ignore_default_error_2, __pyx_k_ignore_default_error_2, sizeof(__pyx_k_ignore_default_error_2), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
@@ -19847,14 +19761,15 @@
   {&__pyx_kp_u_not_found_in_reader_symbol_list, __pyx_k_not_found_in_reader_symbol_list, sizeof(__pyx_k_not_found_in_reader_symbol_list), 0, 1, 0, 0},
   {&__pyx_n_u_null, __pyx_k_null, sizeof(__pyx_k_null), 0, 1, 0, 1},
   {&__pyx_n_s_null_read_block, __pyx_k_null_read_block, sizeof(__pyx_k_null_read_block), 0, 0, 1, 1},
   {&__pyx_n_s_num_block_records, __pyx_k_num_block_records, sizeof(__pyx_k_num_block_records), 0, 0, 1, 1},
   {&__pyx_n_s_num_records, __pyx_k_num_records, sizeof(__pyx_k_num_records), 0, 0, 1, 1},
   {&__pyx_n_s_offset, __pyx_k_offset, sizeof(__pyx_k_offset), 0, 0, 1, 1},
   {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
+  {&__pyx_n_s_options, __pyx_k_options, sizeof(__pyx_k_options), 0, 0, 1, 1},
   {&__pyx_n_s_parse_schema, __pyx_k_parse_schema, sizeof(__pyx_k_parse_schema), 0, 0, 1, 1},
   {&__pyx_kp_u_position, __pyx_k_position, sizeof(__pyx_k_position), 0, 1, 0, 0},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_property, __pyx_k_property, sizeof(__pyx_k_property), 0, 0, 1, 1},
   {&__pyx_kp_u_python_snappy, __pyx_k_python_snappy, sizeof(__pyx_k_python_snappy), 0, 1, 0, 0},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_r_schema, __pyx_k_r_schema, sizeof(__pyx_k_r_schema), 0, 0, 1, 1},
@@ -19867,29 +19782,32 @@
   {&__pyx_n_u_reader, __pyx_k_reader, sizeof(__pyx_k_reader), 0, 1, 0, 1},
   {&__pyx_n_s_reader___init, __pyx_k_reader___init, sizeof(__pyx_k_reader___init), 0, 0, 1, 1},
   {&__pyx_n_s_reader_schema, __pyx_k_reader_schema, sizeof(__pyx_k_reader_schema), 0, 0, 1, 1},
   {&__pyx_n_s_reader_type, __pyx_k_reader_type, sizeof(__pyx_k_reader_type), 0, 0, 1, 1},
   {&__pyx_n_u_record, __pyx_k_record, sizeof(__pyx_k_record), 0, 1, 0, 1},
   {&__pyx_kp_u_records, __pyx_k_records, sizeof(__pyx_k_records), 0, 1, 0, 0},
   {&__pyx_n_s_return_record_name, __pyx_k_return_record_name, sizeof(__pyx_k_return_record_name), 0, 0, 1, 1},
+  {&__pyx_n_u_return_record_name, __pyx_k_return_record_name, sizeof(__pyx_k_return_record_name), 0, 1, 0, 1},
   {&__pyx_n_s_return_record_name_override, __pyx_k_return_record_name_override, sizeof(__pyx_k_return_record_name_override), 0, 0, 1, 1},
+  {&__pyx_n_u_return_record_name_override, __pyx_k_return_record_name_override, sizeof(__pyx_k_return_record_name_override), 0, 1, 0, 1},
   {&__pyx_n_s_schema, __pyx_k_schema, sizeof(__pyx_k_schema), 0, 0, 1, 1},
   {&__pyx_n_s_schema_2, __pyx_k_schema_2, sizeof(__pyx_k_schema_2), 0, 0, 1, 1},
   {&__pyx_kp_u_schema_mismatch, __pyx_k_schema_mismatch, sizeof(__pyx_k_schema_mismatch), 0, 1, 0, 0},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_u_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 1, 0, 1},
   {&__pyx_kp_u_size_2, __pyx_k_size_2, sizeof(__pyx_k_size_2), 0, 1, 0, 0},
   {&__pyx_kp_u_size_is_different_than, __pyx_k_size_is_different_than, sizeof(__pyx_k_size_is_different_than), 0, 1, 0, 0},
   {&__pyx_n_s_snappy, __pyx_k_snappy, sizeof(__pyx_k_snappy), 0, 0, 1, 1},
   {&__pyx_n_u_snappy, __pyx_k_snappy, sizeof(__pyx_k_snappy), 0, 1, 0, 1},
   {&__pyx_n_s_snappy_read_block, __pyx_k_snappy_read_block, sizeof(__pyx_k_snappy_read_block), 0, 0, 1, 1},
   {&__pyx_n_s_split, __pyx_k_split, sizeof(__pyx_k_split), 0, 0, 1, 1},
   {&__pyx_n_s_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 0, 1, 1},
+  {&__pyx_n_u_strict, __pyx_k_strict, sizeof(__pyx_k_strict), 0, 1, 0, 1},
   {&__pyx_n_u_string, __pyx_k_string, sizeof(__pyx_k_string), 0, 1, 0, 1},
   {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
   {&__pyx_n_u_symbols, __pyx_k_symbols, sizeof(__pyx_k_symbols), 0, 1, 0, 1},
   {&__pyx_n_u_sync, __pyx_k_sync, sizeof(__pyx_k_sync), 0, 1, 0, 1},
   {&__pyx_n_s_sync_marker, __pyx_k_sync_marker, sizeof(__pyx_k_sync_marker), 0, 0, 1, 1},
   {&__pyx_n_s_tell, __pyx_k_tell, sizeof(__pyx_k_tell), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
@@ -19914,264 +19832,269 @@
   {&__pyx_n_s_zstandard, __pyx_k_zstandard, sizeof(__pyx_k_zstandard), 0, 0, 1, 1},
   {&__pyx_n_u_zstandard, __pyx_k_zstandard, sizeof(__pyx_k_zstandard), 0, 1, 0, 1},
   {&__pyx_n_s_zstandard_read_block, __pyx_k_zstandard_read_block, sizeof(__pyx_k_zstandard_read_block), 0, 0, 1, 1},
   {&__pyx_n_s_zstd, __pyx_k_zstd, sizeof(__pyx_k_zstd), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 870, __pyx_L1_error)
-  __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 1061, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 847, __pyx_L1_error)
+  __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 1031, __pyx_L1_error)
   __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 163, __pyx_L1_error)
   __pyx_builtin_EOFError = __Pyx_GetBuiltinName(__pyx_n_s_EOFError); if (!__pyx_builtin_EOFError) __PYX_ERR(0, 274, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 370, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 825, __pyx_L1_error)
-  __pyx_builtin_DeprecationWarning = __Pyx_GetBuiltinName(__pyx_n_s_DeprecationWarning); if (!__pyx_builtin_DeprecationWarning) __PYX_ERR(0, 1066, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 1072, __pyx_L1_error)
-  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 1081, __pyx_L1_error)
-  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 1132, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 802, __pyx_L1_error)
+  __pyx_builtin_DeprecationWarning = __Pyx_GetBuiltinName(__pyx_n_s_DeprecationWarning); if (!__pyx_builtin_DeprecationWarning) __PYX_ERR(0, 1036, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 1042, __pyx_L1_error)
+  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 1063, __pyx_L1_error)
+  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 1133, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "fastavro/_read.pyx":825
+  /* "fastavro/_read.pyx":450
+ *         if reader_schema:
+ *             for i in range(block_count):
+ *                 key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))             # <<<<<<<<<<<<<<
+ *                 read_items[key] = _read_data(
+ *                     fo,
+ */
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_handle_unicode_errors, __pyx_n_u_strict); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+
+  /* "fastavro/_read.pyx":802
  *     """Skip an expected sync marker, complaining if it doesn't match"""
  *     if fo.read(SYNC_SIZE) != sync_marker:
  *         raise ValueError("expected sync marker not found")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_expected_sync_marker_not_found); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 825, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_expected_sync_marker_not_found); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 802, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "fastavro/_read.pyx":1026
- *                                       return_record_name, return_record_name_override)
+  /* "fastavro/_read.pyx":996
+ *             self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None, self.options)
  *         except (StopIteration, EOFError):
  *             raise ValueError("cannot read header - is it an avro file?")             # <<<<<<<<<<<<<<
  * 
  *         # `meta` values are bytes. So, the actual decoding has to be external.
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_cannot_read_header_is_it_an_avro); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 1026, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_cannot_read_header_is_it_an_avro); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 996, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "fastavro/_read.pyx":1034
+  /* "fastavro/_read.pyx":1004
  * 
  *         self._schema = json.loads(self.metadata["avro.schema"])
  *         self.codec = self.metadata.get("avro.codec", "null")             # <<<<<<<<<<<<<<
  * 
  *         self._named_schemas = {"writer": {}, "reader": {}}
  */
-  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_kp_u_avro_codec, __pyx_n_u_null); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 1034, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__14 = PyTuple_Pack(2, __pyx_kp_u_avro_codec, __pyx_n_u_null); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 1004, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "fastavro/_read.pyx":1064
+  /* "fastavro/_read.pyx":1034
  *     def schema(self):
  *         import warnings
  *         warnings.warn(             # <<<<<<<<<<<<<<
  *             "The 'schema' attribute is deprecated. Please use 'writer_schema'",
  *             DeprecationWarning,
  */
-  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_kp_u_The_schema_attribute_is_deprecat, __pyx_builtin_DeprecationWarning); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 1064, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__15 = PyTuple_Pack(2, __pyx_kp_u_The_schema_attribute_is_deprecat, __pyx_builtin_DeprecationWarning); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 1034, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "fastavro/_read.pyx":33
  * 
  * decimal_context = Context()
  * epoch = datetime(1970, 1, 1, tzinfo=timezone.utc)             # <<<<<<<<<<<<<<
  * epoch_naive = datetime(1970, 1, 1)
  * 
  */
-  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_1970, __pyx_int_1, __pyx_int_1); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 33, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__16 = PyTuple_Pack(3, __pyx_int_1970, __pyx_int_1, __pyx_int_1); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "fastavro/_read.pyx":871
+  /* "fastavro/_read.pyx":848
  *     import snappy
  * except ImportError:
  *     BLOCK_READERS["snappy"] = missing_codec_lib("snappy", "python-snappy")             # <<<<<<<<<<<<<<
  * else:
  *     BLOCK_READERS["snappy"] = snappy_read_block
  */
-  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_u_snappy, __pyx_kp_u_python_snappy); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 871, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_u_snappy, __pyx_kp_u_python_snappy); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 848, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "fastavro/_read.pyx":885
+  /* "fastavro/_read.pyx":862
  *     import zstandard as zstd
  * except ImportError:
  *     BLOCK_READERS["zstandard"] = missing_codec_lib("zstandard", "zstandard")             # <<<<<<<<<<<<<<
  * else:
  *     BLOCK_READERS["zstandard"] = zstandard_read_block
  */
-  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_u_zstandard, __pyx_n_u_zstandard); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 885, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_u_zstandard, __pyx_n_u_zstandard); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 862, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
-  /* "fastavro/_read.pyx":899
+  /* "fastavro/_read.pyx":876
  *     import lz4.block
  * except ImportError:
  *     BLOCK_READERS["lz4"] = missing_codec_lib("lz4", "lz4")             # <<<<<<<<<<<<<<
  * else:
  *     BLOCK_READERS["lz4"] = lz4_read_block
  */
-  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_u_lz4, __pyx_n_u_lz4); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 899, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__19 = PyTuple_Pack(2, __pyx_n_u_lz4, __pyx_n_u_lz4); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 876, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
-  /* "fastavro/_read.pyx":904
+  /* "fastavro/_read.pyx":881
  * 
  * 
  * def _iter_avro_records(             # <<<<<<<<<<<<<<
  *     fo,
  *     header,
  */
-  __pyx_tuple__14 = PyTuple_Pack(13, __pyx_n_s_fo, __pyx_n_s_header, __pyx_n_s_codec, __pyx_n_s_writer_schema, __pyx_n_s_named_schemas, __pyx_n_s_reader_schema, __pyx_n_s_return_record_name, __pyx_n_s_return_record_name_override, __pyx_n_s_i, __pyx_n_s_sync_marker, __pyx_n_s_read_block, __pyx_n_s_block_count, __pyx_n_s_block_fo); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 904, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(8, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_iter_avro_records, 904, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 904, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(12, __pyx_n_s_fo, __pyx_n_s_header, __pyx_n_s_codec, __pyx_n_s_writer_schema, __pyx_n_s_named_schemas, __pyx_n_s_reader_schema, __pyx_n_s_options, __pyx_n_s_i, __pyx_n_s_sync_marker, __pyx_n_s_read_block, __pyx_n_s_block_count, __pyx_n_s_block_fo); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 881, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(7, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_iter_avro_records, 881, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 881, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":940
+  /* "fastavro/_read.pyx":915
  * 
  * 
  * def _iter_avro_blocks(             # <<<<<<<<<<<<<<
  *     fo,
  *     header,
  */
-  __pyx_tuple__15 = PyTuple_Pack(14, __pyx_n_s_fo, __pyx_n_s_header, __pyx_n_s_codec, __pyx_n_s_writer_schema, __pyx_n_s_named_schemas, __pyx_n_s_reader_schema, __pyx_n_s_return_record_name, __pyx_n_s_return_record_name_override, __pyx_n_s_sync_marker, __pyx_n_s_read_block, __pyx_n_s_offset, __pyx_n_s_num_block_records, __pyx_n_s_block_bytes, __pyx_n_s_size); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 940, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(8, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_iter_avro_blocks, 940, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 940, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(13, __pyx_n_s_fo, __pyx_n_s_header, __pyx_n_s_codec, __pyx_n_s_writer_schema, __pyx_n_s_named_schemas, __pyx_n_s_reader_schema, __pyx_n_s_options, __pyx_n_s_sync_marker, __pyx_n_s_read_block, __pyx_n_s_offset, __pyx_n_s_num_block_records, __pyx_n_s_block_bytes, __pyx_n_s_size); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 915, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(7, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_iter_avro_blocks, 915, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 915, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":976
+  /* "fastavro/_read.pyx":950
  * 
  * class Block:
  *     def __init__(             # <<<<<<<<<<<<<<
- *             self,
- *             bytes_,
+ *         self,
+ *         bytes_,
  */
-  __pyx_tuple__16 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_bytes_2, __pyx_n_s_num_records, __pyx_n_s_codec, __pyx_n_s_reader_schema, __pyx_n_s_writer_schema, __pyx_n_s_named_schemas, __pyx_n_s_offset, __pyx_n_s_size, __pyx_n_s_return_record_name, __pyx_n_s_return_record_name_override); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 976, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(11, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_init, 976, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 976, __pyx_L1_error)
-  __pyx_tuple__18 = PyTuple_Pack(2, ((PyObject *)Py_False), ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 976, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__22 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_bytes_2, __pyx_n_s_num_records, __pyx_n_s_codec, __pyx_n_s_reader_schema, __pyx_n_s_writer_schema, __pyx_n_s_named_schemas, __pyx_n_s_offset, __pyx_n_s_size, __pyx_n_s_options); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(10, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_init, 950, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 950, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":999
- *         self.return_record_name_override = return_record_name_override
+  /* "fastavro/_read.pyx":972
+ *         self.options = options
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         for i in range(self.num_records):
  *             yield _read_data(
  */
-  __pyx_tuple__19 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_i); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 999, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_iter, 999, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 999, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_i); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 972, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_iter, 972, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 972, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1010
+  /* "fastavro/_read.pyx":982
  *             )
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return (
  *             f"Avro block: {len(self.bytes_)} bytes, {self.num_records} records, "
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 1010, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_str, 1010, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 1010, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 982, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_str, 982, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 982, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1018
+  /* "fastavro/_read.pyx":990
  * 
  * class file_reader:
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
+ *     def __init__(self, fo, reader_schema=None, options={}):             # <<<<<<<<<<<<<<
  *         self.fo = fo
- *         self.return_record_name = return_record_name
+ *         self.options = options
  */
-  __pyx_tuple__22 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_fo, __pyx_n_s_reader_schema, __pyx_n_s_return_record_name, __pyx_n_s_return_record_name_override, __pyx_n_s_ignore_default_error_2, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 1018, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(5, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_init, 1018, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 1018, __pyx_L1_error)
-  __pyx_tuple__24 = PyTuple_Pack(3, ((PyObject *)Py_None), ((PyObject *)Py_False), ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 1018, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__27 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_fo, __pyx_n_s_reader_schema, __pyx_n_s_options, __pyx_n_s_ignore_default_error_2, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 990, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_init, 990, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 990, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1062
+  /* "fastavro/_read.pyx":1032
  * 
  *     @property
  *     def schema(self):             # <<<<<<<<<<<<<<
  *         import warnings
  *         warnings.warn(
  */
-  __pyx_tuple__25 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_warnings); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 1062, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_schema_2, 1062, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 1062, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_warnings); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 1032, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_schema_2, 1032, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 1032, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1070
+  /* "fastavro/_read.pyx":1040
  *         return self._schema
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         if not self._elems:
  *             raise NotImplementedError
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 1070, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_iter, 1070, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 1070, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 1040, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_iter, 1040, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 1040, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1075
+  /* "fastavro/_read.pyx":1045
  *         return self._elems
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         return next(self._elems)
  * 
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 1075, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_next, 1075, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 1075, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 1045, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_next, 1045, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 1045, __pyx_L1_error)
 
-  /* "fastavro/_read.pyx":1080
+  /* "fastavro/_read.pyx":1050
  * 
  * class reader(file_reader):
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
- * 
+ *     def __init__(             # <<<<<<<<<<<<<<
+ *         self,
+ *         fo,
  */
-  __pyx_tuple__31 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_fo, __pyx_n_s_reader_schema, __pyx_n_s_return_record_name, __pyx_n_s_return_record_name_override); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 1080, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_init, 1080, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 1080, __pyx_L1_error)
-  __pyx_tuple__33 = PyTuple_Pack(3, ((PyObject *)Py_None), ((PyObject *)Py_False), ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 1080, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__35 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_fo, __pyx_n_s_reader_schema, __pyx_n_s_return_record_name, __pyx_n_s_return_record_name_override, __pyx_n_s_handle_unicode_errors, __pyx_n_s_options); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 1050, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(6, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_init, 1050, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 1050, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(4, ((PyObject *)Py_None), ((PyObject *)Py_False), ((PyObject *)Py_False), ((PyObject*)__pyx_n_u_strict)); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 1050, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
 
-  /* "fastavro/_read.pyx":1094
+  /* "fastavro/_read.pyx":1075
  * 
  * class block_reader(file_reader):
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
- * 
+ *     def __init__(             # <<<<<<<<<<<<<<
+ *         self,
+ *         fo,
  */
-  __pyx_tuple__34 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_fo, __pyx_n_s_reader_schema, __pyx_n_s_return_record_name, __pyx_n_s_return_record_name_override); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 1094, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_init, 1094, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 1094, __pyx_L1_error)
-  __pyx_tuple__36 = PyTuple_Pack(3, ((PyObject *)Py_None), ((PyObject *)Py_False), ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 1094, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_tuple__38 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_fo, __pyx_n_s_reader_schema, __pyx_n_s_return_record_name, __pyx_n_s_return_record_name_override, __pyx_n_s_handle_unicode_errors, __pyx_n_s_options); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 1075, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(6, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__read_pyx, __pyx_n_s_init, 1075, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 1075, __pyx_L1_error)
+  __pyx_tuple__40 = PyTuple_Pack(4, ((PyObject *)Py_None), ((PyObject *)Py_False), ((PyObject *)Py_False), ((PyObject*)__pyx_n_u_strict)); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 1075, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -20223,31 +20146,31 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_8fastavro_5_read___pyx_scope_struct___iter_avro_records) < 0) __PYX_ERR(0, 904, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8fastavro_5_read___pyx_scope_struct___iter_avro_records) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8fastavro_5_read___pyx_scope_struct___iter_avro_records.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8fastavro_5_read___pyx_scope_struct___iter_avro_records.tp_dictoffset && __pyx_type_8fastavro_5_read___pyx_scope_struct___iter_avro_records.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8fastavro_5_read___pyx_scope_struct___iter_avro_records.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_8fastavro_5_read___pyx_scope_struct___iter_avro_records = &__pyx_type_8fastavro_5_read___pyx_scope_struct___iter_avro_records;
-  if (PyType_Ready(&__pyx_type_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks) < 0) __PYX_ERR(0, 940, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks) < 0) __PYX_ERR(0, 915, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks.tp_dictoffset && __pyx_type_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks = &__pyx_type_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks;
-  if (PyType_Ready(&__pyx_type_8fastavro_5_read___pyx_scope_struct_2___iter__) < 0) __PYX_ERR(0, 999, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8fastavro_5_read___pyx_scope_struct_2___iter__) < 0) __PYX_ERR(0, 972, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8fastavro_5_read___pyx_scope_struct_2___iter__.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8fastavro_5_read___pyx_scope_struct_2___iter__.tp_dictoffset && __pyx_type_8fastavro_5_read___pyx_scope_struct_2___iter__.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8fastavro_5_read___pyx_scope_struct_2___iter__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_8fastavro_5_read___pyx_scope_struct_2___iter__ = &__pyx_type_8fastavro_5_read___pyx_scope_struct_2___iter__;
@@ -20794,15 +20717,15 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_timezone); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_tzinfo, __pyx_t_4) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__10, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__16, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_epoch, __pyx_t_4) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "fastavro/_read.pyx":34
@@ -20810,15 +20733,15 @@
  * epoch = datetime(1970, 1, 1, tzinfo=timezone.utc)
  * epoch_naive = datetime(1970, 1, 1)             # <<<<<<<<<<<<<<
  * 
  * ctypedef int int32
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_datetime); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_epoch_naive, __pyx_t_2) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "fastavro/_read.pyx":42
  * 
@@ -20840,67 +20763,197 @@
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ReadError, __pyx_t_3) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":854
+  /* "fastavro/_read.pyx":342
+ *     named_schemas,
+ *     reader_schema=None,
+ *     options={},             # <<<<<<<<<<<<<<
+ * ):
+ *     """Arrays are encoded as a series of blocks.
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__2 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "fastavro/_read.pyx":337
+ * 
+ * 
+ * cpdef read_array(             # <<<<<<<<<<<<<<
+ *     fo,
+ *     writer_schema,
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__2 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "fastavro/_read.pyx":423
+ *     named_schemas,
+ *     reader_schema=None,
+ *     options={},             # <<<<<<<<<<<<<<
+ * ):
+ *     """Maps are encoded as a series of blocks.
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__3 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "fastavro/_read.pyx":418
+ * 
+ * 
+ * cpdef read_map(             # <<<<<<<<<<<<<<
+ *     fo,
+ *     writer_schema,
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__3 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "fastavro/_read.pyx":505
+ *     named_schemas,
+ *     reader_schema=None,
+ *     options={}             # <<<<<<<<<<<<<<
+ * ):
+ *     """A union is encoded by first writing a long value indicating the
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__5 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "fastavro/_read.pyx":500
+ * 
+ * 
+ * cpdef read_union(             # <<<<<<<<<<<<<<
+ *     fo,
+ *     writer_schema,
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__5 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "fastavro/_read.pyx":582
+ *     named_schemas,
+ *     reader_schema=None,
+ *     options={},             # <<<<<<<<<<<<<<
+ * ):
+ *     """A record is encoded by encoding the values of its fields in the order
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__6 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "fastavro/_read.pyx":577
+ * 
+ * 
+ * cpdef read_record(             # <<<<<<<<<<<<<<
+ *     fo,
+ *     writer_schema,
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__6 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "fastavro/_read.pyx":675
+ *     named_schemas,
+ *     reader_schema=None,
+ *     options={},             # <<<<<<<<<<<<<<
+ * ):
+ *     """Read data from file object according to schema."""
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__7 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "fastavro/_read.pyx":670
+ * 
+ * 
+ * cpdef _read_data(             # <<<<<<<<<<<<<<
+ *     fo,
+ *     writer_schema,
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__7 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "fastavro/_read.pyx":831
  * 
  * BLOCK_READERS = {
  *     "null": null_read_block,             # <<<<<<<<<<<<<<
  *     "deflate": deflate_read_block,
  *     "bzip2": bzip2_read_block,
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 854, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_null_read_block); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 854, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_null_read_block); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_null, __pyx_t_4) < 0) __PYX_ERR(0, 854, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_null, __pyx_t_4) < 0) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fastavro/_read.pyx":855
+  /* "fastavro/_read.pyx":832
  * BLOCK_READERS = {
  *     "null": null_read_block,
  *     "deflate": deflate_read_block,             # <<<<<<<<<<<<<<
  *     "bzip2": bzip2_read_block,
  *     "xz": xz_read_block,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_deflate_read_block); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 855, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_deflate_read_block); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 832, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_deflate, __pyx_t_4) < 0) __PYX_ERR(0, 854, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_deflate, __pyx_t_4) < 0) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fastavro/_read.pyx":856
+  /* "fastavro/_read.pyx":833
  *     "null": null_read_block,
  *     "deflate": deflate_read_block,
  *     "bzip2": bzip2_read_block,             # <<<<<<<<<<<<<<
  *     "xz": xz_read_block,
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_bzip2_read_block); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 856, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_bzip2_read_block); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 833, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_bzip2, __pyx_t_4) < 0) __PYX_ERR(0, 854, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_bzip2, __pyx_t_4) < 0) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fastavro/_read.pyx":857
+  /* "fastavro/_read.pyx":834
  *     "deflate": deflate_read_block,
  *     "bzip2": bzip2_read_block,
  *     "xz": xz_read_block,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_xz_read_block); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 857, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_xz_read_block); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 834, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_xz, __pyx_t_4) < 0) __PYX_ERR(0, 854, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_xz, __pyx_t_4) < 0) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_BLOCK_READERS, __pyx_t_2) < 0) __PYX_ERR(0, 853, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_BLOCK_READERS, __pyx_t_2) < 0) __PYX_ERR(0, 830, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":868
+  /* "fastavro/_read.pyx":845
  * 
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import snappy
  * except ImportError:
  */
   {
@@ -20908,102 +20961,102 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
     __Pyx_XGOTREF(__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_6);
     __Pyx_XGOTREF(__pyx_t_7);
     /*try:*/ {
 
-      /* "fastavro/_read.pyx":869
+      /* "fastavro/_read.pyx":846
  * 
  * try:
  *     import snappy             # <<<<<<<<<<<<<<
  * except ImportError:
  *     BLOCK_READERS["snappy"] = missing_codec_lib("snappy", "python-snappy")
  */
-      __pyx_t_2 = __Pyx_Import(__pyx_n_s_snappy, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 869, __pyx_L2_error)
+      __pyx_t_2 = __Pyx_Import(__pyx_n_s_snappy, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 846, __pyx_L2_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (PyDict_SetItem(__pyx_d, __pyx_n_s_snappy, __pyx_t_2) < 0) __PYX_ERR(0, 869, __pyx_L2_error)
+      if (PyDict_SetItem(__pyx_d, __pyx_n_s_snappy, __pyx_t_2) < 0) __PYX_ERR(0, 846, __pyx_L2_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "fastavro/_read.pyx":868
+      /* "fastavro/_read.pyx":845
  * 
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import snappy
  * except ImportError:
  */
     }
 
-    /* "fastavro/_read.pyx":873
+    /* "fastavro/_read.pyx":850
  *     BLOCK_READERS["snappy"] = missing_codec_lib("snappy", "python-snappy")
  * else:
  *     BLOCK_READERS["snappy"] = snappy_read_block             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else:*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_snappy_read_block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 873, __pyx_L4_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_snappy_read_block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 850, __pyx_L4_except_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 873, __pyx_L4_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 850, __pyx_L4_except_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_n_u_snappy, __pyx_t_2) < 0)) __PYX_ERR(0, 873, __pyx_L4_except_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_n_u_snappy, __pyx_t_2) < 0)) __PYX_ERR(0, 850, __pyx_L4_except_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     goto __pyx_L7_try_end;
     __pyx_L2_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "fastavro/_read.pyx":870
+    /* "fastavro/_read.pyx":847
  * try:
  *     import snappy
  * except ImportError:             # <<<<<<<<<<<<<<
  *     BLOCK_READERS["snappy"] = missing_codec_lib("snappy", "python-snappy")
  * else:
  */
     __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ImportError);
     if (__pyx_t_8) {
       __Pyx_AddTraceback("fastavro._read", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_4, &__pyx_t_1) < 0) __PYX_ERR(0, 870, __pyx_L4_except_error)
+      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_4, &__pyx_t_1) < 0) __PYX_ERR(0, 847, __pyx_L4_except_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "fastavro/_read.pyx":871
+      /* "fastavro/_read.pyx":848
  *     import snappy
  * except ImportError:
  *     BLOCK_READERS["snappy"] = missing_codec_lib("snappy", "python-snappy")             # <<<<<<<<<<<<<<
  * else:
  *     BLOCK_READERS["snappy"] = snappy_read_block
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_missing_codec_lib); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 871, __pyx_L4_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_missing_codec_lib); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 848, __pyx_L4_except_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 871, __pyx_L4_except_error)
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 848, __pyx_L4_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 871, __pyx_L4_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 848, __pyx_L4_except_error)
       __Pyx_GOTREF(__pyx_t_3);
-      if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_n_u_snappy, __pyx_t_9) < 0)) __PYX_ERR(0, 871, __pyx_L4_except_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_n_u_snappy, __pyx_t_9) < 0)) __PYX_ERR(0, 848, __pyx_L4_except_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L3_exception_handled;
     }
     goto __pyx_L4_except_error;
     __pyx_L4_except_error:;
 
-    /* "fastavro/_read.pyx":868
+    /* "fastavro/_read.pyx":845
  * 
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import snappy
  * except ImportError:
  */
     __Pyx_XGIVEREF(__pyx_t_5);
@@ -21015,15 +21068,15 @@
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_XGIVEREF(__pyx_t_7);
     __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_6, __pyx_t_7);
     __pyx_L7_try_end:;
   }
 
-  /* "fastavro/_read.pyx":882
+  /* "fastavro/_read.pyx":859
  * 
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import zstandard as zstd
  * except ImportError:
  */
   {
@@ -21031,103 +21084,103 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_6, &__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_7);
     __Pyx_XGOTREF(__pyx_t_6);
     __Pyx_XGOTREF(__pyx_t_5);
     /*try:*/ {
 
-      /* "fastavro/_read.pyx":883
+      /* "fastavro/_read.pyx":860
  * 
  * try:
  *     import zstandard as zstd             # <<<<<<<<<<<<<<
  * except ImportError:
  *     BLOCK_READERS["zstandard"] = missing_codec_lib("zstandard", "zstandard")
  */
-      __pyx_t_1 = __Pyx_Import(__pyx_n_s_zstandard, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 883, __pyx_L10_error)
+      __pyx_t_1 = __Pyx_Import(__pyx_n_s_zstandard, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 860, __pyx_L10_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (PyDict_SetItem(__pyx_d, __pyx_n_s_zstd, __pyx_t_1) < 0) __PYX_ERR(0, 883, __pyx_L10_error)
+      if (PyDict_SetItem(__pyx_d, __pyx_n_s_zstd, __pyx_t_1) < 0) __PYX_ERR(0, 860, __pyx_L10_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "fastavro/_read.pyx":882
+      /* "fastavro/_read.pyx":859
  * 
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import zstandard as zstd
  * except ImportError:
  */
     }
 
-    /* "fastavro/_read.pyx":887
+    /* "fastavro/_read.pyx":864
  *     BLOCK_READERS["zstandard"] = missing_codec_lib("zstandard", "zstandard")
  * else:
  *     BLOCK_READERS["zstandard"] = zstandard_read_block             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else:*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_zstandard_read_block); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 887, __pyx_L12_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_zstandard_read_block); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L12_except_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 887, __pyx_L12_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 864, __pyx_L12_except_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_n_u_zstandard, __pyx_t_1) < 0)) __PYX_ERR(0, 887, __pyx_L12_except_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_n_u_zstandard, __pyx_t_1) < 0)) __PYX_ERR(0, 864, __pyx_L12_except_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L15_try_end;
     __pyx_L10_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "fastavro/_read.pyx":884
+    /* "fastavro/_read.pyx":861
  * try:
  *     import zstandard as zstd
  * except ImportError:             # <<<<<<<<<<<<<<
  *     BLOCK_READERS["zstandard"] = missing_codec_lib("zstandard", "zstandard")
  * else:
  */
     __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ImportError);
     if (__pyx_t_8) {
       __Pyx_AddTraceback("fastavro._read", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_4, &__pyx_t_2) < 0) __PYX_ERR(0, 884, __pyx_L12_except_error)
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_4, &__pyx_t_2) < 0) __PYX_ERR(0, 861, __pyx_L12_except_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_2);
 
-      /* "fastavro/_read.pyx":885
+      /* "fastavro/_read.pyx":862
  *     import zstandard as zstd
  * except ImportError:
  *     BLOCK_READERS["zstandard"] = missing_codec_lib("zstandard", "zstandard")             # <<<<<<<<<<<<<<
  * else:
  *     BLOCK_READERS["zstandard"] = zstandard_read_block
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_missing_codec_lib); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 885, __pyx_L12_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_missing_codec_lib); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 862, __pyx_L12_except_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 885, __pyx_L12_except_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 862, __pyx_L12_except_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 885, __pyx_L12_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 862, __pyx_L12_except_error)
       __Pyx_GOTREF(__pyx_t_9);
-      if (unlikely(PyObject_SetItem(__pyx_t_9, __pyx_n_u_zstandard, __pyx_t_3) < 0)) __PYX_ERR(0, 885, __pyx_L12_except_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_9, __pyx_n_u_zstandard, __pyx_t_3) < 0)) __PYX_ERR(0, 862, __pyx_L12_except_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       goto __pyx_L11_exception_handled;
     }
     goto __pyx_L12_except_error;
     __pyx_L12_except_error:;
 
-    /* "fastavro/_read.pyx":882
+    /* "fastavro/_read.pyx":859
  * 
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import zstandard as zstd
  * except ImportError:
  */
     __Pyx_XGIVEREF(__pyx_t_7);
@@ -21139,15 +21192,15 @@
     __Pyx_XGIVEREF(__pyx_t_7);
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_6, __pyx_t_5);
     __pyx_L15_try_end:;
   }
 
-  /* "fastavro/_read.pyx":896
+  /* "fastavro/_read.pyx":873
  * 
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import lz4.block
  * except ImportError:
  */
   {
@@ -21155,103 +21208,103 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
     __Pyx_XGOTREF(__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_6);
     __Pyx_XGOTREF(__pyx_t_7);
     /*try:*/ {
 
-      /* "fastavro/_read.pyx":897
+      /* "fastavro/_read.pyx":874
  * 
  * try:
  *     import lz4.block             # <<<<<<<<<<<<<<
  * except ImportError:
  *     BLOCK_READERS["lz4"] = missing_codec_lib("lz4", "lz4")
  */
-      __pyx_t_2 = __Pyx_Import(__pyx_n_s_lz4_block, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 897, __pyx_L18_error)
+      __pyx_t_2 = __Pyx_Import(__pyx_n_s_lz4_block, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 874, __pyx_L18_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (PyDict_SetItem(__pyx_d, __pyx_n_s_lz4, __pyx_t_2) < 0) __PYX_ERR(0, 897, __pyx_L18_error)
+      if (PyDict_SetItem(__pyx_d, __pyx_n_s_lz4, __pyx_t_2) < 0) __PYX_ERR(0, 874, __pyx_L18_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "fastavro/_read.pyx":896
+      /* "fastavro/_read.pyx":873
  * 
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import lz4.block
  * except ImportError:
  */
     }
 
-    /* "fastavro/_read.pyx":901
+    /* "fastavro/_read.pyx":878
  *     BLOCK_READERS["lz4"] = missing_codec_lib("lz4", "lz4")
  * else:
  *     BLOCK_READERS["lz4"] = lz4_read_block             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else:*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_lz4_read_block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 901, __pyx_L20_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_lz4_read_block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 878, __pyx_L20_except_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 901, __pyx_L20_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 878, __pyx_L20_except_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_n_u_lz4, __pyx_t_2) < 0)) __PYX_ERR(0, 901, __pyx_L20_except_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_n_u_lz4, __pyx_t_2) < 0)) __PYX_ERR(0, 878, __pyx_L20_except_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     goto __pyx_L23_try_end;
     __pyx_L18_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "fastavro/_read.pyx":898
+    /* "fastavro/_read.pyx":875
  * try:
  *     import lz4.block
  * except ImportError:             # <<<<<<<<<<<<<<
  *     BLOCK_READERS["lz4"] = missing_codec_lib("lz4", "lz4")
  * else:
  */
     __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ImportError);
     if (__pyx_t_8) {
       __Pyx_AddTraceback("fastavro._read", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_4, &__pyx_t_1) < 0) __PYX_ERR(0, 898, __pyx_L20_except_error)
+      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_4, &__pyx_t_1) < 0) __PYX_ERR(0, 875, __pyx_L20_except_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "fastavro/_read.pyx":899
+      /* "fastavro/_read.pyx":876
  *     import lz4.block
  * except ImportError:
  *     BLOCK_READERS["lz4"] = missing_codec_lib("lz4", "lz4")             # <<<<<<<<<<<<<<
  * else:
  *     BLOCK_READERS["lz4"] = lz4_read_block
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_missing_codec_lib); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 899, __pyx_L20_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_missing_codec_lib); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 876, __pyx_L20_except_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 899, __pyx_L20_except_error)
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 876, __pyx_L20_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 899, __pyx_L20_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BLOCK_READERS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 876, __pyx_L20_except_error)
       __Pyx_GOTREF(__pyx_t_3);
-      if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_n_u_lz4, __pyx_t_9) < 0)) __PYX_ERR(0, 899, __pyx_L20_except_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_n_u_lz4, __pyx_t_9) < 0)) __PYX_ERR(0, 876, __pyx_L20_except_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L19_exception_handled;
     }
     goto __pyx_L20_except_error;
     __pyx_L20_except_error:;
 
-    /* "fastavro/_read.pyx":896
+    /* "fastavro/_read.pyx":873
  * 
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import lz4.block
  * except ImportError:
  */
     __Pyx_XGIVEREF(__pyx_t_5);
@@ -21263,284 +21316,289 @@
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_XGIVEREF(__pyx_t_7);
     __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_6, __pyx_t_7);
     __pyx_L23_try_end:;
   }
 
-  /* "fastavro/_read.pyx":904
+  /* "fastavro/_read.pyx":881
  * 
  * 
  * def _iter_avro_records(             # <<<<<<<<<<<<<<
  *     fo,
  *     header,
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8fastavro_5_read_81_iter_avro_records, NULL, __pyx_n_s_fastavro__read); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 904, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8fastavro_5_read_81_iter_avro_records, NULL, __pyx_n_s_fastavro__read); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 881, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_iter_avro_records, __pyx_t_1) < 0) __PYX_ERR(0, 904, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_iter_avro_records, __pyx_t_1) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":940
+  /* "fastavro/_read.pyx":915
  * 
  * 
  * def _iter_avro_blocks(             # <<<<<<<<<<<<<<
  *     fo,
  *     header,
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8fastavro_5_read_84_iter_avro_blocks, NULL, __pyx_n_s_fastavro__read); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 940, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8fastavro_5_read_84_iter_avro_blocks, NULL, __pyx_n_s_fastavro__read); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 915, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_iter_avro_blocks, __pyx_t_1) < 0) __PYX_ERR(0, 940, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_iter_avro_blocks, __pyx_t_1) < 0) __PYX_ERR(0, 915, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":975
+  /* "fastavro/_read.pyx":949
  * 
  * 
  * class Block:             # <<<<<<<<<<<<<<
  *     def __init__(
- *             self,
+ *         self,
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Block, __pyx_n_s_Block, (PyObject *) NULL, __pyx_n_s_fastavro__read, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 975, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Block, __pyx_n_s_Block, (PyObject *) NULL, __pyx_n_s_fastavro__read, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 949, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "fastavro/_read.pyx":976
+  /* "fastavro/_read.pyx":950
  * 
  * class Block:
  *     def __init__(             # <<<<<<<<<<<<<<
- *             self,
- *             bytes_,
+ *         self,
+ *         bytes_,
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_5Block_1__init__, 0, __pyx_n_s_Block___init, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 976, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_5Block_1__init__, 0, __pyx_n_s_Block___init, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__18);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 976, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 950, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fastavro/_read.pyx":999
- *         self.return_record_name_override = return_record_name_override
+  /* "fastavro/_read.pyx":972
+ *         self.options = options
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         for i in range(self.num_records):
  *             yield _read_data(
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_5Block_3__iter__, 0, __pyx_n_s_Block___iter, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 999, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_5Block_3__iter__, 0, __pyx_n_s_Block___iter, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 972, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_iter, __pyx_t_4) < 0) __PYX_ERR(0, 999, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_iter, __pyx_t_4) < 0) __PYX_ERR(0, 972, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fastavro/_read.pyx":1010
+  /* "fastavro/_read.pyx":982
  *             )
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return (
  *             f"Avro block: {len(self.bytes_)} bytes, {self.num_records} records, "
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_5Block_6__str__, 0, __pyx_n_s_Block___str, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1010, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_5Block_6__str__, 0, __pyx_n_s_Block___str, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 982, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_str, __pyx_t_4) < 0) __PYX_ERR(0, 1010, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_str, __pyx_t_4) < 0) __PYX_ERR(0, 982, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fastavro/_read.pyx":975
+  /* "fastavro/_read.pyx":949
  * 
  * 
  * class Block:             # <<<<<<<<<<<<<<
  *     def __init__(
- *             self,
+ *         self,
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Block, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 975, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Block, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 949, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Block, __pyx_t_4) < 0) __PYX_ERR(0, 975, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Block, __pyx_t_4) < 0) __PYX_ERR(0, 949, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":1017
+  /* "fastavro/_read.pyx":989
  * 
  * 
  * class file_reader:             # <<<<<<<<<<<<<<
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
+ *     def __init__(self, fo, reader_schema=None, options={}):
  *         self.fo = fo
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_file_reader, __pyx_n_s_file_reader, (PyObject *) NULL, __pyx_n_s_fastavro__read, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1017, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_file_reader, __pyx_n_s_file_reader, (PyObject *) NULL, __pyx_n_s_fastavro__read, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 989, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "fastavro/_read.pyx":1018
+  /* "fastavro/_read.pyx":990
  * 
  * class file_reader:
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
+ *     def __init__(self, fo, reader_schema=None, options={}):             # <<<<<<<<<<<<<<
  *         self.fo = fo
- *         self.return_record_name = return_record_name
+ *         self.options = options
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_11file_reader_1__init__, 0, __pyx_n_s_file_reader___init, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1018, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_11file_reader_1__init__, 0, __pyx_n_s_file_reader___init, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__24);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 1018, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_4, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 990, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 990, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_4)->__pyx_arg_options = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_4, __pyx_pf_8fastavro_5_read_90__defaults__);
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 990, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fastavro/_read.pyx":1062
+  /* "fastavro/_read.pyx":1032
  * 
  *     @property
  *     def schema(self):             # <<<<<<<<<<<<<<
  *         import warnings
  *         warnings.warn(
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_11file_reader_3schema, 0, __pyx_n_s_file_reader_schema, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1062, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_11file_reader_3schema, 0, __pyx_n_s_file_reader_schema, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1032, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
-  /* "fastavro/_read.pyx":1061
+  /* "fastavro/_read.pyx":1031
  *         self._elems = None
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def schema(self):
  *         import warnings
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1061, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1031, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_schema_2, __pyx_t_2) < 0) __PYX_ERR(0, 1062, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_schema_2, __pyx_t_2) < 0) __PYX_ERR(0, 1032, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":1070
+  /* "fastavro/_read.pyx":1040
  *         return self._schema
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         if not self._elems:
  *             raise NotImplementedError
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_11file_reader_5__iter__, 0, __pyx_n_s_file_reader___iter, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1070, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_11file_reader_5__iter__, 0, __pyx_n_s_file_reader___iter, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1040, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_iter, __pyx_t_2) < 0) __PYX_ERR(0, 1070, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_iter, __pyx_t_2) < 0) __PYX_ERR(0, 1040, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":1075
+  /* "fastavro/_read.pyx":1045
  *         return self._elems
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         return next(self._elems)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_11file_reader_7__next__, 0, __pyx_n_s_file_reader___next, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1075, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_11file_reader_7__next__, 0, __pyx_n_s_file_reader___next, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1045, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_next, __pyx_t_2) < 0) __PYX_ERR(0, 1075, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_next, __pyx_t_2) < 0) __PYX_ERR(0, 1045, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":1017
+  /* "fastavro/_read.pyx":989
  * 
  * 
  * class file_reader:             # <<<<<<<<<<<<<<
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
+ *     def __init__(self, fo, reader_schema=None, options={}):
  *         self.fo = fo
  */
-  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_file_reader, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1017, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_file_reader, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 989, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_reader, __pyx_t_2) < 0) __PYX_ERR(0, 1017, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_reader, __pyx_t_2) < 0) __PYX_ERR(0, 989, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastavro/_read.pyx":1079
+  /* "fastavro/_read.pyx":1049
  * 
  * 
  * class reader(file_reader):             # <<<<<<<<<<<<<<
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
+ *     def __init__(
+ *         self,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_file_reader); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1079, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_file_reader); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1049, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1079, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1049, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1079, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1049, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_reader, __pyx_n_s_reader, (PyObject *) NULL, __pyx_n_s_fastavro__read, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1079, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_reader, __pyx_n_s_reader, (PyObject *) NULL, __pyx_n_s_fastavro__read, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1049, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1079, __pyx_L1_error)
+  __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1049, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
 
-  /* "fastavro/_read.pyx":1080
+  /* "fastavro/_read.pyx":1050
  * 
  * class reader(file_reader):
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
- * 
+ *     def __init__(             # <<<<<<<<<<<<<<
+ *         self,
+ *         fo,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_6reader_1__init__, 0, __pyx_n_s_reader___init, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1080, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_6reader_1__init__, 0, __pyx_n_s_reader___init, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1050, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_t_3);
   PyList_Append(__pyx_t_9, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__33);
-  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 1080, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__37);
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 1050, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "fastavro/_read.pyx":1079
+  /* "fastavro/_read.pyx":1049
  * 
  * 
  * class reader(file_reader):             # <<<<<<<<<<<<<<
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
+ *     def __init__(
+ *         self,
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_reader, __pyx_t_2, __pyx_t_4, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1079, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_reader, __pyx_t_2, __pyx_t_4, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1049, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_CyFunction_InitClassCell(__pyx_t_9, __pyx_t_3) < 0) __PYX_ERR(0, 1079, __pyx_L1_error)
+  if (__Pyx_CyFunction_InitClassCell(__pyx_t_9, __pyx_t_3) < 0) __PYX_ERR(0, 1049, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reader, __pyx_t_3) < 0) __PYX_ERR(0, 1079, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reader, __pyx_t_3) < 0) __PYX_ERR(0, 1049, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "fastavro/_read.pyx":1093
+  /* "fastavro/_read.pyx":1074
  * 
  * 
  * class block_reader(file_reader):             # <<<<<<<<<<<<<<
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
+ *     def __init__(
+ *         self,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_file_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1093, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_file_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1074, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1093, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1074, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1093, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1074, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_block_reader, __pyx_n_s_block_reader, (PyObject *) NULL, __pyx_n_s_fastavro__read, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1093, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_block_reader, __pyx_n_s_block_reader, (PyObject *) NULL, __pyx_n_s_fastavro__read, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1074, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1093, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1074, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "fastavro/_read.pyx":1094
+  /* "fastavro/_read.pyx":1075
  * 
  * class block_reader(file_reader):
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):             # <<<<<<<<<<<<<<
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
- * 
+ *     def __init__(             # <<<<<<<<<<<<<<
+ *         self,
+ *         fo,
  */
-  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_12block_reader_1__init__, 0, __pyx_n_s_block_reader___init, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1094, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8fastavro_5_read_12block_reader_1__init__, 0, __pyx_n_s_block_reader___init, NULL, __pyx_n_s_fastavro__read, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1075, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_INCREF(__pyx_t_9);
   PyList_Append(__pyx_t_3, __pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_9);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_9, __pyx_tuple__36);
-  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_init, __pyx_t_9) < 0) __PYX_ERR(0, 1094, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_9, __pyx_tuple__40);
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_init, __pyx_t_9) < 0) __PYX_ERR(0, 1075, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "fastavro/_read.pyx":1093
+  /* "fastavro/_read.pyx":1074
  * 
  * 
  * class block_reader(file_reader):             # <<<<<<<<<<<<<<
- *     def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
- *         super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
+ *     def __init__(
+ *         self,
  */
-  __pyx_t_9 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_block_reader, __pyx_t_1, __pyx_t_4, NULL, 0, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1093, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_block_reader, __pyx_t_1, __pyx_t_4, NULL, 0, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1074, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (__Pyx_CyFunction_InitClassCell(__pyx_t_3, __pyx_t_9) < 0) __PYX_ERR(0, 1093, __pyx_L1_error)
+  if (__Pyx_CyFunction_InitClassCell(__pyx_t_3, __pyx_t_9) < 0) __PYX_ERR(0, 1074, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_block_reader, __pyx_t_9) < 0) __PYX_ERR(0, 1093, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_block_reader, __pyx_t_9) < 0) __PYX_ERR(0, 1074, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "fastavro/_read.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
@@ -23002,36 +23060,14 @@
     }
     if (ulength == 1) {
         return PyUnicode_FromOrdinal(*dpos);
     }
     return __Pyx_PyUnicode_BuildFromAscii(ulength, dpos, (int) length, prepend_sign, padding_char);
 }
 
-/* PyObjectCallNoArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
-#else
-    if (likely(PyCFunction_Check(func)))
-#endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
-        }
-    }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
     PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
@@ -23246,14 +23282,36 @@
             return -1;
         }
     }
     return 0;
 #endif
 }
 
+/* PyObjectCallNoArg */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+#if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+    }
+#endif
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+#else
+    if (likely(PyCFunction_Check(func)))
+#endif
+    {
+        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+            return __Pyx_PyObject_CallMethO(func, NULL);
+        }
+    }
+    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+}
+#endif
+
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     PyTypeObject *tp = Py_TYPE(obj);
     PyObject *descr;
     descrgetfunc f = NULL;
```

### Comparing `fastavro-1.7.4/fastavro/_read.pyi` & `fastavro-1.8.0/fastavro/_read.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -23,33 +23,37 @@
     reader_schema: Optional[Schema]
     writer_schema: Schema
     _header: Dict[str, Any]
     def __init__(
         self,
         fo_or_decoder: Union[IO, AvroJSONDecoder],
         reader_schema: Optional[Schema] = ...,
-        return_record_name: bool = ...,
+        options: Dict = ...,
     ): ...
     def __iter__(self) -> Iterator[T]: ...
     def __next__(self) -> T: ...
 
 class reader(file_reader[AvroMessage]):
     def __init__(
         self,
         fo: Union[IO, AvroJSONDecoder],
         reader_schema: Optional[Schema] = ...,
         return_record_name: bool = ...,
+        return_record_name_override: bool = ...,
+        handle_unicode_errors: str = ...,
     ): ...
 
 class block_reader(file_reader[Block]):
     def __init__(
         self,
         fo: IO,
         reader_schema: Optional[Schema] = ...,
         return_record_name: bool = ...,
+        return_record_name_override: bool = ...,
+        handle_unicode_errors: str = ...,
     ): ...
 
 class Block:
     num_records: int
     writer_schema: Dict
     reader_schema: Dict
     offset: int
@@ -59,21 +63,23 @@
         bytes_: bytes,
         num_records: int,
         codec: str,
         reader_schema: Dict,
         writer_schema: Dict,
         offset: int,
         size: int,
-        return_record_name: bool,
+        options: Dict,
     ): ...
     def __iter__(self) -> Iterator[AvroMessage]: ...
     def __str__(self) -> str: ...
 
 def schemaless_reader(
     fo: IO,
     writer_schema: Schema,
     reader_schema: Optional[Schema],
     return_record_name: bool = ...,
+    return_record_name_override: bool = ...,
+    handle_unicode_errors: str = ...,
 ) -> AvroMessage: ...
 def is_avro(path_or_buffer: Union[str, IO]) -> bool: ...
 
 BLOCK_READERS: Dict[str, Callable]
```

### Comparing `fastavro-1.7.4/fastavro/_read.pyx` & `fastavro-1.8.0/fastavro/_read.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -277,19 +277,19 @@
 
 cpdef skip_bytes(fo):
     """Bytes are encoded as a long followed by that many bytes of data."""
     cdef long64 size = read_long(fo)
     fo.read(<long>size)
 
 
-cpdef unicode read_utf8(fo):
+cpdef unicode read_utf8(fo, handle_unicode_errors="strict"):
     """A string is encoded as a long followed by that many bytes of UTF-8
     encoded character data.
     """
-    return read_bytes(fo).decode()
+    return read_bytes(fo).decode(errors=handle_unicode_errors)
 
 
 cpdef skip_utf8(fo):
     """A string is encoded as a long followed by that many bytes of UTF-8
     encoded character data.
     """
     skip_bytes(fo)
@@ -335,16 +335,15 @@
 
 
 cpdef read_array(
     fo,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     """Arrays are encoded as a series of blocks.
 
     Each block consists of a long count value, followed by that many array
     items.  A block with count zero indicates the end of the array.  Each item
     is encoded per the array's item schema.
 
@@ -369,26 +368,24 @@
         if reader_schema:
             for i in range(block_count):
                 read_items.append(_read_data(
                     fo,
                     writer_schema["items"],
                     named_schemas,
                     reader_schema["items"],
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 ))
         else:
             for i in range(block_count):
                 read_items.append(_read_data(
                     fo,
                     writer_schema["items"],
                     named_schemas,
                     None,
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 ))
         block_count = read_long(fo)
 
     return read_items
 
 
 cpdef skip_array(fo, writer_schema, named_schemas):
@@ -419,16 +416,15 @@
 
 
 cpdef read_map(
     fo,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     """Maps are encoded as a series of blocks.
 
     Each block consists of a long count value, followed by that many key/value
     pairs.  A block with count zero indicates the end of the map.  Each item is
     encoded per the map's value schema.
 
@@ -447,33 +443,31 @@
         if block_count < 0:
             block_count = -block_count
             # Read block size, unused
             read_long(fo)
 
         if reader_schema:
             for i in range(block_count):
-                key = read_utf8(fo)
+                key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
                 read_items[key] = _read_data(
                     fo,
                     writer_schema["values"],
                     named_schemas,
                     reader_schema["values"],
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 )
         else:
             for i in range(block_count):
-                key = read_utf8(fo)
+                key = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
                 read_items[key] = _read_data(
                     fo,
                     writer_schema["values"],
                     named_schemas,
                     None,
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 )
         block_count = read_long(fo)
 
     return read_items
 
 
 cpdef skip_map(fo, writer_schema, named_schemas):
@@ -504,16 +498,15 @@
 
 
 cpdef read_union(
     fo,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={}
 ):
     """A union is encoded by first writing a long value indicating the
     zero-based position within the union of the schema of its value.
 
     The value is then encoded per the indicated schema within the union.
     """
     # schema resolution
@@ -525,60 +518,53 @@
         if not isinstance(reader_schema, list):
             if match_types(idx_schema, reader_schema):
                 return _read_data(
                     fo,
                     idx_schema,
                     named_schemas,
                     reader_schema,
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 )
         else:
             for schema in reader_schema:
                 if match_types(idx_schema, schema):
                     return _read_data(
                         fo,
                         idx_schema,
                         named_schemas,
                         schema,
-                        return_record_name,
-                        return_record_name_override,
+                        options,
                     )
         msg = f"schema mismatch: {writer_schema} not found in {reader_schema}"
         raise SchemaResolutionError(msg)
     else:
+        return_record_name_override = options.get("return_record_name_override")
+        return_record_name = options.get("return_record_name")
         if return_record_name_override and is_nullable_union(writer_schema):
-            return _read_data(
-                fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
-            )
+            return _read_data(fo, idx_schema, named_schemas, None, options)
         elif return_record_name and extract_record_type(idx_schema) == "record":
             return (
                 idx_schema["name"],
                 _read_data(
                     fo,
                     idx_schema,
                     named_schemas,
                     None,
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 )
             )
         elif return_record_name and extract_record_type(idx_schema) not in AVRO_TYPES:
             # idx_schema is a named type
             return (
                 named_schemas["writer"][idx_schema]["name"],
-                _read_data(
-                    fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
-                )
+                _read_data(fo, idx_schema, named_schemas, None, options)
             )
 
         else:
-            return _read_data(
-                fo, idx_schema, named_schemas, None, return_record_name, return_record_name_override
-            )
+            return _read_data(fo, idx_schema, named_schemas, None, options)
 
 
 cpdef skip_union(fo, writer_schema, named_schemas):
     """A union is encoded by first writing a long value indicating the
     zero-based position within the union of the schema of its value.
 
     The value is then encoded per the indicated schema within the union.
@@ -589,16 +575,15 @@
 
 
 cpdef read_record(
     fo,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     """A record is encoded by encoding the values of its fields in the order
     that they are declared. In other words, a record is encoded as just the
     concatenation of the encodings of its fields.  Field values are encoded per
     their schema.
 
     Schema Resolution:
@@ -618,16 +603,15 @@
     if reader_schema is None:
         for field in writer_schema["fields"]:
             record[field["name"]] = _read_data(
                 fo,
                 field["type"],
                 named_schemas,
                 None,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
     else:
         readers_field_dict = {}
         aliases_field_dict = {}
         for f in reader_schema["fields"]:
             readers_field_dict[f["name"]] = f
             for alias in f.get("aliases", []):
@@ -640,16 +624,15 @@
             )
             if readers_field:
                 record[readers_field["name"]] = _read_data(
                     fo,
                     field["type"],
                     named_schemas,
                     readers_field["type"],
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 )
             else:
                 _skip_data(fo, field["type"], named_schemas)
 
         # fill in default values
         if len(readers_field_dict) > len(record):
             writer_fields = [f["name"] for f in writer_schema["fields"]]
@@ -685,29 +668,28 @@
 
 
 cpdef _read_data(
     fo,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     """Read data from file object according to schema."""
 
     record_type = extract_record_type(writer_schema)
 
     if reader_schema:
         reader_schema = match_schemas(writer_schema, reader_schema)
 
     try:
         if record_type == "null":
             data = read_null(fo)
         elif record_type == "string":
-            data = read_utf8(fo)
+            data = read_utf8(fo, options.get("handle_unicode_errors", "strict"))
         elif record_type == "int" or record_type == "long":
             data = read_long(fo)
         elif record_type == "float":
             data = read_float(fo)
         elif record_type == "double":
             data = read_double(fo)
         elif record_type == "boolean":
@@ -720,52 +702,47 @@
             data = read_enum(fo, writer_schema, reader_schema)
         elif record_type == "array":
             data = read_array(
                 fo,
                 writer_schema,
                 named_schemas,
                 reader_schema,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
         elif record_type == "map":
             data = read_map(
                 fo,
                 writer_schema,
                 named_schemas,
                 reader_schema,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
         elif record_type == "union" or record_type == "error_union":
             data = read_union(
                 fo,
                 writer_schema,
                 named_schemas,
                 reader_schema,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
         elif record_type == "record" or record_type == "error":
             data = read_record(
                 fo,
                 writer_schema,
                 named_schemas,
                 reader_schema,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
         else:
             return _read_data(
                 fo,
                 named_schemas["writer"][record_type],
                 named_schemas,
                 named_schemas["reader"].get(reader_schema),
-                return_record_name,
-                return_record_name_override,
+                options,
             )
     except ReadError:
         raise EOFError(f"cannot read {record_type} from {fo}")
 
     if "logicalType" in writer_schema:
         logical_type = extract_logical_type(writer_schema)
         fn = LOGICAL_READERS.get(logical_type)
@@ -904,16 +881,15 @@
 def _iter_avro_records(
     fo,
     header,
     codec,
     writer_schema,
     named_schemas,
     reader_schema,
-    return_record_name=False,
-    return_record_name_override=False,
+    options,
 ):
     cdef int32 i
 
     sync_marker = header["sync"]
 
     read_block = BLOCK_READERS.get(codec)
     if not read_block:
@@ -926,30 +902,28 @@
 
         for i in range(block_count):
             yield _read_data(
                 block_fo,
                 writer_schema,
                 named_schemas,
                 reader_schema,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
 
         skip_sync(fo, sync_marker)
 
 
 def _iter_avro_blocks(
     fo,
     header,
     codec,
     writer_schema,
     named_schemas,
     reader_schema,
-    return_record_name=False,
-    return_record_name_override=False,
+    options,
 ):
     sync_marker = header["sync"]
 
     read_block = BLOCK_READERS.get(codec)
     if not read_block:
         raise ValueError(f"Unrecognized codec: {codec}")
 
@@ -964,68 +938,64 @@
 
         skip_sync(fo, sync_marker)
 
         size = fo.tell() - offset
 
         yield Block(
             block_bytes, num_block_records, codec, reader_schema,
-            writer_schema, named_schemas, offset, size, return_record_name, return_record_name_override
+            writer_schema, named_schemas, offset, size, options,
         )
 
 
 class Block:
     def __init__(
-            self,
-            bytes_,
-            num_records,
-            codec,
-            reader_schema,
-            writer_schema,
-            named_schemas,
-            offset,
-            size,
-            return_record_name=False,
-            return_record_name_override=False):
+        self,
+        bytes_,
+        num_records,
+        codec,
+        reader_schema,
+        writer_schema,
+        named_schemas,
+        offset,
+        size,
+        options,
+    ):
         self.bytes_ = bytes_
         self.num_records = num_records
         self.codec = codec
         self.reader_schema = reader_schema
         self.writer_schema = writer_schema
         self._named_schemas = named_schemas
         self.offset = offset
         self.size = size
-        self.return_record_name = return_record_name
-        self.return_record_name_override = return_record_name_override
+        self.options = options
 
     def __iter__(self):
         for i in range(self.num_records):
             yield _read_data(
                 self.bytes_,
                 self.writer_schema,
                 self._named_schemas,
                 self.reader_schema,
-                self.return_record_name,
-                self.return_record_name_override
+                self.options,
             )
 
     def __str__(self):
         return (
             f"Avro block: {len(self.bytes_)} bytes, {self.num_records} records, "
             + f"codec: {self.codec}, position {self.offset}+{self.size}"
         )
 
 
 class file_reader:
-    def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
+    def __init__(self, fo, reader_schema=None, options={}):
         self.fo = fo
-        self.return_record_name = return_record_name
-        self.return_record_name_override= return_record_name_override
+        self.options = options
         try:
-            self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None,
-                                      return_record_name, return_record_name_override)
+            self._header = _read_data(self.fo, HEADER_SCHEMA, {}, None, self.options)
         except (StopIteration, EOFError):
             raise ValueError("cannot read header - is it an avro file?")
 
         # `meta` values are bytes. So, the actual decoding has to be external.
         self.metadata = {
             k: v.decode() for k, v in self._header["meta"].items()
         }
@@ -1073,61 +1043,92 @@
         return self._elems
 
     def __next__(self):
         return next(self._elems)
 
 
 class reader(file_reader):
-    def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
-        super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
+    def __init__(
+        self,
+        fo,
+        reader_schema=None,
+        return_record_name=False,
+        return_record_name_override=False,
+        handle_unicode_errors="strict",
+    ):
+        options = {
+            "return_record_name": return_record_name,
+            "return_record_name_override": return_record_name_override,
+            "handle_unicode_errors": handle_unicode_errors,
+        }
+        super().__init__(fo, reader_schema, options)
 
         self._elems = _iter_avro_records(self.fo,
                                          self._header,
                                          self.codec,
                                          self.writer_schema,
                                          self._named_schemas,
                                          self.reader_schema,
-                                         self.return_record_name,
-                                         self.return_record_name_override)
+                                         self.options)
 
 
 class block_reader(file_reader):
-    def __init__(self, fo, reader_schema=None, return_record_name=False, return_record_name_override=False):
-        super().__init__(fo, reader_schema, return_record_name, return_record_name_override)
+    def __init__(
+        self,
+        fo,
+        reader_schema=None,
+        return_record_name=False,
+        return_record_name_override=False,
+        handle_unicode_errors="strict",
+    ):
+        options = {
+            "return_record_name": return_record_name,
+            "return_record_name_override": return_record_name_override,
+            "handle_unicode_errors": handle_unicode_errors,
+        }
+        super().__init__(fo, reader_schema, options)
 
         self._elems = _iter_avro_blocks(self.fo,
                                         self._header,
                                         self.codec,
                                         self.writer_schema,
                                         self._named_schemas,
                                         self.reader_schema,
-                                        self.return_record_name,
-                                        self.return_record_name_override)
+                                        self.options)
 
 
-cpdef schemaless_reader(fo, writer_schema, reader_schema=None,
-                        return_record_name=False,
-                        return_record_name_override=False):
+cpdef schemaless_reader(
+    fo,
+    writer_schema,
+    reader_schema=None,
+    return_record_name=False,
+    return_record_name_override=False,
+    handle_unicode_errors="strict",
+):
     if writer_schema == reader_schema:
         # No need for the reader schema if they are the same
         reader_schema = None
 
     named_schemas = {"writer": {}, "reader": {}}
     writer_schema = parse_schema(writer_schema, named_schemas["writer"])
 
     if reader_schema:
         reader_schema = parse_schema(reader_schema, named_schemas["reader"])
 
+    options = {
+        "return_record_name": return_record_name,
+        "return_record_name_override": return_record_name_override,
+        "handle_unicode_errors": handle_unicode_errors,
+    }
     return _read_data(
         fo,
         writer_schema,
         named_schemas,
         reader_schema,
-        return_record_name,
-        return_record_name_override,
+        options,
     )
 
 
 cpdef is_avro(path_or_buffer):
     if isinstance(path_or_buffer, str):
         fp = open(path_or_buffer, "rb")
         close = True
```

### Comparing `fastavro-1.7.4/fastavro/_read_common.py` & `fastavro-1.8.0/fastavro/_read_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_read_py.py` & `fastavro-1.8.0/fastavro/_read_py.py`

 * *Files 24% similar despite different names*

```diff
@@ -118,136 +118,129 @@
 
 
 def read_null(
     decoder,
     writer_schema=None,
     named_schemas=None,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     return decoder.read_null()
 
 
 def skip_null(decoder, writer_schema=None, named_schemas=None):
     decoder.read_null()
 
 
 def read_boolean(
     decoder,
     writer_schema=None,
     named_schemas=None,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     return decoder.read_boolean()
 
 
 def skip_boolean(decoder, writer_schema=None, named_schemas=None):
     decoder.read_boolean()
 
 
 def read_int(
     decoder,
     writer_schema=None,
     named_schemas=None,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     return decoder.read_int()
 
 
 def skip_int(decoder, writer_schema=None, named_schemas=None):
     decoder.read_int()
 
 
 def read_long(
     decoder,
     writer_schema=None,
     named_schemas=None,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     return decoder.read_long()
 
 
 def skip_long(decoder, writer_schema=None, named_schemas=None):
     decoder.read_long()
 
 
 def read_float(
     decoder,
     writer_schema=None,
     named_schemas=None,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     return decoder.read_float()
 
 
 def skip_float(decoder, writer_schema=None, named_schemas=None):
     decoder.read_float()
 
 
 def read_double(
     decoder,
     writer_schema=None,
     named_schemas=None,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     return decoder.read_double()
 
 
 def skip_double(decoder, writer_schema=None, named_schemas=None):
     decoder.read_double()
 
 
 def read_bytes(
     decoder,
     writer_schema=None,
     named_schemas=None,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     return decoder.read_bytes()
 
 
 def skip_bytes(decoder, writer_schema=None, named_schemas=None):
     decoder.read_bytes()
 
 
 def read_utf8(
     decoder,
     writer_schema=None,
     named_schemas=None,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
-    return decoder.read_utf8()
+    return decoder.read_utf8(
+        handle_unicode_errors=options.get("handle_unicode_errors", "strict")
+    )
 
 
 def skip_utf8(decoder, writer_schema=None, named_schemas=None):
     decoder.read_utf8()
 
 
 def read_fixed(
     decoder,
     writer_schema,
     named_schemas=None,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     size = writer_schema["size"]
     return decoder.read_fixed(size)
 
 
 def skip_fixed(decoder, writer_schema, named_schemas=None):
     size = writer_schema["size"]
@@ -255,16 +248,15 @@
 
 
 def read_enum(
     decoder,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     symbol = writer_schema["symbols"][decoder.read_enum()]
     if reader_schema and symbol not in reader_schema["symbols"]:
         default = reader_schema.get("default")
         if default:
             return default
         else:
@@ -279,57 +271,49 @@
 
 
 def read_array(
     decoder,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     if reader_schema:
 
-        def item_reader(
-            decoder, w_schema, r_schema, return_record_name, return_record_name_override
-        ):
+        def item_reader(decoder, w_schema, r_schema, options):
             return read_data(
                 decoder,
                 w_schema["items"],
                 named_schemas,
                 r_schema["items"],
-                return_record_name,
-                return_record_name_override,
+                options,
             )
 
     else:
 
-        def item_reader(
-            decoder, w_schema, r_schema, return_record_name, return_record_name_override
-        ):
+        def item_reader(decoder, w_schema, r_schema, options):
             return read_data(
                 decoder,
                 w_schema["items"],
                 named_schemas,
                 None,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
 
     read_items = []
 
     decoder.read_array_start()
 
     for item in decoder.iter_array():
         read_items.append(
             item_reader(
                 decoder,
                 writer_schema,
                 reader_schema,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
         )
 
     decoder.read_array_end()
 
     return read_items
 
@@ -344,39 +328,36 @@
 
 
 def read_map(
     decoder,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     if reader_schema:
 
         def item_reader(decoder, w_schema, r_schema):
             return read_data(
                 decoder,
                 w_schema["values"],
                 named_schemas,
                 r_schema["values"],
-                return_record_name,
-                return_record_name_override,
+                options,
             )
 
     else:
 
         def item_reader(decoder, w_schema, r_schema):
             return read_data(
                 decoder,
                 w_schema["values"],
                 named_schemas,
                 None,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
 
     read_items = {}
 
     decoder.read_map_start()
 
     for item in decoder.iter_map():
@@ -399,79 +380,75 @@
 
 
 def read_union(
     decoder,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     # schema resolution
     index = decoder.read_index()
     idx_schema = writer_schema[index]
 
     if reader_schema:
         # Handle case where the reader schema is just a single type (not union)
         if not isinstance(reader_schema, list):
             if match_types(idx_schema, reader_schema):
                 return read_data(
                     decoder,
                     idx_schema,
                     named_schemas,
                     reader_schema,
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 )
         else:
             for schema in reader_schema:
                 if match_types(idx_schema, schema):
                     return read_data(
                         decoder,
                         idx_schema,
                         named_schemas,
                         schema,
-                        return_record_name,
-                        return_record_name_override,
+                        options,
                     )
         msg = f"schema mismatch: {writer_schema} not found in {reader_schema}"
         raise SchemaResolutionError(msg)
     else:
+        return_record_name_override = options.get("return_record_name_override")
+        return_record_name = options.get("return_record_name")
         if return_record_name_override and is_nullable_union(writer_schema):
             return read_data(
                 decoder,
                 idx_schema,
                 named_schemas,
                 None,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
         elif return_record_name and extract_record_type(idx_schema) == "record":
             return (
                 idx_schema["name"],
                 read_data(
                     decoder,
                     idx_schema,
                     named_schemas,
                     None,
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 ),
             )
         elif return_record_name and extract_record_type(idx_schema) not in AVRO_TYPES:
             # idx_schema is a named type
             return (
                 named_schemas["writer"][idx_schema]["name"],
                 read_data(
                     decoder,
                     idx_schema,
                     named_schemas,
                     None,
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 ),
             )
         else:
             return read_data(decoder, idx_schema, named_schemas)
 
 
 def skip_union(decoder, writer_schema, named_schemas):
@@ -481,16 +458,15 @@
 
 
 def read_record(
     decoder,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     """A record is encoded by encoding the values of its fields in the order
     that they are declared. In other words, a record is encoded as just the
     concatenation of the encodings of its fields.  Field values are encoded per
     their schema.
 
     Schema Resolution:
@@ -510,16 +486,15 @@
     if reader_schema is None:
         for field in writer_schema["fields"]:
             record[field["name"]] = read_data(
                 decoder,
                 field["type"],
                 named_schemas,
                 None,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
     else:
         readers_field_dict = {}
         aliases_field_dict = {}
         for f in reader_schema["fields"]:
             readers_field_dict[f["name"]] = f
             for alias in f.get("aliases", []):
@@ -532,16 +507,15 @@
             )
             if readers_field:
                 record[readers_field["name"]] = read_data(
                     decoder,
                     field["type"],
                     named_schemas,
                     readers_field["type"],
-                    return_record_name,
-                    return_record_name_override,
+                    options,
                 )
             else:
                 skip_data(decoder, field["type"], named_schemas)
 
         # fill in default values
         if len(readers_field_dict) > len(record):
             writer_fields = [f["name"] for f in writer_schema["fields"]]
@@ -618,16 +592,15 @@
 
 
 def read_data(
     decoder,
     writer_schema,
     named_schemas,
     reader_schema=None,
-    return_record_name=False,
-    return_record_name_override=False,
+    options={},
 ):
     """Read data from file object according to schema."""
 
     record_type = extract_record_type(writer_schema)
 
     if reader_schema:
         reader_schema = match_schemas(writer_schema, reader_schema)
@@ -636,16 +609,15 @@
     if reader_fn:
         try:
             data = reader_fn(
                 decoder,
                 writer_schema,
                 named_schemas,
                 reader_schema,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
         except StructError:
             raise EOFError(f"cannot read {record_type} from {decoder.fo}")
 
         if "logicalType" in writer_schema:
             logical_type = extract_logical_type(writer_schema)
             fn = LOGICAL_READERS.get(logical_type)
@@ -658,16 +630,15 @@
             return data
     else:
         return read_data(
             decoder,
             named_schemas["writer"][record_type],
             named_schemas,
             named_schemas["reader"].get(reader_schema),
-            return_record_name,
-            return_record_name_override,
+            options,
         )
 
 
 def skip_data(decoder, writer_schema, named_schemas):
     record_type = extract_record_type(writer_schema)
 
     reader_fn = SKIPS.get(record_type)
@@ -762,16 +733,15 @@
 def _iter_avro_records(
     decoder,
     header,
     codec,
     writer_schema,
     named_schemas,
     reader_schema,
-    return_record_name=False,
-    return_record_name_override=False,
+    options,
 ):
     """Return iterator over avro records."""
     sync_marker = header["sync"]
 
     read_block = BLOCK_READERS.get(codec)
     if not read_block:
         raise ValueError(f"Unrecognized codec: {codec}")
@@ -787,30 +757,28 @@
 
         for i in range(block_count):
             yield read_data(
                 BinaryDecoder(block_fo),
                 writer_schema,
                 named_schemas,
                 reader_schema,
-                return_record_name,
-                return_record_name_override,
+                options,
             )
 
         skip_sync(decoder.fo, sync_marker)
 
 
 def _iter_avro_blocks(
     decoder,
     header,
     codec,
     writer_schema,
     named_schemas,
     reader_schema,
-    return_record_name=False,
-    return_record_name_override=False,
+    options,
 ):
     """Return iterator over avro blocks."""
     sync_marker = header["sync"]
 
     read_block = BLOCK_READERS.get(codec)
     if not read_block:
         raise ValueError(f"Unrecognized codec: {codec}")
@@ -833,16 +801,15 @@
             num_block_records,
             codec,
             reader_schema,
             writer_schema,
             named_schemas,
             offset,
             size,
-            return_record_name,
-            return_record_name_override,
+            options,
         )
 
 
 class Block:
     """An avro block. Will yield records when iterated over
 
     .. attribute:: num_records
@@ -872,37 +839,34 @@
         num_records,
         codec,
         reader_schema,
         writer_schema,
         named_schemas,
         offset,
         size,
-        return_record_name=False,
-        return_record_name_override=False,
+        options,
     ):
         self.bytes_ = bytes_
         self.num_records = num_records
         self.codec = codec
         self.reader_schema = reader_schema
         self.writer_schema = writer_schema
         self._named_schemas = named_schemas
         self.offset = offset
         self.size = size
-        self.return_record_name = return_record_name
-        self.return_record_name_override = return_record_name_override
+        self.options = options
 
     def __iter__(self):
         for i in range(self.num_records):
             yield read_data(
                 BinaryDecoder(self.bytes_),
                 self.writer_schema,
                 self._named_schemas,
                 self.reader_schema,
-                self.return_record_name,
-                self.return_record_name_override,
+                self.options,
             )
 
     def __str__(self):
         return (
             f"Avro block: {len(self.bytes_)} bytes, "
             + f"{self.num_records} records, "
             + f"codec: {self.codec}, position {self.offset}+{self.size}"
@@ -910,16 +874,15 @@
 
 
 class file_reader(Generic[T]):
     def __init__(
         self,
         fo_or_decoder,
         reader_schema=None,
-        return_record_name=False,
-        return_record_name_override=False,
+        options={},
     ):
         if isinstance(fo_or_decoder, AvroJSONDecoder):
             self.decoder = fo_or_decoder
         else:
             # If a decoder was not provided, assume binary
             self.decoder = BinaryDecoder(fo_or_decoder)
 
@@ -927,27 +890,25 @@
         if reader_schema:
             self.reader_schema = parse_schema(
                 reader_schema, self._named_schemas["reader"], _write_hint=False
             )
 
         else:
             self.reader_schema = None
-        self.return_record_name = return_record_name
-        self.return_record_name_override = return_record_name_override
+        self.options = options
         self._elems = None
 
     def _read_header(self):
         try:
             self._header = read_data(
                 self.decoder,
                 HEADER_SCHEMA,
                 self._named_schemas,
                 None,
-                self.return_record_name,
-                self.return_record_name_override,
+                self.options,
             )
         except (StopIteration, EOFError):
             raise ValueError("cannot read header - is it an avro file?")
 
         # `meta` values are bytes. So, the actual decoding has to be external.
         self.metadata = {k: v.decode() for k, v in self._header["meta"].items()}
 
@@ -1007,14 +968,18 @@
         where the first value is the name of the record and the second value is
         the record itself
     return_record_name_override
         If true, this will modify the behavior of return_record_name so that
         the record name is only returned for unions where there is more than
         one record. For unions that only have one record, this option will make
         it so that the record is returned by itself, not a tuple with the name.
+    handle_unicode_errors
+        Default `strict`. Should be set to a valid string that can be used in
+        the errors argument of the string decode() function. Examples include
+        `replace` and `ignore`
 
 
     Example::
 
         from fastavro import reader
         with open('some-file.avro', 'rb') as fo:
             avro_reader = reader(fo)
@@ -1052,18 +1017,22 @@
 
     def __init__(
         self,
         fo: Union[IO, AvroJSONDecoder],
         reader_schema: Optional[Schema] = None,
         return_record_name: bool = False,
         return_record_name_override: bool = False,
+        handle_unicode_errors: str = "strict",
     ):
-        super().__init__(
-            fo, reader_schema, return_record_name, return_record_name_override
-        )
+        options = {
+            "return_record_name": return_record_name,
+            "return_record_name_override": return_record_name_override,
+            "handle_unicode_errors": handle_unicode_errors,
+        }
+        super().__init__(fo, reader_schema, options)
 
         if isinstance(self.decoder, AvroJSONDecoder):
             self.decoder.configure(self.reader_schema, self._named_schemas["reader"])
 
             self.writer_schema = self.reader_schema
             self.reader_schema = None
             self._named_schemas["writer"] = self._named_schemas["reader"]
@@ -1072,16 +1041,15 @@
             def _elems():
                 while not self.decoder.done:
                     yield read_data(
                         self.decoder,
                         self.writer_schema,
                         self._named_schemas,
                         self.reader_schema,
-                        self.return_record_name,
-                        self.return_record_name_override,
+                        self.options,
                     )
                     self.decoder.drain()
 
             self._elems = _elems()
 
         else:
             self._read_header()
@@ -1089,16 +1057,15 @@
             self._elems = _iter_avro_records(
                 self.decoder,
                 self._header,
                 self.codec,
                 self.writer_schema,
                 self._named_schemas,
                 self.reader_schema,
-                self.return_record_name,
-                self.return_record_name_override,
+                self.options,
             )
 
 
 class block_reader(file_reader[Block]):
     """Iterator over :class:`.Block` in an avro file.
 
     Parameters
@@ -1112,14 +1079,18 @@
         where the first value is the name of the record and the second value is
         the record itself
     return_record_name_override
         If true, this will modify the behavior of return_record_name so that
         the record name is only returned for unions where there is more than
         one record. For unions that only have one record, this option will make
         it so that the record is returned by itself, not a tuple with the name.
+    handle_unicode_errors
+        Default `strict`. Should be set to a valid string that can be used in
+        the errors argument of the string decode() function. Examples include
+        `replace` and `ignore`
 
 
     Example::
 
         from fastavro import block_reader
         with open('some-file.avro', 'rb') as fo:
             avro_reader = block_reader(fo)
@@ -1145,39 +1116,43 @@
 
     def __init__(
         self,
         fo: IO,
         reader_schema: Optional[Schema] = None,
         return_record_name: bool = False,
         return_record_name_override: bool = False,
+        handle_unicode_errors: str = "strict",
     ):
-        super().__init__(
-            fo, reader_schema, return_record_name, return_record_name_override
-        )
+        options = {
+            "return_record_name": return_record_name,
+            "return_record_name_override": return_record_name_override,
+            "handle_unicode_errors": handle_unicode_errors,
+        }
+        super().__init__(fo, reader_schema, options)
 
         self._read_header()
 
         self._elems = _iter_avro_blocks(
             self.decoder,
             self._header,
             self.codec,
             self.writer_schema,
             self._named_schemas,
             self.reader_schema,
-            self.return_record_name,
-            self.return_record_name_override,
+            self.options,
         )
 
 
 def schemaless_reader(
     fo: IO,
     writer_schema: Schema,
     reader_schema: Optional[Schema] = None,
     return_record_name: bool = False,
     return_record_name_override: bool = False,
+    handle_unicode_errors: str = "strict",
 ) -> AvroMessage:
     """Reads a single record written using the
     :meth:`~fastavro._write_py.schemaless_writer`
 
     Parameters
     ----------
     fo
@@ -1192,14 +1167,18 @@
         where the first value is the name of the record and the second value is
         the record itself
     return_record_name_override
         If true, this will modify the behavior of return_record_name so that
         the record name is only returned for unions where there is more than
         one record. For unions that only have one record, this option will make
         it so that the record is returned by itself, not a tuple with the name.
+    handle_unicode_errors
+        Default `strict`. Should be set to a valid string that can be used in
+        the errors argument of the string decode() function. Examples include
+        `replace` and `ignore`
 
 
     Example::
 
         parsed_schema = fastavro.parse_schema(schema)
         with open('file', 'rb') as fp:
             record = fastavro.schemaless_reader(fp, parsed_schema)
@@ -1214,21 +1193,26 @@
     writer_schema = parse_schema(writer_schema, named_schemas["writer"])
 
     if reader_schema:
         reader_schema = parse_schema(reader_schema, named_schemas["reader"])
 
     decoder = BinaryDecoder(fo)
 
+    options = {
+        "return_record_name": return_record_name,
+        "return_record_name_override": return_record_name_override,
+        "handle_unicode_errors": handle_unicode_errors,
+    }
+
     return read_data(
         decoder,
         writer_schema,
         named_schemas,
         reader_schema,
-        return_record_name,
-        return_record_name_override,
+        options,
     )
 
 
 def is_avro(path_or_buffer: Union[str, IO]) -> bool:
     """Return True if path (or buffer) points to an Avro file. This will only
     work for avro files that contain the normal avro schema header like those
     create from :func:`~fastavro._write_py.writer`. This function is not intended
```

### Comparing `fastavro-1.7.4/fastavro/_schema.c` & `fastavro-1.8.0/fastavro/_schema.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_schema.pyi` & `fastavro-1.8.0/fastavro/_schema.pyi`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_schema.pyx` & `fastavro-1.8.0/fastavro/_schema.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_schema_common.py` & `fastavro-1.8.0/fastavro/_schema_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_schema_py.py` & `fastavro-1.8.0/fastavro/_schema_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_six.c` & `fastavro-1.8.0/fastavro/_six.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_validate_common.py` & `fastavro-1.8.0/fastavro/_validate_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_validation.c` & `fastavro-1.8.0/fastavro/_validation.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_validation.pyx` & `fastavro-1.8.0/fastavro/_validation.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_validation_py.py` & `fastavro-1.8.0/fastavro/_validation_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_write.c` & `fastavro-1.8.0/fastavro/_write.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_write.pyi` & `fastavro-1.8.0/fastavro/_write.pyi`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_write.pyx` & `fastavro-1.8.0/fastavro/_write.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_write_common.py` & `fastavro-1.8.0/fastavro/_write_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/_write_py.py` & `fastavro-1.8.0/fastavro/_write_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/const.py` & `fastavro-1.8.0/fastavro/const.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/io/binary_decoder.py` & `fastavro-1.8.0/fastavro/io/binary_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,19 @@
         """Bytes are encoded as a long followed by that many bytes of data."""
         size = self.read_long()
         out = self.fo.read(size)
         if len(out) != size:
             raise EOFError(f"Expected {size} bytes, read {len(out)}")
         return out
 
-    def read_utf8(self):
+    def read_utf8(self, handle_unicode_errors="strict"):
         """A string is encoded as a long followed by that many bytes of UTF-8
         encoded character data.
         """
-        return self.read_bytes().decode()
+        return self.read_bytes().decode(errors=handle_unicode_errors)
 
     def read_fixed(self, size):
         """Fixed instances are encoded using the number of bytes declared in the
         schema."""
         out = self.fo.read(size)
         if len(out) < size:
             raise EOFError(f"Expected {size} bytes, read {len(out)}")
```

### Comparing `fastavro-1.7.4/fastavro/io/binary_encoder.py` & `fastavro-1.8.0/fastavro/io/binary_encoder.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/io/json_decoder.py` & `fastavro-1.8.0/fastavro/io/json_decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         symbol = self._parser.advance(Null())
         return self.read_value(symbol)
 
     def read_boolean(self):
         symbol = self._parser.advance(Boolean())
         return self.read_value(symbol)
 
-    def read_utf8(self):
+    def read_utf8(self, handle_unicode_errors="strict"):
         symbol = self._parser.advance(String())
         if self._parser.stack[-1] == MapKeyMarker():
             self._parser.advance(MapKeyMarker())
             for key in self._current:
                 self._key = key
                 break
             return self._key
```

### Comparing `fastavro-1.7.4/fastavro/io/json_encoder.py` & `fastavro-1.8.0/fastavro/io/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/io/parser.py` & `fastavro-1.8.0/fastavro/io/parser.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/io/symbols.py` & `fastavro-1.8.0/fastavro/io/symbols.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/json_read.py` & `fastavro-1.8.0/fastavro/json_read.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/json_write.py` & `fastavro-1.8.0/fastavro/json_write.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/read.py` & `fastavro-1.8.0/fastavro/read.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/repository/flat_dict.py` & `fastavro-1.8.0/fastavro/repository/flat_dict.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/schema.py` & `fastavro-1.8.0/fastavro/schema.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro/utils.py` & `fastavro-1.8.0/fastavro/utils.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/fastavro.egg-info/PKG-INFO` & `fastavro-1.8.0/fastavro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastavro
-Version: 1.7.4
+Version: 1.8.0
 Summary: Fast read/write of AVRO files
 Home-page: https://github.com/fastavro/fastavro
 Author: Miki Tebeka
 Author-email: miki.tebeka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fastavro-1.7.4/fastavro.egg-info/SOURCES.txt` & `fastavro-1.8.0/fastavro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/publish.sh` & `fastavro-1.8.0/publish.sh`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     true # Tag found
 else
     echo "$ver git tag not found. Make sure you run 'make tag' first"
     exit 1
 fi
 
 OSes="win_amd64
-macosx_10_15_x86_64
+macosx_11_0_x86_64
 manylinux_2_17_x86_64.manylinux2014_x86_64
 manylinux_2_17_aarch64.manylinux2014_aarch64
 musllinux_1_1_x86_64
 musllinux_1_1_aarch64"
 
 PyVers="37"
 
@@ -33,19 +33,15 @@
 PyVers="38
 39
 310
 311"
 
 for os in $OSes; do
     for pyver in $PyVers; do
-        if [[ ${os} == "macosx_10_15_x86_64" && ${pyver} == "39" ]]; then
-            wget -q --directory-prefix=dist/ https://github.com/fastavro/fastavro/releases/download/${ver}/fastavro-${ver}-cp${pyver}-cp${pyver}-macosx_11_0_x86_64.whl
-        elif [[ ${os} == "macosx_10_15_x86_64" && ${pyver} == "310" ]]; then
-            wget -q --directory-prefix=dist/ https://github.com/fastavro/fastavro/releases/download/${ver}/fastavro-${ver}-cp${pyver}-cp${pyver}-macosx_11_0_x86_64.whl
-        elif [[ ${os} == "macosx_10_15_x86_64" && ${pyver} == "311" ]]; then
+        if [[ ${os} == "macosx_11_0_x86_64" && ${pyver} == "311" ]]; then
             wget -q --directory-prefix=dist/ https://github.com/fastavro/fastavro/releases/download/${ver}/fastavro-${ver}-cp${pyver}-cp${pyver}-macosx_10_9_universal2.whl
         else
             wget -q --directory-prefix=dist/ https://github.com/fastavro/fastavro/releases/download/${ver}/fastavro-${ver}-cp${pyver}-cp${pyver}-${os}.whl
         fi
     done
 done
```

### Comparing `fastavro-1.7.4/run-tests.cmd` & `fastavro-1.8.0/run-tests.cmd`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/run-tests.sh` & `fastavro-1.8.0/run-tests.sh`

 * *Files 2% similar despite different names*

```diff
@@ -38,11 +38,11 @@
 else
     echo "skipping mypy"
 fi
 
 check-manifest
 
 # Build Cython modules
-python setup.py build_ext --inplace
-pip install -e .
+# python setup.py build_ext --inplace
+# pip install -e .
 
 PYTHONPATH=${PWD} python -m pytest --cov=fastavro -v --cov-report=term-missing --cov-report=html:build/htmlcov $@
```

### Comparing `fastavro-1.7.4/setup.py` & `fastavro-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/deflate.avro` & `fastavro-1.8.0/tests/avro-files/deflate.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/java-generated-uuid.avro` & `fastavro-1.8.0/tests/avro-files/java-generated-uuid.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/null.avro` & `fastavro-1.8.0/tests/avro-files/null.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/snappy.avro` & `fastavro-1.8.0/tests/avro-files/snappy.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/test-deflate-0.avro` & `fastavro-1.8.0/tests/avro-files/test-deflate-0.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/test-deflate-1-A.avro` & `fastavro-1.8.0/tests/avro-files/test-deflate-1-A.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/test-deflate-1.avro` & `fastavro-1.8.0/tests/avro-files/test-deflate-1.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/test-deflate-3-A.avro` & `fastavro-1.8.0/tests/avro-files/test-deflate-3-A.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/test-deflate-6-B.avro` & `fastavro-1.8.0/tests/avro-files/test-deflate-6-B.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/test-deflate-9.avro` & `fastavro-1.8.0/tests/avro-files/test-deflate-9.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/test-null-B.avro` & `fastavro-1.8.0/tests/avro-files/test-null-B.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/test-null.avro` & `fastavro-1.8.0/tests/avro-files/test-null.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/test-snappy.avro` & `fastavro-1.8.0/tests/avro-files/test-snappy.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/weather-legacy-generated.avro` & `fastavro-1.8.0/tests/avro-files/weather-legacy-generated.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/avro-files/weather-legacy-with-names.avro` & `fastavro-1.8.0/tests/avro-files/weather-legacy-with-names.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/conftest.py` & `fastavro-1.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/repository/test_flat_dict.py` & `fastavro-1.8.0/tests/repository/test_flat_dict.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_aliases.py` & `fastavro-1.8.0/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_appendable.py` & `fastavro-1.8.0/tests/test_appendable.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_block_reader.py` & `fastavro-1.8.0/tests/test_block_reader.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_canonical_form.py` & `fastavro-1.8.0/tests/test_canonical_form.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_complex.py` & `fastavro-1.8.0/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_compression.py` & `fastavro-1.8.0/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_fastavro.py` & `fastavro-1.8.0/tests/test_fastavro.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_fingerprint.py` & `fastavro-1.8.0/tests/test_fingerprint.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_json.py` & `fastavro-1.8.0/tests/test_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,15 +708,15 @@
                 self.write_object_key(value)
             else:
                 self.write_value("_" + value)
 
     class CustomJSONDecoder(AvroJSONDecoder):
         """Decoder that will prepend an underscore to all string values"""
 
-        def read_utf8(self):
+        def read_utf8(self, **kwargs):
             symbol = self._parser.advance(String())
             if self._parser.stack[-1] == MapKeyMarker():
                 self._parser.advance(MapKeyMarker())
                 for key in self._current:
                     self._key = key
                     break
                 return self._key
```

### Comparing `fastavro-1.7.4/tests/test_logical_types.py` & `fastavro-1.8.0/tests/test_logical_types.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_main_cli.py` & `fastavro-1.8.0/tests/test_main_cli.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_promotion.py` & `fastavro-1.8.0/tests/test_promotion.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_schema.py` & `fastavro-1.8.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_schema_evolution.py` & `fastavro-1.8.0/tests/test_schema_evolution.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_schemaless.py` & `fastavro-1.8.0/tests/test_schemaless.py`

 * *Files 7% similar despite different names*

```diff
@@ -262,7 +262,32 @@
         "fields": [{"name": "some_field", "type": "string", "default": "test"}],
     }
 
     test_record = {"eggs": "eggs"}
 
     with pytest.raises(ValueError, match="record contains more fields .*? eggs"):
         roundtrip(schema, test_record, writer_kwargs={"strict_allow_default": True})
+
+
+def test_unicode_decode_errors():
+    """https://github.com/fastavro/fastavro/issues/695"""
+    schema = {"type": "string"}
+
+    test_record = b"\x08\xa1\x66\x6f\x6f"
+
+    new_file = BytesIO(test_record)
+
+    new_file.seek(0)
+    with pytest.raises(UnicodeDecodeError):
+        new_record = fastavro.schemaless_reader(new_file, schema)
+
+    new_file.seek(0)
+    new_record = fastavro.schemaless_reader(
+        new_file, schema, handle_unicode_errors="replace"
+    )
+    assert new_record == "�foo"
+
+    new_file.seek(0)
+    new_record = fastavro.schemaless_reader(
+        new_file, schema, handle_unicode_errors="ignore"
+    )
+    assert new_record == "foo"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fastavro-1.7.4/tests/test_str_py3.py` & `fastavro-1.8.0/tests/test_str_py3.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_timezone.py` & `fastavro-1.8.0/tests/test_timezone.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_types.py` & `fastavro-1.8.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_utils.py` & `fastavro-1.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_validation.py` & `fastavro-1.8.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.4/tests/test_write_block.py` & `fastavro-1.8.0/tests/test_write_block.py`

 * *Files identical despite different names*

