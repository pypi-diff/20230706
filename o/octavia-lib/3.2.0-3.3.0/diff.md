# Comparing `tmp/octavia-lib-3.2.0.tar.gz` & `tmp/octavia-lib-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octavia-lib-3.2.0.tar", last modified: Fri Feb 10 16:30:12 2023, max compression
+gzip compressed data, was "octavia-lib-3.3.0.tar", last modified: Thu Jul  6 08:36:20 2023, max compression
```

## Comparing `octavia-lib-3.2.0.tar` & `octavia-lib-3.3.0.tar`

### file list

```diff
@@ -1,118 +1,120 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.903067 octavia-lib-3.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2510 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-02-10 16:30:12.000000 octavia-lib-3.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3796 2023-02-10 16:30:12.000000 octavia-lib-3.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3827 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-02-10 16:30:12.903067 octavia-lib-3.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.883067 octavia-lib-3.2.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.883067 octavia-lib-3.2.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.883067 octavia-lib-3.2.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/source/admin/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.883067 octavia-lib-3.2.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/source/cli/index.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4268 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.883067 octavia-lib-3.2.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.883067 octavia-lib-3.2.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.883067 octavia-lib-3.2.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.883067 octavia-lib-3.2.0/doc/source/library/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/source/library/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.883067 octavia-lib-3.2.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.883067 octavia-lib-3.2.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.887067 octavia-lib-3.2.0/octavia_lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.887067 octavia-lib-3.2.0/octavia_lib/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.891067 octavia-lib-3.2.0/octavia_lib/api/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/api/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12091 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/api/drivers/data_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10720 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/api/drivers/driver_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8947 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/api/drivers/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24798 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/api/drivers/provider_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.891067 octavia-lib-3.2.0/octavia_lib/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11202 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/common/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.891067 octavia-lib-3.2.0/octavia_lib/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11674 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.891067 octavia-lib-3.2.0/octavia_lib/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.891067 octavia-lib-3.2.0/octavia_lib/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.891067 octavia-lib-3.2.0/octavia_lib/tests/unit/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/unit/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.891067 octavia-lib-3.2.0/octavia_lib/tests/unit/api/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/unit/api/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20580 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/unit/api/drivers/test_data_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9187 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/unit/api/drivers/test_driver_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4468 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/unit/api/drivers/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5884 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/unit/api/drivers/test_provider_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.895067 octavia-lib-3.2.0/octavia_lib/tests/unit/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/unit/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9519 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/tests/unit/hacking/test_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/octavia_lib/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.887067 octavia-lib-3.2.0/octavia_lib.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-02-10 16:30:12.000000 octavia-lib-3.2.0/octavia_lib.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2023-02-10 16:30:12.000000 octavia-lib-3.2.0/octavia_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:30:12.000000 octavia-lib-3.2.0/octavia_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:30:12.000000 octavia-lib-3.2.0/octavia_lib.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-10 16:30:12.000000 octavia-lib-3.2.0/octavia_lib.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-02-10 16:30:12.000000 octavia-lib-3.2.0/octavia_lib.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-02-10 16:30:12.000000 octavia-lib-3.2.0/octavia_lib.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.879067 octavia-lib-3.2.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.899067 octavia-lib-3.2.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/Add-PROMETHEUS-listener-protocol-f2903d36f5da91e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/Add-get-methods-to-driver-lib-dae3c217e7ac9e82.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/Initial-cookiecutter-commit-41d89a60d6328b51.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-additional-vip-support-becdb29c5187b514.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-availability-zone-validation-ed853a3ee89570be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-az-to-loadbalancer-1e87b46ba29101d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-constants-66f52c4d4cfd0215.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-failover-stopped-status-722759b7432cad6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-lb-algorithm-source-ip-port-5cc83a9e3fcf4763.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-listener-allowed-cidrs-ef2cd3afbc3a1ebe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-listener-alpn-protocols-ecb49db86b956c71.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-not-found-exception-7f9d188cd22f69e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-pool-alpn-protocols-a791538ab214e780.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/add-tls-protocols-for-listener-and-pool-model-e9083b85afc62ef0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/adding-cipher-list-support-for-provider-drivers-6a4dbec2d0254aae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/drop-python-2-7-f17da6245b0ebc13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/notes/move-to-python-3.8-6a29d13144e8c378.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.899067 octavia-lib-3.2.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.899067 octavia-lib-3.2.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.903067 octavia-lib-3.2.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8520 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2023-02-10 16:30:12.903067 octavia-lib-3.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.903067 octavia-lib-3.2.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1615 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/tools/coding-checks.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3406 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:12.903067 octavia-lib-3.2.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-02-10 16:29:46.000000 octavia-lib-3.2.0/zuul.d/projects.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.351440 octavia-lib-3.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2510 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-07-06 08:36:20.000000 octavia-lib-3.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3893 2023-07-06 08:36:20.000000 octavia-lib-3.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3827 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-07-06 08:36:20.351440 octavia-lib-3.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/source/admin/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/source/cli/index.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4268 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/doc/source/library/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/source/library/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/octavia_lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/octavia_lib/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.347440 octavia-lib-3.3.0/octavia_lib/api/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/api/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12439 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/api/drivers/data_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10720 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/api/drivers/driver_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8947 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/api/drivers/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24798 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/api/drivers/provider_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.347440 octavia-lib-3.3.0/octavia_lib/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11314 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/common/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.347440 octavia-lib-3.3.0/octavia_lib/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11674 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.347440 octavia-lib-3.3.0/octavia_lib/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.347440 octavia-lib-3.3.0/octavia_lib/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.347440 octavia-lib-3.3.0/octavia_lib/tests/unit/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/unit/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.347440 octavia-lib-3.3.0/octavia_lib/tests/unit/api/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/unit/api/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20827 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/unit/api/drivers/test_data_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9187 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/unit/api/drivers/test_driver_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4468 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/unit/api/drivers/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5884 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/unit/api/drivers/test_provider_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.347440 octavia-lib-3.3.0/octavia_lib/tests/unit/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/unit/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9519 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/tests/unit/hacking/test_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/octavia_lib/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.343440 octavia-lib-3.3.0/octavia_lib.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-07-06 08:36:20.000000 octavia-lib-3.3.0/octavia_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3335 2023-07-06 08:36:20.000000 octavia-lib-3.3.0/octavia_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:36:20.000000 octavia-lib-3.3.0/octavia_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:36:20.000000 octavia-lib-3.3.0/octavia_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-06 08:36:20.000000 octavia-lib-3.3.0/octavia_lib.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-07-06 08:36:20.000000 octavia-lib-3.3.0/octavia_lib.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-07-06 08:36:20.000000 octavia-lib-3.3.0/octavia_lib.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.339440 octavia-lib-3.3.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.351440 octavia-lib-3.3.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/Add-PROMETHEUS-listener-protocol-f2903d36f5da91e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/Add-get-methods-to-driver-lib-dae3c217e7ac9e82.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/Added-HSTS-support-7d1fbfc35ee5dc29.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/Initial-cookiecutter-commit-41d89a60d6328b51.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-additional-vip-support-becdb29c5187b514.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-availability-zone-validation-ed853a3ee89570be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-az-to-loadbalancer-1e87b46ba29101d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-constants-66f52c4d4cfd0215.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-failover-stopped-status-722759b7432cad6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-lb-algorithm-source-ip-port-5cc83a9e3fcf4763.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-listener-allowed-cidrs-ef2cd3afbc3a1ebe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-listener-alpn-protocols-ecb49db86b956c71.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-not-found-exception-7f9d188cd22f69e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-pool-alpn-protocols-a791538ab214e780.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/add-tls-protocols-for-listener-and-pool-model-e9083b85afc62ef0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/adding-cipher-list-support-for-provider-drivers-6a4dbec2d0254aae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/drop-python-2-7-f17da6245b0ebc13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/notes/move-to-python-3.8-6a29d13144e8c378.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.351440 octavia-lib-3.3.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.351440 octavia-lib-3.3.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.351440 octavia-lib-3.3.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8520 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2023-07-06 08:36:20.351440 octavia-lib-3.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.351440 octavia-lib-3.3.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1615 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/tools/coding-checks.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3406 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:20.351440 octavia-lib-3.3.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-07-06 08:35:55.000000 octavia-lib-3.3.0/zuul.d/projects.yaml
```

### Comparing `octavia-lib-3.2.0/.pylintrc` & `octavia-lib-3.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/AUTHORS` & `octavia-lib-3.3.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/CONTRIBUTING.rst` & `octavia-lib-3.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/ChangeLog` & `octavia-lib-3.3.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+3.3.0
+-----
+
+* Add support for HTTP Strict Transport Security
+* Update master for stable/2023.1
+
 3.2.0
 -----
 
 * Fix tox4 error
 * Add \*.orig to .gitignore
 * Switch to 2023.1 Python3 unit tests and generic template name
 * Update master for stable/zed
```

### Comparing `octavia-lib-3.2.0/HACKING.rst` & `octavia-lib-3.3.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/LICENSE` & `octavia-lib-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/PKG-INFO` & `octavia-lib-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: octavia-lib
-Version: 3.2.0
+Version: 3.3.0
 Summary: A library to support Octavia provider drivers.
 Home-page: https://docs.openstack.org/octavia-lib/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `octavia-lib-3.2.0/README.rst` & `octavia-lib-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/doc/source/conf.py` & `octavia-lib-3.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/doc/source/index.rst` & `octavia-lib-3.3.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/doc/source/reference/index.rst` & `octavia-lib-3.3.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/__init__.py` & `octavia-lib-3.3.0/octavia_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/api/drivers/data_models.py` & `octavia-lib-3.3.0/octavia_lib/api/drivers/data_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
+import typing as tp
 
 
 class BaseDataModel():
     def to_dict(self, calling_classes=None, recurse=False,
                 render_unsets=False, **kwargs):
         """Converts a data model to a dictionary."""
         calling_classes = calling_classes or []
@@ -129,15 +130,16 @@
                  sni_container_data=Unset, timeout_client_data=Unset,
                  timeout_member_connect=Unset, timeout_member_data=Unset,
                  timeout_tcp_inspect=Unset, client_ca_tls_container_ref=Unset,
                  client_ca_tls_container_data=Unset,
                  client_authentication=Unset, client_crl_container_ref=Unset,
                  client_crl_container_data=Unset, project_id=Unset,
                  allowed_cidrs=Unset, tls_versions=Unset, tls_ciphers=Unset,
-                 alpn_protocols=Unset):
+                 alpn_protocols=Unset, hsts_max_age=Unset,
+                 hsts_include_subdomains=Unset, hsts_preload=Unset):
 
         self.admin_state_up = admin_state_up
         self.connection_limit = connection_limit
         self.default_pool = default_pool
         self.default_pool_id = default_pool_id
         self.default_tls_container_data = default_tls_container_data
         self.default_tls_container_ref = default_tls_container_ref
@@ -161,14 +163,18 @@
         self.client_crl_container_ref = client_crl_container_ref
         self.client_crl_container_data = client_crl_container_data
         self.project_id = project_id
         self.allowed_cidrs = allowed_cidrs
         self.tls_versions = tls_versions
         self.tls_ciphers = tls_ciphers
         self.alpn_protocols = alpn_protocols
+        self.hsts_max_age: tp.Union[int, UnsetType] = hsts_max_age
+        self.hsts_include_subdomains: tp.Union[bool, UnsetType] = (
+            hsts_include_subdomains)
+        self.hsts_preload: tp.Union[bool, UnsetType] = hsts_preload
 
 
 class Pool(BaseDataModel):
     def __init__(self, admin_state_up=Unset, description=Unset,
                  healthmonitor=Unset, lb_algorithm=Unset,
                  loadbalancer_id=Unset, members=Unset, name=Unset,
                  pool_id=Unset, listener_id=Unset, protocol=Unset,
```

### Comparing `octavia-lib-3.2.0/octavia_lib/api/drivers/driver_lib.py` & `octavia-lib-3.3.0/octavia_lib/api/drivers/driver_lib.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/api/drivers/exceptions.py` & `octavia-lib-3.3.0/octavia_lib/api/drivers/exceptions.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/api/drivers/provider_base.py` & `octavia-lib-3.3.0/octavia_lib/api/drivers/provider_base.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/common/constants.py` & `octavia-lib-3.3.0/octavia_lib/common/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,17 @@
 DELAY = 'delay'
 DESCRIPTION = 'description'
 DOMAIN_NAME = 'domain_name'
 EXPECTED_CODES = 'expected_codes'
 FALL_THRESHOLD = 'fall_threshold'
 HEALTHMONITOR = 'healthmonitor'
 HEALTHMONITOR_ID = 'healthmonitor_id'
+HSTS_MAX_AGE = 'hsts_max_age'
+HSTS_INCLUDE_SUBDOMAINS = 'hsts_include_subdomains'
+HSTS_PRELOAD = 'hsts_preload'
 HTTP_METHOD = 'http_method'
 HTTP_VERSION = 'http_version'
 INSERT_HEADERS = 'insert_headers'
 INTERMEDIATES = 'intermediates'
 INVERT = 'invert'
 KEY = 'key'
 L7POLICY_ID = 'l7policy_id'
```

### Comparing `octavia-lib-3.2.0/octavia_lib/hacking/checks.py` & `octavia-lib-3.3.0/octavia_lib/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/i18n.py` & `octavia-lib-3.3.0/octavia_lib/i18n.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/tests/unit/api/drivers/test_data_models.py` & `octavia-lib-3.3.0/octavia_lib/tests/unit/api/drivers/test_data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,19 @@
                           constants.TLS_VERSION_1,
                           constants.TLS_VERSION_1_1,
                           constants.TLS_VERSION_1_2,
                           constants.TLS_VERSION_1_3],
             tls_ciphers=None,
             alpn_protocols=[constants.ALPN_PROTOCOL_HTTP_1_0,
                             constants.ALPN_PROTOCOL_HTTP_1_1,
-                            constants.ALPN_PROTOCOL_HTTP_2])
+                            constants.ALPN_PROTOCOL_HTTP_2],
+            hsts_max_age=None,
+            hsts_include_subdomains=None,
+            hsts_preload=None,
+        )
 
         self.ref_lb = data_models.LoadBalancer(
             admin_state_up=False,
             description='One great load balancer',
             flavor={'cake': 'chocolate'},
             listeners=[self.ref_listener],
             loadbalancer_id=self.loadbalancer_id,
@@ -258,30 +262,35 @@
                              constants.TLS_VERSION_1,
                              constants.TLS_VERSION_1_1,
                              constants.TLS_VERSION_1_2,
                              constants.TLS_VERSION_1_3],
             'tls_ciphers': None,
             'alpn_protocols': [constants.ALPN_PROTOCOL_HTTP_1_0,
                                constants.ALPN_PROTOCOL_HTTP_1_1,
-                               constants.ALPN_PROTOCOL_HTTP_2]}
+                               constants.ALPN_PROTOCOL_HTTP_2],
+            'hsts_max_age': None,
+            'hsts_include_subdomains': None,
+            'hsts_preload': None,
+        }
 
         self.ref_lb_dict_with_listener = {
             'admin_state_up': False,
             'description': 'One great load balancer',
             'flavor': {'cake': 'chocolate'},
             'listeners': [self.ref_listener_dict],
             'loadbalancer_id': self.loadbalancer_id,
             'name': 'favorite_lb',
             'project_id': self.project_id,
             'vip_address': self.vip_address,
             'vip_network_id': self.vip_network_id,
             'vip_port_id': self.vip_port_id,
             'vip_subnet_id': self.vip_subnet_id,
             'vip_qos_policy_id': self.vip_qos_policy_id,
-            'availability_zone': self.availability_zone}
+            'availability_zone': self.availability_zone,
+        }
 
         self.ref_vip_dict = {
             'vip_address': self.vip_address,
             'vip_network_id': self.vip_network_id,
             'vip_port_id': self.vip_port_id,
             'vip_subnet_id': self.vip_subnet_id,
             'vip_qos_policy_id': self.vip_qos_policy_id}
```

### Comparing `octavia-lib-3.2.0/octavia_lib/tests/unit/api/drivers/test_driver_lib.py` & `octavia-lib-3.3.0/octavia_lib/tests/unit/api/drivers/test_driver_lib.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/tests/unit/api/drivers/test_exceptions.py` & `octavia-lib-3.3.0/octavia_lib/tests/unit/api/drivers/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/tests/unit/api/drivers/test_provider_base.py` & `octavia-lib-3.3.0/octavia_lib/tests/unit/api/drivers/test_provider_base.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/tests/unit/base.py` & `octavia-lib-3.3.0/octavia_lib/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/tests/unit/hacking/test_checks.py` & `octavia-lib-3.3.0/octavia_lib/tests/unit/hacking/test_checks.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib/version.py` & `octavia-lib-3.3.0/octavia_lib/version.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/octavia_lib.egg-info/PKG-INFO` & `octavia-lib-3.3.0/octavia_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: octavia-lib
-Version: 3.2.0
+Version: 3.3.0
 Summary: A library to support Octavia provider drivers.
 Home-page: https://docs.openstack.org/octavia-lib/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `octavia-lib-3.2.0/octavia_lib.egg-info/SOURCES.txt` & `octavia-lib-3.3.0/octavia_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 octavia_lib/tests/unit/api/drivers/test_driver_lib.py
 octavia_lib/tests/unit/api/drivers/test_exceptions.py
 octavia_lib/tests/unit/api/drivers/test_provider_base.py
 octavia_lib/tests/unit/hacking/__init__.py
 octavia_lib/tests/unit/hacking/test_checks.py
 releasenotes/notes/Add-PROMETHEUS-listener-protocol-f2903d36f5da91e5.yaml
 releasenotes/notes/Add-get-methods-to-driver-lib-dae3c217e7ac9e82.yaml
+releasenotes/notes/Added-HSTS-support-7d1fbfc35ee5dc29.yaml
 releasenotes/notes/Initial-cookiecutter-commit-41d89a60d6328b51.yaml
 releasenotes/notes/add-additional-vip-support-becdb29c5187b514.yaml
 releasenotes/notes/add-availability-zone-validation-ed853a3ee89570be.yaml
 releasenotes/notes/add-az-to-loadbalancer-1e87b46ba29101d3.yaml
 releasenotes/notes/add-constants-66f52c4d4cfd0215.yaml
 releasenotes/notes/add-failover-stopped-status-722759b7432cad6a.yaml
 releasenotes/notes/add-lb-algorithm-source-ip-port-5cc83a9e3fcf4763.yaml
@@ -67,14 +68,15 @@
 releasenotes/notes/add-listener-alpn-protocols-ecb49db86b956c71.yaml
 releasenotes/notes/add-not-found-exception-7f9d188cd22f69e1.yaml
 releasenotes/notes/add-pool-alpn-protocols-a791538ab214e780.yaml
 releasenotes/notes/add-tls-protocols-for-listener-and-pool-model-e9083b85afc62ef0.yaml
 releasenotes/notes/adding-cipher-list-support-for-provider-drivers-6a4dbec2d0254aae.yaml
 releasenotes/notes/drop-python-2-7-f17da6245b0ebc13.yaml
 releasenotes/notes/move-to-python-3.8-6a29d13144e8c378.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/ussuri.rst
 releasenotes/source/victoria.rst
```

### Comparing `octavia-lib-3.2.0/releasenotes/source/conf.py` & `octavia-lib-3.3.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/requirements.txt` & `octavia-lib-3.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/setup.cfg` & `octavia-lib-3.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/setup.py` & `octavia-lib-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/tools/coding-checks.sh` & `octavia-lib-3.3.0/tools/coding-checks.sh`

 * *Files identical despite different names*

### Comparing `octavia-lib-3.2.0/tox.ini` & `octavia-lib-3.3.0/tox.ini`

 * *Files identical despite different names*

