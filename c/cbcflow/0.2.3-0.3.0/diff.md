# Comparing `tmp/cbcflow-0.2.3.tar.gz` & `tmp/cbcflow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcflow-0.2.3.tar", last modified: Fri May 19 19:22:43 2023, max compression
+gzip compressed data, was "cbcflow-0.3.0.tar", last modified: Thu Jul  6 21:26:55 2023, max compression
```

## Comparing `cbcflow-0.2.3.tar` & `cbcflow-0.3.0.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.095388 cbcflow-0.2.3/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       37 2022-09-02 21:51:00.000000 cbcflow-0.2.3/.gitattributes
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      217 2023-04-17 16:08:35.000000 cbcflow-0.2.3/.gitignore
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1533 2023-04-17 16:08:35.000000 cbcflow-0.2.3/.gitlab-ci.yml
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      873 2023-03-15 15:11:03.000000 cbcflow-0.2.3/.pre-commit-config.yaml
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1078 2023-05-10 19:01:56.000000 cbcflow-0.2.3/CHANGELOG.md
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1084 2023-04-17 16:08:35.000000 cbcflow-0.2.3/LICENSE.md
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      123 2023-04-17 16:08:35.000000 cbcflow-0.2.3/MANIFEST.in
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3027 2023-05-19 19:22:43.095388 cbcflow-0.2.3/PKG-INFO
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2390 2023-04-21 18:28:00.000000 cbcflow-0.2.3/README.md
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.703384 cbcflow-0.2.3/docs/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      613 2023-04-07 19:31:48.000000 cbcflow-0.2.3/docs/Makefile
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2022-09-02 21:51:00.000000 cbcflow-0.2.3/docs/requirements.txt
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.793385 cbcflow-0.2.3/docs/source/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.797385 cbcflow-0.2.3/docs/source/_templates/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      662 2023-04-07 19:31:48.000000 cbcflow-0.2.3/docs/source/_templates/custom-class-template.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1408 2023-04-07 19:31:48.000000 cbcflow-0.2.3/docs/source/_templates/custom-module-template.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1158 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/actionitems.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      690 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/adding-to-the-schema.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       39 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/asimov.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4404 2023-05-05 16:21:05.000000 cbcflow-0.2.3/docs/source/cbcflow-git-merging.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2616 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/conf.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1770 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/configuration.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1444 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/development-setup.rst
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.806385 cbcflow-0.2.3/docs/source/example_mini_schema/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2924 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/example_mini_schema/example.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6391 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.css
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    27212 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.html
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      984 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.min.js
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      458 2023-04-07 19:31:48.000000 cbcflow-0.2.3/docs/source/gwosc.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1255 2023-05-05 16:21:05.000000 cbcflow-0.2.3/docs/source/index.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2799 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries.rst
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.897386 cbcflow-0.2.3/docs/source/libraries_images/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.977387 cbcflow-0.2.3/docs/source/libraries_images/.ipynb_checkpoints/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72683 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     8993 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_1.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15966 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_2.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38016 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_3.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    51488 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_4.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    41435 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_5.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    54941 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_6.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    67345 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_7.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72180 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_8.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    10255 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/library-index-labelling.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1352 2023-05-10 19:01:56.000000 cbcflow-0.2.3/docs/source/library-indices.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3620 2023-05-09 00:07:03.000000 cbcflow-0.2.3/docs/source/library-setup-from-scratch.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1287 2023-05-05 16:21:05.000000 cbcflow-0.2.3/docs/source/local-library-copy-setup.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1782 2023-04-07 19:31:48.000000 cbcflow-0.2.3/docs/source/monitor-usage.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4809 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/reading-the-schema.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      106 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/schema-visualization.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15476 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/updating-metadata-from-the-command-line.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    12152 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/updating-metadata-with-the-python-api.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4916 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/what-is-metadata.rst
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.999387 cbcflow-0.2.3/examples/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7368 2022-09-29 19:29:06.000000 cbcflow-0.2.3/examples/initial_example.md
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      856 2023-04-21 18:28:00.000000 cbcflow-0.2.3/pyproject.toml
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.005387 cbcflow-0.2.3/schema/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-03-16 15:08:33.000000 cbcflow-0.2.3/schema/cbc-meta-data-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-04-25 20:47:59.000000 cbcflow-0.2.3/schema/cbc-meta-data-v2.schema
--rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-05-10 19:01:56.000000 cbcflow-0.2.3/schema/index-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1635 2023-05-19 19:22:43.097388 cbcflow-0.2.3/setup.cfg
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      567 2023-04-08 00:03:25.000000 cbcflow-0.2.3/setup.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.654384 cbcflow-0.2.3/src/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.029388 cbcflow-0.2.3/src/cbcflow/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1462 2023-04-25 20:47:59.000000 cbcflow-0.2.3/src/cbcflow/__init__.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      160 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow/_version.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    14160 2023-05-19 18:18:46.000000 cbcflow-0.2.3/src/cbcflow/asimov.py
--rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     9343 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/cbcflow.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1330 2023-04-25 20:47:59.000000 cbcflow-0.2.3/src/cbcflow/configuration.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    39799 2023-05-19 19:17:47.000000 cbcflow-0.2.3/src/cbcflow/database.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    14407 2023-05-19 19:17:47.000000 cbcflow-0.2.3/src/cbcflow/gracedb.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    14413 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/metadata.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6270 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/monitor.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5096 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/online_pe.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     9016 2023-05-16 15:26:32.000000 cbcflow-0.2.3/src/cbcflow/parser.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    35849 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/process.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.041388 cbcflow-0.2.3/src/cbcflow/schema/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow/schema/cbc-meta-data-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow/schema/cbc-meta-data-v2.schema
--rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow/schema/index-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2779 2023-04-25 20:47:59.000000 cbcflow-0.2.3/src/cbcflow/schema.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7294 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/utils.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.036388 cbcflow-0.2.3/src/cbcflow.egg-info/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3027 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/PKG-INFO
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3290 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/SOURCES.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        1 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/dependency_links.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      599 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/entry_points.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      130 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/requires.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        8 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/top_level.txt
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.048388 cbcflow-0.2.3/tests/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.077388 cbcflow-0.2.3/tests/files_for_testing/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    26759 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/cbc-meta-data-example.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5972 2023-05-05 16:21:05.000000 cbcflow-0.2.3/tests/files_for_testing/merge_test.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       56 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/test-file-for-linking-1.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       86 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/test-file-for-linking-2.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2023-05-05 16:21:05.000000 cbcflow-0.2.3/tests/files_for_testing/test-file-for-linking-3.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3091 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/update_json_1.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1221 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/update_json_2.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1626 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/update_yaml_1.yaml
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      571 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/update_yaml_2.yaml
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.094388 cbcflow-0.2.3/tests/library_for_testing/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5338 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230227hp-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4289 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230331e-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4275 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230401h-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2416 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230402dv-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3353 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230403ae-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5238 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230404hb-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3256 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230404jc-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      193 2023-04-07 19:31:48.000000 cbcflow-0.2.3/tests/library_for_testing/library.cfg
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       90 2023-04-07 19:31:48.000000 cbcflow-0.2.3/tests/library_for_testing/testing-library-index.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1838 2023-05-10 19:01:56.000000 cbcflow-0.2.3/tests/test_database.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38496 2023-05-05 16:21:05.000000 cbcflow-0.2.3/tests/test_merging.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    23545 2023-05-09 00:07:03.000000 cbcflow-0.2.3/tests/test_metadata.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      755 2023-03-27 22:27:03.000000 cbcflow-0.2.3/tests/test_schema.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.416123 cbcflow-0.3.0/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       37 2022-09-02 21:51:00.000000 cbcflow-0.3.0/.gitattributes
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      217 2023-04-17 16:08:35.000000 cbcflow-0.3.0/.gitignore
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1542 2023-06-13 21:02:31.000000 cbcflow-0.3.0/.gitlab-ci.yml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      873 2023-03-15 15:11:03.000000 cbcflow-0.3.0/.pre-commit-config.yaml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1078 2023-05-10 19:01:56.000000 cbcflow-0.3.0/CHANGELOG.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1084 2023-04-17 16:08:35.000000 cbcflow-0.3.0/LICENSE.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      123 2023-04-17 16:08:35.000000 cbcflow-0.3.0/MANIFEST.in
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3027 2023-07-06 21:26:55.417123 cbcflow-0.3.0/PKG-INFO
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2390 2023-04-21 18:28:00.000000 cbcflow-0.3.0/README.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-06-23 01:08:35.000000 cbcflow-0.3.0/asimov.log
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:54.890118 cbcflow-0.3.0/docs/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      613 2023-04-07 19:31:48.000000 cbcflow-0.3.0/docs/Makefile
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/requirements.txt
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.134120 cbcflow-0.3.0/docs/source/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.143120 cbcflow-0.3.0/docs/source/_templates/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      662 2023-04-07 19:31:48.000000 cbcflow-0.3.0/docs/source/_templates/custom-class-template.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1408 2023-04-07 19:31:48.000000 cbcflow-0.3.0/docs/source/_templates/custom-module-template.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1158 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/actionitems.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      690 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/adding-to-the-schema.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       39 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/asimov.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4404 2023-05-05 16:21:05.000000 cbcflow-0.3.0/docs/source/cbcflow-git-merging.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2616 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/conf.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1770 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/configuration.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1444 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/development-setup.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.154120 cbcflow-0.3.0/docs/source/example_mini_schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2924 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/example_mini_schema/example.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6391 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.css
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    27212 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.html
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      984 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.min.js
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      458 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/gwosc.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1255 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/index.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2799 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.323122 cbcflow-0.3.0/docs/source/libraries_images/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.325122 cbcflow-0.3.0/docs/source/libraries_images/.ipynb_checkpoints/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72683 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     8993 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_1.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15966 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_2.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38016 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_3.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    51488 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_4.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    41435 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_5.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    54941 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_6.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    67345 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_7.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72180 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_8.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    10255 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/library-index-labelling.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1352 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/library-indices.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3620 2023-05-09 00:07:03.000000 cbcflow-0.3.0/docs/source/library-setup-from-scratch.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1287 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/local-library-copy-setup.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1782 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/monitor-usage.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4809 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/reading-the-schema.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      106 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/schema-visualization.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15476 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/updating-metadata-from-the-command-line.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    12152 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/updating-metadata-with-the-python-api.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4916 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/what-is-metadata.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.328122 cbcflow-0.3.0/examples/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7368 2022-09-29 19:29:06.000000 cbcflow-0.3.0/examples/initial_example.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      856 2023-04-21 18:28:00.000000 cbcflow-0.3.0/pyproject.toml
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.333122 cbcflow-0.3.0/schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-03-16 15:08:33.000000 cbcflow-0.3.0/schema/cbc-meta-data-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-04-25 20:47:59.000000 cbcflow-0.3.0/schema/cbc-meta-data-v2.schema
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-05-10 19:01:56.000000 cbcflow-0.3.0/schema/index-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1650 2023-07-06 21:26:55.419123 cbcflow-0.3.0/setup.cfg
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      567 2023-04-08 00:03:25.000000 cbcflow-0.3.0/setup.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:54.840117 cbcflow-0.3.0/src/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.358122 cbcflow-0.3.0/src/cbcflow/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1870 2023-06-15 19:48:21.000000 cbcflow-0.3.0/src/cbcflow/__init__.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      160 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow/_version.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15920 2023-06-23 20:14:29.000000 cbcflow-0.3.0/src/cbcflow/asimov.py
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     9326 2023-05-30 19:09:00.000000 cbcflow-0.3.0/src/cbcflow/cbcflow.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1437 2023-06-23 01:08:35.000000 cbcflow-0.3.0/src/cbcflow/configuration.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    42220 2023-07-06 21:24:53.000000 cbcflow-0.3.0/src/cbcflow/database.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    14617 2023-06-23 20:14:29.000000 cbcflow-0.3.0/src/cbcflow/gracedb.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15338 2023-06-23 01:08:45.000000 cbcflow-0.3.0/src/cbcflow/metadata.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6270 2023-06-22 21:22:36.000000 cbcflow-0.3.0/src/cbcflow/monitor.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     9016 2023-05-16 15:26:32.000000 cbcflow-0.3.0/src/cbcflow/parser.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    10017 2023-06-23 20:14:29.000000 cbcflow-0.3.0/src/cbcflow/pe_scraper.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    35849 2023-05-10 19:01:56.000000 cbcflow-0.3.0/src/cbcflow/process.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.371122 cbcflow-0.3.0/src/cbcflow/schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow/schema/cbc-meta-data-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow/schema/cbc-meta-data-v2.schema
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow/schema/index-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2779 2023-04-25 20:47:59.000000 cbcflow-0.3.0/src/cbcflow/schema.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7294 2023-05-10 19:01:56.000000 cbcflow-0.3.0/src/cbcflow/utils.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.366122 cbcflow-0.3.0/src/cbcflow.egg-info/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3027 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/PKG-INFO
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3302 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        1 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      599 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/entry_points.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      144 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/requires.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        8 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/top_level.txt
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.380123 cbcflow-0.3.0/tests/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.395123 cbcflow-0.3.0/tests/files_for_testing/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    26759 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/cbc-meta-data-example.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5972 2023-05-05 16:21:05.000000 cbcflow-0.3.0/tests/files_for_testing/merge_test.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       56 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/test-file-for-linking-1.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       86 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/test-file-for-linking-2.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2023-05-05 16:21:05.000000 cbcflow-0.3.0/tests/files_for_testing/test-file-for-linking-3.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3091 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/update_json_1.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1221 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/update_json_2.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1626 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/update_yaml_1.yaml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      571 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/update_yaml_2.yaml
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.414123 cbcflow-0.3.0/tests/library_for_testing/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5338 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230227hp-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4289 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230331e-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4275 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230401h-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2416 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230402dv-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3353 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230403ae-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5238 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230404hb-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3256 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230404jc-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      193 2023-04-07 19:31:48.000000 cbcflow-0.3.0/tests/library_for_testing/library.cfg
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       90 2023-04-07 19:31:48.000000 cbcflow-0.3.0/tests/library_for_testing/testing-library-index.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3519 2023-06-02 08:52:01.000000 cbcflow-0.3.0/tests/test_database.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38496 2023-05-05 16:21:05.000000 cbcflow-0.3.0/tests/test_merging.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    32821 2023-06-23 01:08:45.000000 cbcflow-0.3.0/tests/test_metadata.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      755 2023-03-27 22:27:03.000000 cbcflow-0.3.0/tests/test_schema.py
```

### Comparing `cbcflow-0.2.3/.gitlab-ci.yml` & `cbcflow-0.3.0/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -70,8 +70,8 @@
     - mkdir public/
     - mv docs/_build/html/* public/
   artifacts:
     paths:
       - public
     expire_in: 30 days
   only:
-    - main
+    - documentation
```

### Comparing `cbcflow-0.2.3/.pre-commit-config.yaml` & `cbcflow-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/CHANGELOG.md` & `cbcflow-0.3.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/LICENSE.md` & `cbcflow-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/PKG-INFO` & `cbcflow-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.2.3
+Version: 0.3.0
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.2.3/README.md` & `cbcflow-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/Makefile` & `cbcflow-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/_templates/custom-class-template.rst` & `cbcflow-0.3.0/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/_templates/custom-module-template.rst` & `cbcflow-0.3.0/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/actionitems.rst` & `cbcflow-0.3.0/docs/source/actionitems.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/adding-to-the-schema.rst` & `cbcflow-0.3.0/docs/source/adding-to-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/cbcflow-git-merging.rst` & `cbcflow-0.3.0/docs/source/cbcflow-git-merging.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/conf.py` & `cbcflow-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/configuration.rst` & `cbcflow-0.3.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/development-setup.rst` & `cbcflow-0.3.0/docs/source/development-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/example_mini_schema/example.schema` & `cbcflow-0.3.0/docs/source/example_mini_schema/example.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.css` & `cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.css`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.html` & `cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.html`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.min.js` & `cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/index.rst` & `cbcflow-0.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/libraries.rst` & `cbcflow-0.3.0/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png` & `cbcflow-0.3.0/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/libraries_images/part_1.png` & `cbcflow-0.3.0/docs/source/libraries_images/part_1.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/libraries_images/part_2.png` & `cbcflow-0.3.0/docs/source/libraries_images/part_2.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/libraries_images/part_3.png` & `cbcflow-0.3.0/docs/source/libraries_images/part_3.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/libraries_images/part_4.png` & `cbcflow-0.3.0/docs/source/libraries_images/part_4.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/libraries_images/part_5.png` & `cbcflow-0.3.0/docs/source/libraries_images/part_5.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/libraries_images/part_6.png` & `cbcflow-0.3.0/docs/source/libraries_images/part_6.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/libraries_images/part_7.png` & `cbcflow-0.3.0/docs/source/libraries_images/part_7.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/libraries_images/part_8.png` & `cbcflow-0.3.0/docs/source/libraries_images/part_8.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/library-index-labelling.rst` & `cbcflow-0.3.0/docs/source/library-index-labelling.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/library-indices.rst` & `cbcflow-0.3.0/docs/source/library-indices.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/library-setup-from-scratch.rst` & `cbcflow-0.3.0/docs/source/library-setup-from-scratch.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/local-library-copy-setup.rst` & `cbcflow-0.3.0/docs/source/local-library-copy-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/monitor-usage.rst` & `cbcflow-0.3.0/docs/source/monitor-usage.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/reading-the-schema.rst` & `cbcflow-0.3.0/docs/source/reading-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/updating-metadata-from-the-command-line.rst` & `cbcflow-0.3.0/docs/source/updating-metadata-from-the-command-line.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/updating-metadata-with-the-python-api.rst` & `cbcflow-0.3.0/docs/source/updating-metadata-with-the-python-api.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/docs/source/what-is-metadata.rst` & `cbcflow-0.3.0/docs/source/what-is-metadata.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/examples/initial_example.md` & `cbcflow-0.3.0/examples/initial_example.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/pyproject.toml` & `cbcflow-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/schema/cbc-meta-data-v1.schema` & `cbcflow-0.3.0/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/schema/cbc-meta-data-v2.schema` & `cbcflow-0.3.0/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/schema/index-v1.schema` & `cbcflow-0.3.0/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/setup.cfg` & `cbcflow-0.3.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 	lscsoft-glue
 	coverage
 	python-benedict
 	jsonmerge
 	PyYAML
 	gwpy
 	python-crontab
+	python-gitlab
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 asimov.hooks.postmonitor = 
 	cbcflow = cbcflow.asimov:Collector
```

### Comparing `cbcflow-0.2.3/setup.py` & `cbcflow-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/src/cbcflow/__init__.py` & `cbcflow-0.3.0/src/cbcflow/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 from typing import Union
 
 from . import _version
 from .utils import setup_logger
 from .cbcflow import from_file, setup_args_metadata
 from .configuration import get_cbcflow_config
 from .metadata import MetaData
+from .database import LocalLibraryDatabase
 from .monitor import generate_crondor, generate_crontab, run_monitor
 from .parser import get_parser_and_default_data
 from .schema import get_schema
 
 __version__ = _version.__version__
 
 
 def get_superevent(
-    sname: str, library: Union[str, None] = None, no_git_library: bool = False
+    sname: str,
+    library: Union[str, "LocalLibraryDatabase", None] = None,
+    no_git_library: bool = False,
 ):
     """
     A helper method to easily fetch information on a given superevent.
 
     Parameters
     ==========
     sname : str
         The sname of the superevent in question, according to GraceDB
-    library : str | None
+    library : str | `cbcflow.database.LocalLibraryDatabase` | None
         The library from which to fetch information
     no_git_library : bool
         If true, don't attempt to treat this library as a git repository
 
     Returns
     =======
     cbcflow.metadata.MetaData
@@ -37,16 +40,25 @@
     schema = get_schema()
     _, default_data = get_parser_and_default_data(schema)
 
     if library is None:
         config_defaults = get_cbcflow_config()
         library = config_defaults["library"]
 
-    metadata = MetaData(
-        sname,
-        local_library_path=library,
-        default_data=default_data,
-        schema=schema,
-        no_git_library=no_git_library,
-    )
+    if isinstance(library, LocalLibraryDatabase):
+        metadata = MetaData(
+            sname,
+            local_library=library,
+            default_data=default_data,
+            schema=schema,
+            no_git_library=no_git_library,
+        )
+    else:
+        metadata = MetaData(
+            sname,
+            local_library_path=library,
+            default_data=default_data,
+            schema=schema,
+            no_git_library=no_git_library,
+        )
 
     return metadata
```

### Comparing `cbcflow-0.2.3/src/cbcflow/asimov.py` & `cbcflow-0.3.0/src/cbcflow/asimov.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,18 @@
     supported_pipelines = ["bayeswave", "bilby", "rift"]
 
     def __init__(self, ledger):
         """
         Collect data from the asimov ledger and write it to a CBCFlow library.
         """
         hook_data = ledger.data["hooks"]["postmonitor"]["cbcflow"]
-        self.library = hook_data["library location"]
+        self.library = cbcflow.database.LocalLibraryDatabase(
+            hook_data["library location"]
+        )
+        self.library.git_pull_from_remote(automated=True)
         self.schema_section = hook_data["schema section"]
         self.ledger = ledger
 
     def run(self):
         """
         Run the hook.
         """
@@ -38,63 +41,98 @@
             # Do setup for the event
             output = {}
             output[self.schema_section] = {}
             pe = output[self.schema_section]["Results"] = []
             metadata = cbcflow.get_superevent(
                 event.meta["ligo"]["sname"], library=self.library
             )
+
+            # Get the metadata that already exists for reference
+            metadata_pe_results = metadata["ParameterEstimation"]["Results"]
+            metadata_pe_results_uids = cbcflow.utils.get_uids_from_object_array(
+                metadata_pe_results
+            )
             for analysis in event.productions:
                 if str(analysis.pipeline).lower() in self.supported_pipelines:
                     analysis_output = {}
                     analysis_output["UID"] = analysis.name
+
+                    if analysis.name in metadata_pe_results_uids:
+                        corresponding_analysis = metadata_pe_results[
+                            metadata_pe_results_uids.index(analysis.name)
+                        ]
+                    else:
+                        corresponding_analysis = None
+
                     analysis_output["InferenceSoftware"] = str(analysis.pipeline)
                     if analysis.status.lower() in self.status_map.keys():
                         analysis_output["RunStatus"] = self.status_map[
                             analysis.status.lower()
                         ]
                     if "waveform" in analysis.meta:
                         if "approximant" in analysis.meta["waveform"]:
                             analysis_output["WaveformApproximant"] = str(
                                 analysis.meta["waveform"]["approximant"]
                             )
+
                     try:
                         ini = analysis.pipeline.production.event.repository.find_prods(
                             analysis.pipeline.production.name,
                             analysis.pipeline.category,
                         )[0]
                         analysis_output["ConfigFile"] = {}
                         analysis_output["ConfigFile"]["Path"] = ini
                     except IndexError:
                         logger.warning("Could not find ini file for this analysis")
+
+                    analysis_output["Notes"] = []
+
                     if analysis.comment is not None:
-                        analysis_output["Notes"] = [analysis.comment]
+                        # We only want to add the comment to the notes if it doesn't already exist
+                        if corresponding_analysis is None:
+                            analysis_output["Notes"].append(analysis.comment)
+                        elif analysis.comment not in corresponding_analysis["Notes"]:
+                            analysis_output["Notes"].append(analysis.comment)
+
                     if analysis.review.status:
                         if analysis.review.status.lower() == "approved":
                             analysis_output["ReviewStatus"] = "pass"
                         elif analysis.review.status.lower() == "rejected":
                             analysis_output["ReviewStatus"] = "fail"
                         elif analysis.review.status.lower() == "deprecated":
                             analysis_output["Deprecated"] = True
                         messages = sorted(
                             analysis.review.messages, key=lambda k: k.timestamp
                         )
                         if len(messages) > 0:
-                            analysis_output["Notes"].append(
+                            if corresponding_analysis is None:
+                                analysis_output["Notes"].append(
+                                    f"{messages[0].timestamp:%Y-%m-%d}: {messages[0].message}"
+                                )
+                            elif (
                                 f"{messages[0].timestamp:%Y-%m-%d}: {messages[0].message}"
-                            )
+                                in corresponding_analysis["Notes"]
+                            ):
+                                analysis_output["Notes"].append(
+                                    f"{messages[0].timestamp:%Y-%m-%d}: {messages[0].message}"
+                                )
+
                     if analysis.finished:
                         # Get the results
                         results = analysis.pipeline.collect_assets()
+
                         if str(analysis.pipeline).lower() == "bayeswave":
                             # If the pipeline is Bayeswave, we slot each psd into its designated spot
                             analysis_output["BayeswaveResults"] = {}
+
                             for ifo, psd in results["psds"].items():
-                                analysis_output["BayeswaveResults"][f"{ifo}PSD"][
-                                    "Path"
-                                ] = psd
+                                analysis_output["BayeswaveResults"][f"{ifo}PSD"] = {
+                                    "Path": psd
+                                }
+
                             if analysis_output["BayeswaveResults"] == {}:
                                 # Cleanup if we fail to write any results
                                 analysis_output.pop("BayeswaveResults")
                         elif str(analysis.pipeline).lower() == "bilby":
                             # If it's bilby, we need to parse out which of possibly multiple merge results we want
                             analysis_output["ResultFile"] = {}
                             if len(results["samples"]) == 0:
@@ -202,23 +240,27 @@
                 else:
                     logger.info(
                         f"Pipeline {analysis.pipeline} is not supported by cbcflow"
                     )
                     logger.info(
                         "If this is a mistake, please contact the cbcflow developers to add support."
                     )
+        self.library.git_push_to_remote()
 
 
 class Applicator:
     """Apply information from CBCFlow to an asimov event"""
 
     def __init__(self, ledger):
         hook_data = ledger.data["hooks"]["applicator"]["cbcflow"]
         self.ledger = ledger
-        self.library = hook_data["library location"]
+        self.library = cbcflow.database.LocalLibraryDatabase(
+            hook_data["library location"]
+        )
+        self.library.git_pull_from_remote(automated=True)
 
     def run(self, sid=None):
 
         metadata = cbcflow.get_superevent(sid, library=self.library)
         detchar = metadata.data["DetectorCharacterization"]
         grace = metadata.data["GraceDB"]
         ifos = detchar["RecommendedDetectors"]
@@ -237,15 +279,15 @@
         ifo_list = []
 
         for ifo in ifos:
             # Grab IFO specific quantities
             ifo_name = ifo["UID"]
             ifo_list.append(ifo_name)
             if "RecommendedDuration" in detchar.keys():
-                data["segment length"] = detchar["RecommendedDuration"]
+                data["segment length"] = int(detchar["RecommendedDuration"])
             if "RecommendedMaximumFrequency" in ifo.keys():
                 max_f[ifo_name] = ifo["RecommendedMaximumFrequency"]
             if "RecommendedMinimumFrequency" in ifo.keys():
                 min_f[ifo_name] = ifo["RecommendedMinimumFrequency"]
             if "RecommendedChannel" in ifo.keys():
                 channels[ifo_name] = ifo["RecommendedChannel"]
             if "FrameType" in ifo.keys():
```

### Comparing `cbcflow-0.2.3/src/cbcflow/cbcflow.py` & `cbcflow-0.3.0/src/cbcflow/cbcflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import glob
 import json
 from typing import Tuple
 
 
 from .configuration import config_defaults
 from .gracedb import fetch_gracedb_information
-from .online_pe import add_onlinepe_information
+from .pe_scraper import add_pe_information
 from .metadata import MetaData
 from .database import LocalLibraryDatabase
 from .parser import get_parser_and_default_data, sname_string
 from .process import process_user_input
 from .schema import get_schema
 from .utils import setup_logger
 
@@ -58,16 +58,16 @@
 
     default_metadata = copy.deepcopy(metadata)
 
     # Pull information from GraceDB
     gdb_data = fetch_gracedb_information(args.sname, args.gracedb_service_url)
     metadata.data.update(gdb_data)
 
-    # Pull information from onlinePE
-    add_onlinepe_information(metadata, args.sname)
+    # Pull information from PE
+    add_pe_information(metadata, args.sname)
 
     try:
         metadata.write_to_library(branch_name=args.branch_name)
     except jsonschema.exceptions.ValidationError:
         logger.info(
             "Recorded meta-data cannot be validated against current schema\n\
             Accordingly, the local library will not be updated"
```

### Comparing `cbcflow-0.2.3/src/cbcflow/configuration.py` & `cbcflow-0.3.0/src/cbcflow/configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,13 +33,15 @@
         section_key = "cbcflow"
         if section_key not in config.sections():
             raise ValueError(f"You need a [cbcflow] section header in {cfile}")
         section = config[section_key]
         for key in config_defaults:
             if key in list(section.keys()):
                 config_defaults[key] = section[key]
+                if config_defaults[key].lower() == "none":
+                    config_defaults[key] = None
     else:
         logger.info("Could not read config file, falling back on defaults.")
     return config_defaults
 
 
 config_defaults = get_cbcflow_config()
```

### Comparing `cbcflow-0.2.3/src/cbcflow/database.py` & `cbcflow-0.3.0/src/cbcflow/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     get_all_schema_def_defaults,
     get_simple_schema_defaults,
     process_update_json,
     process_merge_json,
 )
 from .schema import get_schema
 from .gracedb import fetch_gracedb_information
-from .online_pe import add_onlinepe_information
+from .pe_scraper import add_pe_information
 from .utils import get_dumpable_json_diff, setup_logger
 
 logger = setup_logger()
 
 
 class Labeller(object):
     """A generic parent class for labellers,
@@ -219,38 +219,56 @@
     """The LibraryParent class to use when the parent is GraceDB"""
 
     def __init__(
         self,
         service_url: str,
         library: "LocalLibraryDatabase",
         cred: Union[Tuple[str, str], str, None] = None,
+        pe_rota_token_path: Union[str, None] = None,
     ) -> None:
         """Setup the GraceDbDatabase that this library pairs to
 
         Parameters
         ==========
         service_url : str
             The http address for the gracedb instance that this library pairs to
         library : `LocalLibraryDatabase`
             The library for which this serves as a parent.
+        cred : Union[Tuple[str, str], str, None]
+            The credentials to pass when accessing gracedb
+        pe_rota_token_path : str
+            The path to the token to use when accessing the PE rota
         """
         super(GraceDbDatabase, self).__init__(source_path=service_url, library=library)
         self.cred = cred
+        self.pe_rota_token = pe_rota_token_path
 
     @property
     def cred(self) -> Union[Tuple[str, str], str, None]:
         """Information on the credentials to pass to GraceDb, per
         https://ligo-gracedb.readthedocs.io/en/latest/api.html#ligo.gracedb.rest.GraceDb
         """
         return self._cred
 
     @cred.setter
     def cred(self, input_cred: Union[Tuple[str, str], str, None]) -> None:
         self._cred = input_cred
 
+    @property
+    def pe_rota_token(self) -> Union[None, str]:
+        return self._pe_rota_token
+
+    @pe_rota_token.setter
+    def pe_rota_token(self, path_name: str) -> None:
+        if path_name is not None:
+            with open(path_name, "r") as file:
+                self._pe_rota_token = file.read().strip()
+        else:
+            self._pe_rota_token = None
+
     def pull(self, sname: str) -> dict:
         """Pull information on the superevent with this sname from GraceDB
 
         Parameters
         ==========
         sname : str
             The sname for the superevent in question
@@ -309,18 +327,30 @@
                         default_data=self.library.metadata_default_data,
                     )
                 try:
                     backup_data = copy.deepcopy(metadata.data)
 
                     # Pull information from GraceDB
                     gdb_data = self.pull(superevent_id)
+                    for note in metadata["Info"]["Notes"]:
+                        # If a note already marks this as retracted don't add another
+                        if "retracted" in note.lower():
+                            gdb_data.pop("Info")
+                            break
                     metadata.data.update(gdb_data)
 
-                    # Pull information from onlinePE
-                    add_onlinepe_information(metadata, superevent_id)
+                    try:
+                        # Pull information from PE
+                        add_pe_information(metadata, superevent_id, self.pe_rota_token)
+                    except Exception as e:
+                        logger.warning("Fatal error while scraping PE automatically")
+                        logger.warning(
+                            "Proceeding automatically to maintain library status as best as possible"
+                        )
+                        logger.warning(f"The exception was {e}")
 
                     changes = metadata.get_diff()
                     if "GraceDB" in changes.keys() and len(changes.keys()) == 1:
                         if len(changes["GraceDB"].keys()) == 1:
                             continue
                         # This is a hack to make it not update if the only update would be "LastUpdate"
                         # It may have to change in further schema versions
@@ -481,16 +511,26 @@
                     cred = ast.literal_eval(self.library_config["Monitor"]["cred"])
                 else:
                     logger.info("Using path to credential proxy file")
                     cred = self.library_config["Monitor"]["cred"]
             else:
                 logger.info("Using default credentials")
                 cred = None
+            if self.library_config["Monitor"]["pe_rota_token"] is not None:
+                if self.library_config["Monitor"]["pe_rota_token"].lower() != "none":
+                    pe_rota_token_path = self.library_config["Monitor"]["pe_rota_token"]
+                else:
+                    pe_rota_token_path = None
+            else:
+                pe_rota_token_path = None
             self._library_parent = GraceDbDatabase(
-                service_url=source_path, library=self, cred=cred
+                service_url=source_path,
+                library=self,
+                cred=cred,
+                pe_rota_token_path=pe_rota_token_path,
             )
         elif os.path.exists(source_path):
             # This will be the branch for pulling from a git repo in the local filesystem
             pass
         elif "https" in source_path:
             # This will be the branch for pulling from a non-local git repo on e.g. gitlab
             pass
@@ -546,21 +586,24 @@
             )
             for f in self.filelist
         ]
         for md in metadata_list:
             metadata_dict[md.sname] = md
         self.metadata_dict.update(metadata_dict)
 
-    @property
-    def downselected_metadata_dict(self) -> Dict[str, MetaData]:
-        """The metadata of events that satisfy library inclusion criteria, labelled by sname"""
+    @cached_property
+    def downselected_metadata_keys(self) -> Dict[str, MetaData]:
+
         from gwpy.time import to_gps
 
-        downselected_metadata_dict = dict()
-        self.load_library_metadata_dict()
+        self._downselected_metadata_has_been_computed = True
+
+        downselected_metadata_keys = list()
+        if self.metadata_dict.keys() != self.superevents_in_library:
+            self.load_library_metadata_dict()
         for sname, metadata in self.metadata_dict.items():
             library_created_earliest = to_gps(
                 self.library_config["Events"]["created-since"]
             )
             library_created_latest = to_gps(
                 self.library_config["Events"]["created-before"]
             )
@@ -573,26 +616,37 @@
             if preferred_far == 1 or preferred_time == 0:
                 logger.warning(
                     f"No preferred event was identified for superevent {sname}: something is seriously wrong!\n\
                         Accordingly, this event will not be included in downselected_metadata_dict"
                 )
                 continue
             if sname in self.library_config["Events"]["snames-to-include"]:
-                downselected_metadata_dict[sname] = metadata
+                downselected_metadata_keys.append(sname)
             elif sname in self.library_config["Events"]["snames-to-exclude"]:
                 pass
             elif (
                 preferred_time < library_created_earliest
                 or preferred_time > library_created_latest
             ):
                 continue
             # Right now we *only* check date, FAR threshold, and specific inclusion
             elif preferred_far <= float(self.library_config["Events"]["far-threshold"]):
-                downselected_metadata_dict[sname] = metadata
-        return downselected_metadata_dict
+                downselected_metadata_keys.append(sname)
+        return downselected_metadata_keys
+
+    @property
+    def downselected_metadata_dict(self) -> dict:
+        """The metadata of events that satisfy library inclusion criteria, labelled by sname"""
+        if not hasattr(self, "downselected_metadata_keys"):
+            self.downselected_metadata_keys
+        return {
+            sname: metadata
+            for sname, metadata in self.metadata_dict.items()
+            if sname in self.downselected_metadata_keys
+        }
 
     def validate(self, data) -> None:
         """Check that data satisfies the metadata schema
 
         Parameters
         ==========
         data : dict
@@ -616,15 +670,19 @@
             "far-threshold": 1.2675e-7,
             "pastro-threshold": 0.5,
             "created-since": "2022-01-01",
             "created-before": "now",
             "snames-to-include": [],
             "snames-to-exclude": [],
         }
-        library_defaults["Monitor"] = {"parent": "gracedb", "cred": None}
+        library_defaults["Monitor"] = {
+            "parent": "gracedb",
+            "cred": None,
+            "pe_rota_token": None,
+        }
         if os.path.exists(config_file):
             config.read(config_file)
             for section_key in config.sections():
                 if section_key not in library_defaults.keys():
                     library_defaults[section_key] = dict()
                 section = config[section_key]
                 for key in section.keys():
@@ -745,37 +803,37 @@
             The file from head (changes being applied)
         most_recent_common_ancestor_file : str
             The file from the MRCA (last commit shared by head and base)
         """
         # `cbcflow.process.process_merge_json handles the logic for us`
         # We just need to load in files here
         try:
+            with open(most_recent_common_ancestor_file, "r") as file:
+                mrca_json = json.load(file)
+        except json.decoder.JSONDecodeError as e:
+            logger.info(
+                f"Could not read head with error {e}, proceeding as if it's empty"
+            )
+            mrca_json = {}
+        try:
             with open(our_file, "r") as file:
                 head_json = json.load(file)
         except json.decoder.JSONDecodeError as e:
             logger.info(
                 f"Could not read head with error {e}, proceeding as if it's empty"
             )
-            head_json = {}
+            head_json = copy.deepcopy(mrca_json)
         try:
             with open(their_file, "r") as file:
                 base_json = json.load(file)
         except json.decoder.JSONDecodeError as e:
             logger.info(
                 f"Could not read base with error {e}, proceeding as if it's empty"
             )
-            base_json = {}
-        try:
-            with open(most_recent_common_ancestor_file, "r") as file:
-                mrca_json = json.load(file)
-        except json.decoder.JSONDecodeError as e:
-            logger.info(
-                f"Could not read head with error {e}, proceeding as if it's empty"
-            )
-            mrca_json = {}
+            base_json = copy.deepcopy(mrca_json)
 
         # Now get the merged json and the return status
         merge_json, return_status = process_merge_json(
             base_json=base_json,
             head_json=head_json,
             mrca_json=mrca_json,
             schema=self.metadata_schema,
```

### Comparing `cbcflow-0.2.3/src/cbcflow/gracedb.py` & `cbcflow-0.3.0/src/cbcflow/gracedb.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,30 +35,32 @@
 
     if service_url is None:
         from .configuration import config_defaults
 
         service_url = config_defaults["gracedb_service_url"]
         logger.info("Using configuration default GraceDB service_url")
 
-    data = dict(GraceDB=dict(Events=[]), Cosmology=dict())
+    data = dict(GraceDB=dict(Events=[]), Cosmology=dict(), Info=dict(Notes=[]))
 
     with GraceDb(service_url=service_url, cred=cred) as gdb:
         try:
             # Get the json of metadata for the superevent
             superevent = gdb.superevent(sname).json()
         except HTTPError:
             msg = f"Superevent {sname} not found on {service_url}. "
             msg += "Either it does not exist, or you may need to run ligo-proxy-init."
             raise ValueError(msg)
         # We want the one best event per pipeline
         event_dict = superevent["pipeline_preferred_events"]
         preferred_event = superevent["preferred_event_data"]
+        if "ADVNO" in superevent["labels"]:
+            # If ADVNO is here that means this event is retracted
+            data["Info"]["Notes"].append("Retracted: ADVNO applied in GraceDB")
         if len(event_dict) == 0:
             event_dict[preferred_event["pipeline"]] = preferred_event
-
         for pipeline, event in superevent["pipeline_preferred_events"].items():
             if pipeline.lower().strip() in ["spiir", "mbta", "gstlal", "pycbc"]:
                 try:
                     event_data = dict()
                     # Get the
                     gname = event["graceid"]
                     # Get the preferred event across pipelines
@@ -243,21 +245,21 @@
                         ifo_line = [
                             line for line in trigger_file_lines if "ifo:" in line
                         ][0]
                         sSNR_line = [
                             line for line in trigger_file_lines if "sSNR:" in line
                         ][0]
                         # More string hacking to get ifos
-                        ifos = ifo_line.split("")[1].strip().split()
+                        ifos = ifo_line.split(" ")[1].strip().split()
                         # More string hacking to get sSNRs
                         snrs = [
                             float(x) for x in sSNR_line.split(":")[1].strip().split()
                         ]
                         # Loop to assign SNRs by IFO
-                        for ii, ifo in ifos.enumerate():
+                        for ii, ifo in enumerate(ifos):
                             event_data[f"{ifo}SNR"] = snrs[ii]
                     except HTTPError:
                         logger.warning(
                             f"Was not able to access trigger.txt for G-event {gname}"
                         )
 
                     try:
```

### Comparing `cbcflow-0.2.3/src/cbcflow/metadata.py` & `cbcflow-0.3.0/src/cbcflow/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import os
 import subprocess
 import sys
 from typing import TYPE_CHECKING, Union
 
 import jsondiff
+import jsonschema
 
 from .process import process_update_json
 from .utils import get_date_last_modified
 from .parser import get_parser_and_default_data
 from .schema import get_schema
 from .utils import setup_logger
 
@@ -82,14 +83,22 @@
             logger.info("No library file: creating defaults")
             default_data["Sname"] = self.sname
             self.library.validate(default_data)
             self.data = default_data
 
         self.library.metadata_dict[sname] = self
 
+    def __getitem__(self, item):
+        """The helper method required to make subscripting metadata work the way you think it should"""
+        return self.data[item]
+
+    def __str__(self):
+        """The string representation of the metadata's data"""
+        return json.dumps(self.data, indent=4)
+
     ############################################################################
     ############################################################################
     ####                  System Properties and Operations                  ####
     ############################################################################
     ############################################################################
 
     @property
@@ -180,14 +189,33 @@
         Returns
         =======
         str
             The date and time last modified in iso standard (yyyy-MM-dd hh:mm:ss)
         """
         return get_date_last_modified(self.library_file)
 
+    def validate(self) -> bool:
+        """Check whether this metadata is valid under the schema
+
+        Returns
+        =======
+        bool
+            Whether the metadata is valid
+
+        """
+        try:
+            self.library.validate(self.data)
+            return True
+        except jsonschema.ValidationError as e:
+            logger.info("Validation failed with message:" f"{e}")
+            return False
+        except jsonschema.SchemaError as e:
+            logger.info("Schema failed with message" f"{e}")
+            return False
+
     ############################################################################
     ############################################################################
     ####                   Read Write and Update Methods                    ####
     ############################################################################
     ############################################################################
 
     @staticmethod
@@ -256,14 +284,15 @@
         try:
             self.library.validate(new_metadata_data)
         except jsonschema.ValidationError as e:
             logger.warning("Failed to validate")
             logger.warning(f"Changes are {jsondiff.diff(new_metadata_data, self.data)}")
             raise jsonschema.ValidationError(e.message)
         self.data = new_metadata_data
+        self.library.metadata_dict[self.sname] = self
 
     def load_from_library(self) -> None:
         """Load metadata from a library"""
         with open(self.library_file, "r") as file:
             data = json.load(file)
 
         self.library.validate(data)
```

### Comparing `cbcflow-0.2.3/src/cbcflow/monitor.py` & `cbcflow-0.3.0/src/cbcflow/monitor.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/src/cbcflow/parser.py` & `cbcflow-0.3.0/src/cbcflow/parser.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/src/cbcflow/process.py` & `cbcflow-0.3.0/src/cbcflow/process.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/src/cbcflow/schema/cbc-meta-data-v1.schema` & `cbcflow-0.3.0/src/cbcflow/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/src/cbcflow/schema/cbc-meta-data-v2.schema` & `cbcflow-0.3.0/src/cbcflow/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/src/cbcflow/schema/index-v1.schema` & `cbcflow-0.3.0/src/cbcflow/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/src/cbcflow/schema.py` & `cbcflow-0.3.0/src/cbcflow/schema.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/src/cbcflow/utils.py` & `cbcflow-0.3.0/src/cbcflow/utils.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/src/cbcflow.egg-info/PKG-INFO` & `cbcflow-0.3.0/src/cbcflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.2.3
+Version: 0.3.0
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.2.3/src/cbcflow.egg-info/SOURCES.txt` & `cbcflow-0.3.0/src/cbcflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 CHANGELOG.md
 LICENSE.md
 MANIFEST.in
 README.md
+asimov.log
 pyproject.toml
 setup.cfg
 setup.py
 docs/Makefile
 docs/requirements.txt
 docs/source/actionitems.rst
 docs/source/adding-to-the-schema.rst
@@ -55,16 +56,16 @@
 src/cbcflow/asimov.py
 src/cbcflow/cbcflow.py
 src/cbcflow/configuration.py
 src/cbcflow/database.py
 src/cbcflow/gracedb.py
 src/cbcflow/metadata.py
 src/cbcflow/monitor.py
-src/cbcflow/online_pe.py
 src/cbcflow/parser.py
+src/cbcflow/pe_scraper.py
 src/cbcflow/process.py
 src/cbcflow/schema.py
 src/cbcflow/utils.py
 src/cbcflow.egg-info/PKG-INFO
 src/cbcflow.egg-info/SOURCES.txt
 src/cbcflow.egg-info/dependency_links.txt
 src/cbcflow.egg-info/entry_points.txt
```

### Comparing `cbcflow-0.2.3/src/cbcflow.egg-info/entry_points.txt` & `cbcflow-0.3.0/src/cbcflow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/files_for_testing/cbc-meta-data-example.json` & `cbcflow-0.3.0/tests/files_for_testing/cbc-meta-data-example.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/files_for_testing/merge_test.json` & `cbcflow-0.3.0/tests/files_for_testing/merge_test.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/files_for_testing/update_json_1.json` & `cbcflow-0.3.0/tests/files_for_testing/update_json_1.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/files_for_testing/update_json_2.json` & `cbcflow-0.3.0/tests/files_for_testing/update_json_2.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/files_for_testing/update_yaml_1.yaml` & `cbcflow-0.3.0/tests/files_for_testing/update_yaml_1.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/files_for_testing/update_yaml_2.yaml` & `cbcflow-0.3.0/tests/files_for_testing/update_yaml_2.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/library_for_testing/S230227hp-cbc-metadata.json` & `cbcflow-0.3.0/tests/library_for_testing/S230227hp-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/library_for_testing/S230331e-cbc-metadata.json` & `cbcflow-0.3.0/tests/library_for_testing/S230331e-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/library_for_testing/S230401h-cbc-metadata.json` & `cbcflow-0.3.0/tests/library_for_testing/S230401h-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/library_for_testing/S230402dv-cbc-metadata.json` & `cbcflow-0.3.0/tests/library_for_testing/S230402dv-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/library_for_testing/S230403ae-cbc-metadata.json` & `cbcflow-0.3.0/tests/library_for_testing/S230403ae-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/library_for_testing/S230404hb-cbc-metadata.json` & `cbcflow-0.3.0/tests/library_for_testing/S230404hb-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/library_for_testing/S230404jc-cbc-metadata.json` & `cbcflow-0.3.0/tests/library_for_testing/S230404jc-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/test_merging.py` & `cbcflow-0.3.0/tests/test_merging.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.3/tests/test_metadata.py` & `cbcflow-0.3.0/tests/test_metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -271,14 +271,173 @@
             sname,
             local_library_path=self.test_library_directory,
             **self.default_metadata_kwargs,
         )
         assert metadata.sname == sname
         assert metadata.data["ParameterEstimation"]["Reviewers"] == ["Prospero"]
 
+    def test_read_metadata_subscripting_simple_hierarchy(self):
+        """Test the ability to read metadata through subscripting at a high level"""
+        # Write a metadata file to test
+        tgt = "tests/files_for_testing/cbc-meta-data-example.json"
+        sname = "S220331b"
+        os.makedirs(self.test_library_directory)
+        shutil.copy(
+            tgt, os.path.join(self.test_library_directory, MetaData.get_filename(sname))
+        )
+
+        metadata = MetaData(
+            sname,
+            local_library_path=self.test_library_directory,
+            **self.default_metadata_kwargs,
+        )
+
+        assert metadata["Sname"] == "S220331b"
+        assert metadata["Info"]["Labels"] == ["Testing cbcflow"]
+
+    def test_read_metadata_subscripting_complex_hierarchy(self):
+        """Test the ability to read metadata through subscripting at deep nesting"""
+
+        tgt = "tests/files_for_testing/cbc-meta-data-example.json"
+        sname = "S220331b"
+        os.makedirs(self.test_library_directory)
+        shutil.copy(
+            tgt, os.path.join(self.test_library_directory, MetaData.get_filename(sname))
+        )
+
+        metadata = MetaData(
+            sname,
+            local_library_path=self.test_library_directory,
+            **self.default_metadata_kwargs,
+        )
+
+        assert (
+            metadata["ParameterEstimation"]["Results"][0]["InferenceSoftware"]
+            == "bilby"
+        )
+        assert metadata["ParameterEstimation"]["Results"][0]["Notes"] == ["A note"]
+
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["UID"] == "IMRCT"
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["Analysts"] == ["Miranda"]
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["AnalysisSoftware"] == "tiger"
+        assert (
+            metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0]["UID"] == "TestA1"
+        )
+        assert (
+            metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0]["InferenceSoftware"]
+            == "bilby"
+        )
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0]["Notes"] == [
+            "A note, with high recursion depth"
+        ]
+
+    def test_write_metadata_subscripting_simple_hierarchy(self):
+        """Test the write to read metadata through subscripting at a high level"""
+        # Write a metadata file to test
+        tgt = "tests/files_for_testing/cbc-meta-data-example.json"
+        sname = "S220331b"
+        os.makedirs(self.test_library_directory)
+        shutil.copy(
+            tgt, os.path.join(self.test_library_directory, MetaData.get_filename(sname))
+        )
+
+        metadata = MetaData(
+            sname,
+            local_library_path=self.test_library_directory,
+            **self.default_metadata_kwargs,
+        )
+
+        assert metadata["Sname"] == "S220331b"
+        assert metadata["Cosmology"]["PreferredLowLatencySkymap"] == "A skymap"
+        assert metadata["Info"]["Labels"] == ["Testing cbcflow"]
+
+        metadata["Cosmology"]["PreferredLowLatencySkymap"] = "A different skymap"
+        metadata["Info"]["Labels"].append("Another test")
+
+        assert (
+            metadata["Cosmology"]["PreferredLowLatencySkymap"] == "A different skymap"
+        )
+        assert metadata["Info"]["Labels"] == ["Testing cbcflow", "Another test"]
+
+    def test_write_metadata_subscripting_complex_hierarchy(self):
+        """Test the ability to write metadata through subscripting at deep nesting"""
+
+        tgt = "tests/files_for_testing/cbc-meta-data-example.json"
+        sname = "S220331b"
+        os.makedirs(self.test_library_directory)
+        shutil.copy(
+            tgt, os.path.join(self.test_library_directory, MetaData.get_filename(sname))
+        )
+
+        metadata = MetaData(
+            sname,
+            local_library_path=self.test_library_directory,
+            **self.default_metadata_kwargs,
+        )
+
+        assert (
+            metadata["ParameterEstimation"]["Results"][0]["InferenceSoftware"]
+            == "bilby"
+        )
+        assert metadata["ParameterEstimation"]["Results"][0]["Notes"] == ["A note"]
+
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["UID"] == "IMRCT"
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["Analysts"] == ["Miranda"]
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["AnalysisSoftware"] == "tiger"
+        assert (
+            metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0]["UID"] == "TestA1"
+        )
+        assert (
+            metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0]["InferenceSoftware"]
+            == "bilby"
+        )
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0]["Notes"] == [
+            "A note, with high recursion depth"
+        ]
+
+        metadata["ParameterEstimation"]["Results"][0]["InferenceSoftware"] = "rift"
+        metadata["ParameterEstimation"]["Results"][0]["Notes"].append("Another Note")
+
+        metadata["TestingGR"]["IMRCTAnalyses"][0]["Analysts"].append("Caliban")
+        metadata["TestingGR"]["IMRCTAnalyses"][0]["AnalysisSoftware"] = "nottiger"
+        metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0][
+            "InferenceSoftware"
+        ] = "lalinference"
+        metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0]["Notes"].append(
+            "Something Else"
+        )
+
+        assert (
+            metadata["ParameterEstimation"]["Results"][0]["InferenceSoftware"] == "rift"
+        )
+        assert metadata["ParameterEstimation"]["Results"][0]["Notes"] == [
+            "A note",
+            "Another Note",
+        ]
+
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["UID"] == "IMRCT"
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["Analysts"] == [
+            "Miranda",
+            "Caliban",
+        ]
+        assert (
+            metadata["TestingGR"]["IMRCTAnalyses"][0]["AnalysisSoftware"] == "nottiger"
+        )
+        assert (
+            metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0]["UID"] == "TestA1"
+        )
+        assert (
+            metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0]["InferenceSoftware"]
+            == "lalinference"
+        )
+        assert metadata["TestingGR"]["IMRCTAnalyses"][0]["Results"][0]["Notes"] == [
+            "A note, with high recursion depth",
+            "Something Else",
+        ]
+
     def test_modify_metadata_from_file(self):
         # Write a metadata file to test
         tgt = "tests/files_for_testing/cbc-meta-data-example.json"
         sname = "S220331b"
         os.makedirs(self.test_library_directory)
         shutil.copy(tgt, self.test_library_directory + f"/{sname}.json")
 
@@ -630,10 +789,92 @@
             self.test_sname,
             local_library_path=self.test_library_directory,
             **self.default_metadata_kwargs,
         )
 
         assert altered_metadata.data == self.check_metadata_data
 
+    def test_validate_metadata_correct(self):
+        """A test of whether the function metadata.validate() yields true for valid configurations"""
+        # Same code as update_metadata_with_json_add above
+        if not os.path.exists(self.test_library_directory):
+            os.makedirs(self.test_library_directory)
+
+        metadata = MetaData(
+            self.test_sname,
+            local_library_path=self.test_library_directory,
+            **self.default_metadata_kwargs,
+        )
+
+        metadata.update(self.update_json_1)
+        metadata.update(self.update_json_2)
+
+        assert metadata.validate()
+
+        removal_json = {
+            "Info": {
+                "Labels": ["A test label, showing that appending works"],
+            },
+            "ExtremeMatter": {
+                "Analyses": [{"UID": "TestF1", "Reviewers": ["Prospero"]}]
+            },
+            "TestingGR": {
+                "IMRCTAnalyses": [
+                    {
+                        "UID": "TestF1",
+                        "Analysts": ["Miranda"],
+                        "Results": [{"UID": "TestF1", "Notes": ["A note"]}],
+                    }
+                ]
+            },
+        }
+
+        metadata.update(removal_json, is_removal=True)
+
+        assert metadata.validate()
+
+    def test_validate_metadata_incorrect(self):
+        """A test of whether the function metadata.validate() yields False for invalid configurations"""
+        # Same code as update_metadata_with_json_add above
+        if not os.path.exists(self.test_library_directory):
+            os.makedirs(self.test_library_directory)
+
+        metadata = MetaData(
+            self.test_sname,
+            local_library_path=self.test_library_directory,
+            **self.default_metadata_kwargs,
+        )
+
+        metadata.update(self.update_json_1)
+        metadata.update(self.update_json_2)
+
+        assert metadata.validate()
+
+        # Now we mess this up in various ways
+
+        # First make a list a number
+        original_labels_value = copy.copy(metadata["Info"]["Labels"])
+        metadata["Info"]["Labels"] = 3
+
+        assert not metadata.validate()
+        # Reset to original form, to get a clean test of the next
+        metadata["Info"]["Labels"] = original_labels_value
+
+        # Intentionally violate a regex
+        metadata["GraceDB"]["Events"] = []
+        metadata["GraceDB"]["Events"].append({"UID": "Q11111"})
+
+        assert not metadata.validate()
+        metadata["GraceDB"]["Events"] = []
+
+        # This test *does not* pass because repeated copies of UID is not technically a schema violation
+
+        # # Now make there be two copies of a given UID
+        # original_result_id = copy.copy(metadata["ExtremeMatter"]["Analyses"][1]["UID"])
+        # metadata["ExtremeMatter"]["Analyses"][1]["UID"] = "TestF1"
+
+        # assert not metadata.validate()
+        # metadata["ExtremeMatter"]["Analyses"][1]["UID"] = original_result_id
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `cbcflow-0.2.3/tests/test_schema.py` & `cbcflow-0.3.0/tests/test_schema.py`

 * *Files identical despite different names*

