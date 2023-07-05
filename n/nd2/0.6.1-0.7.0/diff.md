# Comparing `tmp/nd2-0.6.1.tar.gz` & `tmp/nd2-0.7.0.tar.gz`

## Comparing `nd2-0.6.1.tar` & `nd2-0.7.0.tar`

### file list

```diff
@@ -1,55 +1,65 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nd2-0.6.1/.github_changelog_generator
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 nd2-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17666 2020-02-02 00:00:00.000000 nd2-0.6.1/CHANGELOG.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 nd2-0.6.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nd2-0.6.1/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nd2-0.6.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 nd2-0.6.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nd2-0.6.1/.github/workflows/cron.yml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/bf_describe.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/compare.py
--rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/comparison.json
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/download_samples.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/gather.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/nd2_describe.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/__init__.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_binary.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_clx_lite.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_clx_xml.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_util.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_version.py
--rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/index.py
--rw-r--r--   0        0        0    33458 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/nd2file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/py.typed
--rw-r--r--   0        0        0    13163 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/structures.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_legacy/__init__.py
--rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_legacy/_legacy.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_legacy/_legacy_xml.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_pysdk/__init__.py
--rw-r--r--   0        0        0    14682 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_pysdk/_chunk_decode.py
--rw-r--r--   0        0        0    24874 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_pysdk/_parse.py
--rw-r--r--   0        0        0    21321 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_pysdk/_pysdk.py
--rw-r--r--   0        0        0    19912 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_pysdk/_sdk_types.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/conftest.py
--rw-r--r--   0        0        0  5234229 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/readlim_output.json
--rw-r--r--   0        0        0   513829 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/samples_metadata.json
--rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_aicsimage.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_binary.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_dask_dispatch.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_deprecations.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_index.py
--rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_metadata.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_parse.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_reader.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_readme.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_rescue.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_rois.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_segfaults.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_xml.py
--rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/variant.xml
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/variant_CustomDataV2_0.xml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nd2-0.6.1/.gitignore
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 nd2-0.6.1/LICENSE
--rw-r--r--   0        0        0    32117 2020-02-02 00:00:00.000000 nd2-0.6.1/README.md
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 nd2-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    34241 2020-02-02 00:00:00.000000 nd2-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nd2-0.7.0/.github_changelog_generator
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nd2-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    18887 2020-02-02 00:00:00.000000 nd2-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 nd2-0.7.0/mkdocs.yml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 nd2-0.7.0/docs/index.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nd2-0.7.0/docs/API/nd2.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nd2-0.7.0/docs/API/nd2_binary.md
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nd2-0.7.0/docs/API/structures.md
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 nd2-0.7.0/docs/styles/extra.css
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/bf_describe.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/compare.py
+-rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/comparison.json
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/download_samples.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/gather.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/nd2_describe.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/__init__.py
+-rw-r--r--   0        0        0     8543 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_binary.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_clx_lite.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_clx_xml.py
+-rw-r--r--   0        0        0     8440 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_ome.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_util.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_version.py
+-rw-r--r--   0        0        0     9120 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/index.py
+-rw-r--r--   0        0        0    49780 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/nd2file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/py.typed
+-rw-r--r--   0        0        0    14331 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/structures.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_legacy/__init__.py
+-rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_legacy/_legacy.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_legacy/_legacy_xml.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_pysdk/__init__.py
+-rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_pysdk/_chunk_decode.py
+-rw-r--r--   0        0        0    25557 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_pysdk/_parse.py
+-rw-r--r--   0        0        0    21293 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_pysdk/_pysdk.py
+-rw-r--r--   0        0        0    21560 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_pysdk/_sdk_types.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0  5234229 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/readlim_output.json
+-rw-r--r--   0        0        0   513829 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/samples_metadata.json
+-rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_aicsimage.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_binary.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_codspeed.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_dask_dispatch.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_deprecations.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_index.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_metadata.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_ome.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_parse.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_reader.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_readme.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_rescue.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_rois.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_segfaults.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_xml.py
+-rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/variant.xml
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/variant_CustomDataV2_0.xml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nd2-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 nd2-0.7.0/LICENSE
+-rw-r--r--   0        0        0    32417 2020-02-02 00:00:00.000000 nd2-0.7.0/README.md
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 nd2-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    34675 2020-02-02 00:00:00.000000 nd2-0.7.0/PKG-INFO
```

### Comparing `nd2-0.6.1/.pre-commit-config.yaml` & `nd2-0.7.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,29 @@
   autoupdate_schedule: monthly
   autofix_commit_msg: "style(pre-commit.ci): auto fixes [...]"
   autoupdate_commit_msg: "ci(pre-commit.ci): autoupdate"
 
 default_install_hook_types: [pre-commit, commit-msg]
 
 repos:
-
   # - repo: https://github.com/compilerla/conventional-pre-commit
-    # rev: v2.3.0
-    # hooks:
-    #   - id: conventional-pre-commit
-    #     stages: [commit-msg]
+  # rev: v2.3.0
+  # hooks:
+  #   - id: conventional-pre-commit
+  #     stages: [commit-msg]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.272
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.276
     hooks:
       - id: ruff
         args: [--fix]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
@@ -33,13 +32,26 @@
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.13
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         files: "^src/"
         exclude: scripts
-        additional_dependencies: [numpy, lxml-stubs]
+        additional_dependencies:
+          - numpy
+          - types-lxml
+          - ome-types
+          - pydantic
+
+
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.5
+    hooks:
+      - id: codespell
+        exclude: CHANGELOG.md
+        args:
+          - "-L=nd2,nd,pevents"
```

### Comparing `nd2-0.6.1/CHANGELOG.md` & `nd2-0.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # Changelog
 
+## [v0.7.0](https://github.com/tlambert03/nd2/tree/v0.7.0) (2023-07-05)
+
+[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.6.1...v0.7.0)
+
+**Implemented enhancements:**
+
+- feat: add ome\_metadata output to ome-types [\#153](https://github.com/tlambert03/nd2/pull/153) ([tlambert03](https://github.com/tlambert03))
+- feat: add row filtering to nd2.index, as well as binary/roi data [\#151](https://github.com/tlambert03/nd2/pull/151) ([tlambert03](https://github.com/tlambert03))
+
+**Fixed bugs:**
+
+- fix: fix extra kwargs to roi info [\#158](https://github.com/tlambert03/nd2/pull/158) ([tlambert03](https://github.com/tlambert03))
+- fix: fix frame\_metadata and various metadata typing [\#155](https://github.com/tlambert03/nd2/pull/155) ([tlambert03](https://github.com/tlambert03))
+- fix: improve roi parsing for some files [\#150](https://github.com/tlambert03/nd2/pull/150) ([tlambert03](https://github.com/tlambert03))
+
+**Tests & CI:**
+
+- ci: add codspeed benchmarks [\#152](https://github.com/tlambert03/nd2/pull/152) ([tlambert03](https://github.com/tlambert03))
+
+**Documentation:**
+
+- docs: adding docs [\#149](https://github.com/tlambert03/nd2/pull/149) ([tlambert03](https://github.com/tlambert03))
+
 ## [v0.6.1](https://github.com/tlambert03/nd2/tree/v0.6.1) (2023-06-24)
 
 [Full Changelog](https://github.com/tlambert03/nd2/compare/v0.6.0...v0.6.1)
 
 **Implemented enhancements:**
 
 - feat: support files with custom experiment loops [\#148](https://github.com/tlambert03/nd2/pull/148) ([tlambert03](https://github.com/tlambert03))
```

### Comparing `nd2-0.6.1/.github/workflows/ci.yml` & `nd2-0.7.0/.github/workflows/ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -65,14 +65,42 @@
 
       - name: Test
         run: pytest -v --cov=nd2 --cov-report=xml --cov-report=term
 
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v3
 
+  benchmarks:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: "3.11"
+
+      - uses: actions/cache@v3
+        id: cache
+        with:
+          path: tests/data
+          key: ${{ hashFiles('scripts/download_samples.py') }}
+
+      - name: Download Samples
+        if: steps.cache.outputs.cache-hit != 'true'
+        run: |
+          pip install requests
+          python scripts/download_samples.py
+
+      - name: install
+        run: python -m pip install .[test]
+
+      - name: Run benchmarks
+        uses: CodSpeedHQ/action@v1
+        with:
+          run: pytest --codspeed -v --color=yes
+
   deploy:
     needs: test
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/v')
     steps:
       - uses: actions/checkout@v3
         with:
```

### Comparing `nd2-0.6.1/.github/workflows/cron.yml` & `nd2-0.7.0/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/scripts/bf_describe.py` & `nd2-0.7.0/scripts/bf_describe.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/scripts/compare.py` & `nd2-0.7.0/scripts/compare.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/scripts/comparison.json` & `nd2-0.7.0/scripts/comparison.json`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/scripts/download_samples.py` & `nd2-0.7.0/scripts/download_samples.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/scripts/gather.py` & `nd2-0.7.0/scripts/gather.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/scripts/nd2_describe.py` & `nd2-0.7.0/scripts/nd2_describe.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/src/nd2/_binary.py` & `nd2-0.7.0/src/nd2/_binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,45 +16,45 @@
 
 I7 = struct.Struct("<" + "I" * 7)
 I9 = struct.Struct("<" + "I" * 9)
 I2 = struct.Struct("<" + "I" * 2)
 
 
 class BinaryLayer(NamedTuple):
-    """Wrapper for data from a single binary layer in an ND2 file.
+    """Wrapper for data from a single binary layer in an [`nd2.ND2File`][].
 
     `data` will have length of num_sequences, with `None` for any frames
     that lack binary data.
 
-    Parameters
+    Attributes
     ----------
-    data : list of numpy.ndarray or None
+    data : list[numpy.ndarray] | None
         The data for each frame. If a frame has no binary data, the value
         will be None.  Data will have the same length as the number of sequences
         in the file.
-    name: str
+    name : str
         The name of the binary layer.
-    comp_name: str
+    comp_name : str
         The name of the associated component, if Any.
-    comp_order: int
+    comp_order : int
         The order of the associated component, if Any.
-    color: int
+    color : int
         The color of the binary layer.
-    color_mode: int
+    color_mode : int
         The color mode of the binary layer.  I believe this is related to how colors
         are chosen in NIS-Elements software.  Where "0" is direct color (i.e. use,
         the color value), "8" is color by 3D ... and I'm not sure about the rest :)
-    state: int
+    state : int
         The state of the binary layer. (meaning still unclear)
-    file_tag: str
+    file_tag : str
         The key for the binary layer in the CustomData metadata,
         e.g. `RleZipBinarySequence_1_v1`
-    layer_id: int
+    layer_id : int
         The ID of the binary layer.
-    coordinate_shape: tuple of int
+    coordinate_shape : tuple[int, ...]
         The shape of the coordinates for the associated nd2 file.  This is used
         to reshape the data into a 3D array in `asarray`.
     """
 
     data: list[np.ndarray | None]
     name: str
     comp_name: str
@@ -107,16 +107,16 @@
 
     This object is a sequence of `BinaryLayer` objects, one for each binary layer in the
     file.  Each layer has a `name` attribute, and a `data` attribute that is list of
     numpy arrays - one for each frame in the experiment - or None if the layer was not
     present in that frame.
 
     The wrapper can be cast to a numpy array (with `BinaryLayers.asarray()` or
-    np.asarray(BinaryLayers)) to stack all the layers into a single array.  The output
-    array will have shape (n_layers, *coord_shape, *frame_shape).
+    `np.asarray(BinaryLayers)`) to stack all the layers into a single array.  The output
+    array will have shape `(n_layers, *coord_shape, *frame_shape)`.
     """
 
     def __init__(self, data: list[BinaryLayer]) -> None:
         self._data = data
 
     @overload
     def __getitem__(self, key: int) -> BinaryLayer:
@@ -135,15 +135,15 @@
     def __len__(self) -> int:
         return len(self._data)
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__} with {len(self)} layers>"
 
     def __array__(self) -> np.ndarray:
-        """Compatibility with np.asarray(BinaryLayers)."""
+        """Compatibility with `np.asarray(BinaryLayers)`."""
         return self.asarray()
 
     def asarray(self) -> np.ndarray:
         """Stack all the layers/frames into a single array.
 
         The output array will have shape (n_layers, *coord_shape, *frame_shape).
         """
```

### Comparing `nd2-0.6.1/src/nd2/_clx_lite.py` & `nd2-0.7.0/src/nd2/_clx_lite.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/src/nd2/_clx_xml.py` & `nd2-0.7.0/src/nd2/_clx_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         name = LOWER.sub("", name) or name
 
     runtype = node.attrib.get("runtype")
     if runtype in _XMLCAST:
         val = node.attrib.get("value")
         value: JsonValue = _XMLCAST[runtype](val)
     else:
-        value = dict(node.attrib) if include_attrs else {}  # type: ignore
+        value = dict(node.attrib) if include_attrs else {}
         for i, child in enumerate(node):
             cname, cval = _node_name_value(
                 child, strip_prefix, include_attrs  # type: ignore
             )
             # NOTE: "no_name" is the standard name for a list-type node
             # "BinaryItem" is a special case found in the BinaryMetadata_v1 tag...
             # without special handling, you would only get the last item in the list
```

### Comparing `nd2-0.6.1/src/nd2/_util.py` & `nd2-0.7.0/src/nd2/_util.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/src/nd2/index.py` & `nd2-0.7.0/src/nd2/index.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import json
 import sys
 from argparse import RawTextHelpFormatter
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from pathlib import Path
-from typing import Iterable, Iterator, Sequence, cast, no_type_check
+from typing import Any, Iterable, Iterator, Sequence, cast, no_type_check
 
 from typing_extensions import TypedDict
 
 import nd2
 
 try:
     import rich
@@ -29,14 +29,16 @@
     version: str
     kb: float
     acquired: str
     experiment: str
     dtype: str
     shape: list[int]
     axes: str
+    binary: bool
+    rois: bool
     software_name: str
     software_version: str
     grabber: str
 
 
 HEADERS = list(Record.__annotations__)
 TIME_FORMAT = "%Y-%m-%d %H:%M:%S"  # YYYY-MM-DD HH:MM:SS
@@ -44,17 +46,19 @@
 
 def index_file(path: Path) -> Record:
     """Return a dict with the index file data."""
     with nd2.ND2File(path) as nd:
         if nd.is_legacy:
             software: dict = {}
             acquired: str | None = ""
+            binary = False
         else:
             software = nd._rdr._app_info()  # type: ignore
             acquired = nd._rdr._acquisition_date()  # type: ignore
+            binary = nd.binary_data is not None
 
         stat = path.stat()
         exp = [(x.type, x.count) for x in nd.experiment]
         axes, shape = zip(*nd.sizes.items())
         if isinstance(acquired, datetime):
             acquired = acquired.strftime(TIME_FORMAT)
 
@@ -65,14 +69,16 @@
                 "version": ".".join(map(str, nd.version)),
                 "kb": round(stat.st_size / 1000, 2),
                 "acquired": acquired or "",
                 "experiment": ";".join([f"{t}:{c}" for t, c in exp]),
                 "dtype": str(nd.dtype),
                 "shape": list(shape),
                 "axes": "".join(axes),
+                "binary": binary,
+                "rois": bool(nd.rois),
                 "software_name": software.get("SWNameString", ""),
                 "software_version": software.get("VersionString", ""),
                 "grabber": software.get("GrabberString", ""),
             }
         )
 
 
@@ -92,37 +98,53 @@
 ) -> list[Record]:
     with ThreadPoolExecutor() as executor:
         results = list(executor.map(index_file, _gather_files(paths, recurse, glob)))
 
     return results
 
 
-def _pretty_print_table(data: list[Record]) -> None:
+def _pretty_print_table(data: list[Record], sort_column: str | None = None) -> None:
     try:
         from rich.console import Console
         from rich.table import Table
+
     except ImportError:
         raise sys.exit(
             "rich is required to print a pretty table. "
             "Install it with `pip install rich`."
         ) from None
 
     table = Table(show_header=True, header_style="bold")
+    headers = list(data[0])
+
+    # add headers, and highlight any sorted columns
+    sort_col = ""
+    if sort_column:
+        sort_col = (sort_column or "").rstrip("-")
+        direction = " ↓" if sort_column.endswith("-") else " ↑"
+    for header in headers:
+        if header == sort_col:
+            table.add_column(header + direction, style="green")
+        else:
+            table.add_column(header)
 
-    for header in data[0]:
-        table.add_column(header)
     for row in data:
-        table.add_row(*[str(value) for value in row.values()])
+        table.add_row(*[_strify(value) for value in row.values()])
 
     Console().print(table)
 
 
+def _strify(val: Any) -> str:
+    if isinstance(val, bool):
+        return "✅" if val else ""
+    return str(val)
+
+
 def _print_csv(records: list[Record], skip_header: bool = False) -> None:
     import csv
-    import sys
 
     writer = csv.DictWriter(sys.stdout, fieldnames=records[0].keys())
     if not skip_header:
         writer.writeheader()
     writer.writerows(records)
 
 
@@ -187,66 +209,106 @@
     )
     parser.add_argument(
         "--no-header",
         default=False,
         action="store_true",
         help="Don't write the CSV header",
     )
+    parser.add_argument(
+        "--filter",
+        "-F",
+        type=str,
+        action="append",
+        help="Filter the output. Each filter "
+        "should be a python expression (string)\nthat evaluates to True or False. "
+        "It will be evaluated in the context\nof each row. You can use any of the "
+        "column names as variables.\ne.g.: \"acquired > '2020' and kb < 500\". (May "
+        "be used multiple times).",
+    )
 
     return parser.parse_args(argv or sys.argv[1:])
 
 
 @no_type_check
 def _filter_data(
     data: list[Record],
-    to_include: Sequence[str] = (),
     sort_by: str | None = None,
+    include: str | None = None,
     exclude: str | None = None,
+    filters: Sequence[str] = (),
 ) -> list[Record]:
-    unrecognized = set(to_include) - set(HEADERS)
+    """Filter and sort the data.
+
+    Parameters
+    ----------
+    data : list[Record]
+        the data to filter
+    sort_by : str | None, optional
+        Name of column to sort by, by default None
+    include : str | None, optional
+        Comma-separated list of columns to include, by default None
+    exclude : str | None, optional
+        Comma-separated list of columns to exclude, by default None
+    filters : Sequence[str], optional
+        Sequence of python expression strings to filter the data, by default ()
+
+    Returns
+    -------
+    list[Record]
+        _description_
+    """
+    includes = include.split(",") if include else []
+    unrecognized = set(includes) - set(HEADERS)
     if unrecognized:  # pragma: no cover
         print(f"Unrecognized columns: {', '.join(unrecognized)}", file=sys.stderr)
-        to_include = [x for x in to_include if x not in unrecognized]
+        includes = [x for x in includes if x not in unrecognized]
+
+    if sort_by:
+        if sort_by.endswith("-"):
+            data.sort(key=lambda x: x[sort_by[:-1]], reverse=True)
+        else:
+            data.sort(key=lambda x: x[sort_by])
 
-    if to_include:
+    if includes:
         # preserve order of to_include
-        data = [{h: row[h] for h in to_include} for row in data]
+        data = [{h: row[h] for h in includes} for row in data]
 
     to_exclude = cast("list[str]", exclude.split(",") if exclude else [])
 
     if to_exclude:
         data = [{h: row[h] for h in HEADERS if h not in to_exclude} for row in data]
 
-    if sort_by:
-        if sort_by.endswith("-"):
-            data.sort(key=lambda x: x[sort_by[:-1]], reverse=True)
-        else:
-            data.sort(key=lambda x: x[sort_by])
+    if filters:
+        # filters are in the form of a string expression, to be evaluated
+        # against each row. For example, "'TimeLoop' in experiment"
+        for f in filters:
+            try:
+                data = [row for row in data if bool(eval(f, None, row))]
+            except Exception as e:  # pragma: no cover
+                print(f"Error evaluating filter {f!r}: {e}", file=sys.stderr)
+                sys.exit(1)
 
     return data
 
 
 def main(argv: Sequence[str] = ()) -> None:
     """Index ND2 files and print the results as a table."""
     args = _parse_args(argv)
 
-    to_include = cast("list[str]", args.include.split(",") if args.include else [])
-    if args.sort_by and to_include and args.sort_by not in to_include:
-        raise sys.exit(  # pragma: no cover
-            f"The sort column {args.sort_by!r} must be in the "
-            f"included columns: {to_include!r}."
-        )
-
     data = _index_files(paths=args.paths, recurse=args.recurse, glob=args.glob_pattern)
     data = _filter_data(
-        data, to_include=to_include, sort_by=args.sort_by, exclude=args.exclude
+        data,
+        sort_by=args.sort_by,
+        include=args.include,
+        exclude=args.exclude,
+        filters=args.filter,
     )
 
     if args.format == "table":
-        _pretty_print_table(data)
+        _pretty_print_table(data, args.sort_by)
     elif args.format == "csv":
         _print_csv(data, args.no_header)
     elif args.format == "json":
         _print_json(data)
 
 
 if __name__ == "__main__":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nd2-0.6.1/src/nd2/nd2file.py` & `nd2-0.7.0/src/nd2/nd2file.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,16 +20,18 @@
     cached_property = property  # type: ignore
 
 
 if TYPE_CHECKING:
     import mmap
     from typing import Any, Sequence, Sized, SupportsInt
 
+    import dask.array
     import dask.array.core
     import xarray as xr
+    from ome_types import OME
     from typing_extensions import Literal
 
     from ._binary import BinaryLayers
     from ._pysdk._pysdk import ND2Reader as LatestSDKReader
     from ._util import DictOfDicts, DictOfLists, ListOfDicts, StrOrBytesPath
     from .structures import (
         Attributes,
@@ -42,28 +44,50 @@
 
 __all__ = ["ND2File", "imread"]
 
 
 class ND2File:
     """Main objecting for opening and extracting data from an nd2 file.
 
+    ```python
+    with nd2.ND2File("path/to/file.nd2") as nd2_file:
+        ...
+    ```
+
+    The key metadata outputs are:
+
+    - [attributes][nd2.ND2File.attributes]
+    - [metadata][nd2.ND2File.metadata] / [frame_metadata][nd2.ND2File.frame_metadata]
+    - [experiment][nd2.ND2File.experiment]
+    - [text_info][nd2.ND2File.text_info]
+
+    Some files may also have:
+
+    - [binary_data][nd2.ND2File.binary_data]
+    - [rois][nd2.ND2File.rois]
+
+    !!! tip
+
+        For a simple way to read nd2 file data into an array, see [nd2.imread][].
+
     Parameters
     ----------
     path : Path | str
         Filename of an nd2 file.
     validate_frames : bool
         Whether to verify (and attempt to fix) frames whose positions have been
         shifted relative to the predicted offset (i.e. in a corrupted file).
         This comes at a slight performance penalty at file open, but may "rescue"
         some corrupt files. by default False.
     search_window : int
         When validate_frames is true, this is the search window (in KB) that will
         be used to try to find the actual chunk position. by default 100 KB
     read_using_sdk : Optional[bool]
-        DEPRECATED.  No longer does anything.
+        :warning: **DEPRECATED**.  No longer does anything.
+
         If `True`, use the SDK to read the file. If `False`, inspects the chunkmap
         and reads from a `numpy.memmap`. If `None` (the default), uses the SDK if
         the file is compressed, otherwise uses the memmap. Note: using
         `read_using_sdk=False` on a compressed file will result in a ValueError.
     """
 
     _memmap: mmap.mmap
@@ -93,20 +117,27 @@
         self._closed = False
         self._is_legacy = "Legacy" in type(self._rdr).__name__
         self._lock = threading.RLock()
         self._version: tuple[int, ...] | None = None
 
     @staticmethod
     def is_supported_file(path: StrOrBytesPath) -> bool:
-        """Return True if the file is supported by this reader."""
+        """Return `True` if the file is supported by this reader."""
         return is_supported_file(path)
 
     @property
     def version(self) -> tuple[int, ...]:
-        """Return the file format version as a tuple of ints."""
+        """Return the file format version as a tuple of ints.
+
+        Likely values are:
+
+        - `(1, 0)` = a legacy nd2 file (JPEG2000)
+        - `(2, 0)`, `(2, 1)` = non-JPEG2000 nd2 with xml metadata
+        - `(3, 0)` = new format nd2 file with lite variant metadata
+        """
         if self._version is None:
             try:
                 self._version = get_version(self._rdr._fh or self._rdr._path)
             except Exception:
                 self._version = (-1, -1)
                 raise
         return self._version
@@ -118,28 +149,52 @@
 
     @property
     def is_legacy(self) -> bool:
         """Whether file is a legacy nd2 (JPEG2000) file."""
         return self._is_legacy
 
     def open(self) -> None:
-        """Open file for reading."""
+        """Open file for reading.
+
+        !!! note
+
+            Files are best opened using a context manager:
+
+            ```python
+            with nd2.ND2File("path/to/file.nd2") as nd2_file:
+                ...
+            ```
+
+            This will automatically close the file when the context exits.
+        """
         if self.closed:
             self._rdr.open()
             self._closed = False
 
     def close(self) -> None:
-        """Close file (may cause segfault if read when closed in some cases)."""
+        """Close file.
+
+        !!! note
+
+            Files are best opened using a context manager:
+
+            ```python
+            with nd2.ND2File("path/to/file.nd2") as nd2_file:
+                ...
+            ```
+
+            This will automatically close the file when the context exits.
+        """
         if not self.closed:
             self._rdr.close()
             self._closed = True
 
     @property
     def closed(self) -> bool:
-        """Whether the file is closed."""
+        """Return `True` if the file is closed."""
         return self._closed
 
     def __enter__(self) -> ND2File:
         """Open file for reading."""
         self.open()
         return self
 
@@ -170,41 +225,138 @@
         self._lock = threading.RLock()
         self._rdr = _util.get_reader(self._path)
         if self._closed:
             self._rdr.close()
 
     @cached_property
     def attributes(self) -> Attributes:
-        """Core image attributes."""
+        """Core image attributes.
+
+        !!! example "Example Output"
+
+            ```python
+            Attributes(
+                bitsPerComponentInMemory=16,
+                bitsPerComponentSignificant=16,
+                componentCount=2,
+                heightPx=32,
+                pixelDataType='unsigned',
+                sequenceCount=60,
+                widthBytes=128,
+                widthPx=32,
+                compressionLevel=None,
+                compressionType=None,
+                tileHeightPx=None,
+                tileWidthPx=None,
+                channelCount=2
+            )
+            ```
+
+
+        Returns
+        -------
+        attrs : Attributes
+            Core image attributes
+        """
         return self._rdr.attributes
 
     @cached_property
     def text_info(self) -> TextInfo | dict:
-        """Misc text info."""
+        r"""Miscellaneous text info.
+
+        ??? example "Example Output"
+
+            ```python
+            {
+                'description': 'Metadata:\r\nDimensions: T(3) x XY(4) x λ(2) x Z(5)...'
+                'capturing': 'Flash4.0, SN:101412\r\nSample 1:\r\n  Exposure: 100 ms...'
+                'date': '9/28/2021  9:41:27 AM',
+                'optics': 'Plan Fluor 10x Ph1 DLL'
+            }
+            ```
+
+        Returns
+        -------
+        TextInfo | dict
+            If the file is a legacy nd2 file, a dict is returned. Otherwise, a
+            `TextInfo` object is returned.
+        """
         return self._rdr.text_info()
 
     @cached_property
     def rois(self) -> dict[int, ROI]:
-        """Return dict of {id: ROI} for all ROIs found in the metadata."""
+        """Return dict of `{id: ROI}` for all ROIs found in the metadata.
+
+        Returns
+        -------
+        dict[int, ROI]
+            The dict of ROIs is keyed by the ROI ID.
+        """
         key = b"CustomData|RoiMetadata_v1!"
         if self.is_legacy or key not in self._rdr.chunkmap:  # type: ignore
             return {}  # pragma: no cover
 
         data = cast("LatestSDKReader", self._rdr)._decode_chunk(key)
         data = data.get("RoiMetadata_v1", {}).copy()
-        data.pop("Global_Size", None)
+        dicts: list[dict] = []
+        if "Global_Size" in data:
+            dicts.extend(data[f"Global_{i}"] for i in range(data["Global_Size"]))
+        if "2PerMPoint_Size" in data:
+            for i in range(data.get("2PerMPoint_Size", 0)):
+                item: dict = data[f"2PerMPoint_{i}"]
+                dicts.extend(item[str(idx)] for idx in range(item.get("Size", 0)))
+
         try:
-            _rois = [ROI._from_meta_dict(d) for d in data.values()]
+            _rois = [ROI._from_meta_dict(d) for d in dicts]
         except Exception as e:  # pragma: no cover
+            return {}
             raise ValueError(f"Could not parse ROI metadata: {e}") from e
         return {r.id: r for r in _rois}
 
     @cached_property
     def experiment(self) -> list[ExpLoop]:
-        """Loop information for each nd axis."""
+        """Loop information for each axis of an nD acquisition.
+
+        ??? example "Example Output"
+
+            ```python
+            [
+                TimeLoop(
+                    count=3,
+                    nestingLevel=0,
+                    parameters=TimeLoopParams(
+                        startMs=0.0,
+                        periodMs=1.0,
+                        durationMs=0.0,
+                        periodDiff=PeriodDiff(
+                            avg=3674.199951171875,
+                            max=3701.219970703125,
+                            min=3647.179931640625
+                        )
+                    ),
+                    type='TimeLoop'
+                ),
+                ZStackLoop(
+                    count=5,
+                    nestingLevel=1,
+                    parameters=ZStackLoopParams(
+                        homeIndex=2,
+                        stepUm=1.0,
+                        bottomToTop=True,
+                        deviceName='Ti2 ZDrive'
+                    ),
+                    type='ZStackLoop'
+                )
+            ]
+            ```
+
+        Returns
+        -------
+        list[ExpLoop]
+        """
         return self._rdr.experiment()
 
     @overload
     def events(
         self, *, orient: Literal["records"] = ..., null_value: Any = ...
     ) -> ListOfDicts:
         ...
@@ -246,14 +398,20 @@
         orient : {'records', 'dict', 'list'}, default 'records'
             The format of the returned data. See `pandas.DataFrame
                 - 'records' : list of dict - `[{column -> value}, ...]` (default)
                 - 'dict' :    dict of dict - `{column -> {index -> value}, ...}`
                 - 'list' :    dict of list - `{column -> [value, ...]}`
         null_value : Any, default float('nan')
             The value to use for missing data.
+
+
+        Returns
+        -------
+        ListOfDicts | DictOfLists | DictOfDicts
+            Tabular data in the format specified by `orient`.
         """
         if orient not in ("records", "dict", "list"):  # pragma: no cover
             raise ValueError("orient must be one of 'records', 'dict', or 'list'")
 
         if self.is_legacy:  # pragma: no cover
             warnings.warn(
                 "`recorded_data` is not implemented for legacy ND2 files",
@@ -308,25 +466,25 @@
 
         Parameters
         ----------
         strip_prefix : bool, optional
             Whether to strip the type information from the front of the keys in the
             dict. For example, if `True`: `uiModeFQ` becomes `ModeFQ` and `bUsePFS`
             becomes `UsePFS`, etc... by default `True`
-        include : Optional[Set[str]], optional
+        include : set[str] | None, optional
             If provided, only include the specified keys in the output. by default,
             all metadata sections found in the file are included.
-        exclude : Optional[Set[str]], optional
+        exclude : set[str] | None, optional
             If provided, exclude the specified keys from the output. by default `None`
         unnest : bool, optional
-            DEPRECATED.  No longer does anything.
+            :warning: **DEPRECATED**.  No longer does anything.
 
         Returns
         -------
-        Dict[str, Any]
+        dict[str, Any]
             A dict of the unstructured metadata, with keys that are the type of the
             metadata chunk (things like 'CustomData|RoiMetadata_v1' or
             'ImageMetadataLV'), and values that are associated metadata chunk.
         """
         if self.is_legacy:  # pragma: no cover
             raise NotImplementedError(
                 "unstructured_metadata not available for legacy files"
@@ -364,31 +522,277 @@
                 output[key] = rdr._decode_chunk(name, strip_prefix=strip_prefix)
             except Exception:  # pragma: no cover
                 output[key] = rdr._load_chunk(name)
         return output
 
     @cached_property
     def metadata(self) -> Metadata | dict:
-        """Various metadata (will be dict if legacy format)."""
+        """Various metadata (will be `dict` only if legacy format).
+
+        ??? example "Example output"
+
+            ```python
+            Metadata(
+                contents=Contents(channelCount=2, frameCount=15),
+                channels=[
+                    Channel(
+                        channel=ChannelMeta(
+                            name='Widefield Green',
+                            index=0,
+                            colorRGB=65371,
+                            emissionLambdaNm=535.0,
+                            excitationLambdaNm=None
+                        ),
+                        loops=LoopIndices(
+                            NETimeLoop=None,
+                            TimeLoop=0,
+                            XYPosLoop=None,
+                            ZStackLoop=1
+                        ),
+                        microscope=Microscope(
+                            objectiveMagnification=10.0,
+                            objectiveName='Plan Fluor 10x Ph1 DLL',
+                            objectiveNumericalAperture=0.3,
+                            zoomMagnification=1.0,
+                            immersionRefractiveIndex=1.0,
+                            projectiveMagnification=None,
+                            pinholeDiameterUm=None,
+                            modalityFlags=['fluorescence']
+                        ),
+                        volume=Volume(
+                            axesCalibrated=[True, True, True],
+                            axesCalibration=[
+                                0.652452890023035,
+                                0.652452890023035,
+                                1.0
+                            ],
+                            axesInterpretation=['distance', 'distance', 'distance'],
+                            bitsPerComponentInMemory=16,
+                            bitsPerComponentSignificant=16,
+                            cameraTransformationMatrix=[
+                                -0.9998932296054086,
+                                -0.014612644841559427,
+                                0.014612644841559427,
+                                -0.9998932296054086
+                            ],
+                            componentCount=1,
+                            componentDataType='unsigned',
+                            voxelCount=[32, 32, 5],
+                            componentMaxima=[0.0],
+                            componentMinima=[0.0],
+                            pixelToStageTransformationMatrix=None
+                        )
+                    ),
+                    Channel(
+                        channel=ChannelMeta(
+                            name='Widefield Red',
+                            index=1,
+                            colorRGB=22015,
+                            emissionLambdaNm=620.0,
+                            excitationLambdaNm=None
+                        ),
+                        loops=LoopIndices(
+                            NETimeLoop=None,
+                            TimeLoop=0,
+                            XYPosLoop=None,
+                            ZStackLoop=1
+                        ),
+                        microscope=Microscope(
+                            objectiveMagnification=10.0,
+                            objectiveName='Plan Fluor 10x Ph1 DLL',
+                            objectiveNumericalAperture=0.3,
+                            zoomMagnification=1.0,
+                            immersionRefractiveIndex=1.0,
+                            projectiveMagnification=None,
+                            pinholeDiameterUm=None,
+                            modalityFlags=['fluorescence']
+                        ),
+                        volume=Volume(
+                            axesCalibrated=[True, True, True],
+                            axesCalibration=[
+                                0.652452890023035,
+                                0.652452890023035,
+                                1.0
+                            ],
+                            axesInterpretation=['distance', 'distance', 'distance'],
+                            bitsPerComponentInMemory=16,
+                            bitsPerComponentSignificant=16,
+                            cameraTransformationMatrix=[
+                                -0.9998932296054086,
+                                -0.014612644841559427,
+                                0.014612644841559427,
+                                -0.9998932296054086
+                            ],
+                            componentCount=1,
+                            componentDataType='unsigned',
+                            voxelCount=[32, 32, 5],
+                            componentMaxima=[0.0],
+                            componentMinima=[0.0],
+                            pixelToStageTransformationMatrix=None
+                        )
+                    )
+                ]
+            )
+            ```
+
+        Returns
+        -------
+        Metadata | dict
+            dict if legacy format, else `Metadata`
+        """
         return self._rdr.metadata()
 
     def frame_metadata(self, seq_index: int | tuple) -> FrameMetadata | dict:
         """Metadata for specific frame.
 
+        :eyes: **See also:** [metadata][nd2.ND2File.metadata]
+
         This includes the global metadata from the metadata function.
         (will be dict if legacy format).
 
+        ??? example "Example output"
+
+            ```python
+            FrameMetadata(
+                contents=Contents(channelCount=2, frameCount=15),
+                channels=[
+                    FrameChannel(
+                        channel=ChannelMeta(
+                            name='Widefield Green',
+                            index=0,
+                            colorRGB=65371,
+                            emissionLambdaNm=535.0,
+                            excitationLambdaNm=None
+                        ),
+                        loops=LoopIndices(
+                            NETimeLoop=None,
+                            TimeLoop=0,
+                            XYPosLoop=None,
+                            ZStackLoop=1
+                        ),
+                        microscope=Microscope(
+                            objectiveMagnification=10.0,
+                            objectiveName='Plan Fluor 10x Ph1 DLL',
+                            objectiveNumericalAperture=0.3,
+                            zoomMagnification=1.0,
+                            immersionRefractiveIndex=1.0,
+                            projectiveMagnification=None,
+                            pinholeDiameterUm=None,
+                            modalityFlags=['fluorescence']
+                        ),
+                        volume=Volume(
+                            axesCalibrated=[True, True, True],
+                            axesCalibration=[
+                                0.652452890023035,
+                                0.652452890023035,
+                                1.0
+                            ],
+                            axesInterpretation=['distance', 'distance', 'distance'],
+                            bitsPerComponentInMemory=16,
+                            bitsPerComponentSignificant=16,
+                            cameraTransformationMatrix=[
+                                -0.9998932296054086,
+                                -0.014612644841559427,
+                                0.014612644841559427,
+                                -0.9998932296054086
+                            ],
+                            componentCount=1,
+                            componentDataType='unsigned',
+                            voxelCount=[32, 32, 5],
+                            componentMaxima=[0.0],
+                            componentMinima=[0.0],
+                            pixelToStageTransformationMatrix=None
+                        ),
+                        position=Position(
+                            stagePositionUm=StagePosition(
+                                x=26950.2,
+                                y=-1801.6000000000001,
+                                z=494.3
+                            ),
+                            pfsOffset=None,
+                            name=None
+                        ),
+                        time=TimeStamp(
+                            absoluteJulianDayNumber=2459486.0682717753,
+                            relativeTimeMs=580.3582921028137
+                        )
+                    ),
+                    FrameChannel(
+                        channel=ChannelMeta(
+                            name='Widefield Red',
+                            index=1,
+                            colorRGB=22015,
+                            emissionLambdaNm=620.0,
+                            excitationLambdaNm=None
+                        ),
+                        loops=LoopIndices(
+                            NETimeLoop=None,
+                            TimeLoop=0,
+                            XYPosLoop=None,
+                            ZStackLoop=1
+                        ),
+                        microscope=Microscope(
+                            objectiveMagnification=10.0,
+                            objectiveName='Plan Fluor 10x Ph1 DLL',
+                            objectiveNumericalAperture=0.3,
+                            zoomMagnification=1.0,
+                            immersionRefractiveIndex=1.0,
+                            projectiveMagnification=None,
+                            pinholeDiameterUm=None,
+                            modalityFlags=['fluorescence']
+                        ),
+                        volume=Volume(
+                            axesCalibrated=[True, True, True],
+                            axesCalibration=[
+                                0.652452890023035,
+                                0.652452890023035,
+                                1.0
+                            ],
+                            axesInterpretation=['distance', 'distance', 'distance'],
+                            bitsPerComponentInMemory=16,
+                            bitsPerComponentSignificant=16,
+                            cameraTransformationMatrix=[
+                                -0.9998932296054086,
+                                -0.014612644841559427,
+                                0.014612644841559427,
+                                -0.9998932296054086
+                            ],
+                            componentCount=1,
+                            componentDataType='unsigned',
+                            voxelCount=[32, 32, 5],
+                            componentMaxima=[0.0],
+                            componentMinima=[0.0],
+                            pixelToStageTransformationMatrix=None
+                        ),
+                        position=Position(
+                            stagePositionUm=StagePosition(
+                                x=26950.2,
+                                y=-1801.6000000000001,
+                                z=494.3
+                            ),
+                            pfsOffset=None,
+                            name=None
+                        ),
+                        time=TimeStamp(
+                            absoluteJulianDayNumber=2459486.0682717753,
+                            relativeTimeMs=580.3582921028137
+                        )
+                    )
+                ]
+            )
+            ```
+
         Parameters
         ----------
         seq_index : Union[int, tuple]
             frame index
 
         Returns
         -------
-        Union[FrameMetadata, dict]
+        FrameMetadata | dict
             dict if legacy format, else FrameMetadata
         """
         idx = cast(
             int,
             self._seq_index_from_coords(seq_index)
             if isinstance(seq_index, tuple)
             else seq_index,
@@ -398,25 +802,42 @@
     @cached_property
     def custom_data(self) -> dict[str, Any]:
         """Dict of various unstructured custom metadata."""
         return self._rdr._custom_data()
 
     @cached_property
     def ndim(self) -> int:
-        """Number of dimensions."""
+        """Number of dimensions (i.e. `len(`[`self.shape`][nd2.ND2File.shape]`)`)."""
         return len(self.shape)
 
     @cached_property
     def shape(self) -> tuple[int, ...]:
-        """Size of each axis."""
+        """Size of each axis.
+
+        Examples
+        --------
+        >>> ndfile.shape
+        (3, 5, 2, 512, 512)
+        """
         return self._coord_shape + self._frame_shape
 
     @cached_property
     def sizes(self) -> dict[str, int]:
-        """Names and sizes for each axis."""
+        """Names and sizes for each axis.
+
+        This is an ordered dict, with the same order
+        as the corresponding [shape][nd2.ND2File.shape]
+
+        Examples
+        --------
+        >>> ndfile.sizes
+        {'T': 3, 'Z': 5, 'C': 2, 'Y': 512, 'X': 512}
+        >>> ndfile.shape
+        (3, 5, 2, 512, 512)
+        """
         attrs = self.attributes
         dims = {AXIS._MAP[c[1]]: c[2] for c in self._rdr._coord_info()}
         dims[AXIS.CHANNEL] = (
             dims.pop(AXIS.CHANNEL)
             if AXIS.CHANNEL in dims
             else (attrs.channelCount or 1)
         )
@@ -427,26 +848,26 @@
         else:
             # if not exactly 3 channels, throw them all into monochrome channels
             dims[AXIS.CHANNEL] = attrs.componentCount
         return {k: v for k, v in dims.items() if v != 1}
 
     @property
     def is_rgb(self) -> bool:
-        """Whether the image is rgb."""
+        """Whether the image is rgb (i.e. it has 3 or 4 components per channel)."""
         return self.components_per_channel in (3, 4)
 
     @property
     def components_per_channel(self) -> int:
         """Number of components per channel (e.g. 3 for rgb)."""
         attrs = self.attributes
         return attrs.componentCount // (attrs.channelCount or 1)
 
     @property
     def size(self) -> int:
-        """Total number of pixels in the volume."""
+        """Total number of voxels in the volume (the product of the shape)."""
         return int(np.prod(self.shape))
 
     @property
     def nbytes(self) -> int:
         """Total bytes of image data."""
         return self.size * self.dtype.itemsize
 
@@ -469,24 +890,26 @@
         -------
         VoxelSize
             Named tuple with attrs `x`, `y`, and `z`.
         """
         return _util.VoxelSize(*self._rdr.voxel_size())
 
     def asarray(self, position: int | None = None) -> np.ndarray:
-        """Read image into numpy array.
+        """Read image into a [numpy.ndarray][].
+
+        For a simple way to read a file into a numpy array, see [nd2.imread][].
 
         Parameters
         ----------
         position : int, optional
             A specific XY position to extract, by default (None) reads all.
 
         Returns
         -------
-        np.ndarray
+        array : np.ndarray
 
         Raises
         ------
         ValueError
             if `position` is a string and is not a valid position name
         IndexError
             if `position` is provided and is out of range
@@ -540,31 +963,31 @@
         will very likely cause segmentation faults in many cases.  But setting
         one of them to `False`, may slightly improve read speed in certain
         cases.
 
         Parameters
         ----------
         wrapper : bool
-            If True (the default), the returned obect will be a thin subclass of
-            a :class:`dask.array.Array` (an
-            `ResourceBackedDaskArray`) that manages the opening and closing of this file
-            when getting chunks via compute(). If `wrapper` is `False`, then a pure
-            `dask.array.core.Array` will be returned. However, when that array is
-            computed, it will incur a file open/close on *every* chunk that is read (in
-            the `_dask_block` method).  As such `wrapper` will generally be much faster,
-            however, it *may* fail (i.e. result in segmentation faults) with certain
-            dask schedulers.
+            If `True` (the default), the returned object will be a thin subclass of a
+            [`dask.array.Array`][] (a `ResourceBackedDaskArray`) that manages the
+            opening and closing of this file when getting chunks via compute(). If
+            `wrapper` is `False`, then a pure `dask.array.core.Array` will be returned.
+            However, when that array is computed, it will incur a file open/close on
+            *every* chunk that is read (in the `_dask_block` method).  As such `wrapper`
+            will generally be much faster, however, it *may* fail (i.e. result in
+            segmentation faults) with certain dask schedulers.
         copy : bool
             If `True` (the default), the dask chunk-reading function will return
             an array copy. This can avoid segfaults in certain cases, though it
             may also add overhead.
 
         Returns
         -------
-        dask.array.core.Array
+        dask_array: dask.array.Array
+            A dask array representing the image data.
         """
         from dask.array.core import map_blocks
 
         chunks = [(1,) * x for x in self._coord_shape]
         chunks += [(x,) for x in self._frame_shape]
         dask_arr = map_blocks(
             self._dask_block,
@@ -614,15 +1037,18 @@
     def to_xarray(
         self,
         delayed: bool = True,
         squeeze: bool = True,
         position: int | None = None,
         copy: bool = True,
     ) -> xr.DataArray:
-        """Create labeled xarray representing image.
+        """Return a labeled [xarray.DataArray][] representing image.
+
+        Xarrays are a powerful way to label and manipulate n-dimensional data with
+        axis-associated coordinates.
 
         `array.dims` will be populated according to image metadata, and coordinates
         will be populated based on pixel spacings. Additional metadata is available
         in `array.attrs['metadata']`.
 
         Parameters
         ----------
@@ -777,27 +1203,23 @@
             details = " (closed)" if self.closed else f" {self.dtype}: {self.sizes!r}"
             extra = f": {Path(self.path).name!r}{details}"
         except Exception:
             extra = ""
         return f"<ND2File at {hex(id(self))}{extra}>"
 
     @property
-    def recorded_data(
-        self,
-    ) -> DictOfLists:
+    def recorded_data(self) -> DictOfLists:
         """Return tabular data recorded for each frame of the experiment.
 
-        This method returns a dict of equal-length sequences (passable to
-        pd.DataFrame()). It matches the tabular data reported in the Image Properties >
-        Recorded Data tab of the NIS Viewer.
+        !!! warning "Deprecated"
 
-        (There will be a column for each tag in the `CustomDataV2_0` section of
-        `ND2File.custom_data`)
-
-        Legacy ND2 files are not supported.
+            This method is deprecated and will be removed in a future version.
+            Please use the [`events`][nd2.ND2File.events] method instead. To get the
+            same dict-of-lists output that `recorded_data` returns, use
+            `ndfile.events(orient='list')`
         """
         warnings.warn(
             "recorded_data is deprecated and will be removed in a future version."
             "Please use the `events` method instead. To get the same dict-of-lists "
             "output, use `events(orient='list')`",
             FutureWarning,
             stacklevel=2,
@@ -839,46 +1261,52 @@
         >>> np.asarray(f.binary_data).shape  # cast all layers to array
         (4, 3, 4, 5, 32, 32)
         """
         from ._binary import BinaryLayers
 
         return BinaryLayers.from_nd2file(self)
 
+    def ome_metadata(self) -> OME:
+        """Return OME metadata for the file."""
+        from ._ome import nd2_ome_metadata
+
+        return nd2_ome_metadata(self)
+
 
 @overload
 def imread(
     file: Path | str,
     *,
-    dask: Literal[False],
-    xarray: Literal[False],
-    validate_frames: bool = False,
+    dask: Literal[False] = ...,
+    xarray: Literal[False] = ...,
+    validate_frames: bool = ...,
     read_using_sdk: bool | None = None,
 ) -> np.ndarray:
     ...
 
 
 @overload
 def imread(
     file: Path | str,
     *,
     dask: bool = ...,
     xarray: Literal[True],
-    validate_frames: bool = False,
+    validate_frames: bool = ...,
     read_using_sdk: bool | None = None,
 ) -> xr.DataArray:
     ...
 
 
 @overload
 def imread(
     file: Path | str,
     *,
     dask: Literal[True],
-    xarray: Literal[False],
-    validate_frames: bool = False,
+    xarray: Literal[False] = ...,
+    validate_frames: bool = ...,
     read_using_sdk: bool | None = None,
 ) -> dask.array.core.Array:
     ...
 
 
 def imread(
     file: Path | str,
@@ -888,15 +1316,15 @@
     validate_frames: bool = False,
     read_using_sdk: bool | None = None,
 ) -> np.ndarray | xr.DataArray | dask.array.core.Array:
     """Open `file`, return requested array type, and close `file`.
 
     Parameters
     ----------
-    file : Union[Path, str]
+    file : Path | str
         Filepath (`str`) or `Path` object to ND2 file.
     dask : bool
         If `True`, returns a (delayed) `dask.array.Array`. This will avoid reading
         any data from disk until specifically requested by using `.compute()` or
         casting to a numpy array with `np.asarray()`. By default `False`.
     xarray : bool
         If `True`, returns an `xarray.DataArray`, `array.dims` will be populated
@@ -906,15 +1334,16 @@
         By default `False`.
     validate_frames : bool
         Whether to verify (and attempt to fix) frames whose positions have been
         shifted relative to the predicted offset (i.e. in a corrupted file).
         This comes at a slight performance penalty at file open, but may "rescue"
         some corrupt files. by default False.
     read_using_sdk : Optional[bool]
-        DEPRECATED: no longer used.
+        :warning: **DEPRECATED**.  No longer used.
+
         If `True`, use the SDK to read the file. If `False`, inspects the chunkmap and
         reads from a `numpy.memmap`. If `None` (the default), uses the SDK if the file
         is compressed, otherwise uses the memmap.
         Note: using `read_using_sdk=False` on a compressed file will result in a
         ValueError.
 
     Returns
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nd2-0.6.1/src/nd2/structures.py` & `nd2-0.7.0/src/nd2/structures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import builtins
 from dataclasses import dataclass, field
 from enum import IntEnum
-from typing import NamedTuple, Union
+from typing import TYPE_CHECKING, NamedTuple, Union
 
-from typing_extensions import Literal, TypeAlias, TypedDict
+from typing_extensions import Literal, TypedDict
 
 from ._pysdk._sdk_types import EventMeaning, StimulationType
 
+if TYPE_CHECKING:
+    from ._pysdk._sdk_types import AxisInterpretation, LoopTypeString
+
 
 class TextInfo(TypedDict, total=False):
     imageId: str
     type: str
     group: str
     sampleId: str
     author: str
@@ -38,17 +41,14 @@
     SpectLoop = 6
     CustomLoop = 7
     NETimeLoop = 8
     ManTimeLoop = 9
     ZStackLoopAccurate = 10
 
 
-AxisInterpretation: TypeAlias = Literal["distance", "time"]
-
-
 # tuples
 
 
 class Attributes(NamedTuple):
     bitsPerComponentInMemory: int
     bitsPerComponentSignificant: int
     componentCount: int
@@ -69,28 +69,14 @@
     height: int
     components: int
     bits_per_pixel: int
 
 
 # experiment #################
 
-LoopTypeString = Literal[
-    "Unknown",
-    "TimeLoop",
-    "XYPosLoop",
-    "XYDiscrLoop",
-    "ZStackLoop",
-    "PolarLoop",
-    "SpectLoop",
-    "CustomLoop",
-    "NETimeLoop",
-    "ManTimeLoop",
-    "ZStackLoopAccurate",
-]
-
 
 @dataclass
 class _Loop:
     count: int
     nestingLevel: int
     parameters: LoopParams | None
     type: LoopTypeString
@@ -111,14 +97,16 @@
 
 
 #####
 
 
 @dataclass
 class TimeLoop(_Loop):
+    """The time dimension of an experiment."""
+
     parameters: TimeLoopParams
     type: Literal["TimeLoop"] = "TimeLoop"
 
     def __post_init__(self) -> None:
         # TODO: make superclass do this
         if isinstance(self.parameters, dict):
             if "periodDiff" not in self.parameters:
@@ -146,14 +134,16 @@
 
 
 ######
 
 
 @dataclass
 class NETimeLoop(_Loop):
+    """The time dimension of an nD experiment."""
+
     parameters: NETimeLoopParams
     type: Literal["NETimeLoop"] = "NETimeLoop"
 
     def __post_init__(self) -> None:
         if isinstance(self.parameters, dict):
             self.parameters = NETimeLoopParams(**self.parameters)
 
@@ -293,24 +283,56 @@
     NETimeLoop: int | None = None
     TimeLoop: int | None = None
     XYPosLoop: int | None = None
     ZStackLoop: int | None = None
     CustomLoop: int | None = field(default=None, repr=False, compare=False)
 
 
+ModalityFlags = Literal[
+    "aux",
+    "brightfield",
+    "camera",
+    "diContrast",
+    "dsdConfocal",
+    "fluorescence",
+    "gaasp",
+    "iSIM",
+    "laserScanConfocal",
+    "liveSR",
+    "multiphoton",
+    "nonDescannedDetector",
+    "phaseContrast",
+    "pmt",
+    "RCM",
+    "remainder",
+    "SIM",
+    "sora",
+    "spectral",
+    "spinningDiskConfocal",
+    "sweptFieldConfocalPinhole",
+    "sweptFieldConfocalSlit",
+    "TIRF",
+    "transmitDetector",
+    "vaasIF",
+    "vaasNF",
+    "VCS",
+    "virtualFilter",
+]
+
+
 @dataclass
 class Microscope:
     objectiveMagnification: float | None = None
     objectiveName: str | None = None
     objectiveNumericalAperture: float | None = None
     zoomMagnification: float | None = None
     immersionRefractiveIndex: float | None = None
     projectiveMagnification: float | None = None
     pinholeDiameterUm: float | None = None
-    modalityFlags: list[str] = field(default_factory=list)
+    modalityFlags: list[ModalityFlags] = field(default_factory=list)
 
 
 @dataclass
 class Volume:
     axesCalibrated: tuple[bool, bool, bool]
     axesCalibration: tuple[float, float, float]
     axesInterpretation: tuple[
@@ -389,15 +411,15 @@
     x: float = 0
     y: float = 0
     z: float = 0
 
 
 class ExtrudedShape(NamedTuple):
     sizeZ: float = 0
-    basePoints: list[XYPoint] = []
+    basePoints: list[XYPoint] = field(default_factory=list)
 
     @classmethod
     def _from_meta_dict(cls, val: dict) -> ExtrudedShape:
         return cls(
             sizeZ=val.get("SizeZ") or val.get("sizeZ") or 0,
             basePoints=[
                 XYPoint(*val[f"BasePoints_{i}"].get("", []))
@@ -414,30 +436,56 @@
     info: RoiInfo
     guid: str
     animParams: list[AnimParam] = field(default_factory=list)
 
     def __post_init__(self) -> None:
         if isinstance(self.info, dict):
             self.info = RoiInfo(**self.info)
-        self.animParams = [AnimParam(**i) for i in self.animParams]  # type: ignore
+        self.animParams = [
+            AnimParam(**i) if isinstance(i, dict) else i for i in self.animParams
+        ]
 
     @classmethod
     def _from_meta_dict(cls, val: dict) -> ROI:
+        # val has keys:
+        # 'Id', 'Info', 'GUID', 'AnimParams_Size', 'AnimParams_{i}'
+        # where GUID and AnimParams keys are optional
         anim_params = [
-            {_lower0(k): v for k, v in val[f"AnimParams_{i}"].items()}
-            for i in range(val.pop("AnimParams_Size", 0))
+            AnimParam(
+                **{
+                    _lower0(k): v
+                    for k, v in val[f"AnimParams_{i}"].items()
+                    if _lower0(k) in AnimParam.__annotations__
+                }
+            )
+            for i in range(val.get("AnimParams_Size", 0))
         ]
+        info = RoiInfo(
+            **{
+                _lower0(k): v
+                for k, v in val["Info"].items()
+                if _lower0(k) in RoiInfo.__annotations__
+            }
+        )
         return cls(
             id=val["Id"],
-            info={_lower0(k): v for k, v in val["Info"].items()},  # type: ignore
+            info=info,
             guid=val.get("GUID", ""),
-            animParams=anim_params,  # type: ignore
+            animParams=anim_params,
         )
 
 
+class T(TypedDict):
+    Id: int
+    Info: dict
+    GUID: str
+    AnimParams_Size: int
+    # AnimParams_{i}: dict
+
+
 @dataclass
 class AnimParam:
     """Parameters of ROI position/shape."""
 
     timeMs: float = 0
     enabled: bool = True
     centerX: float = 0
@@ -446,15 +494,19 @@
     rotationZ: float = 0
     boxShape: BoxShape = field(default_factory=BoxShape)
     extrudedShape: ExtrudedShape = field(default_factory=ExtrudedShape)
 
     def __post_init__(self) -> None:
         if isinstance(self.boxShape, dict):
             self.boxShape = BoxShape(
-                **{_lower0(k): v for k, v in self.boxShape.items()}
+                **{
+                    _lower0(k): v
+                    for k, v in self.boxShape.items()
+                    if _lower0(k) in BoxShape.__annotations__
+                }
             )
         if isinstance(self.extrudedShape, dict):
             self.extrudedShape = ExtrudedShape._from_meta_dict(self.extrudedShape)
 
     @property
     def center(self) -> XYZPoint:
         """Center point as a named tuple (x, y, z)."""
```

### Comparing `nd2-0.6.1/src/nd2/_legacy/_legacy.py` & `nd2-0.7.0/src/nd2/_legacy/_legacy.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/src/nd2/_legacy/_legacy_xml.py` & `nd2-0.7.0/src/nd2/_legacy/_legacy_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             return type_(node.attrib["value"])
         except ValueError:
             return node.attrib["value"]
 
     attrs = node.attrib
     attrs.pop("runtype", "")
     attrs.pop("version", "")
-    result.update(node.attrib)  # type: ignore
+    result.update(node.attrib)
 
     # [<Element CustomTagDescription_v1.0 at 0x12a29ac40>]
     for element in node:
         # Remove namespace prefix
         key = element.tag.split("}")[1] if "}" in element.tag else element.tag
         key = lower.sub("", key) or key
```

### Comparing `nd2-0.6.1/src/nd2/_pysdk/_chunk_decode.py` & `nd2-0.7.0/src/nd2/_pysdk/_chunk_decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,15 @@
     channels as well as RGB components).  Frames are laid out as (Y, X, C),
     and the `frame_shape` should match the expected frame size.  If
     `frame_shape` is not provided, a guess will be made about the vector shape
     of each frame, but it may be incorrect.
 
     Parameters
     ----------
-    handle : Union[BinaryIO,str]
+    handle : BinaryIO | str
         Filepath string, or binary file handle (For example
         `handle = open('some.nd2', 'rb')`)
     frame_shape : Tuple[int, ...], optional
         expected shape of each frame, by default a 1 dimensional array will
         be yielded for each frame, which can be reshaped later if desired.
         NOTE: nd2 frames are generally ordered as
         (height, width, true_channels, rgbcomponents).
```

### Comparing `nd2-0.6.1/src/nd2/_pysdk/_parse.py` & `nd2-0.7.0/src/nd2/_pysdk/_parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 from nd2 import structures as strct
 
 from ._sdk_types import ELxModalityMask, EventMeaning, StimulationType
 
 if TYPE_CHECKING:
     from typing_extensions import TypeGuard
 
-    from nd2.structures import AxisInterpretation, ExpLoop, XYPosLoopParams
+    from nd2.structures import ExpLoop, XYPosLoopParams
 
     from ._sdk_types import (
+        AxisInterpretation,
         CompressionType,
         FilterDict,
         FluorescentProbeDict,
         GlobalMetadata,
+        LoopTypeString,
         NETimeLoopPars,
         PicturePlanesDict,
         PlaneDict,
         RawAttributesDict,
         RawExperimentDict,
         RawExperimentRecordDict,
         RawLiteEventDict,
@@ -461,87 +463,83 @@
 
 def load_global_metadata(
     attrs: strct.Attributes,
     raw_meta: RawMetaDict,
     exp_loops: list[ExpLoop],
     text_info: strct.TextInfo,
 ) -> GlobalMetadata:
-    axesInterpretation: list[AxisInterpretation] = ["distance", "distance", "distance"]
-    axesCalibrated: list[bool] = [False, False, False]
-    axesCalibration: list[float] = [1.0, 1.0, 1.0]
-    if raw_meta.get("ePictureXAxis") == 2:
-        axesInterpretation[0] = "time"
-    if raw_meta.get("ePictureYAxis") == 2:
-        axesInterpretation[1] = "time"
-    axesCalibrated[:2] = [raw_meta["bCalibrated"]] * 2
-    axesCalibration[:2] = [raw_meta["dCalibration"]] * 2
+    axesCalibrated: tuple[bool, bool, bool] = (raw_meta["bCalibrated"],) * 2 + (False,)
+    axesCalibration: list[float] = [raw_meta["dCalibration"]] * 2 + [1.0]
+    axInterp: tuple[AxisInterpretation, AxisInterpretation, AxisInterpretation] = (
+        "time" if raw_meta.get("ePictureXAxis") == 2 else "distance",
+        "time" if raw_meta.get("ePictureYAxis") == 2 else "distance",
+        "distance",
+    )
 
     voxel_count: list[int] = [attrs.widthPx or 0, attrs.heightPx or 0, 1]
-    loops: dict[str, int] = {}
+    loops: dict[LoopTypeString, int] = {}
     for i, loop in enumerate(exp_loops):
-        loops[str(loop.type)] = i
+        loops[loop.type] = i
         if loop.type == "ZStackLoop":
             voxel_count[2] = loop.count
             axesCalibration[2] = abs(loop.parameters.stepUm)
-            axesCalibrated[2] = bool(axesCalibration[2] > 0)
+            axesCalibrated = axesCalibrated[:2] + (bool(axesCalibration[2] > 0),)
 
     dtype = "float" if attrs.bitsPerComponentSignificant == 32 else "unsigned"
-    volume = {
-        "axesCalibrated": axesCalibrated,
-        "axesCalibration": [i if i > 0 else 1.0 for i in axesCalibration],
-        "axesInterpretation": axesInterpretation,
-        "bitsPerComponentInMemory": attrs.bitsPerComponentInMemory,
-        "bitsPerComponentSignificant": attrs.bitsPerComponentSignificant,
-        "cameraTransformationMatrix": [
-            raw_meta.get("dStgLgCT11", 1.0),
-            raw_meta.get("dStgLgCT12", 0.0),
-            raw_meta.get("dStgLgCT21", 0.0),
-            raw_meta.get("dStgLgCT22", 1.0),
-        ],
-        "componentDataType": dtype,
-        "voxelCount": voxel_count,
-    }
     mag = raw_meta.get("dObjectiveMag", 0.0)
     if mag <= 0 and "optics" in text_info:
         match = re.search(r"\s?(\d+)?x", text_info["optics"], re.IGNORECASE)
         if match:
             mag = float(match[1])
     projectiveMagnification = raw_meta.get("dProjectiveMag")
     if projectiveMagnification and projectiveMagnification < 0:
         projectiveMagnification = None
     pinhole = raw_meta.get("dPinholeRadius", 0) * 2
     na = raw_meta.get("dObjectiveNA", -1)
     zoom = raw_meta.get("dZoom", -1)
     imm = raw_meta.get("dRefractIndex1") or raw_meta.get("dRefractIndex2")
-    microscope = {
-        "objectiveMagnification": mag if mag > 0 else None,
-        "objectiveName": raw_meta.get("wsObjectiveName") or None,
-        "objectiveNumericalAperture": na if na > 0 else None,
-        "projectiveMagnification": projectiveMagnification,
-        "zoomMagnification": zoom if zoom > 0 else None,
-        "immersionRefractiveIndex": imm if imm and imm > 0 else None,
-        "pinholeDiameterUm": pinhole if pinhole > 0 else None,
-    }
 
     return {
         "contents": {"frameCount": attrs.sequenceCount},
         "loops": loops,
-        "microscope": microscope,
+        "microscope": {
+            "objectiveMagnification": mag if mag > 0 else None,
+            "objectiveName": raw_meta.get("wsObjectiveName") or None,
+            "objectiveNumericalAperture": na if na > 0 else None,
+            "projectiveMagnification": projectiveMagnification,
+            "zoomMagnification": zoom if zoom > 0 else None,
+            "immersionRefractiveIndex": imm if imm and imm > 0 else None,
+            "pinholeDiameterUm": pinhole if pinhole > 0 else None,
+        },
         "position": {
-            "stagePositionUm": [
+            "stagePositionUm": (
                 raw_meta.get("dXPos", 0.0),
                 raw_meta.get("dYPos", 0.0),
                 raw_meta.get("dZPos", 0.0),
-            ]
+            )
         },
         "time": {
             "relativeTimeMs": raw_meta.get("dTimeMSec", 0.0),
             "absoluteJulianDayNumber": raw_meta.get("dTimeAbsolute", 0.0),
         },
-        "volume": volume,
+        "volume": {
+            "axesCalibrated": axesCalibrated,
+            "axesCalibration": tuple(i if i > 0 else 1.0 for i in axesCalibration),  # type: ignore  # noqa: E501
+            "axesInterpretation": axInterp,
+            "bitsPerComponentInMemory": attrs.bitsPerComponentInMemory,
+            "bitsPerComponentSignificant": attrs.bitsPerComponentSignificant,
+            "cameraTransformationMatrix": (
+                raw_meta.get("dStgLgCT11", 1.0),
+                raw_meta.get("dStgLgCT12", 0.0),
+                raw_meta.get("dStgLgCT21", 0.0),
+                raw_meta.get("dStgLgCT22", 1.0),
+            ),
+            "componentDataType": dtype,  # type: ignore
+            "voxelCount": tuple(voxel_count),  # type: ignore
+        },
     }
 
 
 def load_metadata(raw_meta: RawMetaDict, global_meta: GlobalMetadata) -> strct.Metadata:
     pplanes: PicturePlanesDict = raw_meta.get("sPicturePlanes", {})
     raw_planes = pplanes.get("sPlaneNew", None) or pplanes.get("sPlane", {})
     raw_sample_settings = pplanes.get("sSampleSetting", {})
@@ -572,15 +570,17 @@
         volume = global_meta["volume"].copy()
         microscope = global_meta["microscope"].copy()
         camera_matrix = volume.get("cameraTransformationMatrix")
         matrix = srcSampleSettings.get("matCameraToStage")
         if matrix and (matrix.get("Columns") == 2 and matrix.get("Rows") == 2):
             # matrix["Data"] is a list of int64, we need to recast to float
             data = bytearray(matrix["Data"])
-            matrix_data: list[float] = [i[0] for i in strctd.iter_unpack(data)]
+            matrix_data: tuple[float, float, float, float] = tuple(  # type: ignore
+                i[0] for i in strctd.iter_unpack(data)
+            )
             volume["cameraTransformationMatrix"] = matrix_data
 
         _pixel_to_stage = pixel_to_stage
         if camera_matrix:
             # XXX: Not sure if this is correct, specifically with regards to keeping
             # pixel_to_stage of previous channels, vs clearing it for each channel.
             m11, m12, m21, m22 = camera_matrix
@@ -604,27 +604,40 @@
                             invY * calY * m22,
                             -0.5
                             * (invY * calX * m21 * width + invY * calY * m22 * height),
                         ]
                         if _pixel_to_stage is not None:
                             pixel_to_stage = _pixel_to_stage
 
-        volume["pixelToStageTransformationMatrix"] = _pixel_to_stage
         if plane.get("dPinholeDiameter", -1) > 0:
             microscope["pinholeDiameterUm"] = plane["dPinholeDiameter"]
 
-        loops = (
-            strct.LoopIndices(**global_meta["loops"]) if global_meta["loops"] else None
-        )
+        glb_loops = global_meta["loops"]
+        if glb_loops:
+            loops = strct.LoopIndices(
+                NETimeLoop=glb_loops.get("NETimeLoop"),
+                TimeLoop=glb_loops.get("TimeLoop"),
+                XYPosLoop=glb_loops.get("XYPosLoop"),
+                ZStackLoop=glb_loops.get("ZStackLoop"),
+                CustomLoop=glb_loops.get("CustomLoop"),
+            )
+        else:
+            loops = None
+
         channel = strct.Channel(
             channel=channel_meta,
             loops=loops,
-            microscope=strct.Microscope(**microscope, modalityFlags=flags),
+            microscope=strct.Microscope(
+                **microscope, modalityFlags=flags  # type: ignore
+            ),
             volume=strct.Volume(
                 **volume,
+                pixelToStageTransformationMatrix=(
+                    None if _pixel_to_stage is None else tuple(_pixel_to_stage)  # type: ignore  # noqa
+                ),
                 componentCount=compCount,
                 componentMinima=[0.0] * compCount,  # FIXME
                 componentMaxima=[0.0] * compCount,  # FIXME
             ),
         )
         channels.append(channel)
 
@@ -633,24 +646,24 @@
 
 
 def load_frame_metadata(
     global_meta: GlobalMetadata,
     meta: strct.Metadata,
     exp_loops: list[ExpLoop],
     frame_time: float,
-    seq_index: int,
+    loop_indices: tuple[int, ...],
 ) -> strct.FrameMetadata:
     xy_loop_idx = global_meta["loops"].get("XYPosLoop", -1)
     z_loop_idx = global_meta["loops"].get("ZStackLoop", -1)
     if 0 <= xy_loop_idx < len(exp_loops):
-        params = cast("XYPosLoopParams", exp_loops[xy_loop_idx].parameters)
-        point = params.points[seq_index]
+        xy_params = cast("XYPosLoopParams", exp_loops[xy_loop_idx].parameters)
+        point = xy_params.points[loop_indices[xy_loop_idx]]
         name = point.name
         x, y, z = point.stagePositionUm
-        if not params.isSettingZ:
+        if not xy_params.isSettingZ:
             z = global_meta["position"]["stagePositionUm"][2]
     else:
         name = None
         x, y, z = global_meta["position"]["stagePositionUm"]
 
     if np.isfinite(frame_time):
         julian_day = global_meta["time"].get("absoluteJulianDayNumber", 0)
```

### Comparing `nd2-0.6.1/src/nd2/_pysdk/_pysdk.py` & `nd2-0.7.0/src/nd2/_pysdk/_pysdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import mmap
 import os
 import warnings
+from itertools import product
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, Sequence, cast
 
 import numpy as np
 
 from nd2 import structures
 from nd2._clx_lite import json_from_clx_lite_variant
@@ -127,15 +128,15 @@
     def attributes(self) -> structures.Attributes:
         """Load and return the image attributes."""
         if self._attributes is None:
             k = b"ImageAttributesLV!" if self.version >= (3, 0) else b"ImageAttributes!"
             attrs = self._decode_chunk(k, strip_prefix=False)
             attrs = attrs.get("SLxImageAttributes", attrs)  # for v3 only
             self._raw_attributes = cast("RawAttributesDict", attrs)
-            raw_meta = self._get_raw_image_metadata()  # ugly
+            raw_meta = self._cached_raw_metadata()  # ugly
             n_channels = raw_meta.get("sPicturePlanes", {}).get("uiCount", 1)
             self._attributes = load_attributes(self._raw_attributes, n_channels)
         return self._attributes
 
     def _load_chunk(self, name: bytes) -> bytes:
         """Load raw bytes from a specific chunk in the chunkmap.
 
@@ -168,16 +169,14 @@
             If True, strip the lowercase "type" prefix from the tag names, by default
             False.
         """
         if name not in self._cached_decoded_chunks:
             data = self._load_chunk(name)
             if data.startswith(b"<"):
                 decoded: Any = json_from_clx_variant(data, strip_prefix=strip_prefix)
-            elif self.version < (3, 0):
-                decoded = json_from_clx_variant(data, strip_prefix=strip_prefix)
             else:
                 decoded = json_from_clx_lite_variant(data, strip_prefix=strip_prefix)
             self._cached_decoded_chunks[name] = decoded
         return self._cached_decoded_chunks[name]
 
     @property
     def version(self) -> tuple[int, int]:
@@ -186,56 +185,54 @@
             try:
                 self._version = get_version(self._fh or self._path)
             except Exception:
                 self._version = (-1, -1)
                 raise
         return self._version
 
-    def _get_raw_image_metadata(self) -> RawMetaDict:
-        if not self._raw_image_metadata:
+    def _cached_raw_metadata(self) -> RawMetaDict:
+        if self._raw_image_metadata is None:
             k = (
                 b"ImageMetadataSeqLV|0!"
                 if self.version >= (3, 0)
                 else b"ImageMetadataSeq|0!"
             )
-            if k not in self.chunkmap:
-                self._raw_image_metadata = {}
-            else:
-                meta = self._decode_chunk(k, strip_prefix=False)
-                meta = meta.get("SLxPictureMetadata", meta)  # for v3 only
-                self._raw_image_metadata = cast("RawMetaDict", meta)
+            meta = self._decode_chunk(k, strip_prefix=False)
+            meta = meta.get("SLxPictureMetadata", meta)  # for v3 only
+            self._raw_image_metadata = cast("RawMetaDict", meta)
         return self._raw_image_metadata
 
     def _cached_global_metadata(self) -> GlobalMetadata:
         if not self._global_metadata:
             self._global_metadata = load_global_metadata(
                 attrs=self.attributes,
-                raw_meta=self._get_raw_image_metadata(),
+                raw_meta=self._cached_raw_metadata(),
                 exp_loops=self.experiment(),
                 text_info=self.text_info(),
             )
             if self._global_metadata["time"]["absoluteJulianDayNumber"] < 1:
                 julian_day = os.stat(self._path).st_ctime / 86400.0 + 2440587.5
                 self._global_metadata["time"]["absoluteJulianDayNumber"] = julian_day
 
         return self._global_metadata
 
     def metadata(self) -> structures.Metadata:
         if not self._metadata:
             self._metadata = load_metadata(
-                raw_meta=self._get_raw_image_metadata(),
+                raw_meta=self._cached_raw_metadata(),
                 global_meta=self._cached_global_metadata(),
             )
         return self._metadata
 
     def frame_metadata(self, seq_index: int) -> structures.FrameMetadata:
         frame_time = self._cached_frame_times()[seq_index]
         global_meta = self._cached_global_metadata()
+        loop_indices = self.loop_indices()[seq_index]
         return load_frame_metadata(
-            global_meta, self.metadata(), self.experiment(), frame_time, seq_index
+            global_meta, self.metadata(), self.experiment(), frame_time, loop_indices
         )
 
     def text_info(self) -> structures.TextInfo:
         if self._text_info is None:
             k = b"ImageTextInfoLV!" if self.version >= (3, 0) else b"ImageTextInfo!"
             if k not in self.chunkmap:
                 self._text_info = {}
@@ -254,14 +251,17 @@
             else:
                 exp = self._decode_chunk(k, strip_prefix=False)
                 exp = exp.get("SLxExperiment", exp)  # for v3 only
                 self._raw_experiment = cast("RawExperimentDict", exp)
                 self._experiment = load_experiment(0, self._raw_experiment)
         return self._experiment
 
+    def loop_indices(self) -> list[tuple[int, ...]]:
+        return list(product(*[range(x.count) for x in self.experiment()]))
+
     def _img_exp_events(self) -> list[structures.ExperimentEvent]:
         """Parse and return all Image and Experiment events."""
         if not self._events:
             events = []
             for key in (
                 b"ImageEvents",
                 b"ImageEventsLV!",
```

### Comparing `nd2-0.6.1/src/nd2/_pysdk/_sdk_types.py` & `nd2-0.7.0/src/nd2/_pysdk/_sdk_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         uiSequenceCount: int
         uiTileWidth: int
         uiTileHeight: int
         eCompression: int
         dCompressionParam: float
         uiVirtualComponents: int
 
-    class RawMetaDict(TypedDict, total=False):
+    class RawMetaDict(TypedDict):
         ePictureXAxis: int
         ePictureYAxis: int
         bCalibrated: bool
         dCalibration: float
         dStgLgCT11: float
         dStgLgCT12: float
         dStgLgCT21: float
@@ -318,35 +318,88 @@
         T: int  # eType
         L: int  # uiLoopIdx
         P: int  # uiPosition
         D: str  # wsDescription
 
     class RawTagDict(TypedDict):
         ID: str  # name of the tag
-        Type: int
-        Group: int
+        Type: Literal[
+            0,  # Unknown
+            1,  # String
+            2,  # Int
+            3,  # Double
+        ]
+        Group: Literal[
+            0,  # Undefined
+            1,  # Device
+            2,  # Camera
+            3,  # Plugin
+            4,  # Macro
+        ]
         Size: int
         Desc: str
         Unit: str
 
     # These dicts are intermediate dicts created in the process of parsing raw meta
     # they mimic intermediate parsing done by the SDK... but needn't stay this way.
 
+    AxisInterpretation = Literal["distance", "time"]
     CompressionType = Literal["lossless", "lossy", "none"]
+    LoopTypeString = Literal[
+        "Unknown",
+        "TimeLoop",
+        "XYPosLoop",
+        "XYDiscrLoop",
+        "ZStackLoop",
+        "PolarLoop",
+        "SpectLoop",
+        "CustomLoop",
+        "NETimeLoop",
+        "ManTimeLoop",
+        "ZStackLoopAccurate",
+    ]
 
     class ContentsDict(TypedDict):
         frameCount: int
 
     class GlobalMetadata(TypedDict):
         contents: ContentsDict
-        loops: dict
-        microscope: dict
-        position: dict
-        time: dict
-        volume: dict
+        loops: dict[LoopTypeString, int]
+        microscope: MicroscopeDict
+        position: PositionDict
+        time: TimeDict
+        volume: VolumeDict
+
+    class MicroscopeDict(TypedDict):
+        objectiveMagnification: float | None
+        objectiveName: str | None
+        objectiveNumericalAperture: float | None
+        projectiveMagnification: float | None
+        zoomMagnification: float | None
+        immersionRefractiveIndex: float | None
+        pinholeDiameterUm: float | None
+
+    class PositionDict(TypedDict):
+        stagePositionUm: tuple[float, float, float]
+
+    class TimeDict(TypedDict):
+        relativeTimeMs: float
+        absoluteJulianDayNumber: float
+
+    class VolumeDict(TypedDict):
+        axesCalibrated: tuple[bool, bool, bool]
+        axesCalibration: tuple[float, float, float]
+        axesInterpretation: tuple[
+            AxisInterpretation, AxisInterpretation, AxisInterpretation
+        ]
+        bitsPerComponentInMemory: int
+        bitsPerComponentSignificant: int
+        cameraTransformationMatrix: tuple[float, float, float, float]
+        componentDataType: Literal["float", "unsigned"]
+        voxelCount: tuple[int, int, int]
 
 
 class ELxModalityMask(IntEnum):
     fluorescence = 0x0000000000000001
     brightfield = 0x0000000000000002
     phaseContrast = 0x0000000000000010
     diContrast = 0x0000000000000020
```

### Comparing `nd2-0.6.1/tests/conftest.py` & `nd2-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/readlim_output.json` & `nd2-0.7.0/tests/readlim_output.json`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/samples_metadata.json` & `nd2-0.7.0/tests/samples_metadata.json`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/test_aicsimage.py` & `nd2-0.7.0/tests/test_aicsimage.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/test_binary.py` & `nd2-0.7.0/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/test_dask_dispatch.py` & `nd2-0.7.0/tests/test_dask_dispatch.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/test_index.py` & `nd2-0.7.0/tests/test_index.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,45 +12,51 @@
 
 
 @pytest.mark.parametrize("fmt", ["csv", "json", "table"])
 def test_format(records, fmt, capsys):
     filtered = nd2.index._filter_data(records)
 
     if fmt == "table":
-        nd2.index._pretty_print_table(filtered)
+        nd2.index._pretty_print_table(filtered, sort_column="name")
     elif fmt == "csv":
         nd2.index._print_csv(filtered)
     elif fmt == "json":
         nd2.index._print_json(filtered)
     captured = capsys.readouterr()
-    assert "path" in captured.out
+    assert captured.out
+    assert not captured.err
 
 
 @pytest.mark.parametrize(
     "filters",
     [
         {},
-        {"to_include": ["path", "name", "version"]},
+        {"include": "path,name,version"},
         {"sort_by": "version"},
         {"sort_by": "version-"},
         {"exclude": "path"},
+        {"filters": ("'TimeLoop' in experiment",)},
+        {"filters": ["acquired > '2020' and kb < 500"], "sort_by": "kb-"},
     ],
 )
-def test_filter_data(records, filters: dict):
+def test_filter_data(records, filters: dict) -> None:
     filtered = nd2.index._filter_data(records, **filters)
     assert isinstance(filtered, list)
-    assert len(filtered) == len(records)
     if filters.get("to_include"):
         assert len(filtered[0]) == len(filters["to_include"])
     sb = filters.get("sort_by")
     if sb:
         first_version = filtered[0]["version"]
         # ascending / descending
         assert first_version == "3.0" if sb.endswith("-") else "1.0"
     if filters.get("exclude"):
         assert "path" not in filtered[0]
+    if filters.get("filters"):
+        assert len(filtered) < len(records)
+    else:
+        assert len(filtered) == len(records)
 
 
 def test_index(capsys):
     nd2.index.main([str(DATA), "--format", "csv"])
     captured = capsys.readouterr()
     assert "path" in captured.out
```

### Comparing `nd2-0.6.1/tests/test_metadata.py` & `nd2-0.7.0/tests/test_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,24 +63,26 @@
         assert not nd.closed
 
         assert isinstance(nd._rdr._seq_count(), int)
         assert isinstance(nd.attributes, structures.Attributes)
 
         # TODO: deal with typing when metadata is completely missing
         assert isinstance(nd.metadata, structures.Metadata)
-        assert isinstance(nd.frame_metadata(0), structures.FrameMetadata)
+        for i in range(nd._rdr._seq_count()):
+            assert isinstance(nd.frame_metadata(i), structures.FrameMetadata)
         assert isinstance(nd.experiment, list)
         assert isinstance(nd.text_info, dict)
         assert isinstance(nd.sizes, dict)
         assert isinstance(nd.custom_data, dict)
         assert isinstance(nd.shape, tuple)
         assert isinstance(nd.size, int)
         assert isinstance(nd.closed, bool)
         assert isinstance(nd.ndim, int)
         _bd = nd.binary_data
+        assert all(isinstance(x, structures.ROI) for x in nd.rois.values())
         assert isinstance(nd.is_rgb, bool)
         assert isinstance(nd.nbytes, int)
 
         assert isinstance(nd.unstructured_metadata(), dict)
         assert isinstance(nd.events(), list)
         with pytest.warns(FutureWarning):
             assert isinstance(nd.recorded_data, dict)
```

### Comparing `nd2-0.6.1/tests/test_parse.py` & `nd2-0.7.0/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/test_reader.py` & `nd2-0.7.0/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/test_readme.py` & `nd2-0.7.0/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/test_rescue.py` & `nd2-0.7.0/tests/test_rescue.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/test_xml.py` & `nd2-0.7.0/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/variant.xml` & `nd2-0.7.0/tests/variant.xml`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/tests/variant_CustomDataV2_0.xml` & `nd2-0.7.0/tests/variant_CustomDataV2_0.xml`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/.gitignore` & `nd2-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/LICENSE` & `nd2-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nd2-0.6.1/README.md` & `nd2-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # nd2
 
 [![License](https://img.shields.io/pypi/l/nd2.svg?color=green)](https://github.com/tlambert03/nd2/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/nd2.svg?color=green)](https://pypi.org/project/nd2)
 [![Python Version](https://img.shields.io/pypi/pyversions/nd2.svg?color=green)](https://python.org)
 [![Tests](https://github.com/tlambert03/nd2/actions/workflows/ci.yml/badge.svg)](https://github.com/tlambert03/nd2/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/tlambert03/nd2/branch/main/graph/badge.svg)](https://codecov.io/gh/tlambert03/nd2)
+[![Benchmarks](https://img.shields.io/badge/⏱-codspeed-%23FF7B53)](https://codspeed.io/tlambert03/nd2)
 
 `.nd2` (Nikon NIS Elements) file reader.
 
 This reader provides a pure python implementation the official Nikon ND2 SDK.
 
 > It *used* to wrap the official SDK with Cython, but has since been completely
 > rewritten to be pure python (for performance, ease of distribution, and
@@ -21,14 +22,16 @@
 for lazy and/or annotated arrays.
 
 This library is tested against many nd2 files with the goal of maximizing
 compatibility and data extraction. (If you find an nd2 file that fails in some
 way, please [open an issue](https://github.com/tlambert03/nd2/issues/new) with
 the file!)
 
+### :book: [Documentation](https://tlambert03.github.io/nd2)
+
 ## install
 
 ```sh
 pip install nd2
 ```
 
 or from conda:
@@ -52,15 +55,20 @@
 `nd2` will use [`lxml`](https://pypi.org/project/lxml/) which is much faster
 than the built-in `xml` module.  To install with support for `lxml` use:
 
 ```sh
 pip install nd2 lxml
 ```
 
-## usage and API
+## Usage and API
+
+Full API documentation is available at
+[https://tlambert03.github.io/nd2](https://tlambert03.github.io/nd2)
+
+Quick summary below:
 
 ```python
 import nd2
 import numpy as np
 
 my_array = nd2.imread('some_file.nd2')                          # read to numpy array
 my_array = nd2.imread('some_file.nd2', dask=True)               # read to dask array
@@ -107,19 +115,19 @@
 f.custom_data       # bits of unstructured metadata that start with CustomData
 f.events()          # returns tabular "Recorded Data" view from in NIS Elements/Viewer
                     # with info for each frame in the experiment.
                     # output is passabled to pandas.DataFrame
 
 # allll the metadata we can find...
 # no attempt made to standardize or parse it
-# look in here if you're searching for metdata that isn't exposed in the above
+# look in here if you're searching for metadata that isn't exposed in the above
 # but try not to rely on it, as it's not guaranteed to be stable
 f.unstructured_metadata()
 
-f.close()           # don't forget to close when not using a contet manager!
+f.close()           # don't forget to close when not using a context manager!
 f.closed            # boolean, whether the file is closed
 ```
 
 ## Metadata structures
 
 These follow the structure of the nikon SDK outputs (where relevant).
 Here are some example outputs
```

### Comparing `nd2-0.6.1/pyproject.toml` & `nd2-0.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 ]
 dynamic = ["version"]
 dependencies = ["resource-backed-dask-array", "typing-extensions", "numpy"]
 
 [project.optional-dependencies]
 legacy = ["imagecodecs"]
 test = [
-    "lxml; python_version<'3.11'",
-    "aicsimageio; python_version<'3.11'",
+    "aicsimageio",
     "dask[array]",
-    "imagecodecs; platform_system=='Windows' or python_version<'3.11'",
+    "imagecodecs",
+    "lxml",
+    "ome-types",
     "psutil",
+    "pytest-codspeed",
     "pytest-cov",
-    "pytest>=6.0",
     "pytest-pretty",
+    "pytest>=6.0",
     "xarray",
 ]
 dev = [
     "aicsimageio",
     "black",
     "dask[array]",
     "imagecodecs",
@@ -46,16 +48,17 @@
     "pre-commit",
     "psutil",
     "pytest-cov",
     "pytest",
     "rich",
     "ruff",
     "xarray",
-    "lxml-stubs",
+    "types-lxml",
 ]
+docs = ["mkdocs", "mkdocs-material", "mkdocstrings-python"]
 
 [project.urls]
 homepage = "https://github.com/tlambert03/nd2"
 repository = "https://github.com/tlambert03/nd2"
 changelog = "https://github.com/tlambert03/nd2/blob/main/CHANGELOG.md"
 
 # https://hatch.pypa.io/latest/config/metadata/
@@ -123,14 +126,18 @@
 [tool.mypy]
 files = "src"
 strict = true
 disallow_any_generics = false
 show_column_numbers = true
 show_error_codes = true
 pretty = true
+plugins = ["pydantic.mypy"]
+
+[tool.pydantic-mypy]
+init_typed = false
 
 [[tool.mypy.overrides]]
 module = ["imagecodecs", "resource_backed_dask_array"]
 ignore_missing_imports = true
 
 # https://coverage.readthedocs.io/en/6.4/config.html
 [tool.coverage.report]
@@ -139,14 +146,16 @@
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "@overload",
     "\\.\\.\\.",
     "except ImportError",
     "except NotImplementedError",
     "if __name__ == .__main__.:",
+    " in flags:",                 # all the OME modality flags... don't need to test
+    "return None",                # just there for mypy
 ]
 
 [tool.coverage.run]
 source = ["src"]
 
 # https://github.com/mgedmin/check-manifest#configuration
 [tool.check-manifest]
```

### Comparing `nd2-0.6.1/PKG-INFO` & `nd2-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nd2
-Version: 0.6.1
+Version: 0.7.0
 Summary: Yet another nd2 (Nikon NIS Elements) file reader
 Project-URL: homepage, https://github.com/tlambert03/nd2
 Project-URL: repository, https://github.com/tlambert03/nd2
 Project-URL: changelog, https://github.com/tlambert03/nd2/blob/main/CHANGELOG.md
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
@@ -22,44 +22,51 @@
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: aicsimageio; extra == 'dev'
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: dask[array]; extra == 'dev'
 Requires-Dist: imagecodecs; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
-Requires-Dist: lxml-stubs; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: psutil; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: types-lxml; extra == 'dev'
 Requires-Dist: xarray; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: mkdocs; extra == 'docs'
+Requires-Dist: mkdocs-material; extra == 'docs'
+Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: legacy
 Requires-Dist: imagecodecs; extra == 'legacy'
 Provides-Extra: test
-Requires-Dist: aicsimageio; python_version < '3.11' and extra == 'test'
+Requires-Dist: aicsimageio; extra == 'test'
 Requires-Dist: dask[array]; extra == 'test'
-Requires-Dist: imagecodecs; platform_system == 'Windows' or python_version < '3.11' and extra == 'test'
-Requires-Dist: lxml; python_version < '3.11' and extra == 'test'
+Requires-Dist: imagecodecs; extra == 'test'
+Requires-Dist: lxml; extra == 'test'
+Requires-Dist: ome-types; extra == 'test'
 Requires-Dist: psutil; extra == 'test'
+Requires-Dist: pytest-codspeed; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-pretty; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
 Requires-Dist: xarray; extra == 'test'
 Description-Content-Type: text/markdown
 
 # nd2
 
 [![License](https://img.shields.io/pypi/l/nd2.svg?color=green)](https://github.com/tlambert03/nd2/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/nd2.svg?color=green)](https://pypi.org/project/nd2)
 [![Python Version](https://img.shields.io/pypi/pyversions/nd2.svg?color=green)](https://python.org)
 [![Tests](https://github.com/tlambert03/nd2/actions/workflows/ci.yml/badge.svg)](https://github.com/tlambert03/nd2/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/tlambert03/nd2/branch/main/graph/badge.svg)](https://codecov.io/gh/tlambert03/nd2)
+[![Benchmarks](https://img.shields.io/badge/⏱-codspeed-%23FF7B53)](https://codspeed.io/tlambert03/nd2)
 
 `.nd2` (Nikon NIS Elements) file reader.
 
 This reader provides a pure python implementation the official Nikon ND2 SDK.
 
 > It *used* to wrap the official SDK with Cython, but has since been completely
 > rewritten to be pure python (for performance, ease of distribution, and
@@ -72,14 +79,16 @@
 for lazy and/or annotated arrays.
 
 This library is tested against many nd2 files with the goal of maximizing
 compatibility and data extraction. (If you find an nd2 file that fails in some
 way, please [open an issue](https://github.com/tlambert03/nd2/issues/new) with
 the file!)
 
+### :book: [Documentation](https://tlambert03.github.io/nd2)
+
 ## install
 
 ```sh
 pip install nd2
 ```
 
 or from conda:
@@ -103,15 +112,20 @@
 `nd2` will use [`lxml`](https://pypi.org/project/lxml/) which is much faster
 than the built-in `xml` module.  To install with support for `lxml` use:
 
 ```sh
 pip install nd2 lxml
 ```
 
-## usage and API
+## Usage and API
+
+Full API documentation is available at
+[https://tlambert03.github.io/nd2](https://tlambert03.github.io/nd2)
+
+Quick summary below:
 
 ```python
 import nd2
 import numpy as np
 
 my_array = nd2.imread('some_file.nd2')                          # read to numpy array
 my_array = nd2.imread('some_file.nd2', dask=True)               # read to dask array
@@ -158,19 +172,19 @@
 f.custom_data       # bits of unstructured metadata that start with CustomData
 f.events()          # returns tabular "Recorded Data" view from in NIS Elements/Viewer
                     # with info for each frame in the experiment.
                     # output is passabled to pandas.DataFrame
 
 # allll the metadata we can find...
 # no attempt made to standardize or parse it
-# look in here if you're searching for metdata that isn't exposed in the above
+# look in here if you're searching for metadata that isn't exposed in the above
 # but try not to rely on it, as it's not guaranteed to be stable
 f.unstructured_metadata()
 
-f.close()           # don't forget to close when not using a contet manager!
+f.close()           # don't forget to close when not using a context manager!
 f.closed            # boolean, whether the file is closed
 ```
 
 ## Metadata structures
 
 These follow the structure of the nikon SDK outputs (where relevant).
 Here are some example outputs
```

