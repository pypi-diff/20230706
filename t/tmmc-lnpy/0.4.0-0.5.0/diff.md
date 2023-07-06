# Comparing `tmp/tmmc-lnpy-0.4.0.tar.gz` & `tmp/tmmc-lnpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmmc-lnpy-0.4.0.tar", last modified: Fri May 12 20:08:59 2023, max compression
+gzip compressed data, was "tmmc-lnpy-0.5.0.tar", last modified: Thu Jul  6 19:19:49 2023, max compression
```

## Comparing `tmmc-lnpy-0.4.0.tar` & `tmmc-lnpy-0.5.0.tar`

### file list

```diff
@@ -1,97 +1,100 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.759583 tmmc-lnpy-0.4.0/
--rw-r--r--   0 wpk      (42033)    36681     1492 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/.editorconfig
--rw-r--r--   0 wpk      (42033)    36681     1347 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3683 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      684 2023-05-04 19:22:49.000000 tmmc-lnpy-0.4.0/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-04-24 16:21:31.000000 tmmc-lnpy-0.4.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681     2087 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9663 2023-05-04 19:22:49.000000 tmmc-lnpy-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-13 20:07:49.000000 tmmc-lnpy-0.4.0/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      285 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681    11436 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/Makefile
--rw-r--r--   0 wpk      (42033)    36681     9142 2023-05-12 20:08:59.759097 tmmc-lnpy-0.4.0/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     4460 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.726364 tmmc-lnpy-0.4.0/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.726737 tmmc-lnpy-0.4.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.728287 tmmc-lnpy-0.4.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.734166 tmmc-lnpy-0.4.0/environment/
--rw-r--r--   0 wpk      (42033)    36681      979 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      356 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      108 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       79 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      670 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      523 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       53 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      207 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033)    36681       25 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      198 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033)    36681      187 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment.yaml
--rw-r--r--   0 wpk      (42033)    36681     6155 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.738529 tmmc-lnpy-0.4.0/scripts/
--rw-r--r--   0 wpk      (42033)    36681      840 2023-05-04 19:22:49.000000 tmmc-lnpy-0.4.0/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033)    36681      312 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033)    36681     1099 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      266 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/scripts/lint.mk
--rw-r--r--   0 wpk      (42033)    36681      598 2023-05-04 19:22:49.000000 tmmc-lnpy-0.4.0/scripts/recipe-append.sh
--rw-r--r--   0 wpk      (42033)    36681       91 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033)    36681      489 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033)    36681       38 2023-05-12 20:08:59.759688 tmmc-lnpy-0.4.0/setup.cfg
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.714485 tmmc-lnpy-0.4.0/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.739950 tmmc-lnpy-0.4.0/src/lnPi/
--rw-r--r--   0 wpk      (42033)    36681      815 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnPi/__init__.py
--rw-r--r--   0 wpk      (42033)    36681      111 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnPi/collectionlnpiutils.py
--rw-r--r--   0 wpk      (42033)    36681       90 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnPi/stability.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.746514 tmmc-lnpy-0.4.0/src/lnpy/
--rw-r--r--   0 wpk      (42033)    36681     1744 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnpy/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     2664 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnpy/bracket.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.750374 tmmc-lnpy-0.4.0/src/lnpy/data/
--rw-r--r--   0 wpk      (42033)    36681   243309 2022-09-28 17:20:41.000000 tmmc-lnpy-0.4.0/src/lnpy/data/hsmix_example.json.gz
--rw-r--r--   0 wpk      (42033)    36681    38953 2023-04-14 22:51:35.000000 tmmc-lnpy-0.4.0/src/lnpy/data/lj_sub_example.json
--rw-r--r--   0 wpk      (42033)    36681    38751 2023-04-14 22:51:35.000000 tmmc-lnpy-0.4.0/src/lnpy/data/lj_sup_example.json
--rw-r--r--   0 wpk      (42033)    36681   450917 2022-09-28 17:20:41.000000 tmmc-lnpy-0.4.0/src/lnpy/data/ljmix_sup_example.json.gz
--rw-r--r--   0 wpk      (42033)    36681    61595 2023-04-14 22:51:35.000000 tmmc-lnpy-0.4.0/src/lnpy/data/watermof_example.json
--rw-r--r--   0 wpk      (42033)    36681     2270 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/docstrings.py
--rw-r--r--   0 wpk      (42033)    36681    34518 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/ensembles.py
--rw-r--r--   0 wpk      (42033)    36681     5004 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/src/lnpy/examples.py
--rw-r--r--   0 wpk      (42033)    36681    13203 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/extensions.py
--rw-r--r--   0 wpk      (42033)    36681    18031 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnpy/lnpicollectionutils.py
--rw-r--r--   0 wpk      (42033)    36681    18795 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/lnpidata.py
--rw-r--r--   0 wpk      (42033)    36681    22908 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/lnpienergy.py
--rw-r--r--   0 wpk      (42033)    36681    26234 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/lnpiseries.py
--rw-r--r--   0 wpk      (42033)    36681    15148 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/maskedlnpi_legacy.py
--rw-r--r--   0 wpk      (42033)    36681     6050 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnpy/molfrac.py
--rw-r--r--   0 wpk      (42033)    36681     3127 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/options.py
--rw-r--r--   0 wpk      (42033)    36681    20437 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/segment.py
--rw-r--r--   0 wpk      (42033)    36681    26446 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/stability.py
--rw-r--r--   0 wpk      (42033)    36681    14481 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnpy/utils.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.752957 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     9142 2023-05-12 20:08:59.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2083 2023-05-12 20:08:59.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-05-12 20:08:59.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681      112 2023-05-12 20:08:59.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681       10 2023-05-12 20:08:59.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-05-04 19:23:42.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.756067 tmmc-lnpy-0.4.0/tests/
--rw-r--r--   0 wpk      (42033)    36681     2540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/tests/test_hs_mix.py
--rw-r--r--   0 wpk      (42033)    36681       24 2023-04-05 21:34:36.000000 tmmc-lnpy-0.4.0/tests/test_import.py
--rw-r--r--   0 wpk      (42033)    36681     1852 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/tests/test_lj_mix_0.py
--rw-r--r--   0 wpk      (42033)    36681     5240 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/tests/test_lnPi.py
--rw-r--r--   0 wpk      (42033)    36681     5843 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/tests/test_single_comp_sub.py
--rw-r--r--   0 wpk      (42033)    36681     5081 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/tests/test_single_comp_super.py
--rw-r--r--   0 wpk      (42033)    36681     2802 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/tests/test_water_cluster.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.758416 tmmc-lnpy-0.4.0/tests/water_cluster/
--rw-r--r--   0 wpk      (42033)    36681      559 2022-09-14 17:15:37.000000 tmmc-lnpy-0.4.0/tests/water_cluster/data_0.csv
--rw-r--r--   0 wpk      (42033)    36681      116 2022-09-14 17:15:37.000000 tmmc-lnpy-0.4.0/tests/water_cluster/data_0_dw.csv
--rw-r--r--   0 wpk      (42033)    36681     3953 2022-09-14 17:15:37.000000 tmmc-lnpy-0.4.0/tests/water_cluster/data_1.csv
--rw-r--r--   0 wpk      (42033)    36681     4784 2022-09-14 17:15:37.000000 tmmc-lnpy-0.4.0/tests/water_cluster/data_1_dw.csv
--rw-r--r--   0 wpk      (42033)    36681      367 2023-04-14 22:51:35.000000 tmmc-lnpy-0.4.0/tests/water_cluster/water_MOF_ensemble.json
--rw-r--r--   0 wpk      (42033)    36681    29453 2022-09-14 17:15:37.000000 tmmc-lnpy-0.4.0/tests/water_cluster/water_MOF_example.csv
--rw-r--r--   0 wpk      (42033)    36681     4088 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.473082 tmmc-lnpy-0.5.0/
+-rw-r--r--   0 wpk      (42033)    36681     1487 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/.editorconfig
+-rw-r--r--   0 wpk      (42033)    36681     1402 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3683 2023-06-14 20:39:21.000000 tmmc-lnpy-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      684 2023-06-14 20:39:23.000000 tmmc-lnpy-0.5.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-04-24 16:21:31.000000 tmmc-lnpy-0.5.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681     2444 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681    11080 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-13 20:07:49.000000 tmmc-lnpy-0.5.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      285 2023-06-14 20:39:58.000000 tmmc-lnpy-0.5.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681     9596 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681     9764 2023-07-06 19:19:49.472289 tmmc-lnpy-0.5.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     4460 2023-06-14 20:40:01.000000 tmmc-lnpy-0.5.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.443077 tmmc-lnpy-0.5.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.443581 tmmc-lnpy-0.5.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.444429 tmmc-lnpy-0.5.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.450160 tmmc-lnpy-0.5.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      356 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/base.yaml
+-rw-r--r--   0 wpk      (42033)    36681      979 2023-05-12 20:08:22.000000 tmmc-lnpy-0.5.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      578 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      280 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/dist-pypi.txt
+-rw-r--r--   0 wpk      (42033)    36681      225 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      670 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      558 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681      207 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/environment/lint.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.451500 tmmc-lnpy-0.5.0/environment/lock/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/lock/py310.yaml
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/lock/py311.yaml
+-rw-r--r--   0 wpk      (42033)    36681       63 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/lock/py38.yaml
+-rw-r--r--   0 wpk      (42033)    36681       63 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/lock/py39.yaml
+-rw-r--r--   0 wpk      (42033)    36681      193 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/test-extras.txt
+-rw-r--r--   0 wpk      (42033)    36681      265 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      416 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      425 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/environment/typing.yaml
+-rw-r--r--   0 wpk      (42033)    36681      187 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/environment.yaml
+-rw-r--r--   0 wpk      (42033)    36681    32067 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/noxfile.py
+-rw-r--r--   0 wpk      (42033)    36681     7368 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/pyproject.toml
+-rw-r--r--   0 wpk      (42033)    36681       38 2023-07-06 19:19:49.473243 tmmc-lnpy-0.5.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.433661 tmmc-lnpy-0.5.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.452931 tmmc-lnpy-0.5.0/src/lnPi/
+-rw-r--r--   0 wpk      (42033)    36681      815 2023-04-04 21:54:21.000000 tmmc-lnpy-0.5.0/src/lnPi/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681      111 2023-04-04 21:54:21.000000 tmmc-lnpy-0.5.0/src/lnPi/collectionlnpiutils.py
+-rw-r--r--   0 wpk      (42033)    36681    15436 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnPi/maskedlnpi_legacy.py
+-rw-r--r--   0 wpk      (42033)    36681       90 2023-04-04 21:54:21.000000 tmmc-lnpy-0.5.0/src/lnPi/stability.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.458743 tmmc-lnpy-0.5.0/src/lnpy/
+-rw-r--r--   0 wpk      (42033)    36681     1164 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681      330 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/_lazy_imports.py
+-rw-r--r--   0 wpk      (42033)    36681      160 2023-07-06 19:19:49.000000 tmmc-lnpy-0.5.0/src/lnpy/_version.py
+-rw-r--r--   0 wpk      (42033)    36681     2664 2023-04-04 21:54:21.000000 tmmc-lnpy-0.5.0/src/lnpy/bracket.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.461578 tmmc-lnpy-0.5.0/src/lnpy/data/
+-rw-r--r--   0 wpk      (42033)    36681   243309 2022-09-28 17:20:41.000000 tmmc-lnpy-0.5.0/src/lnpy/data/hsmix_example.json.gz
+-rw-r--r--   0 wpk      (42033)    36681    38953 2023-04-14 22:51:35.000000 tmmc-lnpy-0.5.0/src/lnpy/data/lj_sub_example.json
+-rw-r--r--   0 wpk      (42033)    36681    38751 2023-04-14 22:51:35.000000 tmmc-lnpy-0.5.0/src/lnpy/data/lj_sup_example.json
+-rw-r--r--   0 wpk      (42033)    36681   450917 2022-09-28 17:20:41.000000 tmmc-lnpy-0.5.0/src/lnpy/data/ljmix_sup_example.json.gz
+-rw-r--r--   0 wpk      (42033)    36681    61595 2023-04-14 22:51:35.000000 tmmc-lnpy-0.5.0/src/lnpy/data/watermof_example.json
+-rw-r--r--   0 wpk      (42033)    36681     2270 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/src/lnpy/docstrings.py
+-rw-r--r--   0 wpk      (42033)    36681    34085 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/ensembles.py
+-rw-r--r--   0 wpk      (42033)    36681     4999 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/examples.py
+-rw-r--r--   0 wpk      (42033)    36681    13203 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/src/lnpy/extensions.py
+-rw-r--r--   0 wpk      (42033)    36681    18045 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/lnpicollectionutils.py
+-rw-r--r--   0 wpk      (42033)    36681    18808 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/lnpidata.py
+-rw-r--r--   0 wpk      (42033)    36681    22911 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/lnpienergy.py
+-rw-r--r--   0 wpk      (42033)    36681    26909 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/lnpiseries.py
+-rw-r--r--   0 wpk      (42033)    36681     6014 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/molfrac.py
+-rw-r--r--   0 wpk      (42033)    36681     3127 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/src/lnpy/options.py
+-rw-r--r--   0 wpk      (42033)    36681    20537 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/segment.py
+-rw-r--r--   0 wpk      (42033)    36681    26467 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/stability.py
+-rw-r--r--   0 wpk      (42033)    36681    14889 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/src/lnpy/utils.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.463878 tmmc-lnpy-0.5.0/src/tmmc_lnpy.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681     9764 2023-07-06 19:19:49.000000 tmmc-lnpy-0.5.0/src/tmmc_lnpy.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2129 2023-07-06 19:19:49.000000 tmmc-lnpy-0.5.0/src/tmmc_lnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-07-06 19:19:49.000000 tmmc-lnpy-0.5.0/src/tmmc_lnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681      783 2023-07-06 19:19:49.000000 tmmc-lnpy-0.5.0/src/tmmc_lnpy.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       10 2023-07-06 19:19:49.000000 tmmc-lnpy-0.5.0/src/tmmc_lnpy.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-05-04 19:23:42.000000 tmmc-lnpy-0.5.0/src/tmmc_lnpy.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.467448 tmmc-lnpy-0.5.0/tests/
+-rw-r--r--   0 wpk      (42033)    36681     2540 2023-06-30 14:23:19.000000 tmmc-lnpy-0.5.0/tests/test_hs_mix.py
+-rw-r--r--   0 wpk      (42033)    36681      132 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/tests/test_import.py
+-rw-r--r--   0 wpk      (42033)    36681     1852 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/tests/test_lj_mix_0.py
+-rw-r--r--   0 wpk      (42033)    36681     5240 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/tests/test_lnPi.py
+-rw-r--r--   0 wpk      (42033)    36681     5843 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/tests/test_single_comp_sub.py
+-rw-r--r--   0 wpk      (42033)    36681     5081 2023-05-03 03:04:44.000000 tmmc-lnpy-0.5.0/tests/test_single_comp_super.py
+-rw-r--r--   0 wpk      (42033)    36681     2802 2023-05-12 20:08:22.000000 tmmc-lnpy-0.5.0/tests/test_water_cluster.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.470698 tmmc-lnpy-0.5.0/tests/water_cluster/
+-rw-r--r--   0 wpk      (42033)    36681      559 2022-09-14 17:15:37.000000 tmmc-lnpy-0.5.0/tests/water_cluster/data_0.csv
+-rw-r--r--   0 wpk      (42033)    36681      116 2022-09-14 17:15:37.000000 tmmc-lnpy-0.5.0/tests/water_cluster/data_0_dw.csv
+-rw-r--r--   0 wpk      (42033)    36681     3953 2022-09-14 17:15:37.000000 tmmc-lnpy-0.5.0/tests/water_cluster/data_1.csv
+-rw-r--r--   0 wpk      (42033)    36681     4784 2022-09-14 17:15:37.000000 tmmc-lnpy-0.5.0/tests/water_cluster/data_1_dw.csv
+-rw-r--r--   0 wpk      (42033)    36681      367 2023-04-14 22:51:35.000000 tmmc-lnpy-0.5.0/tests/water_cluster/water_MOF_ensemble.json
+-rw-r--r--   0 wpk      (42033)    36681    29453 2022-09-14 17:15:37.000000 tmmc-lnpy-0.5.0/tests/water_cluster/water_MOF_example.csv
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 19:19:49.471322 tmmc-lnpy-0.5.0/tools/
+-rw-r--r--   0 wpk      (42033)    36681    24175 2023-07-06 19:19:12.000000 tmmc-lnpy-0.5.0/tools/noxtools.py
```

### Comparing `tmmc-lnpy-0.4.0/.cruft.json` & `tmmc-lnpy-0.5.0/.cruft.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'checkout'": "'feature/nox'", "'commit'": "'08c4262605dd01f05a64f2edfc7e2dd65ddb0b4d'"}*

```diff
@@ -1,10 +1,10 @@
 {
-    "checkout": "feature/markdown",
-    "commit": "a0209ae199aa6f953364fc929e50d41d58082173",
+    "checkout": "feature/nox",
+    "commit": "08c4262605dd01f05a64f2edfc7e2dd65ddb0b4d",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
```

### Comparing `tmmc-lnpy-0.4.0/.editorconfig` & `tmmc-lnpy-0.5.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/.gitignore` & `tmmc-lnpy-0.5.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox/
+.nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 .hypothesis/
@@ -102,12 +103,16 @@
 .mypy_cache/
 
 # IDE settings
 .vscode/
 pyrightconfig.json
 .autoenv.zsh
 .autoenv_leave.zsh
+.noxconfig.toml
+cruft.patch
 /docs/**/generated/
 /monkeytype.sqlite3
-/dist-conda/*
-!/dist-conda/Makefile
+/dist-conda/
+/tmp/
 /tmmc-lnpy-feedstock*/
+/src/**/_version.py
+tuna-loadtime.log
```

### Comparing `tmmc-lnpy-0.4.0/.pre-commit-config.yaml` & `tmmc-lnpy-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/.recipe-append.yaml` & `tmmc-lnpy-0.5.0/.recipe-append.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/CHANGELOG.md` & `tmmc-lnpy-0.5.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,30 @@
 
 ## Unreleased
 
 See the fragment files in [changelog.d](https://github.com/usnistgov/tmmc-lnpy)
 
 <!-- scriv-insert-here -->
 
+## v0.5.0 — 2023-07-06
+
+### Added
+
+- Now use [lazy_loader](https://github.com/scientific-python/lazy_loader) to
+  speed up initial load time.
+
+Full set of changes:
+[`v0.4.0...0.5.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.4.0...v0.5.0)
+
 ## v0.4.0 — 2023-05-12
 
 ### Added
 
-- Package now available on conda-forge
+- Package now available on conda-forge Full set of changes:
+  [`v0.3.0...0.4.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.3.0...v0.4.0)
 
 ### Changed
 
 - Changed `examples.load_example_maskddata` to
   `examples.load_example_lnpimasked` for consistency with other method names.
 
 ## v0.3.0 — 2023-05-02
@@ -29,15 +40,15 @@
 
 - Moved `_docstrings` -> `docstrings` to make available
 - Moved from local docfiller to module_utilities.docfiller
 - Moved from local cached module to module-utilities.cached
 - Add support for python3.11
 
 Full set of changes:
-[`v0.2.2...0.3.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.2.2...0.3.0)
+[`v0.2.2...0.3.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.2.2...v0.3.0)
 
 ### Changed
 
 - Update package layout
 - New linters via pre-commit
 - Development env now handled by tox
```

### Comparing `tmmc-lnpy-0.4.0/CONTRIBUTING.md` & `tmmc-lnpy-0.5.0/CONTRIBUTING.md`

 * *Files 16% similar despite different names*

```diff
@@ -39,74 +39,88 @@
 <https://github.com/usnistgov/tmmc-lnpy/issues>.
 
 If you are proposing a feature:
 
 - Explain in detail how it would work.
 - Keep the scope as narrow as possible, to make it easier to implement.
 - Remember that this is a volunteer-driven project, and that contributions are
-  welcome :)
+  welcome!
 
 ## Get Started
 
 ### Environment setup
 
 [pipx]: https://github.com/pypa/pipx
 [condax]: https://github.com/mariusvniekerk/condax
 [mamba]: https://github.com/mamba-org/mamba
 [conda-fast-setup]:
   https://www.anaconda.com/blog/a-faster-conda-for-a-growing-community
 [pre-commit]: https://pre-commit.com/
+[nox]: https://github.com/wntrblm/nox
+[noxopt]: https://github.com/rmorshea/noxopt
 [tox]: https://tox.wiki/en/latest/
-[tox-conda]: https://github.com/tox-dev/tox-conda
 [cruft]: https://github.com/cruft/cruft
-[conda-merge]: https://github.com/amitbeka/conda-merge
+[cog]: https://github.com/nedbat/cog
 [git-flow]: https://github.com/nvie/gitflow
 [scriv]: https://github.com/nedbat/scriv
 [conventional-style]: https://www.conventionalcommits.org/en/v1.0.0/
 [commitizen]: https://github.com/commitizen-tools/commitizen
 [nb_conda_kernels]: https://github.com/Anaconda-Platform/nb_conda_kernels
+[pyproject2conda]: https://github.com/wpk-nist-gov/pyproject2conda
 
 This project uses a host of tools to (hopefully) make development easier. We
 recommend installing some of these tools system wide. For this, we recommend
 using either [pipx] or [condax]. We mostly use conda/condax, but the choice is
 yours. For conda, we recommend actually using [mamba]. Alternatively, you can
 setup `conda` to use the faster `mamba` solver. See [here][conda-fast-setup] for
 details.
 
 Additional tools are:
 
 - [pre-commit]
-- [tox] and [tox-conda]
+- [nox] with [noxopt]
 - [cruft]
-- [conda-merge]
 - [scriv]
+- [commitizen] (optional)
+- [pyproject2conda] (optional)
+- [cog] (optional)
 
 These are setup using the following:
 
 ```console
-condax install pre-commit
-condax install tox
-condax inject tox tox-conda
-condax install cruft
-condax install conda-merge
-condax install commitizen
+condax/pipx install pre-commit
+condax/pipx install cruft
+condax/pipx install commitizen # optional
 pipx install scriv
+pipx install pyproject2conda # optional
+condax/pipx install cogapp # optional
 ```
 
-Alternatively, you can install these dependencies using:
+if using pipx, nox can be installed with:
 
-```console
-conda env update -n {env-name} environment/tools.yaml
+```bash
+pipx install nox
+pipx inject nox ruamel.yaml
+pipx inject nox noxopt
+```
+
+If using condax, you'll need to use:
+
+```bash
+condax install nox
+condax inject nox ruamel.yaml
+conda activate ~/.condax/nox
+pip install noxopt
 ```
 
 ### Getting the repo
 
-Ready to contribute? Here's how to set up `lnpy` for local development.
+Ready to contribute? Here's how to set up `tmmc-lnpy` for local development.
 
-- Fork the `lnpy` repo on GitHub.
+- Fork the `tmmc-lnpy` repo on GitHub.
 
 - Clone your fork locally:
 
   ```bash
   git clone git@github.com:your_name_here/tmmc-lnpy.git
   ```
 
@@ -123,56 +137,40 @@
   cd tmmc-lnpy
   git submodule update --init --recursive
   ```
 
 - Create development environment. There are two options to create the
   development environment.
 
-  - The recommended method is to use tox by using either:
-
-    ```bash
-    tox -e dev
-    ```
-
-    or
+  - The recommended method is to use nox. First you'll need to create the
+    environment files using:
 
     ```bash
-    make dev-env
+    nox -e pyproject2conda
     ```
 
-    These create a development environment located at `.tox/dev`.
+    Then run:
 
     ```bash
-    make tox-ipykernel-display-name
+    nox -e dev
     ```
 
-    This will add a meaningful display name for the kernel (assuming you're
-    using [nb_conda_kernels])
+    This create a development environment located at `.nox/dev`.
 
   - Alternativley, you can create centrally located conda environmentment using
     the command:
 
     ```bash
-    make mamba-dev
+    conda/mamba env create -n {env-name} -f environment/dev.yaml
     ```
 
-    This will create a conda environment 'lnpy-env' in the default location.
-
-    To install (an editable version) of the current package:
-
     ```bash
     pip install -e . --no-deps
     ```
 
-    or
-
-    ```bash
-    make install-dev
-    ```
-
 - Initiate [pre-commit] with:
 
   ```bash
   pre-commit install
   ```
 
   To update the recipe, periodically run:
@@ -205,24 +203,18 @@
 
   To run tests, use:
 
   ```bash
   pytest
   ```
 
-  To test against multiple python versions, use tox:
-
-  ```bash
-  tox
-  ```
-
-  or using the `make`:
+  To test against multiple python versions, use [nox]:
 
   ```bash
-  make test-all
+  nox -s test
   ```
 
   Additionally, you should run the following:
 
   ```bash
   make pre-commit-lint-markdown
   make pre-commit-codespell
@@ -250,152 +242,199 @@
   cz commit
   ```
 
 - Submit a pull request through the GitHub website.
 
 ### Dependency management
 
-Dependencies need to be placed in a few locations, which depend on the nature of
-the dependency.
-
-- Package dependency: `environment.yaml` and `dependencies` section of
-  `pyproject.toml`
-- Documentation dependency: `environment/docs-extras.yaml` and `test` section of
-  `pyproject.toml`
-- Development dependency: `environment/dev-extras.yaml` and `dev` section of
-  `pyproject.toml`
-
-Note that total yaml files are build using [conda-merge]. For example,
-`environment.yaml` is combined with `environment/docs-extras.yaml` to produce
-`environment/docs.yaml`. This is automated in the `Makefile`. You can also run,
-after doing any updates,
+We use [pyproject2conda] to handle conda `environment.yaml` files. This extracts
+the dependencies from `pyproject.toml`. See [pyproject2conda] for info. To make
+the `environment.yaml` files, run:
 
 ```bash
-make environment-files-build
+nox -s pyproject2conda -- [--pyproject2conda-force]
 ```
 
-which will rebuild all the needed yaml files.
+Where the option in brackets is optional.
 
 ## Pull Request Guidelines
 
 Before you submit a pull request, check that it meets these guidelines:
 
 - The pull request should include tests.
 - If the pull request adds functionality, the docs should be updated. Put your
   new functionality into a function with a docstring, and add the feature to the
   list in CHANGELOG.md. You should use [scriv] for this.
 - The pull request should work for Python 3.8, 3.9, 3.10.
 
-## Building the docs
+## ipykernel
 
-We use [tox] to isolate the documentation build. Useful commands are as follows.
+The environments created by nox `dev` and `docs` will try to add meaningful
+display names for ipykernel (assuming you're using [nb_conda_kernels])
 
-- Build the docs:
+## Building the docs
 
-  ```bash
-  tox -e docs -- build
-  ```
+We use [nox] to isolate the documentation build. Specific tasks can be run with
 
-- Spellcheck the docs:
+```bash
+nox -s docs -- -d [commands]
+```
 
-  ```bash
-  tox -e docs -- spelling
-  ```
+where commands can be one of:
 
-- Create a release of the docs:
+- clean : remove old doc build
+- build/html : build html documentation
+- spelling : check spelling
+- linkcheck : check the links
+- symlink : rebuild symlinks from `examples` to `docs/examples`
+- release : make pages branch for documentation hosting (using
+  [ghp-import](https://github.com/c-w/ghp-import))
+- livehtml : Live documentation updates
+- open : open the documentation in a web browser
 
-  ```bash
-  tox -e docs -- release
-  ```
+## Testing with nox
 
-  If you make any changes to `docs/examples`, you should run:
+The basic command is:
 
-  ```bash
-  make docs-examples-symlink
-  ```
+```bash
+nox -s test -- [--test-opts] [--no-cov]
+```
 
-  to update symlinks from `docs/examples` to `examples`.
+where you can pass in additional pytest options (properly escaped) via
+`--test-opts`. For example:
 
-  After this, the docs can be pushed to the correct branch for distribution.
+```bash
+nox -s test -- --test-opts "'-v'"
+# or
+nox -s test -- --test-opts "\-v"
+```
 
-- Live documentation updates using
+## Building distribution for conda
 
-  ```bash
-  make docs-livehtml
-  ```
+[grayskull]: https://github.com/conda/grayskull
 
-## Using tox
+For the most part, we use [grayskull] to create the conda recipe. However, I've
+had issues getting it to play nice with `pyproject.toml` for some of the 'extra'
+variables. So, we use grayskull to build the majority of the recipe, and append
+the file `.recipe-append.yaml`. For some edge cases (install name different from
+package name, etc), you'll need to manually edit this file to create the final
+recipe.
 
-The package is setup to use tox to test, build and release pip and conda
-distributions, and release the docs. Most of these tasks have a command in the
-`Makefile`. To test against multiple versions, use:
+The basic command is:
 
 ```bash
-make test-all
+nox -s dist-conda -- -c [command]
 ```
 
-To build the documentation in an isolated environment, use:
+Where `command` is one of:
+
+- clean
+- recipe : create recipe via [grayskull]
+- build : build the distribution
+
+To upload the recipe, you'll need to run an external command like:
 
 ```bash
-make docs-build
+nox -s dist-conda -- --dist-conda-run "anaconda upload PATH-TO-TARBALL"
 ```
 
-To release the documentation use:
+## Building distribution for pypi
+
+The basic command is:
 
 ```bash
-make docs-release release_args='-m "commit message" -r origin -p'
+nox -s dist-pypi -- -p [command]
 ```
 
-Where posargs is are passed to ghp-import. Note that the branch created is
-called `nist-pages`. This can be changed in `tox.ini`.
+where `command` is one of:
+
+- clean : clean out old distribution
+- build : build distribution (if specify only this, clean will be called first)
+- testrelease : upload to testpypi
+- release : upload to pypi
 
-To build the distribution, use:
+## Testing pypi or conda installs
+
+Run:
 
 ```bash
-make dist-pypi-[build-testrelease-release]
+nox -s testdist-pypi -- --version [version]
 ```
 
-where `build` build to distro, `testrelease` tests putting on `testpypi` and
-release puts the distro on pypi.
+to test a specific version from pypi and
+
+```bash
+nox -s testdist-conda -- --version [version]
+```
+
+to to likewise from conda.
+
+## Type checking
 
-To build the conda distribution, use:
+Run:
 
 ```bash
-make dist-conda-[recipe, build]
+nox -s typing -- -m [commands] [options]
 ```
 
-where `recipe` makes the conda recipe (using grayskull), and `build` makes the
-distro. This can be manually added to a channel.
+## Package version
+
+[setuptools_scm]: https://github.com/pypa/setuptools_scm
 
-To test the created distributions, you can use one of:
+Versioning is handled with [setuptools_scm].The package version is set by the
+git tag. For convenience, you can override the version with nox setting
+`--version ...`. This is useful for updating the docs, etc.
+
+We use the `write_to` option to [setuptools_scm]. This stores the current
+version in `_version.py`. Note that if you build the package (or, build docs
+with the `--version` flag), this will overwrite information in `_version.py` in
+the `src` directory. To refresh the version, run:
 
 ```bash
-tox -e test-dist-[pypi, conda]-[local,remote]-py[38,39,...]
+make version-scm
 ```
 
-or
+This scheme avoids having to install `setuptools-scm` (and `setuptools`) in each
+environment.
+
+## Notes on [nox]
+
+One downside of using [tox] with this particular workflow is the need for
+multiple scripts/makefiles, while with [nox], most everything is self contained
+in the file `noxfile.py`. [nox] also is allows for a mix of conda and virtualenv
+environments.
+
+We use a mix of conda environments and virtualenv with nox. For example, for
+building the distribution, we use virtualenv, while for development, the default
+is to create a conda environment. To facilitate this, we need to let virtualenv
+know where different python interpreters are. I've had trouble mixing pyenv with
+conda. Instead, I use conda to create multiple invironments to hold different
+python version:
 
 ```bash
-make test-dist-[pypi, conda]-[local,remote] py=[38, 39, 310]
+$ for version in 3.8 3.9 3.10 3.11; do
+    conda create -n test-3.8 python=3.8
+  done
 ```
 
-where one options in the brackets should be choosen.
+To tell nox where these environments live, create the file `.noxconfig.toml`
+with the following:
 
-## Package version
+```toml
+[nox.python]
+paths = ["~/.conda/envs/test-3.*/bin"]
 
-[setuptools_scm]: https://github.com/pypa/setuptools_scm
+```
 
-Versioning is handled with [setuptools_scm].The pacakge version is set by the
-git tag. For convenience, you can override the version in the makefile (calling
-tox) by setting `version=v{major}.{minor}.{micro}`. This is useful for updating
-the docs, etc.
+where `~/.conda/envs` should be replaced by whatever prefix you have setup on
+your machine. The noxfile will add this to the search path for python versions
+when creating virtualenvs.
 
-## Creating conda recipe
+## Serving the documentation
 
-[grayskull]: https://github.com/conda/grayskull
+To view to documentation with js headers/footers, you'll need to serve them:
 
-For the most part, we use [grayskull] to create the conda recipe. However, I've
-had issues getting it to play nice with `pyproject.toml` for some of the 'extra'
-variables. So, we use grayskull to build the majority of the recipe, and append
-the file `.recipe-append.yaml`. For some edge cases (install name different from
-package name, etc), you'll need to manually edit this file to create the final
-recipe.
+```bash
+python -m http.server -d docs/_build/html
+```
+
+Then open the address `localhost:8000` in a webbrowser.
```

### Comparing `tmmc-lnpy-0.4.0/LICENSE` & `tmmc-lnpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/Makefile` & `tmmc-lnpy-0.5.0/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 clean-pyc: ## remove Python file artifacts
 	find . -name '*.pyc' -exec rm -f {} +
 	find . -name '*.pyo' -exec rm -f {} +
 	find . -name '*~' -exec rm -f {} +
 	find . -name '__pycache__' -exec rm -fr {} +
 
 clean-test: ## remove test and coverage artifacts
-	rm -fr .tox/
+	rm -fr .nox/
 	rm -f .coverage
 	rm -fr htmlcov/
 	rm -fr .pytest_cache
 
 
 
 
@@ -99,15 +99,15 @@
 
 
 ################################################################################
 # my convenience functions
 ################################################################################
 .PHONY: user-venv user-autoenv-zsh user-all
 user-venv: ## create .venv file with name of conda env
-	echo $${PWD}/.tox/dev > .venv
+	echo $${PWD}/.nox/dev > .venv
 
 user-autoenv-zsh: ## create .autoenv.zsh files
 	echo conda activate $$(cat .venv) > .autoenv.zsh
 	echo conda deactivate > .autoenv_leave.zsh
 
 user-all: user-venv user-autoenv-zsh ## runs user scripts
 
@@ -129,178 +129,129 @@
 	$(BROWSER) htmlcov/index.html
 
 
 ################################################################################
 # versioning
 ################################################################################
 .PHONY: version-scm version-import version
-version-scm: ## check version of package
+
+version-scm: ## check/update version of package with setuptools-scm
 	python -m setuptools_scm
 
 version-import: ## check version from python import
-	python -c 'import lnpy; print(lnpy.__version__)'
+	-python -c 'import lnpy; print(lnpy.__version__)'
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
-ENVIRONMENTS = $(addsuffix .yaml,$(addprefix environment/, dev docs test))
-PRETTIER = bash scripts/run-prettier.sh
-
-environment/%.yaml: environment.yaml environment/%-extras.yaml ## create combined environment/{dev,docs,test}.yaml
-	conda-merge $^ > $@
-	$(PRETTIER) $@
-
-environment/dev.yaml: ## development environment yaml file
-environment/test.yaml: ## testing environment yaml file
-enviornment/docs.yaml: ## docs environment yaml file
-
-
-# special for linters
-environment/lint.yaml: environment.yaml $(addsuffix .yaml, $(addprefix environment/, test-extras lint-extras)) ## mypy environment
-	echo $^
-	conda-merge $^ > $@
-	$(PRETTIER) $@
-
-ENVIRONMENTS += environment/lint.yaml
-
 .PHONY: environment-files-clean
 environment-files-clean: ## clean all created environment/{dev,docs,test}.yaml
 	-rm $(ENVIRONMENTS) 2> /dev/null || true
 
 .PHONY: environment-files-build
-environment-files-build: $(ENVIRONMENTS) ## rebuild all environment files
+environment-files-build: pyproject.toml ## rebuild all environment files
+	nox -s pyproject2conda
+
+environment/%.yaml: pyproject.toml
+	nox -s pyproject2conda
 
 ################################################################################
 # virtual env
 ################################################################################
-.PHONY: mamba-env mamba-dev mamba-env-update mamba-dev-update
-
-mamba-env: environment.yaml ## create base environment
-	mamba env create -f $<
+.PHONY: mamba-env-update mamba-dev-update
 
-mamba-env-update: environment.yaml ## update base environment
-	mamba env update -f $<
-
-mamba-dev: environment/dev.yaml ## create development environment
+mamba-dev: environment/dev.yaml environment-files-build ## create development environment
 	mamba env create -f $<
 
-mamba-dev-update: environment/dev.yaml ## update development environment
+mamba-dev-update: environment/dev.yaml environment-files-build ## update development environment
 	mamba env update -f $<
 
 ################################################################################
-# TOX
+# NOX
 ###############################################################################
-tox_args?=-v
-version?=
-TOX=CONDA_EXE=mamba SETUPTOOLS_SCM_PRETEND_VERSION=$(version) tox $(tox_args)
-
-.PHONY: tox-ipykernel-display-name
-tox-ipykernel-display-name: ## Update display-name for any tox env with ipykernel
-	bash ./scripts/tox-ipykernel-display-name.sh lnpy
-
 ## dev env
+NOX=nox
 .PHONY: dev-env
-dev-env: environment/dev.yaml ## create development environment using tox
-	tox -e dev
+dev-env: environment/dev.yaml ## create development environment using nox
+	$(NOX) -e dev
 
 ## testing
 .PHONY: test-all
-test-all: environment/test.yaml ## run tests on every Python version with tox.  can pass posargs=...
-	$(TOX) -- $(posargs)
+test-all: environment/test.yaml ## run tests on every Python version with nox.
+	$(NOX) -s test
 
 ## docs
-.PHONY: docs-examples-symlink
-docs-examples-symlink: ## create symlinks to notebooks from /examples/ to /docs/examples.
-	bash ./scripts/docs-examples-symlinks.sh
-
-
 .PHONY: docs-build docs-release docs-clean docs-command
 docs-build: ## build docs in isolation
-	$(TOX) -e docs -- build
+	$(NOX) -s docs -- -d build
 docs-clean: ## clean docs
 	rm -rf docs/_build/*
 	rm -rf docs/generated/*
 	rm -rf docs/reference/generated/*
 docs-clean-build: docs-clean docs-build ## clean and build
-docs-release: ## release docs.  use release_args=... to override stuff
-	$(TOX) -e docs -- release
-docs-command: ## run command with command=...
-	$(TOX) -e docs -- command
+docs-release: ## release docs.
+	$(NOX) -s docs -- -d release
+docs-command: ## run arbitrary command with command=...
+	$(NOX) -s docs -- --docs-run $(command)
 
 .PHONY: .docs-spelling docs-nist-pages docs-open docs-livehtml docs-clean-build docs-linkcheck
 docs-spelling: ## run spell check with sphinx
-	$(TOX) -e docs -- spelling
+	$(NOX) -s docs -- -d spelling
 docs-livehtml: ## use autobuild for docs
-	$(TOX) -e docs -- livehtml
+	$(NOX) -s docs -- -d livehtml
 docs-open: ## open the build
-	$(BROWSER) docs/_build/html/index.html
+	$(NOX) -s docs -- -d open
 docs-linkcheck: ## check links
-	$(TOX) -e docs -- linkcheck
+	$(NOX) -s docs -- -d linkcheck
 
 docs-build docs-release docs-command docs-clean docs-livehtml docs-linkcheck: environment/docs.yaml
 
-## linting
-.PHONY: lint-mypy lint-pyright lint-pytype lint-all lint-command
-lint-mypy: ## run mypy mypy_args=...
-	$(TOX) -e lint -- mypy
-lint-pyright: ## run pyright pyright_args=...
-	$(TOX) -e lint -- pyright
-lint-pytype: ## run pytype pytype_args=...
-	$(TOX) -e lint -- pytype
-lint-all:
-	$(TOX) -e lint -- all
-lint-command:
-	$(TOX) -e lint -- command
-
-lint-mypy lint-pyright lint-pytype lint-all lint-command: environment/lint.yaml
+## typing
+.PHONY: typing-mypy typing-pyright typing-pytype typing-all typing-command
+typing-mypy: ## run mypy mypy_args=...
+	$(NOX) -s typing -- -m mypy
+typing-pyright: ## run pyright pyright_args=...
+	$(NOX) -s typing -- -m pyright
+typing-pytype: ## run pytype pytype_args=...
+	$(NOX) -s typing -- -m pytype
+typing-all:
+	$(NOX) -s typing -- -m mypy pyright pytype
+typing-command:
+	$(NOX) -s typing -- --typing-run $(command)
+typing-mypy typing-pyright typing-pytype typing-all typing-command: environment/typing.yaml
 
 ## distribution
 .PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command
 
 dist-pypi-build: ## build dist
-	$(TOX) -e dist-pypi -- build
+	$(NOX) -s dist-pypi -- -p build
 dist-pypi-testrelease: ## test release on testpypi
-	$(TOX) -e dist-pypi -- testrelease
+	$(NOX) -s dist-pypi -- -p testrelease
 dist-pypi-release: ## release to pypi, can pass posargs=...
-	$(TOX) -e dist-pypi -- release
+	$(NOX) -s dist-pypi -- -p release
 dist-pypi-command: ## run command with command=...
-	$(TOX) -e dist-pypi -- command
+	$(NOX) -s dist-pypi -- --dist-pypi-run $(command)
 dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command: environment/dist-pypi.yaml
 
 .PHONY: dist-conda-recipe dist-conda-build dist-conda-command
 dist-conda-recipe: ## build conda recipe can pass posargs=...
-	$(TOX) -e dist-conda -- recipe
+	$(NOX) -s dist-conda -- -c recipe
 dist-conda-build: ## build conda recipe can pass posargs=...
-	$(TOX) -e dist-conda -- build
+	$(NOX) -s dist-conda -- -c build
 dist-conda-command: ## run command with command=...
-	$(TOX) -e dist-conda -- command
+	$(NOX) -s dist-conda -- -dist-conda-run $(command)
 dist-conda-build dist-conda-recipe dist-conda-command: environment/dist-conda.yaml
 
 
-## test distribution
-.PHONY: testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local
-
-py?=310
-testdist-pypi-remote: ## testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39.  Can specify version setting, eg,  TEST_VERSION='==0.1.0'.  Note that the the format should be '=={version}'.
-	$(TOX) -e $@-py$(py) -- $(posargs)
-testdist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
-	$(TOX) -e $@-py$(py) -- $(poasargs)
-testdist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
-	$(TOX) -e $@-py$(py) -- $(posargs)
-testdist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
-	$(TOX) -e $@-py$(py) -- $(poasargs)
-
-testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local: environment/test.yaml
-
 ## list all options
-.PHONY: tox-list
-tox-list:
-	$(TOX) -a
+.PHONY: nox-list
+nox-list:
+	$(NOX) --list
 
 
 ################################################################################
 # installation
 ################################################################################
 .PHONY: install install-dev
 install: ## install the package to the active Python's site-packages (run clean?)
@@ -316,7 +267,14 @@
 
 # Note that this requires `auto-changelog`, which can be installed with pip(x)
 auto-changelog: ## autogenerate changelog and print to stdout
 	auto-changelog -u -r usnistgov -v unreleased --tag-prefix v --stdout --template changelog.d/templates/auto-changelog/template.jinja2
 
 commitizen-changelog:
 	cz changelog --unreleased-version unreleased --dry-run --incremental
+
+# tuna analyze load time:
+.PHONY: tuna-analyze
+tuna-import: ## Analyze load time for module
+	python -X importtime -c 'import lnpy' 2> tuna-loadtime.log
+	tuna tuna-loadtime.log
+	rm tuna-loadtime.log
```

### Comparing `tmmc-lnpy-0.4.0/PKG-INFO` & `tmmc-lnpy-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmmc-lnpy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Analysis of lnPi results from TMMC simulation
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/tmmc-lnpy
 Project-URL: documentation, https://pages.nist.gov/tmmc-lnpy/
 Keywords: tmmc-lnpy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,14 +17,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: viz
+Provides-Extra: dev-extras
+Provides-Extra: typing-extras
+Provides-Extra: typing
+Provides-Extra: nox
+Provides-Extra: dev
+Provides-Extra: tools
+Provides-Extra: dev-complete
+Provides-Extra: docs
+Provides-Extra: dist-pypi
+Provides-Extra: dist-conda
 License-File: LICENSE
 
 <!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
@@ -186,19 +197,30 @@
 
 ## Unreleased
 
 See the fragment files in [changelog.d](https://github.com/usnistgov/tmmc-lnpy)
 
 <!-- scriv-insert-here -->
 
+## v0.5.0 — 2023-07-06
+
+### Added
+
+- Now use [lazy_loader](https://github.com/scientific-python/lazy_loader) to
+  speed up initial load time.
+
+Full set of changes:
+[`v0.4.0...0.5.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.4.0...v0.5.0)
+
 ## v0.4.0 — 2023-05-12
 
 ### Added
 
-- Package now available on conda-forge
+- Package now available on conda-forge Full set of changes:
+  [`v0.3.0...0.4.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.3.0...v0.4.0)
 
 ### Changed
 
 - Changed `examples.load_example_maskddata` to
   `examples.load_example_lnpimasked` for consistency with other method names.
 
 ## v0.3.0 — 2023-05-02
@@ -209,15 +231,15 @@
 
 - Moved `_docstrings` -> `docstrings` to make available
 - Moved from local docfiller to module_utilities.docfiller
 - Moved from local cached module to module-utilities.cached
 - Add support for python3.11
 
 Full set of changes:
-[`v0.2.2...0.3.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.2.2...0.3.0)
+[`v0.2.2...0.3.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.2.2...v0.3.0)
 
 ### Changed
 
 - Update package layout
 - New linters via pre-commit
 - Development env now handled by tox
```

### Comparing `tmmc-lnpy-0.4.0/README.md` & `tmmc-lnpy-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/changelog.d/templates/auto-changelog/template.jinja2` & `tmmc-lnpy-0.5.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/environment/dev-extras.yaml` & `tmmc-lnpy-0.5.0/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/environment/docs-extras.yaml` & `tmmc-lnpy-0.5.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/pyproject.toml` & `tmmc-lnpy-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -31,54 +31,122 @@
     "scipy",
     "scikit-image",
     "joblib",
     "bottleneck",
     "tqdm",
     "importlib_resources",
     "module-utilities >= 0.1",
+    "lazy_loader",
 ] # additional packages
 
 [project.urls]
 homepage = "https://github.com/usnistgov/tmmc-lnpy"
 documentation = "https://pages.nist.gov/tmmc-lnpy/"
 
 [project.optional-dependencies]
-test = ["pytest"]
+test = [
+    "pytest", #
+    "pytest-xdist",
+    "pytest-cov",
+    "pytest-sugar",
+]
+viz = [
+    "matplotlib", #
+    "ipywidgets",
+]
+dev-extras = [
+    "setuptools-scm", #
+    "pytest-accept", # p2c: -p
+    "ipython",
+    "ipykernel",
+    "tmmc-lnpy[viz]",
+]
+typing-extras = [
+    # "pytype; python_version < '3.11'",
+    "mypy",
+]
+typing = [
+    "tmmc-lnpy[typing-extras]", #
+    "tmmc-lnpy[test]",
+]
+nox = [
+    "nox",
+    "noxopt", # p2c: -p
+    "ruamel.yaml",
+]
+dev = [
+    "tmmc-lnpy[test]", #
+    "tmmc-lnpy[typing-extras]",
+    "tmmc-lnpy[dev-extras]",
+]
+tools = [
+    "pre-commit", #
+    "cruft",
+    "scriv",
+]
+dev-complete = [
+    "tmmc-lnpy[dev]", #
+    "tmmc-lnpy[tools]",
+    "tmmc-lnpy[nox]",
+]
+docs = [
+    "ipython", #
+    "pyenchant",
+    "ghp-import",
+    "sphinx",
+    "sphinx-copybutton",
+    "sphinxcontrib-spelling",
+    "sphinx-autobuild",
+    "myst-nb",
+    "sphinx-book-theme",
+    "autodocsumm",
+    "tmmc-lnpy[viz]",
+]
+# to be parsed with pyproject2conda with --no-base option
+dist-pypi = ["twine", "build"]
+dist-conda = [
+    "anaconda-client", #
+    "grayskull",
+    "conda-build",
+    "conda-verify",
+    "boa",
+]
+
+[tool.pyproject2conda]
+channels = ["conda-forge"]
 
-# dev = []
-# docs = []
 ## grayskull still messes some things up, but use scripts/recipe-append.sh for this
 [tool.setuptools]
 zip-safe = true # if using mypy, must be False
 include-package-data = true
 license-files = ["LICENSE"]
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 ## include = []
 ## exclude = []
-##
 [tool.setuptools.dynamic]
 readme = { file = [
     "README.md",
     "CHANGELOG.md",
     "LICENSE"
 ], content-type = "text/markdown" }
 
 [tool.setuptools_scm]
 fallback_version = "999"
+write_to = "src/lnpy/_version.py"
 
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
-addopts = "--verbose --doctest-modules --doctest-glob='*.md'"
-testpaths = ["README.md", "tests"]
+addopts = "--doctest-modules --doctest-glob='*.md'"
+testpaths = ["tests", "README.md"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = ["lnpy"]
 
 [tool.ruff]
@@ -232,28 +300,28 @@
 
 [tool.mypy]
 files = ["src/lnpy"]
 show_error_codes = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unused_configs = true
-exclude = [".eggs", ".tox", "doc", "docs"]
+exclude = [".eggs", ".tox", "doc", "docs", ".nox"]
 check_untyped_defs = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = []
 
 [[tool.mypy.overrides]]
 ignore_errors = true
 module = []
 
 [tool.pyright]
 include = ["src", "tests"]
-exclude = ["**/__pycache__", ".tox/**", "**/.mypy_cache"]
+exclude = ["**/__pycache__", ".tox/**", ".nox/**", "**/.mypy_cache"]
 pythonVersion = "3.10"
 typeCheckingMode = "basic"
 # enable subset of "strict"
 reportDuplicateImport = true
 reportInvalidStubStatement = true
 reportOverlappingOverload = true
 reportPropertyTypeMismatch = true
```

### Comparing `tmmc-lnpy-0.4.0/src/lnPi/__init__.py` & `tmmc-lnpy-0.5.0/src/lnPi/__init__.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/bracket.py` & `tmmc-lnpy-0.5.0/src/lnpy/bracket.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/data/hsmix_example.json.gz` & `tmmc-lnpy-0.5.0/src/lnpy/data/hsmix_example.json.gz`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/data/lj_sub_example.json` & `tmmc-lnpy-0.5.0/src/lnpy/data/lj_sub_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/data/lj_sup_example.json` & `tmmc-lnpy-0.5.0/src/lnpy/data/lj_sup_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/data/ljmix_sup_example.json.gz` & `tmmc-lnpy-0.5.0/src/lnpy/data/ljmix_sup_example.json.gz`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/data/watermof_example.json` & `tmmc-lnpy-0.5.0/src/lnpy/data/watermof_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/docstrings.py` & `tmmc-lnpy-0.5.0/src/lnpy/docstrings.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/ensembles.py` & `tmmc-lnpy-0.5.0/src/lnpy/ensembles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 """
 Ensemble averages (:mod:`~lnpy.ensembles`)
 ==========================================
 """
 from functools import lru_cache, partial, wraps
 
-import numpy as np
-import xarray as xr
 from module_utilities import cached
 
-from .lnpidata import MaskedlnPiDelayed, lnPiMasked
-from .lnpiseries import lnPiCollection
-from .maskedlnpi_legacy import MaskedlnPiLegacy
+from ._lazy_imports import np, xr
 from .utils import dim_to_suffix_dataset
 
 # always check_use_cache here.
 cached_prop = partial(cached.prop, check_use_cache=True)
 cached_meth = partial(cached.meth, check_use_cache=True)
 
 
@@ -173,18 +169,14 @@
             return out
 
         return wrapper
 
     return decorator
 
 
-@lnPiMasked.decorate_accessor("xge")
-@MaskedlnPiDelayed.decorate_accessor("xge")
-@MaskedlnPiLegacy.decorate_accessor("xge")
-@lnPiCollection.decorate_accessor("xge")
 def xge_accessor(parent):
     """Accessor to :class:`~lnpy.ensembles.xGrandCanonical`."""
     return xGrandCanonical(parent)
 
 
 class xGrandCanonical:
     """
@@ -872,17 +864,14 @@
     def S_n(self, lnpi_zero=None, ndim=3):
         r"""Scaled entropy per particle :math:`S / (N k_{\rm B})`."""
 
         return self.S(lnpi_zero, ndim) / self.ntot
 
 
 # NOTE: Using function accessor to override the docstring
-@lnPiMasked.decorate_accessor("xce")
-@MaskedlnPiDelayed.decorate_accessor("xce")
-@MaskedlnPiLegacy.decorate_accessor("xce")
 def xce_accessor(parent):
     """Accessor to :class:`~lnpy.ensembles.xCanonical`"""
     return xCanonical(parent)
 
 
 class xCanonical:
     """
```

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/examples.py` & `tmmc-lnpy-0.5.0/src/lnpy/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 except ImportError:
     import importlib.resources as resources
 
 import json
 from collections.abc import Callable
 from dataclasses import asdict, dataclass
 
-import numpy as np
-import xarray as xr
+from ._lazy_imports import np, xr
 
 # from .lnpiseries import lnPiCollection
 from .lnpidata import lnPiMasked
 from .segment import PhaseCreator
 from .utils import dataset_to_lnpimasked
```

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/extensions.py` & `tmmc-lnpy-0.5.0/src/lnpy/extensions.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/lnpicollectionutils.py` & `tmmc-lnpy-0.5.0/src/lnpy/lnpicollectionutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Set of helper utilities to work with single component system"""
 
 # from functools import partial
 
-import numpy as np
-from scipy.optimize import brentq
-
+from ._lazy_imports import np
 from .lnpiseries import lnPiCollection
 
 
 def tag_phases_singlecomp(x):
     """
     Function to tag phases with a unique id.
 
@@ -85,14 +83,15 @@
         if True, return solve parameters
 
     Returns
     -------
     phases : Phases object as solution lnz
     solution_parameters : optional
     """
+    from scipy.optimize import brentq
 
     if phase_id is not None and phase_id not in C.index.get_level_values("phase"):
         raise ValueError(f"no phase {phase_id}")
 
     lnz_idx = build_phases.index
     if isinstance(component, str) and component.lower() == "none":
```

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/lnpidata.py` & `tmmc-lnpy-0.5.0/src/lnpy/lnpidata.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 lnPi data classes and routines (:mod:`~lnpy.lnpidata`)
 ======================================================
 """
 ################################################################################
 # Delayed
 from functools import lru_cache
 
-import numpy as np
-import pandas as pd
 from module_utilities import cached
 
+from lnpy.ensembles import xce_accessor, xge_accessor
+
+from ._lazy_imports import np, pd
 from .docstrings import docfiller_shared
 from .extensions import AccessorMixin
 from .utils import labels_to_masks, masks_change_convention
 
-# from scipy.ndimage import filters
-
 
 @lru_cache(maxsize=20)
 def _get_n_ranges(shape, dtype):
     return [np.arange(s, dtype=dtype) for s in shape]
 
 
 @lru_cache(maxsize=20)
@@ -62,15 +61,15 @@
     @docfiller_shared
     def __init__(
         self,
         lnz,
         data,
         state_kws=None,
         extra_kws=None,
-        fill_value=np.nan,
+        fill_value=None,
         copy=False,
     ):
         """
         Parameters
         ----------
         {lnz}
         {data}
@@ -80,14 +79,16 @@
         {copy}
         """
 
         lnz = np.atleast_1d(lnz)
         data = np.array(data, copy=copy)
         assert data.ndim == len(lnz)
 
+        fill_value = fill_value or np.nan
+
         if state_kws is None:
             state_kws = {}
         if extra_kws is None:
             extra_kws = {}
 
         self._data = data
         # make data read only
@@ -254,15 +255,15 @@
         cls,
         lnz,
         lnz_data,
         data,
         mask=None,
         state_kws=None,
         extra_kws=None,
-        fill_value=np.nan,
+        fill_value=None,
         copy=False,
     ):
         """
         Create :class:`lnPiMasked` object from raw data.
 
         Parameters
         ----------
@@ -278,14 +279,16 @@
         {copy}
 
         Returns
         -------
         out : lnPiMasked
         """
 
+        fill_value = fill_value or np.nan
+
         base = cls._DataClass(
             lnz=lnz_data,
             data=data,
             state_kws=state_kws,
             extra_kws=extra_kws,
             fill_value=fill_value,
             copy=copy,
@@ -719,16 +722,10 @@
             convention=False,
             check_features=check_features,
             **kwargs,
         )
         return self.list_from_masks(masks, convention=False)
 
 
-from warnings import warn
-
-
-class MaskedlnPiDelayed(lnPiMasked):
-    """Deprecated alias for lnPiMasked"""
-
-    def __init__(self, *args, **kwargs):
-        warn("MaskedlnPiDelayed is deprecated.  Please use lnPiMasked instead")
-        super().__init__(*args, **kwargs)
+# --- Register accessors ---------------------------------------------------------------
+lnPiMasked.register_accessor("xge", xge_accessor)
+lnPiMasked.register_accessor("xce", xce_accessor)
```

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/lnpienergy.py` & `tmmc-lnpy-0.5.0/src/lnpy/lnpienergy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 Local free energy of lnPi (:mod:`~lnpy.lnpienergy`)
 ===================================================
 """
 import itertools
 import warnings
 
-import numpy as np
-import pandas as pd
-import xarray as xr
 from module_utilities import cached
-from skimage import segmentation
 
+from ._lazy_imports import np, pd, xr
 from .docstrings import docfiller_shared
-from .lnpiseries import lnPiCollection
 from .utils import get_tqdm_calc as get_tqdm
-from .utils import labels_to_masks, masks_change_convention, parallel_map_func_starargs
+from .utils import (
+    labels_to_masks,
+    masks_change_convention,
+    parallel_map_func_starargs,
+)
 
 
 def find_boundaries(masks, mode="thick", connectivity=None, **kws):
     """
     Find boundary region for masks
 
     Parameters
@@ -38,14 +38,16 @@
         boundaries using `segmentation.find_boundaries`
 
     See Also
     --------
     skimage.segmentation.find_boundaries
 
     """
+    from skimage import segmentation
+
     if connectivity is None:
         connectivity = np.asarray(masks[0]).ndim
 
     return [
         segmentation.find_boundaries(m, connectivity=connectivity, mode=mode, **kws)
         for m in masks
     ]
@@ -115,15 +117,15 @@
 
 @docfiller_shared
 def find_masked_extrema(
     data,
     masks,
     convention="image",
     extrema="max",
-    fill_val=np.nan,
+    fill_val=None,
     fill_arg=None,
     unravel=True,
 ):
     """
     Find position and value of extrema of masked data.
 
     Parameters
@@ -147,14 +149,16 @@
     -------
     out_arg : list of int
         index of extrema, one for each `mask`
     out_val : ndarray
         value of extrema, one for each `mask`
     """
 
+    fill_val = fill_val or np.nan
+
     if extrema == "max":
         func = np.argmax
     elif extrema == "min":
         func = np.argmin
     else:
         raise ValueError('extrema must be on of {"min", "max}')
 
@@ -735,42 +739,42 @@
             nebrs = [x for x in idx_nebr if x in index]
 
         if len(nebrs) == 0:
             return np.inf
         return dw.sel(phase=idx, phase_nebr=nebrs).min("phase_nebr").values
 
 
-@lnPiCollection.decorate_accessor("wfe")
+# @lnPiCollection.decorate_accessor("wfe")
 def wfe_accessor(parent):
     """Accessor to :class:`~lnpy.lnpienergy.wFreeEnergyCollection` from `self.wfe`."""
     return wFreeEnergyCollection(parent)
 
 
-@lnPiCollection.decorate_accessor("wfe_phases")
+# @lnPiCollection.decorate_accessor("wfe_phases")
 def wfe_phases_accessor(parent):
     """Accessor to :class:`~lnpy.lnpienergy.wFreeEnergyPhases` from `self.wfe_phases`."""
     return wFreeEnergyPhases(parent)
 
 
 from warnings import warn
 
 
 # create alias accessors
-@lnPiCollection.decorate_accessor("wlnPi")
+# @lnPiCollection.decorate_accessor("wlnPi")
 def wlnPi_accessor(parent):
     """
     Deprecated accessor to :class:`~lnpy.lnpienergy.wFreeEnergyCollection` from `self.wlnPi`.
 
     Alias to `self.wfe`
     """
     warn("Using `wlnPi` accessor is deprecated.  Please use `wfe` accessor instead")
     return parent.wfe
 
 
-@lnPiCollection.decorate_accessor("wlnPi_single")
+# @lnPiCollection.decorate_accessor("wlnPi_single")
 def wlnPi_single_accessor(parent):
     """
     Deprecated accessor to :class:`~lnpy.lnpienergy.wFreeEnergyPhases` from `self.wlnPi_single`.
 
     Alias to `self.wfe_single`
     """
     warn("Using `wlnPi_single is deprecated.  Please use `self.wfe_phases` instead")
```

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/lnpiseries.py` & `tmmc-lnpy-0.5.0/src/lnpy/lnpiseries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 """
 Collection of lnPi objects (:mod:`~lnpy.lnpiseries`)
 ====================================================
 """
 
-import numpy as np
-import pandas as pd
-import xarray as xr
 from module_utilities import cached
 
+from lnpy.ensembles import xge_accessor
+from lnpy.lnpienergy import (
+    wfe_accessor,
+    wfe_phases_accessor,
+    wlnPi_accessor,
+    wlnPi_single_accessor,
+)
+
+from ._lazy_imports import np, pd, xr
 from .extensions import AccessorMixin
 from .utils import get_tqdm_build as get_tqdm
+
+# lazy loads
 from .utils import labels_to_masks, masks_to_labels
 from .utils import parallel_map_build as parallel_map
 
 
 class SeriesWrapper(AccessorMixin):
     """wrap object in series"""
 
@@ -688,16 +696,27 @@
         for data, idx in L:
             items += data
             index += list(idx)
         return cls.from_list(items, index, base_class=base_class, *args, **kwargs)
 
     ################################################################################
     # dataarray io
-    def to_dataarray(self, dtype=np.uint8, reset_index=True, **kwargs):
-        """Convert collection to a :class:`~xarray.DataArray`"""
+    def to_dataarray(self, dtype=None, reset_index=True, **kwargs):
+        """
+        Convert collection to a :class:`~xarray.DataArray`
+
+        Parameters
+        ----------
+        dtype : data-type, optional
+            Default to :class:`numpy.uint8`.
+        reset_index : bool, default=True
+        """
+
+        dtype = dtype or np.uint8
+
         labels = []
         indexes = []
 
         for meta, g in self.groupby_allbut("phase"):
             indexes.append(g.index[[0]])
 
             features = np.array(g.index.get_level_values("phase")) + 1
@@ -835,14 +854,21 @@
             check_features=check_features,
             **kwargs,
         )  # yapf: disable
 
 
 ################################################################################
 # Accessors for ColleectionlnPi
+lnPiCollection.register_accessor("xge", xge_accessor)
+lnPiCollection.register_accessor("wfe", wfe_accessor)
+lnPiCollection.register_accessor("wfe_phases", wfe_phases_accessor)
+lnPiCollection.register_accessor("wlnPi", wlnPi_accessor)
+lnPiCollection.register_accessor("wlnPi_single", wlnPi_single_accessor)
+
+
 @SeriesWrapper.decorate_accessor("zloc")
 class _LocIndexer_unstack_zloc:
     """positional indexer for everything but phase"""
 
     def __init__(self, parent, level=["phase"]):
         self._parent = parent
         self._level = level
```

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/maskedlnpi_legacy.py` & `tmmc-lnpy-0.5.0/src/lnPi/maskedlnpi_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
-Legacy lnPi array routines (:mod:`~lnpy.maskedlnpi_legacy`)
+Legacy lnPi array routines (:mod:`~lnPi.maskedlnpi_legacy`)
 ===========================================================
 """
 from warnings import warn
 
-import numpy as np
-import pandas as pd
 from module_utilities import cached
-from scipy import ndimage
 
-from .extensions import AccessorMixin
-from .utils import labels_to_masks, masks_change_convention
+from lnpy._lazy_imports import np, pd
+from lnpy.ensembles import xce_accessor, xge_accessor
+from lnpy.extensions import AccessorMixin
+from lnpy.utils import labels_to_masks, masks_change_convention
 
 # NOTE : This is a rework of core.
 # [ ] : split xarray functionality into wrapper(s)
 # [ ] : split splitting into separate classes
 
 
 class MaskedlnPiLegacy(np.ma.MaskedArray, AccessorMixin):
@@ -184,15 +183,15 @@
     # @cached.meth
     def local_maxmask(self, *args, **kwargs):
         return self == self.local_max(*args, **kwargs)
 
     @cached.prop
     def edge_distance_matrix(self):
         """Matrix of distance from upper bound"""
-        from .utils import distance_matrix
+        from lnpy.utils import distance_matrix
 
         return distance_matrix(~self.mask)
 
     def edge_distance(self, ref, *args, **kwargs):
         return ref.edge_distance_matrix[self.local_argmax(*args, **kwargs)]
 
     # make these top level
@@ -240,15 +239,15 @@
         Returns
         -------
         out : object
             padded object
         """
         import bottleneck
 
-        from .utils import bfill, ffill
+        from lnpy.utils import bfill, ffill
 
         if axes is None:
             axes = range(self.ndim)
 
         data = self.data
         datas = []
 
@@ -365,22 +364,23 @@
         **kwargs
             Extra arguments to ``gaussian_filter``.
 
         See Also
         --------
         ~scipy.ndimage.gaussian_filter
         """
+        from scipy.ndimage import gaussian_filter
 
         if inplace:
             new = self
             new._clear_cache()
         else:
             new = self.copy()
 
-        ndimage.gaussian_filter(
+        gaussian_filter(
             new.data,
             output=new.data,
             mode=mode,
             truncate=truncate,
             sigma=sigma,
             **kwargs,
         )
@@ -549,7 +549,12 @@
             features=features,
             include_boundary=include_boundary,
             convention=False,
             check_features=check_features,
             **kwargs,
         )
         return self.list_from_masks(masks, convention=False)
+
+
+# --- register accessors ---------------------------------------------------------------
+MaskedlnPiLegacy.register_accessor("xge", xge_accessor)
+MaskedlnPiLegacy.register_accessor("xce", xce_accessor)
```

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/molfrac.py` & `tmmc-lnpy-0.5.0/src/lnpy/molfrac.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """routines to find constant molfracs"""
 
-import numpy as np
-from scipy import optimize
-
-# from .segment import get_default_PhaseCreator
+from ._lazy_imports import np
 
 
 def _initial_bracket_molfrac(
     target,
     C,
     build_phases,
     phase_id=0,
@@ -144,14 +141,15 @@
 
     Returns
     -------
     output : lnPi_phases object
         object with desired molfraction
     info : solver info (optional, returned if full_output is `True`)
     """
+    from scipy.optimize import brentq
 
     if build_kws is None:
         build_kws = {}
 
     if component is None:
         component = build_phases.index
 
@@ -195,15 +193,15 @@
             #     .values
             # )
         else:
             mf = np.inf
 
         return mf - target
 
-    xx, r = optimize.brentq(f, a, b, full_output=True, **kwargs)
+    xx, r = brentq(f, a, b, full_output=True, **kwargs)
     r.residual = f(xx)
 
     if np.abs(r.residual) > tol:
         raise RuntimeError("something went wrong with solve")
     return f.lnpi, r
```

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/options.py` & `tmmc-lnpy-0.5.0/src/lnpy/options.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/segment.py` & `tmmc-lnpy-0.5.0/src/lnpy/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,17 @@
  4. combination of 1-3.
 """
 
 import warnings
 from collections.abc import Iterable
 from functools import lru_cache
 
-import bottleneck
-import numpy as np
 from module_utilities.docfiller import DocFiller
-from skimage import feature, morphology, segmentation
 
+from ._lazy_imports import np
 from .docstrings import DOCFILLER_SHARED
 from .lnpienergy import wFreeEnergy
 from .lnpiseries import lnPiCollection
 
 # * Common doc strings
 _docstrings_local = r"""
 Parameters
@@ -112,14 +110,17 @@
     The option `mask` is passed as the value `labels` in :func:`~skimage.feature.peak_local_max`
 
     See Also
     --------
     ~skimage.feature.peak_local_max
     ~skimage.morphology.label
     """
+    import bottleneck
+    from skimage.feature import peak_local_max
+    from skimage.morphology import label as morphology_label
 
     assert style in ["indices", "mask", "marker"]
 
     if min_distance is None:
         min_distance = [5, 10, 15, 20, 25]
 
     if num_peaks_max is None:
@@ -129,15 +130,15 @@
         min_distance = [min_distance]
 
     data = data - bottleneck.nanmin(data)
     kwargs = dict(dict(exclude_border=False), **kwargs)
 
     n = idx = None
     for md in min_distance:
-        idx = feature.peak_local_max(
+        idx = peak_local_max(
             data,
             min_distance=md,
             labels=mask,
             threshold_abs=threshold_abs,
             threshold_rel=threshold_rel,
             # this option removed in future
             **kwargs,
@@ -164,15 +165,15 @@
     if style == "indices":
         out = idx
     else:
         out = np.zeros_like(data, dtype=bool)
         out[idx] = True
 
         if style == "marker":
-            out = morphology.label(out, connectivity=connectivity)
+            out = morphology_label(out, connectivity=connectivity)
 
     return out
 
 
 @docfiller_shared
 class Segmenter:
     """
@@ -263,19 +264,20 @@
         labels : ndarray of int
             Values > 0 correspond to found regions
 
         See Also
         --------
         ~skimage.segmentation.watershed
         """
+        from skimage.segmentation import watershed
 
         if connectivity is None:
             connectivity = data.ndim
         kwargs = dict(self.watershed_kws, connectivity=connectivity, *kwargs)
-        return segmentation.watershed(data, markers=markers, mask=mask, **kwargs)
+        return watershed(data, markers=markers, mask=mask, **kwargs)
 
     @docfiller_shared
     def segment_lnpi(
         self,
         lnpi,
         markers=None,
         find_peaks=True,
@@ -401,15 +403,15 @@
         self.lnPiFreeEnergy_kws = lnPiFreeEnergy_kws
 
         if merge_kws is None:
             merge_kws = {}
         merge_kws = dict(merge_kws, convention=False, nfeature_max=self.nmax)
         self.merge_kws = merge_kws
 
-    def _merge_phase_ids(sel, ref, phase_ids, lnpis):
+    def _merge_phase_ids(self, ref, phase_ids, lnpis):
         """Perform merge of phase_ids/index"""
         from scipy.spatial.distance import pdist
 
         if len(phase_ids) == 1:
             # only single phase_id
             return phase_ids, lnpis
```

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/stability.py` & `tmmc-lnpy-0.5.0/src/lnpy/stability.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 Thermodynamic stability (:mod:`~lnpy.stability`)
 ================================================
 
 Calculation of spinodal and binodal
 """
 import itertools
 
-import numpy as np
 from module_utilities import cached
-from scipy import optimize
 
+from ._lazy_imports import np
 from .lnpiseries import lnPiCollection
 
 
 # ###############################################################################
 # Spinodal routines
 def _initial_bracket_spinodal_right(
     C,
@@ -164,14 +163,15 @@
     Returns
     -------
     left,right : lnPiCollection
         left and right phases bracketing spinodal
 
     r : :class:`scipy.optimize.zeros.RootResults` object
     """
+    from scipy.optimize import RootResults
 
     doneLeft = False
     doneRight = False
     if build_kws is None:
         build_kws = {}
     if close_kws is None:
         close_kws = {}
@@ -188,24 +188,24 @@
         if dw > vmin and dw < efac:
             doneRight = True
 
         #########
         # checks
         if doneLeft and doneRight:
             # find bracket
-            r = optimize.RootResults(root=None, iterations=i, function_calls=i, flag=1)
+            r = RootResults(root=None, iterations=i, function_calls=i, flag=1)
             return left, right, r
 
         ########
         # converged?
         if np.allclose(left._get_lnz(), right._get_lnz(), **close_kws):
             # we've reached a breaking point
             if doneLeft:
                 # can't find a lower bound to efac, just return where we're at
-                r = optimize.RootResults(
+                r = RootResults(
                     root=left._get_lnz(), iterations=i + 1, function_calls=i, flag=0
                 )
                 for k, val in [
                     ("left", left),
                     ("right", right),
                     ("doneleft", doneLeft),
                     ("doneright", "doneRight"),
@@ -213,17 +213,15 @@
                 ]:
                     setattr(r, k, val)
                 return left, right, r
 
             # elif not doneLeft and not doneRight:
             else:
                 # all close, and no good on either end -> no spinodal
-                r = optimize.RootResults(
-                    root=None, iterations=i + 1, function_calls=i, flag=1
-                )
+                r = RootResults(root=None, iterations=i + 1, function_calls=i, flag=1)
                 for k, val in [
                     ("left", left),
                     ("right", right),
                     ("doneleft", doneLeft),
                     ("doneright", "doneRight"),
                     ("info", "all close and doneleft"),
                 ]:
@@ -264,28 +262,30 @@
     """
     )
 
 
 def _solve_spinodal(
     a, b, build_phases, idx, idx_nebr=None, efac=1.0, ref=None, build_kws=None, **kwargs
 ):
+    from scipy.optimize import brentq
+
     if build_kws is None:
         build_kws = {}
 
     def f(x):
         c = build_phases(x, ref=ref, **build_kws)
         dw = c.wfe_phases.get_dw(idx, idx_nebr)
         out = dw - efac
 
         f._lnpi = c
         f._out = out
 
         return out
 
-    xx, r = optimize.brentq(f, a, b, full_output=True, **kwargs)
+    xx, r = brentq(f, a, b, full_output=True, **kwargs)
 
     r.residual = f(xx)
     lnz = f._lnpi._get_lnz(build_phases.index)
     return lnz, r, f._lnpi
 
 
 def _get_step(C, idx, idx_nebr):
@@ -499,14 +499,15 @@
     stats : object, optional
         Solve stats object from ``brentq`` (optional, returned if full_output is True)
 
     See Also
     --------
     scipy.optimize.brentq
     """
+    from scipy.optimize import brentq
 
     IDs = list(IDs)
     assert len(IDs) == 2
 
     if build_kws is None:
         build_kws = {}
 
@@ -517,15 +518,15 @@
     def f(x):
         p = build_phases(x, ref=ref, **build_kws)
         f.lnpi = p
         # Omegas = c.omega_phase()
         # return Omegas[IDs[0]] - Omegas[IDs[1]]
         return p.xge.betaOmega().reindex(phase=IDs).diff("phase").squeeze().values
 
-    xx, r = optimize.brentq(f, a, b, full_output=True, **kwargs)
+    xx, r = brentq(f, a, b, full_output=True, **kwargs)
     r.residual = f(xx)
     if full_output:
         return f.lnpi, r
     else:
         return f.lnpi
```

### Comparing `tmmc-lnpy-0.4.0/src/lnpy/utils.py` & `tmmc-lnpy-0.5.0/src/lnpy/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 """
 Utility functions (:mod:`~lnpy.utils`)
 ======================================
 """
 
-from functools import partial
+from functools import lru_cache, partial
 
-import numpy as np
-
-# import pandas as pd
-import xarray as xr
-from scipy import ndimage as ndi
-from skimage import segmentation
+from ._lazy_imports import np
+from .options import OPTIONS
 
-# --------------------------------------------------
-# TQDM stuff
-try:
-    import tqdm as _tqdm
-
-    _HAS_TQDM = True
-except ImportError:
-    _HAS_TQDM = False
 
-if _HAS_TQDM:
+# --- TQDM setup -----------------------------------------------------------------------
+@lru_cache
+def _get_tqdm():
     try:
-        from IPython import get_ipython
+        import tqdm
+    except ImportError:
+        tqdm = None
+    return tqdm
 
-        p = get_ipython()
-        if p is not None and p.has_trait("kernel"):
-            from tqdm.notebook import tqdm as tqdm_default
-        else:
+
+@lru_cache
+def _get_tqdm_default():
+    _tqdm = _get_tqdm()
+    if _tqdm:
+        try:
+            from IPython import get_ipython
+
+            p = get_ipython()
+            if p is not None and p.has_trait("kernel"):
+                from tqdm.notebook import tqdm as tqdm_default
+            else:
+                tqdm_default = _tqdm.tqdm
+        except ImportError:
             tqdm_default = _tqdm.tqdm
-    except ImportError:
-        tqdm_default = _tqdm.tqdm
+    else:
+        tqdm_default = None
 
-from .options import OPTIONS
+    return tqdm_default
 
 
 def tqdm(*args, **kwargs):
     opt = OPTIONS["tqdm_bar"]
     if opt == "text":
-        func = _tqdm.tqdm
+        func = _get_tqdm().tqdm
     elif opt == "notebook":
-        func = _tqdm.tqdm_notebook
+        func = _get_tqdm().tqdm_notebook
     else:
-        func = tqdm_default
-
+        func = _get_tqdm_default()
     return func(*args, **kwargs)
 
 
 def get_tqdm(seq, len_min, leave=None, **kwargs):
     n = kwargs.get("total", None)
+    _tqdm = _get_tqdm()
 
     if isinstance(len_min, str):
         len_min = OPTIONS[len_min]
 
     if n is None:
         n = len(seq)
-    if _HAS_TQDM and OPTIONS["tqdm_use"] and n >= len_min:
+    if _tqdm and OPTIONS["tqdm_use"] and n >= len_min:
         if leave is None:
             leave = OPTIONS["tqdm_leave"]
         seq = tqdm(seq, leave=leave, **kwargs)
     return seq
 
 
 get_tqdm_calc = partial(get_tqdm, len_min="tqdm_len_calc")
@@ -76,92 +79,94 @@
 #     if len_min is None:
 #         len_min = OPTIONS['tqdm_len_build']
 #     return _get_tqdm(seq, len_min=len_min, leave=leave, **kwargs)
 
 
 # --------------------------------------------------
 # JOBLIB stuff
-try:
-    from joblib import Parallel, delayed
-
-    _HAS_JOBLIB = True
-except ImportError:
-    _HAS_JOBLIB = False
-
-
-from operator import attrgetter
+@lru_cache
+def _get_joblib():
+    try:
+        import joblib
+    except ImportError:
+        joblib = None
+    return joblib
 
 
 def parallel_map_build(func, items, *args, **kwargs):
-    if (
-        _HAS_JOBLIB
-        and OPTIONS["joblib_use"]
-        and len(items) >= OPTIONS["joblib_len_build"]
-    ):
-        return Parallel(
+    joblib = _get_joblib()
+    if joblib and OPTIONS["joblib_use"] and len(items) >= OPTIONS["joblib_len_build"]:
+        return joblib.Parallel(
             n_jobs=OPTIONS["joblib_n_jobs"],
             backend=OPTIONS["joblib_backend"],
             **OPTIONS["joblib_kws"],
-        )(delayed(func)(x, *args, **kwargs) for x in items)
+        )(joblib.delayed(func)(x, *args, **kwargs) for x in items)
     else:
         return [func(x, *args, **kwargs) for x in items]
 
 
 def _func_call(x, *args, **kwargs):
     return x(*args, **kwargs)
 
 
 def parallel_map_call(items, use_joblib, *args, **kwargs):
+    joblib = _get_joblib()
     if (
         use_joblib
-        and _HAS_JOBLIB
+        and joblib
         and OPTIONS["joblib_use"]
         and len(items) >= OPTIONS["joblib_len_calc"]
     ):
-        return Parallel(
+        return joblib.Parallel(
             n_jobs=OPTIONS["joblib_n_jobs"],
             backend=OPTIONS["joblib_backend"],
             **OPTIONS["joblib_kws"],
-        )(delayed(_func_call)(x, *args, **kwargs) for x in items)
+        )(joblib.delayed(_func_call)(x, *args, **kwargs) for x in items)
     else:
         return [x(*args, **kwargs) for x in items]
 
 
 def parallel_map_attr(attr, use_joblib, items):
+    from operator import attrgetter
+
+    joblib = _get_joblib()
     func = attrgetter(attr)
+
     if (
         use_joblib
-        and _HAS_JOBLIB
+        and joblib
         and OPTIONS["joblib_use"]
         and len(items) >= OPTIONS["joblib_len_calc"]
     ):
-        return Parallel(
+        return joblib.Parallel(
             n_jobs=OPTIONS["joblib_n_jobs"],
             backend=OPTIONS["joblib_backend"],
             **OPTIONS["joblib_kws"],
-        )(delayed(func)(x) for x in items)
+        )(joblib.delayed(func)(x) for x in items)
     else:
         return [func(x) for x in items]
 
 
 def parallel_map_func_starargs(func, use_joblib, items, total=None):
     if total is None:
         total = len(items)
 
+    joblib = _get_joblib()
+
     if (
         use_joblib
-        and _HAS_JOBLIB
+        and joblib
         and OPTIONS["joblib_use"]
         and total >= OPTIONS["joblib_len_calc"]
     ):
-        return Parallel(
+        return joblib.Parallel(
             n_jobs=OPTIONS["joblib_n_jobs"],
             backend=OPTIONS["joblib_backend"],
             **OPTIONS["joblib_kws"],
-        )(delayed(func)(*x) for x in items)
+        )(joblib.delayed(func)(*x) for x in items)
     else:
         return [func(*x) for x in items]
 
 
 # ----------------------------------------
 # pandas stuff
 def allbut(levels, *names):
@@ -185,17 +190,19 @@
     for k in out:
         if dim in out[k].dims:
             out = out.drop(k).update(table[k].pipe(dim_to_suffix_dataarray, dim, join))
     return out
 
 
 def dim_to_suffix(ds, dim="component", join="_"):
-    if isinstance(ds, xr.DataArray):
+    from xarray import DataArray, Dataset
+
+    if isinstance(ds, DataArray):
         f = dim_to_suffix_dataarray
-    elif isinstance(ds, xr.Dataset):
+    elif isinstance(ds, Dataset):
         f = dim_to_suffix_dataset
     else:
         raise ValueError("`ds` must be `DataArray` or `Dataset`")
     return f(ds, dim=dim, join=join)
 
 
 def _convention_to_bool(convention):
@@ -320,14 +327,15 @@
 
     See Also
     --------
     masks_to_labels
     :func:`skimage.segmentation.find_boundaries`
 
     """
+    from skimage import segmentation
 
     if include_boundary:
         kwargs = dict(dict(mode="outer", connectivity=labels.ndim), **kwargs)
     if features is None:
         features = [i for i in np.unique(labels) if i > 0]
     elif check_features:
         vals = np.unique(labels)
@@ -500,26 +508,27 @@
         Distance from possible feature elements to background
 
 
     See Also
     --------
     ~scipy.ndimage.distance_transform_edt
     """
+    from scipy.ndimage import distance_transform_edt
 
     mask = np.asarray(mask, dtype=bool)
     mask = masks_change_convention(mask, convention_in=convention, convention_out=True)
 
     # pad mask
     # add padding to end of matrix in each dimension
     ndim = mask.ndim
     pad_width = ((0, 1),) * ndim
     mask = np.pad(mask, pad_width=pad_width, mode="constant", constant_values=False)
 
     # distance filter
-    dist = ndi.distance_transform_edt(mask)
+    dist = distance_transform_edt(mask)
 
     # remove padding
     s = (slice(None, -1),) * ndim
     return dist[s]
 
 
 def lnpimasked_to_dataset(data, keys=("lnpi", "PE")):
```

### Comparing `tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/PKG-INFO` & `tmmc-lnpy-0.5.0/src/tmmc_lnpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmmc-lnpy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Analysis of lnPi results from TMMC simulation
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/tmmc-lnpy
 Project-URL: documentation, https://pages.nist.gov/tmmc-lnpy/
 Keywords: tmmc-lnpy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,14 +17,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: viz
+Provides-Extra: dev-extras
+Provides-Extra: typing-extras
+Provides-Extra: typing
+Provides-Extra: nox
+Provides-Extra: dev
+Provides-Extra: tools
+Provides-Extra: dev-complete
+Provides-Extra: docs
+Provides-Extra: dist-pypi
+Provides-Extra: dist-conda
 License-File: LICENSE
 
 <!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
@@ -186,19 +197,30 @@
 
 ## Unreleased
 
 See the fragment files in [changelog.d](https://github.com/usnistgov/tmmc-lnpy)
 
 <!-- scriv-insert-here -->
 
+## v0.5.0 — 2023-07-06
+
+### Added
+
+- Now use [lazy_loader](https://github.com/scientific-python/lazy_loader) to
+  speed up initial load time.
+
+Full set of changes:
+[`v0.4.0...0.5.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.4.0...v0.5.0)
+
 ## v0.4.0 — 2023-05-12
 
 ### Added
 
-- Package now available on conda-forge
+- Package now available on conda-forge Full set of changes:
+  [`v0.3.0...0.4.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.3.0...v0.4.0)
 
 ### Changed
 
 - Changed `examples.load_example_maskddata` to
   `examples.load_example_lnpimasked` for consistency with other method names.
 
 ## v0.3.0 — 2023-05-02
@@ -209,15 +231,15 @@
 
 - Moved `_docstrings` -> `docstrings` to make available
 - Moved from local docfiller to module_utilities.docfiller
 - Moved from local cached module to module-utilities.cached
 - Add support for python3.11
 
 Full set of changes:
-[`v0.2.2...0.3.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.2.2...0.3.0)
+[`v0.2.2...0.3.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.2.2...v0.3.0)
 
 ### Changed
 
 - Update package layout
 - New linters via pre-commit
 - Development env now handled by tox
```

### Comparing `tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/SOURCES.txt` & `tmmc-lnpy-0.5.0/src/tmmc_lnpy.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -9,52 +9,53 @@
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 environment.yaml
+noxfile.py
 pyproject.toml
-tox.ini
 changelog.d/README.txt
 changelog.d/templates/new_fragment.md.j2
 changelog.d/templates/auto-changelog/macros.jinja2
 changelog.d/templates/auto-changelog/template.jinja2
+environment/base.yaml
 environment/dev-extras.yaml
 environment/dev.yaml
 environment/dist-conda.yaml
+environment/dist-pypi.txt
 environment/dist-pypi.yaml
 environment/docs-extras.yaml
 environment/docs.yaml
-environment/lint-extras.yaml
 environment/lint.yaml
+environment/test-extras.txt
 environment/test-extras.yaml
 environment/test.yaml
-environment/tools.yaml
-scripts/dist-conda.mk
-scripts/dist-pypi.mk
-scripts/docs-examples-symlinks.sh
-scripts/lint.mk
-scripts/recipe-append.sh
-scripts/run-prettier.sh
-scripts/tox-ipykernel-display-name.sh
+environment/typing.yaml
+environment/lock/py310.yaml
+environment/lock/py311.yaml
+environment/lock/py38.yaml
+environment/lock/py39.yaml
 src/lnPi/__init__.py
 src/lnPi/collectionlnpiutils.py
+src/lnPi/maskedlnpi_legacy.py
 src/lnPi/stability.py
 src/lnpy/__init__.py
+src/lnpy/_lazy_imports.py
+src/lnpy/_version.py
 src/lnpy/bracket.py
 src/lnpy/docstrings.py
 src/lnpy/ensembles.py
 src/lnpy/examples.py
 src/lnpy/extensions.py
 src/lnpy/lnpicollectionutils.py
 src/lnpy/lnpidata.py
 src/lnpy/lnpienergy.py
 src/lnpy/lnpiseries.py
-src/lnpy/maskedlnpi_legacy.py
 src/lnpy/molfrac.py
 src/lnpy/options.py
 src/lnpy/segment.py
 src/lnpy/stability.py
 src/lnpy/utils.py
 src/lnpy/data/hsmix_example.json.gz
 src/lnpy/data/lj_sub_example.json
@@ -75,8 +76,9 @@
 tests/test_single_comp_super.py
 tests/test_water_cluster.py
 tests/water_cluster/data_0.csv
 tests/water_cluster/data_0_dw.csv
 tests/water_cluster/data_1.csv
 tests/water_cluster/data_1_dw.csv
 tests/water_cluster/water_MOF_ensemble.json
-tests/water_cluster/water_MOF_example.csv
+tests/water_cluster/water_MOF_example.csv
+tools/noxtools.py
```

### Comparing `tmmc-lnpy-0.4.0/tests/test_hs_mix.py` & `tmmc-lnpy-0.5.0/tests/test_hs_mix.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/tests/test_lj_mix_0.py` & `tmmc-lnpy-0.5.0/tests/test_lj_mix_0.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/tests/test_lnPi.py` & `tmmc-lnpy-0.5.0/tests/test_lnPi.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/tests/test_single_comp_sub.py` & `tmmc-lnpy-0.5.0/tests/test_single_comp_sub.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/tests/test_single_comp_super.py` & `tmmc-lnpy-0.5.0/tests/test_single_comp_super.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/tests/test_water_cluster.py` & `tmmc-lnpy-0.5.0/tests/test_water_cluster.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/tests/water_cluster/data_0.csv` & `tmmc-lnpy-0.5.0/tests/water_cluster/data_0.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/tests/water_cluster/data_1.csv` & `tmmc-lnpy-0.5.0/tests/water_cluster/data_1.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/tests/water_cluster/data_1_dw.csv` & `tmmc-lnpy-0.5.0/tests/water_cluster/data_1_dw.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.4.0/tests/water_cluster/water_MOF_example.csv` & `tmmc-lnpy-0.5.0/tests/water_cluster/water_MOF_example.csv`

 * *Files identical despite different names*

