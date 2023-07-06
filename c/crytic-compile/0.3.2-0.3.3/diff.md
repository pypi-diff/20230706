# Comparing `tmp/crytic-compile-0.3.2.tar.gz` & `tmp/crytic-compile-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crytic-compile-0.3.2.tar", last modified: Fri Jun 23 16:19:02 2023, max compression
+gzip compressed data, was "crytic-compile-0.3.3.tar", last modified: Thu Jul  6 15:45:04 2023, max compression
```

## Comparing `crytic-compile-0.3.2.tar` & `crytic-compile-0.3.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.838333 crytic-compile-0.3.2/crytic_compile/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/compilation_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.838333 crytic-compile-0.3.2/crytic_compile/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    23466 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/crytic_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.838333 crytic-compile-0.3.2/crytic_compile/cryticparser/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/cryticparser/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15605 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/cryticparser/cryticparser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/cryticparser/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/crytic_compile/platform/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/abstract_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/all_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/all_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/archive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8496 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/brownie.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9543 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/buidler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8641 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/dapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10118 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/embark.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8281 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/etherlime.py
--rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/etherscan.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3417 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/foundry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12109 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/hardhat.py
--rw-r--r--   0 runner    (1001) docker     (123)    28897 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/solc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/solc_standard_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/standard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18595 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/truffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/vyper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13587 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/waffle.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/source_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/crytic_compile/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/name_collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/natspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/npm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/unit_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.838333 crytic-compile-0.3.2/crytic_compile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/tests/test_zip_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.609070 crytic-compile-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-06 15:45:04.609070 crytic-compile-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.601070 crytic-compile-0.3.3/crytic_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/compilation_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.601070 crytic-compile-0.3.3/crytic_compile/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23517 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/crytic_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.601070 crytic-compile-0.3.3/crytic_compile/cryticparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/cryticparser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15605 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/cryticparser/cryticparser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/cryticparser/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.605070 crytic-compile-0.3.3/crytic_compile/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/abstract_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/all_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/all_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8496 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/brownie.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9543 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/buidler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8641 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/dapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10118 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/embark.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8281 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/etherlime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/etherscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3417 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/foundry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12036 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/hardhat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28897 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/solc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/solc_standard_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/standard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18378 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/truffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/vyper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13370 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/source_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.609070 crytic-compile-0.3.3/crytic_compile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/name_collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/npm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/unit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.601070 crytic-compile-0.3.3/crytic_compile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 15:45:04.609070 crytic-compile-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.609070 crytic-compile-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/tests/test_zip_archive.py
```

### Comparing `crytic-compile-0.3.2/LICENSE` & `crytic-compile-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/PKG-INFO` & `crytic-compile-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: crytic-compile
-Version: 0.3.2
+Version: 0.3.3
 Summary: Util to facilitate smart contracts compilation.
 Home-page: https://github.com/crytic/crytic-compile
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # Crytic-compile
-[![Build Status](https://img.shields.io/github/workflow/status/crytic/crytic-compile/CI/master)](https://github.com/crytic/crytic-compile/actions?query=workflow%3ACI)
-[![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/crytic/crytic-compile/ci.yml?branch=master)](https://github.com/crytic/crytic-compile/actions?query=workflow%3ACI)
+[![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc)
 [![PyPI version](https://badge.fury.io/py/crytic-compile.svg)](https://badge.fury.io/py/crytic-compile)
 
 Library to help smart contract compilation. It includes support for:
 - Direct solc compilation
 - [Brownie](https://github.com/iamdefinitelyahuman/brownie)
 - [Buidler](https://github.com/nomiclabs/buidler)
 - [Dapp](https://dapp.tools/dapp/)
```

### Comparing `crytic-compile-0.3.2/README.md` & `crytic-compile-0.3.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Crytic-compile
-[![Build Status](https://img.shields.io/github/workflow/status/crytic/crytic-compile/CI/master)](https://github.com/crytic/crytic-compile/actions?query=workflow%3ACI)
-[![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/crytic/crytic-compile/ci.yml?branch=master)](https://github.com/crytic/crytic-compile/actions?query=workflow%3ACI)
+[![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc)
 [![PyPI version](https://badge.fury.io/py/crytic-compile.svg)](https://badge.fury.io/py/crytic-compile)
 
 Library to help smart contract compilation. It includes support for:
 - Direct solc compilation
 - [Brownie](https://github.com/iamdefinitelyahuman/brownie)
 - [Buidler](https://github.com/nomiclabs/buidler)
 - [Dapp](https://dapp.tools/dapp/)
```

### Comparing `crytic-compile-0.3.2/crytic_compile/__main__.py` & `crytic-compile-0.3.3/crytic_compile/__main__.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/compilation_unit.py` & `crytic-compile-0.3.3/crytic_compile/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/compiler/compiler.py` & `crytic-compile-0.3.3/crytic_compile/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/crytic_compile.py` & `crytic-compile-0.3.3/crytic_compile/crytic_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
 logging.basicConfig()
 
 
 # pylint: disable=too-many-lines
 
 
 def get_platforms() -> List[Type[AbstractPlatform]]:
-    """Return the available platforms classes
+    """Return the available platforms classes in order of preference
 
     Returns:
         List[Type[AbstractPlatform]]: Available platforms
     """
     platforms = [getattr(all_platforms, name) for name in dir(all_platforms)]
     platforms = [d for d in platforms if inspect.isclass(d) and issubclass(d, AbstractPlatform)]
-    return sorted(platforms, key=lambda platform: platform.TYPE)
+    return sorted(platforms, key=lambda platform: (platform.TYPE.priority(), platform.TYPE))
 
 
 def is_supported(target: str) -> bool:
     """Check if the target is supporte. Iterate over all known platforms
 
     Args:
         target (str): path to the target
```

### Comparing `crytic-compile-0.3.2/crytic_compile/cryticparser/cryticparser.py` & `crytic-compile-0.3.3/crytic_compile/cryticparser/cryticparser.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/cryticparser/defaults.py` & `crytic-compile-0.3.3/crytic_compile/cryticparser/defaults.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/abstract_platform.py` & `crytic-compile-0.3.3/crytic_compile/platform/abstract_platform.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/all_platforms.py` & `crytic-compile-0.3.3/crytic_compile/platform/all_platforms.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/archive.py` & `crytic-compile-0.3.3/crytic_compile/platform/archive.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/brownie.py` & `crytic-compile-0.3.3/crytic_compile/platform/brownie.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/buidler.py` & `crytic-compile-0.3.3/crytic_compile/platform/buidler.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/dapp.py` & `crytic-compile-0.3.3/crytic_compile/platform/dapp.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/embark.py` & `crytic-compile-0.3.3/crytic_compile/platform/embark.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/etherlime.py` & `crytic-compile-0.3.3/crytic_compile/platform/etherlime.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/etherscan.py` & `crytic-compile-0.3.3/crytic_compile/platform/etherscan.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/foundry.py` & `crytic-compile-0.3.3/crytic_compile/platform/foundry.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/hardhat.py` & `crytic-compile-0.3.3/crytic_compile/platform/hardhat.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,20 +208,18 @@
         Returns:
             bool: True if the target is an hardhat project
         """
         hardhat_ignore = kwargs.get("hardhat_ignore", False)
         if hardhat_ignore:
             return False
 
-        # If there is both foundry and hardhat, foundry takes priority
-        if os.path.isfile(os.path.join(target, "foundry.toml")):
-            return False
-
-        return os.path.isfile(os.path.join(target, "hardhat.config.js")) | os.path.isfile(
-            os.path.join(target, "hardhat.config.ts")
+        return (
+            os.path.isfile(os.path.join(target, "hardhat.config.js"))
+            or os.path.isfile(os.path.join(target, "hardhat.config.ts"))
+            or os.path.isfile(os.path.join(target, "hardhat.config.cjs"))
         )
 
     def is_dependency(self, path: str) -> bool:
         """Check if the path is a dependency
 
         Args:
             path (str): path to the target
```

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/solc.py` & `crytic-compile-0.3.3/crytic_compile/platform/solc.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/solc_standard_json.py` & `crytic-compile-0.3.3/crytic_compile/platform/solc_standard_json.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/standard.py` & `crytic-compile-0.3.3/crytic_compile/platform/standard.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/truffle.py` & `crytic-compile-0.3.3/crytic_compile/platform/truffle.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,20 +301,14 @@
         Returns:
             bool: True if the target is a truffle project
         """
         truffle_ignore = kwargs.get("truffle_ignore", False)
         if truffle_ignore:
             return False
 
-        # Avoid conflicts with hardhat
-        if os.path.isfile(os.path.join(target, "hardhat.config.js")) | os.path.isfile(
-            os.path.join(target, "hardhat.config.ts")
-        ):
-            return False
-
         return os.path.isfile(os.path.join(target, "truffle.js")) or os.path.isfile(
             os.path.join(target, "truffle-config.js")
         )
 
     # pylint: disable=no-self-use
     def is_dependency(self, path: str) -> bool:
         """Check if the path is a dependency
```

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/types.py` & `crytic-compile-0.3.3/crytic_compile/platform/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -62,7 +62,28 @@
         if self == Type.BUILDER:
             return "Builder"
         if self == Type.BROWNIE:
             return "Browner"
         if self == Type.FOUNDRY:
             return "Foundry"
         raise ValueError
+
+    def priority(self) -> int:
+        """Return the priority for a certain platform.
+
+        A lower priority means the platform is more preferable. This is used to
+        consistently select a platform when two or more are available.
+
+        Returns:
+            int: priority number
+        """
+
+        if self == Type.FOUNDRY:
+            return 100
+
+        if self == Type.HARDHAT:
+            return 200
+
+        if self in [Type.TRUFFLE, Type.WAFFLE]:
+            return 300
+
+        return 1000
```

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/vyper.py` & `crytic-compile-0.3.3/crytic_compile/platform/vyper.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/platform/waffle.py` & `crytic-compile-0.3.3/crytic_compile/platform/waffle.py`

 * *Files 5% similar despite different names*

```diff
@@ -241,20 +241,14 @@
         Returns:
             bool: True if the target is a waffle project
         """
         waffle_ignore = kwargs.get("waffle_ignore", False)
         if waffle_ignore:
             return False
 
-        # Avoid conflicts with hardhat
-        if os.path.isfile(os.path.join(target, "hardhat.config.js")) | os.path.isfile(
-            os.path.join(target, "hardhat.config.ts")
-        ):
-            return False
-
         if os.path.isfile(os.path.join(target, "waffle.json")) or os.path.isfile(
             os.path.join(target, ".waffle.json")
         ):
             return True
 
         if os.path.isfile(os.path.join(target, "package.json")):
             with open(os.path.join(target, "package.json"), encoding="utf8") as file_desc:
```

### Comparing `crytic-compile-0.3.2/crytic_compile/source_unit.py` & `crytic-compile-0.3.3/crytic_compile/source_unit.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/utils/naming.py` & `crytic-compile-0.3.3/crytic_compile/utils/naming.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/utils/natspec.py` & `crytic-compile-0.3.3/crytic_compile/utils/natspec.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/utils/npm.py` & `crytic-compile-0.3.3/crytic_compile/utils/npm.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/utils/subprocess.py` & `crytic-compile-0.3.3/crytic_compile/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/utils/unit_tests.py` & `crytic-compile-0.3.3/crytic_compile/utils/unit_tests.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile/utils/zip.py` & `crytic-compile-0.3.3/crytic_compile/utils/zip.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/crytic_compile.egg-info/PKG-INFO` & `crytic-compile-0.3.3/crytic_compile.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: crytic-compile
-Version: 0.3.2
+Version: 0.3.3
 Summary: Util to facilitate smart contracts compilation.
 Home-page: https://github.com/crytic/crytic-compile
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # Crytic-compile
-[![Build Status](https://img.shields.io/github/workflow/status/crytic/crytic-compile/CI/master)](https://github.com/crytic/crytic-compile/actions?query=workflow%3ACI)
-[![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/crytic/crytic-compile/ci.yml?branch=master)](https://github.com/crytic/crytic-compile/actions?query=workflow%3ACI)
+[![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc)
 [![PyPI version](https://badge.fury.io/py/crytic-compile.svg)](https://badge.fury.io/py/crytic-compile)
 
 Library to help smart contract compilation. It includes support for:
 - Direct solc compilation
 - [Brownie](https://github.com/iamdefinitelyahuman/brownie)
 - [Buidler](https://github.com/nomiclabs/buidler)
 - [Dapp](https://dapp.tools/dapp/)
```

### Comparing `crytic-compile-0.3.2/crytic_compile.egg-info/SOURCES.txt` & `crytic-compile-0.3.3/crytic_compile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/pyproject.toml` & `crytic-compile-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/setup.py` & `crytic-compile-0.3.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     long_description = f.read()
 
 setup(
     name="crytic-compile",
     description="Util to facilitate smart contracts compilation.",
     url="https://github.com/crytic/crytic-compile",
     author="Trail of Bits",
-    version="0.3.2",
+    version="0.3.3",
     packages=find_packages(),
     python_requires=">=3.8",
-    install_requires=["pycryptodome>=3.4.6", "cbor2", "solc-select>=v1.0.2"],
+    install_requires=["pycryptodome>=3.4.6", "cbor2", "solc-select>=v1.0.4"],
     extras_require={
         "test": [
             "pytest",
             "pytest-cov",
         ],
         "lint": [
             "black==22.3.0",
@@ -31,10 +31,11 @@
         ],
         "dev": [
             "crytic-compile[test,doc,lint]",
         ],
     },
     license="AGPL-3.0",
     long_description=long_description,
+    long_description_content_type="text/markdown",
     package_data={"crytic_compile": ["py.typed"]},
     entry_points={"console_scripts": ["crytic-compile = crytic_compile.__main__:main"]},
 )
```

### Comparing `crytic-compile-0.3.2/tests/test_metadata.py` & `crytic-compile-0.3.3/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.2/tests/test_zip_archive.py` & `crytic-compile-0.3.3/tests/test_zip_archive.py`

 * *Files identical despite different names*

