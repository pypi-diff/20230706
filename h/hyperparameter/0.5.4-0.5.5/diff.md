# Comparing `tmp/hyperparameter-0.5.4.tar.gz` & `tmp/hyperparameter-0.5.5.tar.gz`

## Comparing `hyperparameter-0.5.4.tar` & `hyperparameter-0.5.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 hyperparameter-0.5.4/Cargo.toml
--rw-r--r--   0     1001      123      834 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      123      126 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0     1001      123      595 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      123      706 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/.github/workflows/codecov.yml
--rw-r--r--   0     1001      123      845 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/.github/workflows/mkdocs.yml
--rw-r--r--   0     1001      123     1262 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/.github/workflows/python-publish.yml
--rw-r--r--   0     1001      123     2001 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/.gitignore
--rw-r--r--   0     1001      123      356 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     5202 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    24124 2023-05-25 07:12:21.000000 hyperparameter-0.5.4/Cargo.lock
--rw-r--r--   0     1001      123    11356 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/LICENSE
--rw-r--r--   0     1001      123     3861 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/README.md
--rw-r--r--   0     1001      123     3457 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/README.zh.md
--rw-r--r--   0     1001      123     2846 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/docs/examples/optimization.md
--rw-r--r--   0     1001      123     2868 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/docs/examples/optimization.zh.md
--rw-r--r--   0     1001      123     3861 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/docs/index.md
--rw-r--r--   0     1001      123     3457 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/docs/index.zh.md
--rw-r--r--   0     1001      123     3000 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/docs/quick_start.md
--rw-r--r--   0     1001      123     3000 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/docs/quick_start.zh.md
--rw-r--r--   0     1001      123       48 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/docs/reference.md
--rw-r--r--   0     1001      123      110 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/docs/requirements.txt
--rw-r--r--   0     1001      123     6738 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/docs/structured_parameter.md
--rw-r--r--   0     1001      123      337 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/application/README.md
--rw-r--r--   0     1001      123      789 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/application/app.py
--rw-r--r--   0     1001      123       46 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/application/cfg.json
--rw-r--r--   0     1001      123     4733 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/automl_optuna_mnist/automl_mnist.py
--rw-r--r--   0     1001      123     2737 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/cpp/cxx_test.cc
--rw-r--r--   0     1001      123      433 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/cpp/cxx_test.py
--rw-r--r--   0     1001      123      237 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/cpp/cxx_test.sh
--rw-r--r--   0     1001      123      152 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/mnist/README.md
--rw-r--r--   0     1001      123     5625 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/mnist/main.py
--rw-r--r--   0     1001      123     5899 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/mnist/main_with_hp.py
--rw-r--r--   0     1001      123     6202 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/mnist/main_with_hp_with_mlflow.py
--rw-r--r--   0     1001      123       18 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/mnist/requirements.txt
--rw-r--r--   0     1001      123     2846 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/optuna/README.md
--rw-r--r--   0     1001      123      230 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/optuna/example.py
--rw-r--r--   0     1001      123      527 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/optuna/example_hp.py
--rw-r--r--   0     1001      123      727 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/optuna/example_hp_nested.py
--rw-r--r--   0     1001      123     1650 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/sparse_lr/README.md
--rw-r--r--   0     1001      123      581 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/sparse_lr/example_1.py
--rw-r--r--   0     1001      123      934 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/sparse_lr/example_2.py
--rw-r--r--   0     1001      123     1059 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/sparse_lr/example_mlflow.py
--rw-r--r--   0     1001      123      867 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/sparse_lr/model.py
--rw-r--r--   0     1001      123     1631 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/examples/storage.rs
--rw-r--r--   0     1001      123        0 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/hparam/__init__.py
--rw-r--r--   0     1001      123     3710 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/hparam/__main__.py
--rw-r--r--   0     1001      123      314 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/hyperparameter/__init__.py
--rw-r--r--   0     1001      123    17127 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/hyperparameter/api.py
--rw-r--r--   0     1001      123     7715 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/hyperparameter/hyperparameter.h
--rw-r--r--   0     1001      123      828 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/hyperparameter/loader.py
--rw-r--r--   0     1001      123     4196 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/hyperparameter/storage.py
--rw-r--r--   0     1001      123     2223 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/hyperparameter/tune.py
--rw-r--r--   0     1001      123     1249 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/mkdocs.yml
--rw-r--r--   0     1001      123      938 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/pyproject.toml
--rwxr-xr-x   0     1001      123      814 2023-05-25 07:11:59.000000 hyperparameter-0.5.4/run-maturin-action.sh
--rw-r--r--   0     1001      123     6151 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/src/entry.rs
--rw-r--r--   0     1001      123     6580 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/src/ext.rs
--rw-r--r--   0     1001      123     2038 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/src/ffi.rs
--rw-r--r--   0     1001      123      106 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/src/lib.rs
--rw-r--r--   0     1001      123     8129 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/src/storage.rs
--rw-r--r--   0     1001      123     4528 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/src/xxh.rs
--rwxr-xr-x   0     1001      123    40754 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/tests/a.out
--rw-r--r--   0     1001      123      912 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/tests/test_auto_param.py
--rw-r--r--   0     1001      123     3769 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/tests/test_param_scope.py
--rw-r--r--   0     1001      123      697 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/tests/test_param_scope_thread.py
--rw-r--r--   0     1001      123     2988 2023-05-25 07:11:16.000000 hyperparameter-0.5.4/tests/test_rust_backend.py
--rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 hyperparameter-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 hyperparameter-0.5.5/Cargo.toml
+-rw-r--r--   0     1001      123      834 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      126 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0     1001      123      595 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123      706 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/workflows/codecov.yml
+-rw-r--r--   0     1001      123      845 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/workflows/mkdocs.yml
+-rw-r--r--   0     1001      123     1262 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/workflows/python-publish.yml
+-rw-r--r--   0     1001      123     2001 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.gitignore
+-rw-r--r--   0     1001      123      356 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     5202 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    25260 2023-07-06 11:54:56.000000 hyperparameter-0.5.5/Cargo.lock
+-rw-r--r--   0     1001      123    11356 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/LICENSE
+-rw-r--r--   0     1001      123     3027 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/README.md
+-rw-r--r--   0     1001      123     2871 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/README.zh.md
+-rw-r--r--   0     1001      123     2846 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/examples/optimization.md
+-rw-r--r--   0     1001      123     2868 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/examples/optimization.zh.md
+-rw-r--r--   0     1001      123     3027 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/index.md
+-rw-r--r--   0     1001      123     2871 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/index.zh.md
+-rw-r--r--   0     1001      123     3000 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/quick_start.md
+-rw-r--r--   0     1001      123     3000 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/quick_start.zh.md
+-rw-r--r--   0     1001      123       48 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/reference.md
+-rw-r--r--   0     1001      123      110 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/requirements.txt
+-rw-r--r--   0     1001      123     6738 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/structured_parameter.md
+-rw-r--r--   0     1001      123      337 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/application/README.md
+-rw-r--r--   0     1001      123      789 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/application/app.py
+-rw-r--r--   0     1001      123       46 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/application/cfg.json
+-rw-r--r--   0     1001      123     4733 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/automl_optuna_mnist/automl_mnist.py
+-rw-r--r--   0     1001      123     2737 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/cpp/cxx_test.cc
+-rw-r--r--   0     1001      123      436 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/cpp/cxx_test.py
+-rw-r--r--   0     1001      123      237 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/cpp/cxx_test.sh
+-rw-r--r--   0     1001      123      152 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/mnist/README.md
+-rw-r--r--   0     1001      123     5625 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/mnist/main.py
+-rw-r--r--   0     1001      123     5899 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/mnist/main_with_hp.py
+-rw-r--r--   0     1001      123     6202 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/mnist/main_with_hp_with_mlflow.py
+-rw-r--r--   0     1001      123       18 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/mnist/requirements.txt
+-rw-r--r--   0     1001      123     2846 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/optuna/README.md
+-rw-r--r--   0     1001      123      230 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/optuna/example.py
+-rw-r--r--   0     1001      123      527 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/optuna/example_hp.py
+-rw-r--r--   0     1001      123      727 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/optuna/example_hp_nested.py
+-rw-r--r--   0     1001      123     1650 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/sparse_lr/README.md
+-rw-r--r--   0     1001      123      581 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/sparse_lr/example_1.py
+-rw-r--r--   0     1001      123      934 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/sparse_lr/example_2.py
+-rw-r--r--   0     1001      123     1059 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/sparse_lr/example_mlflow.py
+-rw-r--r--   0     1001      123      867 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/sparse_lr/model.py
+-rw-r--r--   0     1001      123     1631 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/storage.rs
+-rw-r--r--   0     1001      123        0 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hparam/__init__.py
+-rw-r--r--   0     1001      123     3710 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hparam/__main__.py
+-rw-r--r--   0     1001      123      320 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/__init__.py
+-rw-r--r--   0     1001      123    17127 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/api.py
+-rw-r--r--   0     1001      123     7715 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/hyperparameter.h
+-rw-r--r--   0     1001      123      828 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/loader.py
+-rw-r--r--   0     1001      123     4202 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/storage.py
+-rw-r--r--   0     1001      123     2223 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/tune.py
+-rw-r--r--   0     1001      123     1249 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/mkdocs.yml
+-rw-r--r--   0     1001      123      941 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/pyproject.toml
+-rwxr-xr-x   0     1001      123      814 2023-07-06 11:54:36.000000 hyperparameter-0.5.5/run-maturin-action.sh
+-rw-r--r--   0     1001      123     6151 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/entry.rs
+-rw-r--r--   0     1001      123     6583 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/ext.rs
+-rw-r--r--   0     1001      123     2038 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/ffi.rs
+-rw-r--r--   0     1001      123      106 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/lib.rs
+-rw-r--r--   0     1001      123     8129 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/storage.rs
+-rw-r--r--   0     1001      123     4528 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/xxh.rs
+-rwxr-xr-x   0     1001      123    40754 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/tests/a.out
+-rw-r--r--   0     1001      123      912 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/tests/test_auto_param.py
+-rw-r--r--   0     1001      123     3769 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/tests/test_param_scope.py
+-rw-r--r--   0     1001      123      697 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/tests/test_param_scope_thread.py
+-rw-r--r--   0     1001      123     2991 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/tests/test_rust_backend.py
+-rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 hyperparameter-0.5.5/PKG-INFO
```

### Comparing `hyperparameter-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md` & `hyperparameter-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md` & `hyperparameter-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/.github/workflows/codecov.yml` & `hyperparameter-0.5.5/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/.github/workflows/mkdocs.yml` & `hyperparameter-0.5.5/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/.github/workflows/python-publish.yml` & `hyperparameter-0.5.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/.gitignore` & `hyperparameter-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/CODE_OF_CONDUCT.md` & `hyperparameter-0.5.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/Cargo.lock` & `hyperparameter-0.5.5/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "atty"
-version = "0.2.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
-]
-
-[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "base-x"
@@ -28,14 +17,20 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cc"
@@ -47,21 +42,21 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "colored"
-version = "2.0.0"
+version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3616f750b84d8f0de8a58bda93e08e2a81ad3f523089b05f1dffecab48c6cbd"
+checksum = "2674ec482fbc38012cf31e6c42ba0177b431a0cb6f15fe40efa5aab1bda516f6"
 dependencies = [
- "atty",
+ "is-terminal",
  "lazy_static",
- "winapi",
+ "windows-sys",
 ]
 
 [[package]]
 name = "const_fn"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fbdcdcb6d86f71c5e97409ad45898af11cbc995b4ee8112d59095a28d376c935"
@@ -85,61 +80,61 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "cxx"
-version = "1.0.94"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
+checksum = "bd99fdd577aa186de8a711654cfabc63a7b2024e8d392f87153af428deaa4f71"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
-version = "1.0.94"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
+checksum = "f9204071a5d00b4da785ebe22f863cffd365f3357b6dba4070177bfe2e75f160"
 
 [[package]]
 name = "cxxbridge-macro"
-version = "1.0.94"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
+checksum = "59f6a87b1e7f773ec602b9af278e06da3d1b46c98bc0ee09751c2477d97d3b0b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "darling"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d706e75d87e35569db781a9b5e2416cff1236a47ed380831f959382ccd5f858"
@@ -218,36 +213,45 @@
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
-name = "fnv"
-version = "1.0.7"
+name = "errno"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys",
+]
 
 [[package]]
-name = "hermit-abi"
-version = "0.1.19"
+name = "errno-dragonfly"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
 dependencies = [
+ "cc",
  "libc",
 ]
 
 [[package]]
+name = "fnv"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
+
+[[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "hyperparameter"
 version = "0.5.2"
 dependencies = [
  "cxx",
  "lazy_static",
@@ -265,174 +269,197 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "is-terminal"
+version = "0.4.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24fddda5af7e54bf7da53067d6e802dbcc381d0a8eef629df528e3ebf68755cb"
+dependencies = [
+ "hermit-abi",
+ "rustix",
+ "windows-sys",
+]
+
+[[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "link-cplusplus"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
+checksum = "9d240c6f7e1ba3a28b0249f774e6a9dd0175054b52dfbb61b16eb8505c3785c9"
 dependencies = [
  "cc",
 ]
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
+
+[[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "phf"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
+checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
 dependencies = [
  "phf_macros",
  "phf_shared",
 ]
 
 [[package]]
 name = "phf_generator"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1181c94580fa345f50f19d738aaa39c0ed30a600d95cb2d3e23f94266f14fbf"
+checksum = "48e4cc64c2ad9ebe670cb8fd69dd50ae301650392e81c05f9bfcb2d5bdbc24b0"
 dependencies = [
  "phf_shared",
  "rand",
 ]
 
 [[package]]
 name = "phf_macros"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92aacdc5f16768709a569e913f7451034034178b05bdc8acda226659a3dccc66"
+checksum = "3444646e286606587e49f3bcf1679b8cef1dc2c5ecc29ddacaffc305180d464b"
 dependencies = [
  "phf_generator",
  "phf_shared",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "phf_shared"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
+checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
@@ -477,17 +504,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -523,19 +550,19 @@
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "rspec"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89389e7c690310e855df3d9b507985ca0d323e2e766b2fedf369b02671e70e0a"
@@ -553,18 +580,31 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "138e3e0acb6c9fb258b19b67cb8abd63c00679d2851805ea151465464fe9030a"
 dependencies = [
  "semver",
 ]
 
 [[package]]
+name = "rustix"
+version = "0.38.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac5ffa1efe7548069688cd7028f32591853cd7b5b756d41bcffd2353e4fc75b4"
+dependencies = [
+ "bitflags 2.3.3",
+ "errno",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys",
+]
+
+[[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
@@ -581,34 +621,34 @@
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.166"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "d01b7404f9d441d3ad40e6a636a7782c377d2abdbe4fa2440e2edcc2f4f10db8"
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.166"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "5dd83d6dde2b6b2d466e14d9d1acce8816dedee94f735eac6395808b3483c6d6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -630,17 +670,17 @@
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "standback"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e113fb6f3de07a243d434a56ec6f186dfd51cb08448239fe7bcae73f87ff28ff"
 dependencies = [
@@ -711,28 +751,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.16"
+version = "2.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
+checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "time"
 version = "0.2.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4752a97f8eebd6854ff91f1c1824cd6160626ac4bd44287f7f4ea2035a02a242"
 dependencies = [
@@ -766,17 +806,17 @@
  "quote",
  "standback",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -784,65 +824,65 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -860,70 +900,70 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `hyperparameter-0.5.4/LICENSE` & `hyperparameter-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/docs/examples/optimization.md` & `hyperparameter-0.5.5/docs/examples/optimization.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/docs/examples/optimization.zh.md` & `hyperparameter-0.5.5/docs/examples/optimization.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/docs/quick_start.md` & `hyperparameter-0.5.5/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/docs/quick_start.zh.md` & `hyperparameter-0.5.5/docs/quick_start.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/docs/structured_parameter.md` & `hyperparameter-0.5.5/docs/structured_parameter.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/application/app.py` & `hyperparameter-0.5.5/examples/application/app.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/automl_optuna_mnist/automl_mnist.py` & `hyperparameter-0.5.5/examples/automl_optuna_mnist/automl_mnist.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/cpp/cxx_test.cc` & `hyperparameter-0.5.5/examples/cpp/cxx_test.cc`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/mnist/main.py` & `hyperparameter-0.5.5/examples/mnist/main.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/mnist/main_with_hp.py` & `hyperparameter-0.5.5/examples/mnist/main_with_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/mnist/main_with_hp_with_mlflow.py` & `hyperparameter-0.5.5/examples/mnist/main_with_hp_with_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/optuna/README.md` & `hyperparameter-0.5.5/examples/optuna/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/optuna/example_hp.py` & `hyperparameter-0.5.5/examples/optuna/example_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/optuna/example_hp_nested.py` & `hyperparameter-0.5.5/examples/optuna/example_hp_nested.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/sparse_lr/README.md` & `hyperparameter-0.5.5/examples/sparse_lr/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/sparse_lr/example_1.py` & `hyperparameter-0.5.5/examples/sparse_lr/example_1.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/sparse_lr/example_2.py` & `hyperparameter-0.5.5/examples/sparse_lr/example_2.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/sparse_lr/example_mlflow.py` & `hyperparameter-0.5.5/examples/sparse_lr/example_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/sparse_lr/model.py` & `hyperparameter-0.5.5/examples/sparse_lr/model.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/examples/storage.rs` & `hyperparameter-0.5.5/examples/storage.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/hparam/__main__.py` & `hyperparameter-0.5.5/hparam/__main__.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/hyperparameter/api.py` & `hyperparameter-0.5.5/hyperparameter/api.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/hyperparameter/hyperparameter.h` & `hyperparameter-0.5.5/hyperparameter/hyperparameter.h`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/hyperparameter/loader.py` & `hyperparameter-0.5.5/hyperparameter/loader.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/hyperparameter/storage.py` & `hyperparameter-0.5.5/hyperparameter/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,16 +147,16 @@
 
 def xxh64(*args, **kwargs):
     raise RuntimeError("hyperparameter is not build with rust backend")
 
 
 try:
     if os.environ.get("HYPERPARAMETER_BACKEND", "RUST") == "RUST":
-        from hyperparameter.rbackend import KVStorage
-        from hyperparameter.rbackend import xxh64
+        from hyperparameter.librbackend import KVStorage
+        from hyperparameter.librbackend import xxh64
 
         TLSKVStorage = KVStorage
         has_rust_backend = True
 except:
     import traceback
 
     traceback.print_exc()
```

### Comparing `hyperparameter-0.5.4/hyperparameter/tune.py` & `hyperparameter-0.5.5/hyperparameter/tune.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/mkdocs.yml` & `hyperparameter-0.5.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/pyproject.toml` & `hyperparameter-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "hyperparameter"
-version = "0.5.4"
+version = "0.5.5"
 authors = [{ name = "Reiase", email = "reiase@gmail.com" }]
 description = "A hyper-parameter library for researchers, data scientists and machine learning engineers."
 requires-python = ">=3.7"
 readme = "README.md"
 license = { text = "Apache License Version 2.0" }
 
 [tool.maturin]
-module-name = "hyperparameter.rbackend"
+module-name = "hyperparameter.librbackend"
 features = ["pyo3/extension-module"]
 include = ["hyperparameter/hyperparameter.h"]
 
 [tool.black]
 line-length = 88
 
 [tool.flake8]
```

### Comparing `hyperparameter-0.5.4/run-maturin-action.sh` & `hyperparameter-0.5.5/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/src/entry.rs` & `hyperparameter-0.5.5/src/entry.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/src/ext.rs` & `hyperparameter-0.5.5/src/ext.rs`

 * *Files 0% similar despite different names*

```diff
@@ -197,12 +197,12 @@
 
 #[pyfunction]
 pub fn xxh64(s: &str) -> u64 {
     xxhstr(s)
 }
 
 #[pymodule]
-fn rbackend(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
+fn librbackend(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<KVStorage>()?;
     m.add_function(wrap_pyfunction!(xxh64, m)?)?;
     Ok(())
 }
```

### Comparing `hyperparameter-0.5.4/src/ffi.rs` & `hyperparameter-0.5.5/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/src/storage.rs` & `hyperparameter-0.5.5/src/storage.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/src/xxh.rs` & `hyperparameter-0.5.5/src/xxh.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/tests/a.out` & `hyperparameter-0.5.5/tests/a.out`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/tests/test_auto_param.py` & `hyperparameter-0.5.5/tests/test_auto_param.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/tests/test_param_scope.py` & `hyperparameter-0.5.5/tests/test_param_scope.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/tests/test_param_scope_thread.py` & `hyperparameter-0.5.5/tests/test_param_scope_thread.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.4/tests/test_rust_backend.py` & `hyperparameter-0.5.5/tests/test_rust_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from hyperparameter.rbackend import KVStorage
+from hyperparameter.librbackend import KVStorage
 
 
 class TestRBackend(TestCase):
     def test_kvstorage_create(self):
         s = KVStorage()
         self.assertDictEqual(s.storage(), {})
```

