# Comparing `tmp/deepdiff-6.3.0.tar.gz` & `tmp/deepdiff-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdiff-6.3.0.tar", last modified: Fri Mar 17 18:16:30 2023, max compression
+gzip compressed data, was "deepdiff-6.3.1.tar", last modified: Thu Jul  6 14:28:39 2023, max compression
```

## Comparing `deepdiff-6.3.0.tar` & `deepdiff-6.3.1.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-03-17 18:16:30.622944 deepdiff-6.3.0/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4673 2023-03-17 18:15:49.000000 deepdiff-6.3.0/AUTHORS.md
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1131 2021-04-28 22:25:20.000000 deepdiff-6.3.0/LICENSE
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      442 2023-01-06 05:04:29.000000 deepdiff-6.3.0/MANIFEST.in
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4533 2023-03-17 18:16:30.622944 deepdiff-6.3.0/PKG-INFO
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3450 2023-03-17 18:15:49.000000 deepdiff-6.3.0/README.md
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3571 2022-08-28 02:43:58.000000 deepdiff-6.3.0/conftest.py
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-03-17 18:16:30.610944 deepdiff-6.3.0/deepdiff/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      386 2023-03-17 18:15:49.000000 deepdiff-6.3.0/deepdiff/__init__.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2002 2021-02-01 00:46:22.000000 deepdiff-6.3.0/deepdiff/anyset.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2057 2021-02-01 00:46:22.000000 deepdiff-6.3.0/deepdiff/base.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10041 2023-03-17 18:15:49.000000 deepdiff-6.3.0/deepdiff/commands.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    20112 2022-08-28 02:43:58.000000 deepdiff-6.3.0/deepdiff/deephash.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    27282 2022-08-28 02:43:58.000000 deepdiff-6.3.0/deepdiff/delta.py
--rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    77674 2023-03-17 18:15:49.000000 deepdiff-6.3.0/deepdiff/diff.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10699 2021-12-17 19:31:57.000000 deepdiff-6.3.0/deepdiff/distance.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    18756 2023-03-17 18:15:49.000000 deepdiff-6.3.0/deepdiff/helper.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6848 2021-02-01 00:46:22.000000 deepdiff-6.3.0/deepdiff/lfucache.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    39148 2023-03-17 18:15:49.000000 deepdiff-6.3.0/deepdiff/model.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1264 2023-03-17 18:15:49.000000 deepdiff-6.3.0/deepdiff/operator.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5114 2021-12-17 19:31:57.000000 deepdiff-6.3.0/deepdiff/path.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    12408 2021-04-29 06:21:17.000000 deepdiff-6.3.0/deepdiff/search.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    20925 2023-03-17 18:15:49.000000 deepdiff-6.3.0/deepdiff/serialization.py
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-03-17 18:16:30.610944 deepdiff-6.3.0/deepdiff.egg-info/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4533 2023-03-17 18:16:30.000000 deepdiff-6.3.0/deepdiff.egg-info/PKG-INFO
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3822 2023-03-17 18:16:30.000000 deepdiff-6.3.0/deepdiff.egg-info/SOURCES.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        1 2023-03-17 18:16:30.000000 deepdiff-6.3.0/deepdiff.egg-info/dependency_links.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       48 2023-03-17 18:16:30.000000 deepdiff-6.3.0/deepdiff.egg-info/entry_points.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       77 2023-03-17 18:16:30.000000 deepdiff-6.3.0/deepdiff.egg-info/requires.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        9 2023-03-17 18:16:30.000000 deepdiff-6.3.0/deepdiff.egg-info/top_level.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        1 2023-01-06 05:03:23.000000 deepdiff-6.3.0/deepdiff.egg-info/zip-safe
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-03-17 18:16:30.614944 deepdiff-6.3.0/docs/
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-03-17 18:16:30.614944 deepdiff-6.3.0/docs/_static/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    33163 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    33204 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=10000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    27892 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/_static/benchmark_big_jsons__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    30167 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/_static/benchmark_big_jsons__pypy3.6__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    22641 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    21556 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=5000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    20752 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    19635 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=500__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    32429 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/_static/benchmark_numpy_array__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5414 2023-03-17 18:15:49.000000 deepdiff-6.3.0/docs/authors.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6885 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/basics.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7075 2023-03-17 18:15:49.000000 deepdiff-6.3.0/docs/changelog.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     8030 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/commandline.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    12063 2023-03-17 18:15:49.000000 deepdiff-6.3.0/docs/custom.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6444 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/deep_distance.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      160 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/deephash.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17755 2022-08-28 02:43:58.000000 deepdiff-6.3.0/docs/deephash_doc.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17311 2023-03-17 18:15:49.000000 deepdiff-6.3.0/docs/delta.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      361 2022-04-11 00:27:20.000000 deepdiff-6.3.0/docs/diff.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    13080 2023-03-17 18:15:49.000000 deepdiff-6.3.0/docs/diff_doc.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      222 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/dsearch.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3595 2022-08-28 02:43:58.000000 deepdiff-6.3.0/docs/exclude_paths.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      133 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/extract.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3273 2021-12-17 18:08:47.000000 deepdiff-6.3.0/docs/faq.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    14344 2021-10-13 18:10:55.000000 deepdiff-6.3.0/docs/ignore_order.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    14455 2023-03-17 18:15:49.000000 deepdiff-6.3.0/docs/ignore_types_or_values.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3626 2023-03-17 18:15:49.000000 deepdiff-6.3.0/docs/index.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7224 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/numbers.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    12126 2023-03-17 18:15:49.000000 deepdiff-6.3.0/docs/optimizations.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3215 2022-04-11 00:27:20.000000 deepdiff-6.3.0/docs/other.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2648 2021-04-29 06:21:17.000000 deepdiff-6.3.0/docs/search_doc.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3932 2021-02-16 20:18:34.000000 deepdiff-6.3.0/docs/serialization.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2982 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/stats.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      516 2021-04-29 06:21:17.000000 deepdiff-6.3.0/docs/support.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      616 2021-02-01 00:46:22.000000 deepdiff-6.3.0/docs/troubleshoot.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    13411 2021-04-29 06:21:17.000000 deepdiff-6.3.0/docs/view.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       58 2021-02-01 00:46:22.000000 deepdiff-6.3.0/pytest.ini
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       25 2022-12-11 22:15:27.000000 deepdiff-6.3.0/requirements-cli.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      182 2023-03-17 18:15:49.000000 deepdiff-6.3.0/requirements-dev-3.7.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      296 2023-03-17 18:15:49.000000 deepdiff-6.3.0/requirements-dev.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        7 2023-03-17 18:15:49.000000 deepdiff-6.3.0/requirements-optimize.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       26 2023-03-17 18:15:49.000000 deepdiff-6.3.0/requirements.txt
--rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)       48 2021-02-01 00:46:22.000000 deepdiff-6.3.0/run_tests.sh
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      433 2023-03-17 18:16:30.622944 deepdiff-6.3.0/setup.cfg
--rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)     2254 2023-03-17 18:15:49.000000 deepdiff-6.3.0/setup.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      447 2022-09-02 18:37:29.000000 deepdiff-6.3.0/temp.py
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-03-17 18:16:30.618944 deepdiff-6.3.0/tests/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2090 2022-09-04 22:40:39.000000 deepdiff-6.3.0/tests/__init__.py
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-03-17 18:16:30.622944 deepdiff-6.3.0/tests/fixtures/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      182 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/another.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       57 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/c_t1.csv
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       59 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/c_t2.csv
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      964 2022-09-04 22:40:39.000000 deepdiff-6.3.0/tests/fixtures/compare_func_result1.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      861 2021-04-29 06:21:17.000000 deepdiff-6.3.0/tests/fixtures/compare_func_t1.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      834 2021-04-29 06:21:17.000000 deepdiff-6.3.0/tests/fixtures/compare_func_t2.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/d_t1.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/d_t2.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       18 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/invalid_yaml.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5391 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/nested_a_result.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1772 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/nested_a_t1.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1839 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/nested_a_t2.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      487 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/nested_b_result.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      165 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/nested_b_t1.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      167 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/nested_b_t2.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       72 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/patch1.pickle
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       80 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t1.csv
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       49 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t1.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       28 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t1.pickle
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      510 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t1.toml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t1.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       50 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t1_corrupt.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       80 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t2.csv
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       71 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t2.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       28 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t2.pickle
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      496 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t2.toml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t2.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       24 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/fixtures/t2_json.csv
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1297 2022-04-10 05:44:35.000000 deepdiff-6.3.0/tests/test_anyset.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7425 2022-08-28 02:43:58.000000 deepdiff-6.3.0/tests/test_cache.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5110 2023-03-17 18:15:49.000000 deepdiff-6.3.0/tests/test_command.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    56034 2023-03-17 18:15:49.000000 deepdiff-6.3.0/tests/test_delta.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4067 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/test_diff_math.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5961 2023-03-17 18:15:49.000000 deepdiff-6.3.0/tests/test_diff_numpy.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4301 2022-04-10 05:44:35.000000 deepdiff-6.3.0/tests/test_diff_other.py
--rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    58977 2023-03-17 18:15:49.000000 deepdiff-6.3.0/tests/test_diff_text.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6266 2023-03-17 18:15:49.000000 deepdiff-6.3.0/tests/test_diff_tree.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     9166 2022-04-10 05:44:35.000000 deepdiff-6.3.0/tests/test_distance.py
--rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    30975 2022-08-28 02:43:58.000000 deepdiff-6.3.0/tests/test_hash.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    16559 2022-12-11 22:15:27.000000 deepdiff-6.3.0/tests/test_helper.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    38877 2022-09-04 22:40:39.000000 deepdiff-6.3.0/tests/test_ignore_order.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1766 2021-02-01 00:46:22.000000 deepdiff-6.3.0/tests/test_lfucache.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7746 2021-10-13 18:10:55.000000 deepdiff-6.3.0/tests/test_model.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7946 2023-03-17 18:15:49.000000 deepdiff-6.3.0/tests/test_operators.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1075 2021-10-13 18:10:55.000000 deepdiff-6.3.0/tests/test_path.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17641 2021-04-29 06:21:17.000000 deepdiff-6.3.0/tests/test_search.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    15667 2023-01-06 05:04:29.000000 deepdiff-6.3.0/tests/test_serialization.py
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-07-06 14:28:39.925486 deepdiff-6.3.1/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5210 2023-07-06 14:26:54.000000 deepdiff-6.3.1/AUTHORS.md
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1131 2021-04-28 22:25:20.000000 deepdiff-6.3.1/LICENSE
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      442 2023-01-06 05:04:29.000000 deepdiff-6.3.1/MANIFEST.in
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5741 2023-07-06 14:28:39.929485 deepdiff-6.3.1/PKG-INFO
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4678 2023-07-06 14:27:45.000000 deepdiff-6.3.1/README.md
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3571 2022-08-28 02:43:58.000000 deepdiff-6.3.1/conftest.py
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-07-06 14:28:39.913488 deepdiff-6.3.1/deepdiff/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      386 2023-07-06 14:27:45.000000 deepdiff-6.3.1/deepdiff/__init__.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2002 2021-02-01 00:46:22.000000 deepdiff-6.3.1/deepdiff/anyset.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2057 2021-02-01 00:46:22.000000 deepdiff-6.3.1/deepdiff/base.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10041 2023-03-17 18:15:49.000000 deepdiff-6.3.1/deepdiff/commands.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    20741 2023-07-06 14:07:33.000000 deepdiff-6.3.1/deepdiff/deephash.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    27784 2023-07-06 14:07:33.000000 deepdiff-6.3.1/deepdiff/delta.py
+-rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    77872 2023-07-06 14:07:33.000000 deepdiff-6.3.1/deepdiff/diff.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10699 2021-12-17 19:31:57.000000 deepdiff-6.3.1/deepdiff/distance.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    18936 2023-07-06 14:07:33.000000 deepdiff-6.3.1/deepdiff/helper.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6848 2021-02-01 00:46:22.000000 deepdiff-6.3.1/deepdiff/lfucache.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    39148 2023-03-17 18:15:49.000000 deepdiff-6.3.1/deepdiff/model.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1264 2023-03-17 18:15:49.000000 deepdiff-6.3.1/deepdiff/operator.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5697 2023-07-06 14:07:33.000000 deepdiff-6.3.1/deepdiff/path.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    12408 2021-04-29 06:21:17.000000 deepdiff-6.3.1/deepdiff/search.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    21144 2023-07-06 14:07:33.000000 deepdiff-6.3.1/deepdiff/serialization.py
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-07-06 14:28:39.913488 deepdiff-6.3.1/deepdiff.egg-info/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5741 2023-07-06 14:28:39.000000 deepdiff-6.3.1/deepdiff.egg-info/PKG-INFO
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3850 2023-07-06 14:28:39.000000 deepdiff-6.3.1/deepdiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        1 2023-07-06 14:28:39.000000 deepdiff-6.3.1/deepdiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       47 2023-07-06 14:28:39.000000 deepdiff-6.3.1/deepdiff.egg-info/entry_points.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       77 2023-07-06 14:28:39.000000 deepdiff-6.3.1/deepdiff.egg-info/requires.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        9 2023-07-06 14:28:39.000000 deepdiff-6.3.1/deepdiff.egg-info/top_level.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        1 2023-01-06 05:03:23.000000 deepdiff-6.3.1/deepdiff.egg-info/zip-safe
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-07-06 14:28:39.917487 deepdiff-6.3.1/docs/
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-07-06 14:28:39.921487 deepdiff-6.3.1/docs/_static/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    33163 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    33204 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=10000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    27892 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/_static/benchmark_big_jsons__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    30167 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/_static/benchmark_big_jsons__pypy3.6__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    22641 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    21556 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=5000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    20752 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    19635 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=500__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    32429 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/_static/benchmark_numpy_array__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5996 2023-07-06 14:27:25.000000 deepdiff-6.3.1/docs/authors.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6885 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/basics.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7666 2023-07-06 14:22:47.000000 deepdiff-6.3.1/docs/changelog.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     8030 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/commandline.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    12063 2023-03-17 18:15:49.000000 deepdiff-6.3.1/docs/custom.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6444 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/deep_distance.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      160 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/deephash.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17755 2022-08-28 02:43:58.000000 deepdiff-6.3.1/docs/deephash_doc.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    18328 2023-07-06 14:07:33.000000 deepdiff-6.3.1/docs/delta.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      361 2022-04-11 00:27:20.000000 deepdiff-6.3.1/docs/diff.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    13080 2023-03-17 18:15:49.000000 deepdiff-6.3.1/docs/diff_doc.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      222 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/dsearch.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3595 2022-08-28 02:43:58.000000 deepdiff-6.3.1/docs/exclude_paths.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      133 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/extract.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3273 2021-12-17 18:08:47.000000 deepdiff-6.3.1/docs/faq.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    14344 2021-10-13 18:10:55.000000 deepdiff-6.3.1/docs/ignore_order.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    14455 2023-03-17 18:15:49.000000 deepdiff-6.3.1/docs/ignore_types_or_values.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4087 2023-07-06 14:27:45.000000 deepdiff-6.3.1/docs/index.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7224 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/numbers.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    12126 2023-03-17 18:15:49.000000 deepdiff-6.3.1/docs/optimizations.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3215 2022-04-11 00:27:20.000000 deepdiff-6.3.1/docs/other.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2648 2021-04-29 06:21:17.000000 deepdiff-6.3.1/docs/search_doc.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3932 2021-02-16 20:18:34.000000 deepdiff-6.3.1/docs/serialization.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2982 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/stats.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      516 2021-04-29 06:21:17.000000 deepdiff-6.3.1/docs/support.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      616 2021-02-01 00:46:22.000000 deepdiff-6.3.1/docs/troubleshoot.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    13411 2021-04-29 06:21:17.000000 deepdiff-6.3.1/docs/view.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       58 2021-02-01 00:46:22.000000 deepdiff-6.3.1/pytest.ini
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       25 2022-12-11 22:15:27.000000 deepdiff-6.3.1/requirements-cli.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      265 2023-07-06 14:07:33.000000 deepdiff-6.3.1/requirements-dev-3.7.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      341 2023-07-06 14:07:33.000000 deepdiff-6.3.1/requirements-dev.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        7 2023-03-17 18:15:49.000000 deepdiff-6.3.1/requirements-optimize.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       26 2023-03-17 18:15:49.000000 deepdiff-6.3.1/requirements.txt
+-rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)       48 2021-02-01 00:46:22.000000 deepdiff-6.3.1/run_tests.sh
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      433 2023-07-06 14:28:39.929485 deepdiff-6.3.1/setup.cfg
+-rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)     2254 2023-07-06 14:27:45.000000 deepdiff-6.3.1/setup.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      447 2022-09-02 18:37:29.000000 deepdiff-6.3.1/temp.py
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-07-06 14:28:39.925486 deepdiff-6.3.1/tests/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2090 2022-09-04 22:40:39.000000 deepdiff-6.3.1/tests/__init__.py
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-07-06 14:28:39.925486 deepdiff-6.3.1/tests/fixtures/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      182 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/another.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       57 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/c_t1.csv
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       59 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/c_t2.csv
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      964 2022-09-04 22:40:39.000000 deepdiff-6.3.1/tests/fixtures/compare_func_result1.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      861 2021-04-29 06:21:17.000000 deepdiff-6.3.1/tests/fixtures/compare_func_t1.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      834 2021-04-29 06:21:17.000000 deepdiff-6.3.1/tests/fixtures/compare_func_t2.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/d_t1.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/d_t2.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       18 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/invalid_yaml.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5391 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/nested_a_result.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1772 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/nested_a_t1.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1839 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/nested_a_t2.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      487 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/nested_b_result.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      165 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/nested_b_t1.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      167 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/nested_b_t2.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       72 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/patch1.pickle
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       80 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t1.csv
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       49 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t1.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       28 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t1.pickle
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      510 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t1.toml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t1.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       50 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t1_corrupt.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       80 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t2.csv
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       71 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t2.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       28 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t2.pickle
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      496 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t2.toml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t2.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       24 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/fixtures/t2_json.csv
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1297 2022-04-10 05:44:35.000000 deepdiff-6.3.1/tests/test_anyset.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7425 2022-08-28 02:43:58.000000 deepdiff-6.3.1/tests/test_cache.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5110 2023-03-17 18:15:49.000000 deepdiff-6.3.1/tests/test_command.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    56598 2023-07-06 14:07:33.000000 deepdiff-6.3.1/tests/test_delta.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2307 2023-07-06 14:07:33.000000 deepdiff-6.3.1/tests/test_diff_datetime.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4067 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/test_diff_math.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5961 2023-03-17 18:15:49.000000 deepdiff-6.3.1/tests/test_diff_numpy.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4301 2022-04-10 05:44:35.000000 deepdiff-6.3.1/tests/test_diff_other.py
+-rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    59829 2023-07-06 14:07:33.000000 deepdiff-6.3.1/tests/test_diff_text.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6266 2023-03-17 18:15:49.000000 deepdiff-6.3.1/tests/test_diff_tree.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     9166 2022-04-10 05:44:35.000000 deepdiff-6.3.1/tests/test_distance.py
+-rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    31328 2023-07-06 14:07:33.000000 deepdiff-6.3.1/tests/test_hash.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    16559 2022-12-11 22:15:27.000000 deepdiff-6.3.1/tests/test_helper.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    39653 2023-07-06 14:07:33.000000 deepdiff-6.3.1/tests/test_ignore_order.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1766 2021-02-01 00:46:22.000000 deepdiff-6.3.1/tests/test_lfucache.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7746 2021-10-13 18:10:55.000000 deepdiff-6.3.1/tests/test_model.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7946 2023-03-17 18:15:49.000000 deepdiff-6.3.1/tests/test_operators.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1075 2021-10-13 18:10:55.000000 deepdiff-6.3.1/tests/test_path.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17641 2021-04-29 06:21:17.000000 deepdiff-6.3.1/tests/test_search.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    15667 2023-01-06 05:04:29.000000 deepdiff-6.3.1/tests/test_serialization.py
```

### Comparing `deepdiff-6.3.0/AUTHORS.md` & `deepdiff-6.3.1/AUTHORS.md`

 * *Files 10% similar despite different names*

```diff
@@ -48,7 +48,13 @@
 - [dtorres-sf](https://github.com/dtorres-sf) for the fix for diffing using iterable_compare_func with nested objects.
 - [Enric Pou](https://github.com/epou) for bug fix of ValueError when using Decimal 0.x
 - [Uwe Fladrich](https://github.com/uwefladrich) for fixing bug when diff'ing non-sequence iterables
 - [Michal Ozery-Flato](https://github.com/michalozeryflato) for setting equal_nan=ignore_nan_inequality in the call for np.array_equal
 - [martin-kokos](https://github.com/martin-kokos) for using Pytest's tmp_path fixture instead of /tmp/
 - Håvard Thom [havardthom](https://github.com/havardthom) for adding include_obj_callback and include_obj_callback_strict.
 - [Noam Gottlieb](https://github.com/noamgot) for fixing a corner case where numpy's `np.float32` nans are not ignored when using `ignore_nan_equality`.
+- [maggelus](https://github.com/maggelus) for the bugfix deephash for paths.
+- [maggelus](https://github.com/maggelus) for the bugfix deephash compiled regex.
+- [martin-kokos](https://github.com/martin-kokos) for fixing the tests dependent on toml.
+- [kor4ik](https://github.com/kor4ik) for the bugfix for `include_paths` for nested dictionaries.
+- [martin-kokos](https://github.com/martin-kokos) for using tomli and tomli-w for dealing with tomli files.
+- [Alex Sauer-Budge](https://github.com/amsb) for the bugfix for `datetime.date`.
```

### Comparing `deepdiff-6.3.0/LICENSE` & `deepdiff-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/PKG-INFO` & `deepdiff-6.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: deepdiff
-Version: 6.3.0
+Version: 6.3.1
 Summary: Deep Difference and Search of any Python object/data. Recreate objects by adding adding deltas to each other.
 Home-page: https://github.com/seperman/deepdiff
+Download-URL: https://github.com/seperman/deepdiff/tarball/master
 Author: Seperman
 Author-email: sep@zepworks.com
 License: MIT
-Download-URL: https://github.com/seperman/deepdiff/tarball/master
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,15 +21,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: optimize
 License-File: LICENSE
 License-File: AUTHORS.md
 
-# DeepDiff v 6.3.0
+# DeepDiff v 6.3.1
 
 ![Downloads](https://img.shields.io/pypi/dm/deepdiff.svg?style=flat)
 ![Python Versions](https://img.shields.io/pypi/pyversions/deepdiff.svg?style=flat)
 ![License](https://img.shields.io/pypi/l/deepdiff.svg?version=latest)
 [![Build Status](https://github.com/seperman/deepdiff/workflows/Unit%20Tests/badge.svg)](https://github.com/seperman/deepdiff/actions)
 [![codecov](https://codecov.io/gh/seperman/deepdiff/branch/master/graph/badge.svg?token=KkHZ3siA3m)](https://codecov.io/gh/seperman/deepdiff)
 
@@ -41,55 +40,75 @@
 - [DeepHash](https://zepworks.com/deepdiff/current/deephash.html): Hash any object based on their content.
 - [Delta](https://zepworks.com/deepdiff/current/delta.html): Store the difference of objects and apply them to other objects.
 - [Extract](https://zepworks.com/deepdiff/current/extract.html): Extract an item from a nested Python object using its path.
 - [commandline](https://zepworks.com/deepdiff/current/commandline.html): Use DeepDiff from commandline.
 
 Tested on Python 3.7+ and PyPy3.
 
-- **[Documentation](https://zepworks.com/deepdiff/6.3.0/)**
+- **[Documentation](https://zepworks.com/deepdiff/6.3.1/)**
 
 ## What is new?
 
 Please check the [ChangeLog](CHANGELOG.md) file for the detailed information.
 
+DeepDiff 6-3-1
+
+This release includes many bug fixes.
+
+- Bugfix deephash for paths by [maggelus](https://github.com/maggelus)
+- Bugfix deephash compiled regex [maggelus](https://github.com/maggelus)
+- Fix tests dependent on toml by [martin-kokos](https://github.com/martin-kokos)
+- Bugfix for `include_paths` for nested dictionaries by [kor4ik](https://github.com/kor4ik)
+- Use tomli and tomli-w for dealing with tomli files by [martin-kokos](https://github.com/martin-kokos)
+- Bugfix for `datetime.date` by [Alex Sauer-Budge](https://github.com/amsb)
+
+
 DeepDiff 6-3-0
 
-- `PrefixOrSuffixOperator`: This operator will skip strings that are suffix or prefix of each other.
-- `include_obj_callback` and `include_obj_callback_strict` are added by [Håvard Thom](https://github.com/havardthom).
+- [`PrefixOrSuffixOperator`](https://zepworks.com/deepdiff/current/custom.html#prefix-or-suffix-operator-label): This operator will skip strings that are suffix or prefix of each other.
+- [`include_obj_callback`](https://zepworks.com/deepdiff/current/ignore_types_or_values.html#include-obj-callback-label) and `include_obj_callback_strict` are added by [Håvard Thom](https://github.com/havardthom).
 - Fixed a corner case where numpy's `np.float32` nans are not ignored when using `ignore_nan_equality` by [Noam Gottlieb](https://github.com/noamgot)
 - `orjson` becomes optional again.
 - Fix for `ignore_type_in_groups` with numeric values so it does not report number changes when the number types are different.
 
-DeepDiff 6-2-0
-
-- Major improvement in the diff report for lists when items are all hashable and the order of items is important.
-
-
 ## Installation
 
 ### Install from PyPi:
 
 `pip install deepdiff`
 
 If you want to use DeepDiff from commandline:
 
 `pip install "deepdiff[cli]"`
 
 If you want to improve the performance of DeepDiff with certain functionalities such as improved json serialization:
 
 `pip install "deepdiff[optimize]"`
 
+Install optional packages:
+- [yaml](https://pypi.org/project/PyYAML/)
+- [tomli](https://pypi.org/project/tomli/) (python 3.10 and older) and [tomli-w](https://pypi.org/project/tomli-w/) for writing
+- [clevercsv](https://pypi.org/project/clevercsv/) for more rubust CSV parsing
+- [orjson](https://pypi.org/project/orjson/) for speed and memory optimized parsing
+- [pydantic](https://pypi.org/project/pydantic/)
+
+
 # Documentation
 
 <https://zepworks.com/deepdiff/current/>
 
 # ChangeLog
 
 Please take a look at the [CHANGELOG](CHANGELOG.md) file.
 
+# Survey
+
+:mega: **Please fill out our [fast 5-question survey](https://forms.gle/E6qXexcgjoKnSzjB8)** so that we can learn how & why you use DeepDiff, and what improvements we should make. Thank you! :dancers:
+
+
 # Contribute
 
 1. Please make your PR against the dev branch
 2. Please make sure that your PR has tests. Since DeepDiff is used in many sensitive data driven projects, we strive to maintain around 100% test coverage on the code.
 
 Please run `pytest --cov=deepdiff --runslow` to see the coverage report. Note that the `--runslow` flag will run some slow tests too. In most cases you only want to run the fast tests which so you wont add the `--runslow` flag.
 
@@ -97,18 +116,16 @@
 
 Thank you!
 
 # Citing
 
 How to cite this library (APA style):
 
-    Dehpour, S. (2022). DeepDiff (Version 6.3.0) [Software]. Available from https://github.com/seperman/deepdiff.
+    Dehpour, S. (2023). DeepDiff (Version 6.3.1) [Software]. Available from https://github.com/seperman/deepdiff.
 
 How to cite this library (Chicago style):
 
-    Dehpour, Sep. 2022. DeepDiff (version 6.3.0).
+    Dehpour, Sep. 2023. DeepDiff (version 6.3.1).
 
 # Authors
 
 Please take a look at the [AUTHORS](AUTHORS.md) file.
-
-
```

### Comparing `deepdiff-6.3.0/conftest.py` & `deepdiff-6.3.1/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/deepdiff/anyset.py` & `deepdiff-6.3.1/deepdiff/anyset.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/deepdiff/base.py` & `deepdiff-6.3.1/deepdiff/base.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/deepdiff/commands.py` & `deepdiff-6.3.1/deepdiff/commands.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/deepdiff/deephash.py` & `deepdiff-6.3.1/deepdiff/deephash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python
+import inspect
 import logging
 from collections.abc import Iterable, MutableMapping
 from collections import defaultdict
 from hashlib import sha1, sha256
+from pathlib import Path
 from enum import Enum
 from deepdiff.helper import (strings, numbers, times, unprocessed, not_hashed, add_to_frozen_set,
                              convert_item_or_items_into_set_else_none, get_doc,
                              convert_item_or_items_into_compiled_regexes_else_none,
                              get_id, type_is_subclass_of_type_group, type_in_type_group,
                              number_to_string, datetime_normalize, KEY_TO_VAL_STR, short_repr,
                              get_truncate_datetime, dict_, add_root_to_paths)
@@ -304,25 +306,36 @@
 
     def items(self):
         return ((i, v[0]) for i, v in self.hashes.items())
 
     def _prep_obj(self, obj, parent, parents_ids=EMPTY_FROZENSET, is_namedtuple=False):
         """prepping objects"""
         original_type = type(obj) if not isinstance(obj, type) else obj
-        try:
-            if is_namedtuple:
-                obj = obj._asdict()
-            else:
-                obj = obj.__dict__
-        except AttributeError:
+
+        obj_to_dict_strategies = []
+        if is_namedtuple:
+            obj_to_dict_strategies.append(lambda o: o._asdict())
+        else:
+            obj_to_dict_strategies.append(lambda o: o.__dict__)
+
+        if hasattr(obj, "__slots__"):
+            obj_to_dict_strategies.append(lambda o: {i: getattr(o, i) for i in o.__slots__})
+        else:
+            obj_to_dict_strategies.append(lambda o: dict(inspect.getmembers(o, lambda m: not inspect.isroutine(m))))
+
+        for get_dict in obj_to_dict_strategies:
             try:
-                obj = {i: getattr(obj, i) for i in obj.__slots__}
+                d = get_dict(obj)
+                break
             except AttributeError:
-                self.hashes[UNPROCESSED_KEY].append(obj)
-                return (unprocessed, 0)
+                pass
+        else:
+            self.hashes[UNPROCESSED_KEY].append(obj)
+            return (unprocessed, 0)
+        obj = d
 
         result, counts = self._prep_dict(obj, parent=parent, parents_ids=parents_ids,
                                          print_as_attribute=True, original_type=original_type)
         result = "nt{}".format(result) if is_namedtuple else "obj{}".format(result)
         return result, counts
 
     def _skip_this(self, obj, parent):
@@ -416,14 +429,20 @@
         result = KEY_TO_VAL_STR.format(type(obj).__name__, result)
 
         return result, counts
 
     def _prep_bool(self, obj):
         return BoolObj.TRUE if obj else BoolObj.FALSE
 
+
+    def _prep_path(self, obj):
+        type_ = obj.__class__.__name__
+        return KEY_TO_VAL_STR.format(type_, obj)
+
+
     def _prep_number(self, obj):
         type_ = "number" if self.ignore_numeric_type_changes else obj.__class__.__name__
         if self.significant_digits is not None:
             obj = self.number_to_string(obj, significant_digits=self.significant_digits,
                                         number_format_notation=self.number_format_notation)
         return KEY_TO_VAL_STR.format(type_, obj)
 
@@ -472,14 +491,17 @@
                 obj,
                 ignore_string_type_changes=self.ignore_string_type_changes,
                 ignore_string_case=self.ignore_string_case,
                 encodings=self.encodings,
                 ignore_encoding_errors=self.ignore_encoding_errors,
             )
 
+        elif isinstance(obj, Path):
+            result = self._prep_path(obj)
+
         elif isinstance(obj, times):
             result = self._prep_datetime(obj)
 
         elif isinstance(obj, numbers):
             result = self._prep_number(obj)
 
         elif isinstance(obj, MutableMapping):
```

### Comparing `deepdiff-6.3.0/deepdiff/delta.py` & `deepdiff-6.3.1/deepdiff/delta.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from deepdiff import DeepDiff
 from deepdiff.serialization import pickle_load, pickle_dump
 from deepdiff.helper import (
     strings, short_repr, numbers,
     np_ndarray, np_array_factory, numpy_dtypes, get_doc,
     not_found, numpy_dtype_string_to_type, dict_,
 )
-from deepdiff.path import _path_to_elements, _get_nested_obj, GET, GETATTR
+from deepdiff.path import _path_to_elements, _get_nested_obj, _get_nested_obj_and_force, GET, GETATTR
 from deepdiff.anyset import AnySet
 
 
 logger = logging.getLogger(__name__)
 
 
 VERIFICATION_MSG = 'Expected the old value for {} to be {} but it is {}. Error found on: {}'
@@ -66,14 +66,15 @@
         deserializer=pickle_load,
         log_errors=True,
         mutate=False,
         raise_errors=False,
         safe_to_import=None,
         serializer=pickle_dump,
         verify_symmetry=False,
+        force=False,
     ):
         if hasattr(deserializer, '__code__') and 'safe_to_import' in set(deserializer.__code__.co_varnames):
             _deserializer = deserializer
         else:
             def _deserializer(obj, safe_to_import=None):
                 return deserializer(obj)
 
@@ -100,14 +101,19 @@
         self.mutate = mutate
         self.verify_symmetry = verify_symmetry
         self.raise_errors = raise_errors
         self.log_errors = log_errors
         self._numpy_paths = self.diff.pop('_numpy_paths', False)
         self.serializer = serializer
         self.deserializer = deserializer
+        self.force = force
+        if force:
+            self.get_nested_obj = _get_nested_obj_and_force
+        else:
+            self.get_nested_obj = _get_nested_obj
         self.reset()
 
     def __repr__(self):
         return "<Delta: {}>".format(short_repr(self.diff, max_length=100))
 
     def reset(self):
         self.post_process_paths_to_convert = dict_()
@@ -158,15 +164,22 @@
         try:
             if action == GET:
                 current_old_value = obj[elem]
             elif action == GETATTR:
                 current_old_value = getattr(obj, elem)
             else:
                 raise DeltaError(INVALID_ACTION_WHEN_CALLING_GET_ELEM.format(action))
-        except (KeyError, IndexError, AttributeError, IndexError, TypeError) as e:
+        except (KeyError, IndexError, AttributeError, TypeError) as e:
+            if self.force:
+                forced_old_value = {}
+                if action == GET:
+                    obj[elem] = forced_old_value
+                elif action == GETATTR:
+                    setattr(obj, elem, forced_old_value)
+                return forced_old_value
             current_old_value = not_found
             if isinstance(path_for_err_reporting, (list, tuple)):
                 path_for_err_reporting = '.'.join([i[0] for i in path_for_err_reporting])
             if self.verify_symmetry:
                 self._raise_or_log(VERIFICATION_MSG.format(
                     path_for_err_reporting,
                     expected_old_value, current_old_value, e))
@@ -347,22 +360,22 @@
             if preprocess_paths:
                 self._do_values_or_type_changed(preprocess_paths, is_type_change=True)
 
     def _get_elements_and_details(self, path):
         try:
             elements = _path_to_elements(path)
             if len(elements) > 1:
-                parent = _get_nested_obj(obj=self, elements=elements[:-2])
+                parent = self.get_nested_obj(obj=self, elements=elements[:-2])
                 parent_to_obj_elem, parent_to_obj_action = elements[-2]
                 obj = self._get_elem_and_compare_to_old_value(
                     obj=parent, path_for_err_reporting=path, expected_old_value=None,
                     elem=parent_to_obj_elem, action=parent_to_obj_action)
             else:
                 parent = parent_to_obj_elem = parent_to_obj_action = None
-                obj = _get_nested_obj(obj=self, elements=elements[:-1])
+                obj = self.get_nested_obj(obj=self, elements=elements[:-1])
             elem, action = elements[-1]
         except Exception as e:
             self._raise_or_log(UNABLE_TO_GET_ITEM_MSG.format(path, e))
             return None
         else:
             if obj is not_found:
                 return None
@@ -454,15 +467,15 @@
         items = self.diff.get('set_item_removed')
         if items:
             self._do_set_or_frozenset_item(items, func='difference')
 
     def _do_set_or_frozenset_item(self, items, func):
         for path, value in items.items():
             elements = _path_to_elements(path)
-            parent = _get_nested_obj(obj=self, elements=elements[:-1])
+            parent = self.get_nested_obj(obj=self, elements=elements[:-1])
             elem, action = elements[-1]
             obj = self._get_elem_and_compare_to_old_value(
                 parent, path_for_err_reporting=path, expected_old_value=None, elem=elem, action=action)
             new_value = getattr(obj, func)(value)
             self._simple_set_elem_value(parent, path_for_err_reporting=path, elem=elem, value=new_value, action=action)
 
     def _do_ignore_order_get_old(self, obj, remove_indexes_per_path, fixed_indexes_values, path_for_err_reporting):
```

### Comparing `deepdiff-6.3.0/deepdiff/diff.py` & `deepdiff-6.3.1/deepdiff/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 from enum import Enum
 from copy import deepcopy
 from math import isclose as is_close
 from collections.abc import Mapping, Iterable, Sequence
 from collections import defaultdict
 from itertools import zip_longest
 from ordered_set import OrderedSet
-from deepdiff.helper import (strings, bytes_type, numbers, uuids, times, ListItemRemovedOrAdded, notpresent,
+from deepdiff.helper import (strings, bytes_type, numbers, uuids, datetimes, ListItemRemovedOrAdded, notpresent,
                              IndexedHash, unprocessed, add_to_frozen_set, basic_types,
                              convert_item_or_items_into_set_else_none, get_type,
                              convert_item_or_items_into_compiled_regexes_else_none,
                              type_is_subclass_of_type_group, type_in_type_group, get_doc,
                              number_to_string, datetime_normalize, KEY_TO_VAL_STR, booleans,
                              np_ndarray, np_floating, get_numpy_ndarray_rows, OrderedSetPlus, RepeatedTimer,
                              TEXT_VIEW, TREE_VIEW, DELTA_VIEW, detailed__dict__, add_root_to_paths,
-                             np, get_truncate_datetime, dict_, CannotCompare, ENUM_INCLUDE_KEYS)
+                             np, get_truncate_datetime, dict_, CannotCompare, ENUM_INCLUDE_KEYS,
+                             PydanticBaseModel, )
 from deepdiff.serialization import SerializationMixin
 from deepdiff.distance import DistanceMixin
 from deepdiff.model import (
     RemapDict, ResultDict, TextResult, TreeResult, DiffLevel,
     DictRelationship, AttributeRelationship, REPORT_KEYS,
     SubscriptableIterableRelationship, NonSubscriptableIterableRelationship,
     SetRelationship, NumpyArrayRelationship, CUSTOM_FIELD, PrettyOrderedSet, )
@@ -448,15 +449,15 @@
         skip = False
         if self.exclude_paths and level_path in self.exclude_paths:
             skip = True
         if self.include_paths and level_path != 'root':
             if level_path not in self.include_paths:
                 skip = True
                 for prefix in self.include_paths:
-                    if level_path.startswith(prefix):
+                    if prefix in level_path or level_path in prefix:
                         skip = False
                         break
         elif self.exclude_regex_paths and any(
                 [exclude_regex_path.search(level_path) for exclude_regex_path in self.exclude_regex_paths]):
             skip = True
         elif self.exclude_types_tuple and \
                 (isinstance(level.t1, self.exclude_types_tuple) or isinstance(level.t2, self.exclude_types_tuple)):
@@ -1525,15 +1526,15 @@
 
         if isinstance(level.t1, booleans):
             self._diff_booleans(level, local_tree=local_tree)
 
         if isinstance(level.t1, strings):
             self._diff_str(level, local_tree=local_tree)
 
-        elif isinstance(level.t1, times):
+        elif isinstance(level.t1, datetimes):
             self._diff_datetimes(level, local_tree=local_tree)
 
         elif isinstance(level.t1, uuids):
             self._diff_uuids(level, local_tree=local_tree)
 
         elif isinstance(level.t1, numbers):
             self._diff_numbers(level, local_tree=local_tree, report_type_change=report_type_change)
@@ -1546,14 +1547,17 @@
 
         elif isinstance(level.t1, (set, frozenset, OrderedSet)):
             self._diff_set(level, local_tree=local_tree)
 
         elif isinstance(level.t1, np_ndarray):
             self._diff_numpy_array(level, parents_ids, local_tree=local_tree)
 
+        elif isinstance(level.t1, PydanticBaseModel):
+            self._diff_obj(level, parents_ids, local_tree=local_tree)
+
         elif isinstance(level.t1, Iterable):
             self._diff_iterable(level, parents_ids, _original_type=_original_type, local_tree=local_tree)
 
         elif isinstance(level.t1, Enum):
             self._diff_enum(level, parents_ids, local_tree=local_tree)
 
         else:
```

### Comparing `deepdiff-6.3.0/deepdiff/distance.py` & `deepdiff-6.3.1/deepdiff/distance.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/deepdiff/helper.py` & `deepdiff-6.3.1/deepdiff/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 from threading import Timer
 
 
 class np_type:
     pass
 
 
+class pydantic_base_model_type:
+    pass
+
+
 try:
     import numpy as np
 except ImportError:  # pragma: no cover. The case without Numpy is tested locally only.
     np = None  # pragma: no cover.
     np_array_factory = 'numpy not available'  # pragma: no cover.
     np_ndarray = np_type  # pragma: no cover.
     np_bool_ = np_type  # pragma: no cover.
@@ -80,14 +84,20 @@
 numpy_dtypes = set(numpy_numbers)
 numpy_dtypes.add(np_bool_)
 
 numpy_dtype_str_to_type = {
     item.__name__: item for item in numpy_dtypes
 }
 
+try:
+    from pydantic.main import BaseModel as PydanticBaseModel
+except ImportError:
+    PydanticBaseModel = pydantic_base_model_type
+
+
 logger = logging.getLogger(__name__)
 
 py_major_version = sys.version_info.major
 py_minor_version = sys.version_info.minor
 
 py_current_version = Decimal("{}.{}".format(py_major_version, py_minor_version))
```

### Comparing `deepdiff-6.3.0/deepdiff/lfucache.py` & `deepdiff-6.3.1/deepdiff/lfucache.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/deepdiff/model.py` & `deepdiff-6.3.1/deepdiff/model.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/deepdiff/operator.py` & `deepdiff-6.3.1/deepdiff/operator.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/deepdiff/path.py` & `deepdiff-6.3.1/deepdiff/path.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,14 +107,32 @@
         if action == GET:
             obj = obj[elem]
         elif action == GETATTR:
             obj = getattr(obj, elem)
     return obj
 
 
+def _get_nested_obj_and_force(obj, elements):
+    for (elem, action) in elements:
+        if action == GET:
+            try:
+                obj = obj[elem]
+            except KeyError:
+                obj[elem] = {}
+                obj = obj[elem]
+            except IndexError:
+                if isinstance(obj, list) and isinstance(elem, int) and elem >= len(obj):
+                    obj.extend([None] * (elem - len(obj)))
+                    obj.append({})
+                    obj = obj[-1]
+        elif action == GETATTR:
+            obj = getattr(obj, elem)
+    return obj
+
+
 def extract(obj, path):
     """
     Get the item from obj based on path.
 
     Example:
 
         >>> from deepdiff import extract
```

### Comparing `deepdiff-6.3.0/deepdiff/search.py` & `deepdiff-6.3.1/deepdiff/search.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/deepdiff/serialization.py` & `deepdiff-6.3.1/deepdiff/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,24 @@
 import ordered_set  # NOQA
 import collections  # NOQA
 try:
     import yaml
 except ImportError:  # pragma: no cover.
     yaml = None  # pragma: no cover.
 try:
-    import toml
+    if sys.version_info >= (3, 11):
+        import tomllib as tomli
+    else:
+        import tomli
+except ImportError:  # pragma: no cover.
+    tomli = None  # pragma: no cover.
+try:
+    import tomli_w
 except ImportError:  # pragma: no cover.
-    toml = None  # pragma: no cover.
+    tomli_w = None  # pragma: no cover.
 try:
     import clevercsv
     csv = None
 except ImportError:  # pragma: no cover.
     import csv
     clevercsv = None  # pragma: no cover.
 try:
@@ -426,18 +433,18 @@
             content = json_loads(the_file.read())
     elif file_type in {'yaml', 'yml'}:
         if yaml is None:  # pragma: no cover.
             raise ImportError('Pyyaml needs to be installed.')  # pragma: no cover.
         with open(path, 'r') as the_file:
             content = yaml.safe_load(the_file)
     elif file_type == 'toml':
-        if toml is None:  # pragma: no cover.
-            raise ImportError('Toml needs to be installed.')  # pragma: no cover.
-        with open(path, 'r') as the_file:
-            content = toml.load(the_file)
+        if tomli is None:  # pragma: no cover.
+            raise ImportError('On python<=3.10 tomli needs to be installed.')  # pragma: no cover.
+        with open(path, 'rb') as the_file:
+            content = tomli.load(the_file)
     elif file_type == 'pickle':
         with open(path, 'rb') as the_file:
             content = the_file.read()
             content = pickle_load(content)
     elif file_type in {'csv', 'tsv'}:
         if clevercsv:  # pragma: no cover.
             content = clevercsv.read_dicts(path)
@@ -491,18 +498,18 @@
             the_file.write(content)
     elif file_type in {'yaml', 'yml'}:
         if yaml is None:  # pragma: no cover.
             raise ImportError('Pyyaml needs to be installed.')  # pragma: no cover.
         with open(path, 'w') as the_file:
             content = yaml.safe_dump(content, stream=the_file)
     elif file_type == 'toml':
-        if toml is None:  # pragma: no cover.
-            raise ImportError('Toml needs to be installed.')  # pragma: no cover.
-        with open(path, 'w') as the_file:
-            content = toml.dump(content, the_file)
+        if tomli_w is None:  # pragma: no cover.
+            raise ImportError('Tomli-w needs to be installed.')  # pragma: no cover.
+        with open(path, 'wb') as the_file:
+            content = tomli_w.dump(content, the_file)
     elif file_type == 'pickle':
         with open(path, 'wb') as the_file:
             content = pickle_dump(content, file_obj=the_file)
     elif file_type in {'csv', 'tsv'}:
         if clevercsv:  # pragma: no cover.
             dict_writer = clevercsv.DictWriter
         else:
```

### Comparing `deepdiff-6.3.0/deepdiff.egg-info/PKG-INFO` & `deepdiff-6.3.1/deepdiff.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: deepdiff
-Version: 6.3.0
+Version: 6.3.1
 Summary: Deep Difference and Search of any Python object/data. Recreate objects by adding adding deltas to each other.
 Home-page: https://github.com/seperman/deepdiff
+Download-URL: https://github.com/seperman/deepdiff/tarball/master
 Author: Seperman
 Author-email: sep@zepworks.com
 License: MIT
-Download-URL: https://github.com/seperman/deepdiff/tarball/master
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,15 +21,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: optimize
 License-File: LICENSE
 License-File: AUTHORS.md
 
-# DeepDiff v 6.3.0
+# DeepDiff v 6.3.1
 
 ![Downloads](https://img.shields.io/pypi/dm/deepdiff.svg?style=flat)
 ![Python Versions](https://img.shields.io/pypi/pyversions/deepdiff.svg?style=flat)
 ![License](https://img.shields.io/pypi/l/deepdiff.svg?version=latest)
 [![Build Status](https://github.com/seperman/deepdiff/workflows/Unit%20Tests/badge.svg)](https://github.com/seperman/deepdiff/actions)
 [![codecov](https://codecov.io/gh/seperman/deepdiff/branch/master/graph/badge.svg?token=KkHZ3siA3m)](https://codecov.io/gh/seperman/deepdiff)
 
@@ -41,55 +40,75 @@
 - [DeepHash](https://zepworks.com/deepdiff/current/deephash.html): Hash any object based on their content.
 - [Delta](https://zepworks.com/deepdiff/current/delta.html): Store the difference of objects and apply them to other objects.
 - [Extract](https://zepworks.com/deepdiff/current/extract.html): Extract an item from a nested Python object using its path.
 - [commandline](https://zepworks.com/deepdiff/current/commandline.html): Use DeepDiff from commandline.
 
 Tested on Python 3.7+ and PyPy3.
 
-- **[Documentation](https://zepworks.com/deepdiff/6.3.0/)**
+- **[Documentation](https://zepworks.com/deepdiff/6.3.1/)**
 
 ## What is new?
 
 Please check the [ChangeLog](CHANGELOG.md) file for the detailed information.
 
+DeepDiff 6-3-1
+
+This release includes many bug fixes.
+
+- Bugfix deephash for paths by [maggelus](https://github.com/maggelus)
+- Bugfix deephash compiled regex [maggelus](https://github.com/maggelus)
+- Fix tests dependent on toml by [martin-kokos](https://github.com/martin-kokos)
+- Bugfix for `include_paths` for nested dictionaries by [kor4ik](https://github.com/kor4ik)
+- Use tomli and tomli-w for dealing with tomli files by [martin-kokos](https://github.com/martin-kokos)
+- Bugfix for `datetime.date` by [Alex Sauer-Budge](https://github.com/amsb)
+
+
 DeepDiff 6-3-0
 
-- `PrefixOrSuffixOperator`: This operator will skip strings that are suffix or prefix of each other.
-- `include_obj_callback` and `include_obj_callback_strict` are added by [Håvard Thom](https://github.com/havardthom).
+- [`PrefixOrSuffixOperator`](https://zepworks.com/deepdiff/current/custom.html#prefix-or-suffix-operator-label): This operator will skip strings that are suffix or prefix of each other.
+- [`include_obj_callback`](https://zepworks.com/deepdiff/current/ignore_types_or_values.html#include-obj-callback-label) and `include_obj_callback_strict` are added by [Håvard Thom](https://github.com/havardthom).
 - Fixed a corner case where numpy's `np.float32` nans are not ignored when using `ignore_nan_equality` by [Noam Gottlieb](https://github.com/noamgot)
 - `orjson` becomes optional again.
 - Fix for `ignore_type_in_groups` with numeric values so it does not report number changes when the number types are different.
 
-DeepDiff 6-2-0
-
-- Major improvement in the diff report for lists when items are all hashable and the order of items is important.
-
-
 ## Installation
 
 ### Install from PyPi:
 
 `pip install deepdiff`
 
 If you want to use DeepDiff from commandline:
 
 `pip install "deepdiff[cli]"`
 
 If you want to improve the performance of DeepDiff with certain functionalities such as improved json serialization:
 
 `pip install "deepdiff[optimize]"`
 
+Install optional packages:
+- [yaml](https://pypi.org/project/PyYAML/)
+- [tomli](https://pypi.org/project/tomli/) (python 3.10 and older) and [tomli-w](https://pypi.org/project/tomli-w/) for writing
+- [clevercsv](https://pypi.org/project/clevercsv/) for more rubust CSV parsing
+- [orjson](https://pypi.org/project/orjson/) for speed and memory optimized parsing
+- [pydantic](https://pypi.org/project/pydantic/)
+
+
 # Documentation
 
 <https://zepworks.com/deepdiff/current/>
 
 # ChangeLog
 
 Please take a look at the [CHANGELOG](CHANGELOG.md) file.
 
+# Survey
+
+:mega: **Please fill out our [fast 5-question survey](https://forms.gle/E6qXexcgjoKnSzjB8)** so that we can learn how & why you use DeepDiff, and what improvements we should make. Thank you! :dancers:
+
+
 # Contribute
 
 1. Please make your PR against the dev branch
 2. Please make sure that your PR has tests. Since DeepDiff is used in many sensitive data driven projects, we strive to maintain around 100% test coverage on the code.
 
 Please run `pytest --cov=deepdiff --runslow` to see the coverage report. Note that the `--runslow` flag will run some slow tests too. In most cases you only want to run the fast tests which so you wont add the `--runslow` flag.
 
@@ -97,18 +116,16 @@
 
 Thank you!
 
 # Citing
 
 How to cite this library (APA style):
 
-    Dehpour, S. (2022). DeepDiff (Version 6.3.0) [Software]. Available from https://github.com/seperman/deepdiff.
+    Dehpour, S. (2023). DeepDiff (Version 6.3.1) [Software]. Available from https://github.com/seperman/deepdiff.
 
 How to cite this library (Chicago style):
 
-    Dehpour, Sep. 2022. DeepDiff (version 6.3.0).
+    Dehpour, Sep. 2023. DeepDiff (version 6.3.1).
 
 # Authors
 
 Please take a look at the [AUTHORS](AUTHORS.md) file.
-
-
```

### Comparing `deepdiff-6.3.0/deepdiff.egg-info/SOURCES.txt` & `deepdiff-6.3.1/deepdiff.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=500__cutoff_intersection_for_pairs=1.png
 docs/_static/benchmark_numpy_array__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
 tests/__init__.py
 tests/test_anyset.py
 tests/test_cache.py
 tests/test_command.py
 tests/test_delta.py
+tests/test_diff_datetime.py
 tests/test_diff_math.py
 tests/test_diff_numpy.py
 tests/test_diff_other.py
 tests/test_diff_text.py
 tests/test_diff_tree.py
 tests/test_distance.py
 tests/test_hash.py
```

### Comparing `deepdiff-6.3.0/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-6.3.1/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=10000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-6.3.1/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=10000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/_static/benchmark_big_jsons__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png` & `deepdiff-6.3.1/docs/_static/benchmark_big_jsons__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/_static/benchmark_big_jsons__pypy3.6__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png` & `deepdiff-6.3.1/docs/_static/benchmark_big_jsons__pypy3.6__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-6.3.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=5000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-6.3.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=5000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-6.3.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=500__cutoff_intersection_for_pairs=1.png` & `deepdiff-6.3.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=500__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/_static/benchmark_numpy_array__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-6.3.1/docs/_static/benchmark_numpy_array__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/authors.rst` & `deepdiff-6.3.1/docs/authors.rst`

 * *Files 10% similar despite different names*

```diff
@@ -67,15 +67,26 @@
 -  `martin-kokos <https://github.com/martin-kokos>`__ for using Pytest’s
    tmp_path fixture instead of /tmp/
 -  Håvard Thom `havardthom <https://github.com/havardthom>`__ for adding
    include_obj_callback and include_obj_callback_strict.
 -  `Noam Gottlieb <https://github.com/noamgot>`__ for fixing a corner
    case where numpy’s ``np.float32`` nans are not ignored when using
    ``ignore_nan_equality``.
-
+-  `maggelus <https://github.com/maggelus>`__ for the bugfix deephash
+   for paths.
+-  `maggelus <https://github.com/maggelus>`__ for the bugfix deephash
+   compiled regex.
+-  `martin-kokos <https://github.com/martin-kokos>`__ for fixing the
+   tests dependent on toml.
+-  `kor4ik <https://github.com/kor4ik>`__ for the bugfix for
+   ``include_paths`` for nested dictionaries.
+-  `martin-kokos <https://github.com/martin-kokos>`__ for using tomli
+   and tomli-w for dealing with tomli files.
+-  `Alex Sauer-Budge <https://github.com/amsb>`__ for the bugfix for
+   ``datetime.date``.
 
 .. _Sep Dehpour (Seperman): http://www.zepworks.com
 .. _Victor Hahn Castell: http://hahncastell.de
 .. _nfvs: https://github.com/nfvs
 .. _brbsix: https://github.com/brbsix
 .. _WangFenjin: https://github.com/WangFenjin
 .. _timoilya: https://github.com/timoilya
```

### Comparing `deepdiff-6.3.0/docs/basics.rst` & `deepdiff-6.3.1/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/changelog.rst` & `deepdiff-6.3.1/docs/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 :doc:`/index`
 
 Changelog
 =========
 
 DeepDiff Changelog
 
+-  v6-3-1
+
+   -  Bugfix deephash for paths by
+      `maggelus <https://github.com/maggelus>`__
+   -  Bugfix deephash compiled regex
+      `maggelus <https://github.com/maggelus>`__
+   -  Fix tests dependent on toml by
+      `martin-kokos <https://github.com/martin-kokos>`__
+   -  Bugfix for ``include_paths`` for nested dictionaries by
+      `kor4ik <https://github.com/kor4ik>`__
+   -  Use tomli and tomli-w for dealing with tomli files by
+      `martin-kokos <https://github.com/martin-kokos>`__
+   -  Bugfix for ``datetime.date`` by `Alex
+      Sauer-Budge <https://github.com/amsb>`__
+
 -  v6-3-0
 
    -  ``PrefixOrSuffixOperator``: This operator will skip strings that
       are suffix or prefix of each other.
    -  ``include_obj_callback`` and ``include_obj_callback_strict`` are
       added by `Håvard Thom <https://github.com/havardthom>`__.
    -  Fixed a corner case where numpy’s ``np.float32`` nans are not
```

### Comparing `deepdiff-6.3.0/docs/commandline.rst` & `deepdiff-6.3.1/docs/commandline.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/custom.rst` & `deepdiff-6.3.1/docs/custom.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/deep_distance.rst` & `deepdiff-6.3.1/docs/deep_distance.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/deephash_doc.rst` & `deepdiff-6.3.1/docs/deephash_doc.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/delta.rst` & `deepdiff-6.3.1/docs/delta.rst`

 * *Files 4% similar despite different names*

```diff
@@ -412,7 +412,54 @@
 >>> delta2 = Delta(diff, raise_errors=False, verify_symmetry=True)
 >>> t4 = delta2 + t3
 Expected the old value for root[0] to be 1 but it is 3. Error found on: while checking the symmetry of the delta. You have applied the delta to an object that has different values than the original object the delta was made from
 >>> t4
 [2]
 
 And if you had set raise_errors=True, then it would have raised the error in addition to logging it.
+
+
+.. _delta_force_label:
+
+Delta Force
+-----------
+
+force : Boolean, default=False
+    force is used to force apply a delta to objects that have a very different structure.
+
+
+>>> from deepdiff import DeepDiff, Delta
+>>> t1 = {
+...     'x': {
+...         'y': [1, 2, 3]
+...     },
+...     'q': {
+...         'r': 'abc',
+...     }
+... }
+>>>
+>>> t2 = {
+...     'x': {
+...         'y': [1, 2, 3, 4]
+...     },
+...     'q': {
+...         'r': 'abc',
+...         't': 0.5,
+...     }
+... }
+>>>
+>>> diff = DeepDiff(t1, t2)
+>>> diff
+{'dictionary_item_added': [root['q']['t']], 'iterable_item_added': {"root['x']['y'][3]": 4}}
+>>> delta = Delta(diff)
+>>> {} + delta
+Unable to get the item at root['x']['y'][3]: 'x'
+Unable to get the item at root['q']['t']
+{}
+
+# Once we set the force to be True
+
+>>> delta = Delta(diff, force=True)
+>>> {} + delta
+{'x': {'y': {3: 4}}, 'q': {'t': 0.5}}
+
+Notice that the force attribute does not know the original object at ['x']['y'] was supposed to be a list, so it assumes it was a dictionary.
```

### Comparing `deepdiff-6.3.0/docs/diff_doc.rst` & `deepdiff-6.3.1/docs/diff_doc.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/exclude_paths.rst` & `deepdiff-6.3.1/docs/exclude_paths.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/faq.rst` & `deepdiff-6.3.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/ignore_order.rst` & `deepdiff-6.3.1/docs/ignore_order.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/ignore_types_or_values.rst` & `deepdiff-6.3.1/docs/ignore_types_or_values.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/index.rst` & `deepdiff-6.3.1/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. DeepDiff documentation master file, created by
    sphinx-quickstart on Mon Jul 20 06:06:44 2015.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 
-DeepDiff 6.3.0 documentation!
+DeepDiff 6.3.1 documentation!
 =============================
 
 *******
 Modules
 *******
 
 The DeepDiff library includes the following modules:
@@ -28,33 +28,46 @@
 - **Commandline** Most of the above functionality is also available via the commandline module  :doc:`/commandline`
 
 ***********
 What is New
 ***********
 
 
+DeepDiff 6-3-1
+--------------
+
+This release includes many bug fixes.
+
+-  Bugfix deephash for paths by
+  `maggelus <https://github.com/maggelus>`__
+-  Bugfix deephash compiled regex
+  `maggelus <https://github.com/maggelus>`__
+-  Fix tests dependent on toml by
+  `martin-kokos <https://github.com/martin-kokos>`__
+-  Bugfix for ``include_paths`` for nested dictionaries by
+  `kor4ik <https://github.com/kor4ik>`__
+-  Use tomli and tomli-w for dealing with tomli files by
+  `martin-kokos <https://github.com/martin-kokos>`__
+-  Bugfix for ``datetime.date`` by `Alex
+  Sauer-Budge <https://github.com/amsb>`__
+
+
 DeepDiff 6-3-0
 --------------
 
 -  :ref:`prefix_or_suffix_operator_label`: This operator will skip strings that are
    suffix or prefix of each other.
 -  :ref:`include_obj_callback_label` and :ref:`include_obj_callback_strict_label` are
    added by `Håvard Thom <https://github.com/havardthom>`__.
 -  Fixed a corner case where numpy’s ``np.float32`` nans are not ignored
    when using ``ignore_nan_equality`` by `Noam
    Gottlieb <https://github.com/noamgot>`__
 -  ``orjson`` becomes optional again.
 -  Fix for ``ignore_type_in_groups`` with numeric values so it does not report number changes when the number types are different.
 
-DeepDiff 6-2-0
---------------
-
--  Major improvement in the diff report for lists when items are all hashable and the order of items is important.
-
-
 *********
 Tutorials
 *********
 
 Tutorials can be found on `Zepworks blog <https://zepworks.com/tags/deepdiff/>`_
 
 ************
```

### Comparing `deepdiff-6.3.0/docs/numbers.rst` & `deepdiff-6.3.1/docs/numbers.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/optimizations.rst` & `deepdiff-6.3.1/docs/optimizations.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/other.rst` & `deepdiff-6.3.1/docs/other.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/search_doc.rst` & `deepdiff-6.3.1/docs/search_doc.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/serialization.rst` & `deepdiff-6.3.1/docs/serialization.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/stats.rst` & `deepdiff-6.3.1/docs/stats.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/support.rst` & `deepdiff-6.3.1/docs/support.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/troubleshoot.rst` & `deepdiff-6.3.1/docs/troubleshoot.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/docs/view.rst` & `deepdiff-6.3.1/docs/view.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/setup.py` & `deepdiff-6.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     sys.exit('Python 2 is not supported anymore. The last version of DeepDiff that supported Py2 was 3.3.0')
 
 # if you are not using vagrant, just delete os.link directly,
 # The hard link only saves a little disk space, so you should not care
 if os.environ.get('USER', '') == 'vagrant':
     del os.link
 
-version = '6.3.0'
+version = '6.3.1'
 
 
 def get_reqs(filename):
     with open(filename, "r") as reqs_file:
         reqs = reqs_file.readlines()
     return reqs
```

### Comparing `deepdiff-6.3.0/tests/__init__.py` & `deepdiff-6.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/fixtures/compare_func_result1.json` & `deepdiff-6.3.1/tests/fixtures/compare_func_result1.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/fixtures/compare_func_t1.json` & `deepdiff-6.3.1/tests/fixtures/compare_func_t1.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/fixtures/compare_func_t2.json` & `deepdiff-6.3.1/tests/fixtures/compare_func_t2.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/fixtures/nested_a_result.json` & `deepdiff-6.3.1/tests/fixtures/nested_a_result.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/fixtures/nested_a_t1.json` & `deepdiff-6.3.1/tests/fixtures/nested_a_t1.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/fixtures/nested_a_t2.json` & `deepdiff-6.3.1/tests/fixtures/nested_a_t2.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_anyset.py` & `deepdiff-6.3.1/tests/test_anyset.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_cache.py` & `deepdiff-6.3.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_command.py` & `deepdiff-6.3.1/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_delta.py` & `deepdiff-6.3.1/tests/test_delta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1664,7 +1664,34 @@
             }
         ]}
 
         ddiff = DeepDiff(t1, t2, iterable_compare_func=self.compare_func, verbose_level=2)
         delta = Delta(ddiff)
         recreated_t2 = t1 + delta
         assert t2 == recreated_t2
+
+    def test_delta_force1(self):
+        t1 = {
+            'x': {
+                'y': [1, 2, 3]
+            },
+            'q': {
+                'r': 'abc',
+            }
+        }
+
+        t2 = {
+            'x': {
+                'y': [1, 2, 3, 4]
+            },
+            'q': {
+                'r': 'abc',
+                't': 0.5,
+            }
+        }
+
+        diff = DeepDiff(t1, t2)
+
+        delta = Delta(diff=diff, force=True)
+        result = {} + delta
+        expected = {'x': {'y': {3: 4}}, 'q': {'t': 0.5}}
+        assert expected == result
```

### Comparing `deepdiff-6.3.0/tests/test_diff_math.py` & `deepdiff-6.3.1/tests/test_diff_math.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_diff_numpy.py` & `deepdiff-6.3.1/tests/test_diff_numpy.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_diff_other.py` & `deepdiff-6.3.1/tests/test_diff_other.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_diff_text.py` & `deepdiff-6.3.1/tests/test_diff_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python
 import datetime
 import pytest
 import logging
 import uuid
 from enum import Enum
+from typing import List
 from decimal import Decimal
 from deepdiff import DeepDiff
-from deepdiff.helper import pypy3
+from deepdiff.helper import pypy3, PydanticBaseModel
 from tests import CustomClass
 
+
 logging.disable(logging.CRITICAL)
 
 
 class TestDeepDiffText:
     """DeepDiff Tests."""
 
     def test_same_objects(self):
@@ -1768,7 +1770,37 @@
                 "root[3]": {
                     "new_value": datetime.datetime(2012, 5, 31, 0, 0),
                     "old_value": datetime.datetime(2015, 5, 31, 0, 0),
                 },
             },
             "iterable_item_removed": {"root[4]": datetime.datetime(2015, 7, 31, 0, 0)},
         }
+
+    def test_pydantic1(self):
+
+        class Foo(PydanticBaseModel):
+            thing: int = None
+            that: str
+
+        t1 = Foo(thing=1, that='yes')
+        t2 = Foo(thing=2, that='yes')
+
+        diff = DeepDiff(t1, t2)
+        expected = {'values_changed': {'root.thing': {'new_value': 2, 'old_value': 1}}}
+        assert expected == diff
+
+    def test_pydantic2(self):
+
+        class Foo(PydanticBaseModel):
+            thing: int = None
+            that: str
+
+        class Bar(PydanticBaseModel):
+            stuff: List[Foo]
+
+        t1 = Bar(stuff=[Foo(thing=1, that='yes')])
+        t2 = Bar(stuff=[Foo(thing=2, that='yes')])
+
+        diff = DeepDiff(t1, t2)
+        expected = {'values_changed': {'root.stuff[0].thing': {'new_value': 2, 'old_value': 1}}}
+        assert expected == diff
+
```

### Comparing `deepdiff-6.3.0/tests/test_diff_tree.py` & `deepdiff-6.3.1/tests/test_diff_tree.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_distance.py` & `deepdiff-6.3.1/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_hash.py` & `deepdiff-6.3.1/tests/test_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 import re
 import pytest
+from pathlib import Path
 import logging
 import datetime
 from collections import namedtuple
 from functools import partial
 from enum import Enum
 from deepdiff import DeepHash
 from deepdiff.deephash import (
@@ -148,14 +149,26 @@
     def test_sha1_hash_not_sensitive_to_bytecode_vs_unicode(self):
         a = 'hello'
         b = b'hello'
         a_hash = DeepHash(a, ignore_string_type_changes=True, hasher=DeepHash.sha1hex)[a]
         b_hash = DeepHash(b, ignore_string_type_changes=True, hasher=DeepHash.sha1hex)[b]
         assert a_hash == b_hash
 
+    def test_path(self):
+        a = Path('testdir')
+        b = Path('testdir2')
+        a_hash = DeepHash(a)[a]
+        b_hash = DeepHash(b)[b]
+        assert a_hash != b_hash
+
+    def test_re(self):
+        import re
+        a = re.compile("asdf.?")
+        a_hash = DeepHash(a)[a]
+        assert not( a_hash is unprocessed)
 
 class TestDeepHashPrep:
     """DeepHashPrep Tests covering object serialization."""
 
     def test_prep_bool_vs_num1(self):
         assert {BoolObj.TRUE: 'bool:true'} == DeepHashPrep(True)
         assert {1: 'int:1'} == DeepHashPrep(1)
```

### Comparing `deepdiff-6.3.0/tests/test_helper.py` & `deepdiff-6.3.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_ignore_order.py` & `deepdiff-6.3.1/tests/test_ignore_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,32 +172,52 @@
                     'value': 4,
                     'new_repeat': 2
                 }
             }
         }
         assert result == ddiff
 
-    # TODO: fix repeition report
-    def test_nested_list_ignore_order_report_repetition_wrong_currently(self):
+    def test_nested_list_ignore_order_report_repetition(self):
         t1 = [1, 2, [3, 4]]
         t2 = [[4, 3, 3], 2, 1]
-        ddiff = DeepDiff(t1, t2, ignore_order=True, report_repetition=True)
+        ddiff = DeepDiff(t1, t2, ignore_order=True, report_repetition=False)
+        assert not ddiff
+
+        ddiff2 = DeepDiff(t1, t2, ignore_order=True, report_repetition=True)
         result = {
             'repetition_change': {
                 'root[2][0]': {
                     'old_repeat': 1,
+                    'new_repeat': 2,
+                    'old_indexes': [0],
                     'new_indexes': [1, 2],
-                    'old_indexes': [1],
-                    'value': 3,
-                    'new_repeat': 2
+                    'value': 3
                 }
             }
         }
-        assert result != ddiff
-        assert {"root[2][0]"} == ddiff.affected_paths
+        assert result == ddiff2
+        assert {"root[2][0]"} == ddiff2.affected_paths
+
+    @pytest.mark.skip
+    def test_nested_list_and_dict_ignore_order_report_repetition(self):
+        """
+        This test shows that ignore order is not doing the right thing.
+
+        It should have said that root[1] and root[2] are removed.
+        """
+        t1 = [{"id": 1}, {"id": 1}, {"id": 1}]
+        t2 = [{"id": 1, "name": 1}]
+        ddiff = DeepDiff(t1, t2, ignore_order=True)
+        result = {'dictionary_item_added': ["root[0]['name']"]}
+        assert result == ddiff
+
+        # Here there is nothing that is "repeated" in an iterable
+        ddiff2 = DeepDiff(t1, t2, ignore_order=True, report_repetition=True)
+        assert result == ddiff2
+        assert {"root[2][0]"} == ddiff2.affected_paths
 
     def test_list_of_unhashable_difference_ignore_order(self):
         t1 = [{"a": 2}, {"b": [3, 4, {1: 1}]}]
         t2 = [{"b": [3, 4, {1: 1}]}, {"a": 2}]
         ddiff = DeepDiff(t1, t2, ignore_order=True)
         assert {} == ddiff
```

### Comparing `deepdiff-6.3.0/tests/test_lfucache.py` & `deepdiff-6.3.1/tests/test_lfucache.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_model.py` & `deepdiff-6.3.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_operators.py` & `deepdiff-6.3.1/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_path.py` & `deepdiff-6.3.1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_search.py` & `deepdiff-6.3.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.3.0/tests/test_serialization.py` & `deepdiff-6.3.1/tests/test_serialization.py`

 * *Files identical despite different names*

