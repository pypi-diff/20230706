# Comparing `tmp/bowtie_json_schema-2023.6.4.tar.gz` & `tmp/bowtie_json_schema-2023.7.2.tar.gz`

## Comparing `bowtie_json_schema-2023.6.4.tar` & `bowtie_json_schema-2023.7.2.tar`

### file list

```diff
@@ -1,50 +1,82 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.flake8
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.readthedocs.yml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/action.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/test-requirements.in
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/SECURITY.md
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/release.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/workflows/images.yml
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/__main__.py
--rw-r--r--   0        0        0    31499 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/_cli.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/cli.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/conf.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/requirements.in
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/requirements.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/_static/dreamed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/conftest.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/LICENSE
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/README.rst
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/pyproject.toml
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.flake8
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.readthedocs.yml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/action.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/test-requirements.in
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/SECURITY.md
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/release.yml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/build-frontend.yml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/deploy-frontend.yml
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/images.yml
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/__main__.py
+-rw-r--r--   0        0        0    31499 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/_cli.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/cli.rst
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/conf.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/contributing.rst
+-rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/requirements.in
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/requirements.txt
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/_static/dreamed.png
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/.eslintrc.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/index.html
+-rw-r--r--   0        0        0   126070 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/package-lock.json
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/package.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/vite.config.js
+-rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/public/favicon.ico
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/MainContainer.jsx
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/ReportDataHandler.jsx
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/ReportView.jsx
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/index.jsx
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/CopyToClipboard.jsx
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/LoadingAnimation.jsx
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/NavBar.jsx
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Cases/AccordionItem.jsx
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Cases/AccordionSvg.jsx
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Cases/CasesSection.jsx
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Cases/SchemaDisplay.jsx
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/DragAndDrop/DragAndDrop.jsx
+-rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Modals/DetailsButtonModal.jsx
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Modals/RunTimeInfoModal.jsx
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/RunInfo/RunInfoSection.jsx
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Summary/ImplementationRow.jsx
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Summary/SummarySection.jsx
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Summary/SummaryTable.jsx
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/context/BowtieVersionContext.jsx
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/context/ThemeContext.jsx
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/data/runInfo.js
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/data/summary.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/conftest.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/LICENSE
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/README.rst
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.6.4/.flake8` & `bowtie_json_schema-2023.7.2/.flake8`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/.pre-commit-config.yaml` & `bowtie_json_schema-2023.7.2/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -13,23 +13,23 @@
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.4.0
+    rev: v3.8.0
     hooks:
       - id: pyupgrade
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.270"
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.0.276"
     hooks:
       - id: ruff
   - repo: https://github.com/Riverside-Healthcare/djLint
-    rev: v1.30.2
+    rev: v1.31.1
     hooks:
       - id: djlint-jinja
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - name: black (python implementations & bowtie internals)
         id: black
@@ -64,19 +64,30 @@
   - repo: https://github.com/jumanjihouse/pre-commit-hooks
     rev: "3.0.0"
     hooks:
       - name: rubocop (ruby implementations)
         id: rubocop
         args: ["--auto-correct"]
   - repo: https://github.com/JohnnyMorganz/StyLua
-    rev: v0.17.1
+    rev: v0.18.0
     hooks:
       - name: stylua (lua implementations)
         id: stylua
         exclude: .*/json.lua
         args: ["--config-path", "implementations/lua-jsonschema/stylua.toml"]
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v16.0.4
+    rev: v16.0.6
     hooks:
       - name: clang-format (c/c++/c#/java implementations)
         id: clang-format
         types_or: [c++, c, c#, java, objective-c]
+  - repo: https://github.com/pre-commit/mirrors-eslint
+    rev: v8.44.0
+    hooks:
+      - name: eslint
+        id: eslint
+        files: ^frontend/src/.*\.jsx?$
+        types: [file]
+        additional_dependencies:
+          - eslint@8.43.0
+          - eslint-plugin-react@7.32.2
+          - eslint-plugin-react-hooks@4.6.0
```

### Comparing `bowtie_json_schema-2023.6.4/noxfile.py` & `bowtie_json_schema-2023.7.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/test-requirements.txt` & `bowtie_json_schema-2023.7.2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/.github/SECURITY.md` & `bowtie_json_schema-2023.7.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/.github/dependabot.yml` & `bowtie_json_schema-2023.7.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/.github/workflows/ci.yml` & `bowtie_json_schema-2023.7.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.7.2/.github/workflows/dependabot-merge.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 jobs:
   dependabot:
     runs-on: ubuntu-latest
     if: ${{ github.actor == 'dependabot[bot]' }}
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.5.1
+        uses: dependabot/fetch-metadata@v1.6.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
       - name: Enable auto-merge for Dependabot PRs
         run: gh pr merge --auto --merge "$PR_URL"
         env:
           PR_URL: ${{ github.event.pull_request.html_url }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `bowtie_json_schema-2023.6.4/.github/workflows/images.yml` & `bowtie_json_schema-2023.7.2/.github/workflows/images.yml`

 * *Files 1% similar despite different names*

```diff
@@ -83,13 +83,13 @@
           tags: ${{ steps.build_image.outputs.tags }}
           registry: ghcr.io/${{ github.repository_owner }}
           username: ${{ github.actor }}
           password: ${{ github.token }}
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
 
       - name: Install Bowtie
-        uses: bowtie-json-schema/bowtie@v2023.05.14
+        uses: bowtie-json-schema/bowtie@v2023.06.4
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
 
       - name: Smoke Test
         run: bowtie smoke -i "${{ steps.build_image.outputs.image-with-tag }}"
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
```

### Comparing `bowtie_json_schema-2023.6.4/.github/workflows/report.yml` & `bowtie_json_schema-2023.7.2/.github/workflows/report.yml`

 * *Files 21% similar despite different names*

```diff
@@ -41,51 +41,21 @@
           python-version: "3.x"
 
       - name: Install Bowtie
         run: python3 -m pip install bowtie-json-schema
 
       - name: Generate the Report
         run: |
-          bowtie suite $(find implementations/ -mindepth 1 -maxdepth 1 -type d | sed 's/implementations\//-i /') https://github.com/json-schema-org/JSON-Schema-Test-Suite/tree/main/tests/${{ matrix.version }} | tee ${{ matrix.version }}.jsonl | bowtie report --badges badges --generate-dialect-navigation --out ${{ matrix.version }}.html
+          bowtie suite $(find implementations/ -mindepth 1 -maxdepth 1 -type d | sed 's/implementations\//-i /') https://github.com/json-schema-org/JSON-Schema-Test-Suite/tree/main/tests/${{ matrix.version }} | tee ${{ matrix.version }}.json | bowtie report --badges badges --generate-dialect-navigation --out ${{ matrix.version }}.html
 
       - uses: actions/upload-artifact@v3
         with:
           name: report
           path: |
-            ${{ matrix.version }}.html
-            ${{ matrix.version }}.jsonl
+            ${{ matrix.version }}.json
             badges/
 
-  collect:
-    runs-on: ubuntu-latest
+  deploy-frontend:
     needs: test
-
-    steps:
-      - name: Setup Pages
-        id: pages
-        uses: actions/configure-pages@v3
-
-      - run: mkdir _site
-
-      - name: Download the reports
-        uses: actions/download-artifact@v3
-        with:
-          name: report
-          path: _site
-
-      - name: Finish the site structure setup
-        run: |
-          cp _site/draft2020-12.html _site/index.html
-
-      - name: Upload artifact
-        uses: actions/upload-pages-artifact@v1
-
-  deploy:
-    environment:
-      name: github-pages
-      url: ${{ steps.deployment.outputs.page_url }}
-    runs-on: ubuntu-latest
-    needs: collect
-    steps:
-      - name: Deploy to GitHub Pages
-        id: deployment
-        uses: actions/deploy-pages@v2
+    uses: ./.github/workflows/deploy-frontend.yml
+    with:
+      report_artifact_in_scope: true
```

### Comparing `bowtie_json_schema-2023.6.4/bowtie/_cli.py` & `bowtie_json_schema-2023.7.2/bowtie/_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/bowtie/_commands.py` & `bowtie_json_schema-2023.7.2/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/bowtie/_core.py` & `bowtie_json_schema-2023.7.2/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/bowtie/_report.py` & `bowtie_json_schema-2023.7.2/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/bowtie/exceptions.py` & `bowtie_json_schema-2023.7.2/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/docs/Makefile` & `bowtie_json_schema-2023.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/docs/cli.rst` & `bowtie_json_schema-2023.7.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/docs/conf.py` & `bowtie_json_schema-2023.7.2/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 pygments_dark_style = "one-dark"
 
 html_theme = "furo"
 html_logo = str(STATIC / "dreamed.png")
 html_static_path = [str(STATIC)]
 
 rst_prolog = """
+.. |site| replace:: https://bowtie-json-schema.github.io/bowtie/
+
 .. _official test suite: https://github.com/json-schema-org/JSON-Schema-Test-Suite
 """  # noqa: E501
 
 
 def entire_domain(host):
     return r"http.?://" + re.escape(host) + r"($|/.*)"
```

### Comparing `bowtie_json_schema-2023.6.4/docs/contributing.rst` & `bowtie_json_schema-2023.7.2/docs/contributing.rst`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,25 @@
 
     $ nox -s tests-3.11
 
 to run the tests using Python 3.11 (or any other version you'd like).
 
 Before submitting a PR you may want to run the full suite of tests by running ``nox`` with no arguments to run all environments.
 
+Running the UI
+--------------
+
+Bowtie has a frontend interface which can be used to view or query results of Bowtie test runs.
+
+A hosted version of this UI will live at |site|.
+If you are making changes to the UI, you can run it locally by:
+
+    * ensuring you have ``node`` and ``npm`` installed
+    * running ``npm start`` in the ``frontend/`` directory within your repository checkout of Bowtie
+
 
 For Implementers
 ----------------
 
 If you have a new (or not so new) implementation which Bowtie doesn't yet support, contributing support for your implementation is extremely useful.
 
 See the `harness tutorial <implementers>` for details on writing a harness for your implementation, and please do send a PR to add it!
```

### Comparing `bowtie_json_schema-2023.6.4/docs/implementers.rst` & `bowtie_json_schema-2023.7.2/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/docs/index.rst` & `bowtie_json_schema-2023.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/docs/requirements.txt` & `bowtie_json_schema-2023.7.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/docs/_static/dreamed.png` & `bowtie_json_schema-2023.7.2/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/tests/test_integration.py` & `bowtie_json_schema-2023.7.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.7.2/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.7.2/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.7.2/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.7.2/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.7.2/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/.gitignore` & `bowtie_json_schema-2023.7.2/.gitignore`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 /TODO*
 bowtie-report.html
 /badges/
 
+/frontend/node_modules
+/frontend/build
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
@@ -144,17 +147,14 @@
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
-# PyCharm
-#  JetBrains specific template is maintainted in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+# Editor vomit
+.idea/
+.vscode/
 
 # User defined
 _cache
 _templates
```

### Comparing `bowtie_json_schema-2023.6.4/LICENSE` & `bowtie_json_schema-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/README.rst` & `bowtie_json_schema-2023.7.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
   :alt: pre-commit.ci status
   :target: https://results.pre-commit.ci/latest/github/bowtie-json-schema/bowtie/main
 
 |
 
 Bowtie is a *meta*-validator of the `JSON Schema specification <https://json-schema.org/>`_, by which we mean it coordinates executing *other* `validator implementations <https://json-schema.org/implementations.html>`_, collecting and reporting on their results.
 
-To do so it defines a simple input/output protocol (specified in `this JSON Schema <https://github.com/bowtie-json-schema/bowtie/blob/main/io-schema.json>`_ which validator implementations can implement, and it provides a CLI which can execute supported implementations.
+To do so it defines a simple input/output protocol (specified in `this JSON Schema <https://github.com/bowtie-json-schema/bowtie/blob/main/io-schema.json>`_) which validator implementations can implement, and it provides a CLI which can execute supported implementations.
 
 It's called Bowtie because it fans in lots of JSON then fans out lots of results: ``>·<``.
 Looks like a bowtie, no?
 Also because it's elegant – we hope.
 
 For more information, see `Bowtie's documentation <https://bowtie-json-schema.readthedocs.io/>`_.
```

### Comparing `bowtie_json_schema-2023.6.4/pyproject.toml` & `bowtie_json_schema-2023.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.4/PKG-INFO` & `bowtie_json_schema-2023.7.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.6.4
+Version: 2023.7.2
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
@@ -66,14 +66,14 @@
   :alt: pre-commit.ci status
   :target: https://results.pre-commit.ci/latest/github/bowtie-json-schema/bowtie/main
 
 |
 
 Bowtie is a *meta*-validator of the `JSON Schema specification <https://json-schema.org/>`_, by which we mean it coordinates executing *other* `validator implementations <https://json-schema.org/implementations.html>`_, collecting and reporting on their results.
 
-To do so it defines a simple input/output protocol (specified in `this JSON Schema <https://github.com/bowtie-json-schema/bowtie/blob/main/io-schema.json>`_ which validator implementations can implement, and it provides a CLI which can execute supported implementations.
+To do so it defines a simple input/output protocol (specified in `this JSON Schema <https://github.com/bowtie-json-schema/bowtie/blob/main/io-schema.json>`_) which validator implementations can implement, and it provides a CLI which can execute supported implementations.
 
 It's called Bowtie because it fans in lots of JSON then fans out lots of results: ``>·<``.
 Looks like a bowtie, no?
 Also because it's elegant – we hope.
 
 For more information, see `Bowtie's documentation <https://bowtie-json-schema.readthedocs.io/>`_.
```

