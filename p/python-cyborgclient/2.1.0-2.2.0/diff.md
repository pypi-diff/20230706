# Comparing `tmp/python-cyborgclient-2.1.0.tar.gz` & `tmp/python-cyborgclient-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cyborgclient-2.1.0.tar", last modified: Fri Feb 17 10:37:46 2023, max compression
+gzip compressed data, was "python-cyborgclient-2.2.0.tar", last modified: Thu Jul  6 08:34:42 2023, max compression
```

## Comparing `python-cyborgclient-2.1.0.tar` & `python-cyborgclient-2.2.0.tar`

### file list

```diff
@@ -1,139 +1,141 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.211667 python-cyborgclient-2.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2023-02-17 10:37:46.000000 python-cyborgclient-2.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3525 2023-02-17 10:37:46.000000 python-cyborgclient-2.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5946 2023-02-17 10:37:46.211667 python-cyborgclient-2.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.199667 python-cyborgclient-2.1.0/cyborgclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.199667 python-cyborgclient-2.1.0/cyborgclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.199667 python-cyborgclient-2.1.0/cyborgclient/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3516 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/common/apiclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12412 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/common/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4746 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16061 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/common/cliutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13131 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/common/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16234 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/common/httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15110 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.199667 python-cyborgclient-2.1.0/cyborgclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4092 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/osc/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.203667 python-cyborgclient-2.1.0/cyborgclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/osc/v1/accelerator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.203667 python-cyborgclient-2.1.0/cyborgclient/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10625 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/osc/v2/accelerator_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5293 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/osc/v2/deployable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3913 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/osc/v2/device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6208 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/osc/v2/device_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26206 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.203667 python-cyborgclient-2.1.0/cyborgclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.203667 python-cyborgclient-2.1.0/cyborgclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/test_cyborgclient.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.203667 python-cyborgclient-2.1.0/cyborgclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1895 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.203667 python-cyborgclient-2.1.0/cyborgclient/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12756 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/common/test_httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/common/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.203667 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1845 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.203667 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4109 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8646 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/test_accelerator_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2967 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/test_deployable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3061 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/test_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6309 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/test_device_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11138 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5689 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.203667 python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/shell_test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2847 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/test_accelerators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/test_accelerators_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2634 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6284 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/test_deployables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/cyborgclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/v1/accelerators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/v1/accelerators_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4208 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/v1/basemodels.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7165 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2796 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/v1/deployables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/v1/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/cyborgclient/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/source/admin/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/source/cli/index.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2594 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/doc/source/library/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/source/library/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/python_cyborgclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5946 2023-02-17 10:37:46.000000 python-cyborgclient-2.1.0/python_cyborgclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2023-02-17 10:37:46.000000 python-cyborgclient-2.1.0/python_cyborgclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 10:37:46.000000 python-cyborgclient-2.1.0/python_cyborgclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2023-02-17 10:37:46.000000 python-cyborgclient-2.1.0/python_cyborgclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 10:37:46.000000 python-cyborgclient-2.1.0/python_cyborgclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-17 10:37:46.000000 python-cyborgclient-2.1.0/python_cyborgclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-02-17 10:37:46.000000 python-cyborgclient-2.1.0/python_cyborgclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-02-17 10:37:46.000000 python-cyborgclient-2.1.0/python_cyborgclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.195667 python-cyborgclient-2.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.207667 python-cyborgclient-2.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/notes/drop-py-2-7-d47826d4387f40fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/notes/show-dp-by-name-4d22b106b718f215.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/notes/support-project-id-931fc61c818da675.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.211667 python-cyborgclient-2.1.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.211667 python-cyborgclient-2.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:46.211667 python-cyborgclient-2.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8815 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2336 2023-02-17 10:37:46.211667 python-cyborgclient-2.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2023-02-17 10:36:51.000000 python-cyborgclient-2.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.700852 python-cyborgclient-2.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1219 2023-07-06 08:34:42.000000 python-cyborgclient-2.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4378 2023-07-06 08:34:42.000000 python-cyborgclient-2.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5946 2023-07-06 08:34:42.700852 python-cyborgclient-2.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.684852 python-cyborgclient-2.2.0/cyborgclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.684852 python-cyborgclient-2.2.0/cyborgclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.684852 python-cyborgclient-2.2.0/cyborgclient/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3516 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/common/apiclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12412 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/common/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4746 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16061 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/common/cliutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13131 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/common/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16234 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/common/httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15110 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.684852 python-cyborgclient-2.2.0/cyborgclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4092 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/osc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.688852 python-cyborgclient-2.2.0/cyborgclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/osc/v1/accelerator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.688852 python-cyborgclient-2.2.0/cyborgclient/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10625 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/osc/v2/accelerator_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5905 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/osc/v2/attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5293 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/osc/v2/deployable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3913 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/osc/v2/device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6333 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/osc/v2/device_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26205 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.688852 python-cyborgclient-2.2.0/cyborgclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.688852 python-cyborgclient-2.2.0/cyborgclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/test_cyborgclient.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.688852 python-cyborgclient-2.2.0/cyborgclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1895 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.688852 python-cyborgclient-2.2.0/cyborgclient/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12756 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/common/test_httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/common/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.688852 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1845 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.692852 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4641 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9018 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/test_accelerator_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7089 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/test_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4684 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/test_deployable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5033 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/test_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7870 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/test_device_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11138 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5689 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.692852 python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/shell_test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2847 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/test_accelerators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/test_accelerators_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2634 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6284 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/test_deployables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.692852 python-cyborgclient-2.2.0/cyborgclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/v1/accelerators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/v1/accelerators_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4208 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/v1/basemodels.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7165 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2796 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/v1/deployables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/v1/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/cyborgclient/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.692852 python-cyborgclient-2.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.692852 python-cyborgclient-2.2.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.692852 python-cyborgclient-2.2.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/source/admin/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.692852 python-cyborgclient-2.2.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/source/cli/index.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2594 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.692852 python-cyborgclient-2.2.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.696852 python-cyborgclient-2.2.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.696852 python-cyborgclient-2.2.0/doc/source/library/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/source/library/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.696852 python-cyborgclient-2.2.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.696852 python-cyborgclient-2.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.696852 python-cyborgclient-2.2.0/python_cyborgclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5946 2023-07-06 08:34:42.000000 python-cyborgclient-2.2.0/python_cyborgclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3581 2023-07-06 08:34:42.000000 python-cyborgclient-2.2.0/python_cyborgclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:34:42.000000 python-cyborgclient-2.2.0/python_cyborgclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2023-07-06 08:34:42.000000 python-cyborgclient-2.2.0/python_cyborgclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:34:42.000000 python-cyborgclient-2.2.0/python_cyborgclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-06 08:34:42.000000 python-cyborgclient-2.2.0/python_cyborgclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-07-06 08:34:42.000000 python-cyborgclient-2.2.0/python_cyborgclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-07-06 08:34:42.000000 python-cyborgclient-2.2.0/python_cyborgclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.680852 python-cyborgclient-2.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.696852 python-cyborgclient-2.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/notes/drop-py-2-7-d47826d4387f40fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/notes/show-dp-by-name-4d22b106b718f215.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/notes/support-project-id-931fc61c818da675.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.700852 python-cyborgclient-2.2.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.700852 python-cyborgclient-2.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:42.700852 python-cyborgclient-2.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8815 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2668 2023-07-06 08:34:42.700852 python-cyborgclient-2.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2023-07-06 08:34:00.000000 python-cyborgclient-2.2.0/tox.ini
```

### Comparing `python-cyborgclient-2.1.0/AUTHORS` & `python-cyborgclient-2.2.0/AUTHORS`

 * *Files 9% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 Xinran WANG <xin-ran.wang@intel.com>
 Xinran Wang <xin-ran.wang@intel.com>
 XinxinShen <shenxinxin@inspur.com>
 Yumeng_Bao <yumeng_bao@yahoo.com>
 Zane Bitter <zbitter@redhat.com>
 ericxiett <eric_xiett@163.com>
 huang.zhiping <huang.zhiping@99cloud.net>
+jiangzhilin <jiangzhilin@inspur.com>
+leiyuehui <leiyuehui-s@inspur.com>
 lvxianguo <lvxianguo@inspur.com>
 niuke <niuke19970315@163.com>
 pengyuesheng <pengyuesheng@gohighsec.com>
 qiufossen <qiujunting@inspur.com>
 songwenping <songwenping@inspur.com>
 tomas <zhangchg03@inspur.com>
 wangqi <wang.qi@99cloud.net>
 wangzh21 <wangzh21@lenovo.com>
+wangzhiguang <wangzhiguang@inspur.com>
 wu.shiming <wushiming@yovole.com>
 yangyawei <yangyawei@inspur.com>
 zhangbailin <zhangbailin@inspur.com>
 zhangboye <zhangboye@inspur.com>
```

### Comparing `python-cyborgclient-2.1.0/CONTRIBUTING.rst` & `python-cyborgclient-2.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/ChangeLog` & `python-cyborgclient-2.2.0/ChangeLog`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,34 @@
 CHANGES
 =======
 
+2.2.0
+-----
+
+* add negative unit test for delete attribute
+* add negative unit test for delete device profile
+* add negative unit test for show device
+* add negative unit test for show deployable
+* Follow pep8
+* Add ut for show not exist device\_profile client api
+* Add ut for show not exist attribute client api
+* add ut for get deployable client api
+* add ut for get device client api
+* Add ut for delete attribute client api
+* add unittest for delete accelerator request client api
+* add unittest for delete device profile client api
+* improve doc format
+* Add ut for get attribute client api
+* Add ut for create attribute client api
+* Add ut for list attribute client api
+* Add client API for accelerator attribute show
+* Add client API for accelerator attribute delete
+* Add client API for accelerator attribute create
+* Add Attribute api client
+
 2.1.0
 -----
 
 * Use py3 as the default runtime for tox
 * Switch to 2023.1 Python3 unit tests and generic template name
 * Update master for stable/zed
```

### Comparing `python-cyborgclient-2.1.0/LICENSE` & `python-cyborgclient-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/PKG-INFO` & `python-cyborgclient-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-cyborgclient
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python client for cyborg API
 Home-page: https://docs.openstack.org/python-cyborgclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-cyborgclient-2.1.0/README.rst` & `python-cyborgclient-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/__init__.py` & `python-cyborgclient-2.2.0/cyborgclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/common/apiclient/base.py` & `python-cyborgclient-2.2.0/cyborgclient/common/apiclient/base.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/common/apiclient/exceptions.py` & `python-cyborgclient-2.2.0/cyborgclient/common/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/common/base.py` & `python-cyborgclient-2.2.0/cyborgclient/common/base.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/common/cliutils.py` & `python-cyborgclient-2.2.0/cyborgclient/common/cliutils.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/common/http.py` & `python-cyborgclient-2.2.0/cyborgclient/common/http.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/common/httpclient.py` & `python-cyborgclient-2.2.0/cyborgclient/common/httpclient.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/common/utils.py` & `python-cyborgclient-2.2.0/cyborgclient/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/exceptions.py` & `python-cyborgclient-2.2.0/cyborgclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/i18n.py` & `python-cyborgclient-2.2.0/cyborgclient/i18n.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/osc/plugin.py` & `python-cyborgclient-2.2.0/cyborgclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/osc/v1/accelerator.py` & `python-cyborgclient-2.2.0/cyborgclient/osc/v1/accelerator.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/osc/v2/accelerator_request.py` & `python-cyborgclient-2.2.0/cyborgclient/osc/v2/accelerator_request.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/osc/v2/deployable.py` & `python-cyborgclient-2.2.0/cyborgclient/osc/v2/deployable.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/osc/v2/device.py` & `python-cyborgclient-2.2.0/cyborgclient/osc/v2/device.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/osc/v2/device_profile.py` & `python-cyborgclient-2.2.0/cyborgclient/osc/v2/device_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,14 +127,16 @@
         acc_client = self.app.client_manager.accelerator
 
         failures = []
         for uuid in parsed_args.device_profiles:
             try:
                 acc_client.delete_device_profile(uuid, False)
                 print(_('Deleted device_profile %s') % uuid)
+            except sdk_exc.ResourceNotFound:
+                raise exc.CommandError(_('device_profile %s not found') % uuid)
             except exc.ClientException as e:
                 failures.append(_("Failed to delete device_profile \
                                 %(device_profile)s: %(error)s")
                                 % {'uuid': uuid, 'error': e})
         if failures:
             raise exc.ClientException("\n".join(failures))
```

### Comparing `python-cyborgclient-2.1.0/cyborgclient/shell.py` & `python-cyborgclient-2.2.0/cyborgclient/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 import os
 import sys
 
 from oslo_utils import encodeutils
 from oslo_utils import importutils
 from oslo_utils import strutils
 
+from cyborgclient.common import cliutils
+from cyborgclient import exceptions as exc
+from cyborgclient.i18n import _
+from cyborgclient.v1 import client as client_v1
+from cyborgclient.v1 import shell as shell_v1
+from cyborgclient import version
 
 profiler = importutils.try_import("osprofiler.profiler")
 
 HAS_KEYRING = False
 all_errors = ValueError
 try:
     import keyring
@@ -46,21 +52,14 @@
                           gnomekeyring.IOError,
                           gnomekeyring.NoKeyringDaemonError)
     except Exception:
         pass
 except ImportError:
     pass
 
-from cyborgclient.common import cliutils
-from cyborgclient import exceptions as exc
-from cyborgclient.i18n import _
-from cyborgclient.v1 import client as client_v1
-from cyborgclient.v1 import shell as shell_v1
-from cyborgclient import version
-
 LATEST_API_VERSION = ('1', 'latest')
 DEFAULT_INTERFACE = 'public'
 DEFAULT_SERVICE_TYPE = 'accelerator'
 
 logger = logging.getLogger(__name__)
```

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/base.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/base.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/test_cyborgclient.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/test_cyborgclient.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/base.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/common/test_httpclient.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/common/test_httpclient.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/common/test_utils.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/fakes.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/fakes.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/test_plugin.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/test_plugin.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/fakes.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/fakes.py`

 * *Files 15% similar despite different names*

```diff
@@ -104,14 +104,32 @@
     'hostname': accelerator_request_hostname,
     'device_rp_uuid': accelerator_request_device_rp_uuid,
     'instance_uuid': accelerator_request_instance_uuid,
     'attach_handle_type': accelerator_request_attach_handle_type,
     'attach_handle_info': accelerator_request_attach_handle_info,
 }
 
+attribute_created_at = '2023-05-17T00:00:00.000000+00:00'
+attribute_updated_at = '2023-05-17T11:11:11.111111+11:11'
+attribute_id = 1
+attribute_uuid = uuid.uuid4().hex
+attribute_deployable_id = 'fake_attribute_name'
+attribute_key = 'traits1'
+attribute_value = 'CUSTOM_FAKE_DEVICE'
+
+ATTRIBUTE = {
+    'created_at': attribute_created_at,
+    'updated_at': attribute_updated_at,
+    'id': attribute_id,
+    'uuid': attribute_uuid,
+    'deployable_id': attribute_deployable_id,
+    'key': attribute_key,
+    'value': attribute_value,
+}
+
 
 class TestAccelerator(utils.TestCommand):
 
     def setUp(self):
         super(TestAccelerator, self).setUp()
 
         self.app.client_manager.auth_ref = mock.MagicMock(auth_token="TOKEN")
```

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/test_accelerator_request.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/test_accelerator_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,23 @@
         result = self.assertRaises(exc.ClientException,
                                    self.cmd.take_action,
                                    parsed_args)
         self.assertIn("No accelerator_request with UUID " +
                       acc_fakes.accelerator_request_uuid + " exists",
                       str(result))
 
+    def test_accelerator_request_delete(self):
+        arglist = [acc_fakes.accelerator_request_uuid]
+        verifylist = []
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+        self.cmd.take_action(parsed_args)
+
+        self.mock_acc_client.delete_accelerator_request.assert_called_with(
+            acc_fakes.accelerator_request_uuid, False)
+
 
 class TestAcceleratorRequestCreate(TestAcceleratorRequest):
 
     def setUp(self):
         super(TestAcceleratorRequestCreate, self).setUp()
 
         fake_arq = acc_fakes.FakeAcceleratorResource(
```

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/test_deployable.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/test_deployable.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 #
+
+
 import copy
 
+from cyborgclient import exceptions as exc
 from cyborgclient.osc.v2 import deployable as osc_deployable
 from cyborgclient.tests.unit.osc.v2 import fakes as acc_fakes
+from openstack import exceptions as sdk_exc
 
 
 class TestDeployable(acc_fakes.TestAccelerator):
 
     def setUp(self):
         super(TestDeployable, self).setUp()
 
@@ -90,7 +94,57 @@
             acc_fakes.deployable_parent_id,
             acc_fakes.deployable_root_id,
             acc_fakes.deployable_name,
             acc_fakes.deployable_num_accelerators,
             acc_fakes.deployable_device_id,
         ), ]
         self.assertEqual(datalist, list(data))
+
+
+class TestDeployableShow(TestDeployable):
+
+    def setUp(self):
+        super(TestDeployableShow, self).setUp()
+
+        fake_arq = acc_fakes.FakeAcceleratorResource(
+            None,
+            copy.deepcopy(acc_fakes.DEPLOYABLE),
+            loaded=True)
+        self.mock_acc_client.get_deployable.return_value = fake_arq
+        self.cmd = osc_deployable.ShowDeployable(self.app, None)
+
+    def test_deployable_show(self):
+        arglist = [acc_fakes.deployable_uuid]
+        verifylist = []
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+        columns, data = self.cmd.take_action(parsed_args)
+
+        self.mock_acc_client.get_deployable.assert_called_with(
+            acc_fakes.deployable_uuid)
+
+        collist = (
+            'created_at',
+            'updated_at',
+            'uuid',
+            'name'
+        )
+
+        self.assertEqual(collist, columns)
+
+        datalist = [
+            acc_fakes.deployable_created_at,
+            acc_fakes.deployable_updated_at,
+            acc_fakes.deployable_uuid,
+            acc_fakes.deployable_name
+        ]
+        self.assertEqual(datalist, list(data))
+
+    def test_deployable_show_not_exist(self):
+        get_arq_req = self.mock_acc_client.get_deployable
+        get_arq_req.side_effect = sdk_exc.ResourceNotFound
+        arglist = [acc_fakes.deployable_uuid]
+        verifylist = []
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+        self.assertRaisesRegex(
+            exc.CommandError,
+            'deployable not found: %s' % acc_fakes.deployable_uuid,
+            self.cmd.take_action, parsed_args)
```

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/osc/v2/test_device_profile.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/osc/v2/test_device_profile.py`

 * *Files 19% similar despite different names*

```diff
@@ -133,14 +133,25 @@
         )
         formatters = {'data': utils.json_formatter}
         expected = oscutils.get_dict_properties(acc_fakes.DEVICE_PROFILE,
                                                 columns,
                                                 formatters=formatters)
         self.assertEqual(result, (columns, expected))
 
+    def test_device_profile_show_not_exist(self):
+        get_arq_req = self.mock_acc_client.get_device_profile
+        get_arq_req.side_effect = sdk_exc.ResourceNotFound
+        arglist = [acc_fakes.device_profile_name]
+        verifylist = []
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+        self.assertRaisesRegex(
+            exc.CommandError,
+            'device_profile %s not found' % acc_fakes.device_profile_name,
+            self.cmd.take_action, parsed_args)
+
 
 class TestDeviceProfileCreate(TestDeviceProfile):
 
     def setUp(self):
         super(TestDeviceProfileCreate, self).setUp()
 
         fake_dp = acc_fakes.FakeAcceleratorResource(
@@ -175,7 +186,35 @@
             acc_fakes.device_profile_updated_at,
             acc_fakes.device_profile_uuid,
             acc_fakes.device_profile_name,
             acc_fakes.device_profile_groups,
             acc_fakes.device_profile_description,
         ]
         self.assertEqual(datalist, list(data))
+
+
+class TestDeviceProfileDelete(TestDeviceProfile):
+
+    def setUp(self):
+        super(TestDeviceProfileDelete, self).setUp()
+        self.cmd = osc_device_profile.DeleteDeviceProfile(self.app, None)
+
+    def test_device_profile_delete(self):
+
+        arglist = [acc_fakes.device_profile_uuid]
+        verifylist = []
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+        self.cmd.take_action(parsed_args)
+
+        self.mock_acc_client.delete_device_profile.assert_called_with(
+            acc_fakes.device_profile_uuid, False)
+
+    def test_device_profile_delete_not_exist(self):
+        get_arq_req = self.mock_acc_client.delete_device_profile
+        get_arq_req.side_effect = sdk_exc.ResourceNotFound
+        arglist = [acc_fakes.device_profile_uuid]
+        verifylist = []
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+        self.assertRaisesRegex(
+            exc.CommandError,
+            'device_profile %s not found' % acc_fakes.device_profile_uuid,
+            self.cmd.take_action, parsed_args)
```

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/test_shell.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/utils.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/shell_test_base.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/shell_test_base.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/test_accelerators.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/test_accelerators.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/test_accelerators_shell.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/test_accelerators_shell.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/test_client.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/tests/unit/v1/test_deployables.py` & `python-cyborgclient-2.2.0/cyborgclient/tests/unit/v1/test_deployables.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/v1/accelerators.py` & `python-cyborgclient-2.2.0/cyborgclient/v1/accelerators.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/v1/accelerators_shell.py` & `python-cyborgclient-2.2.0/cyborgclient/v1/accelerators_shell.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/v1/basemodels.py` & `python-cyborgclient-2.2.0/cyborgclient/v1/basemodels.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/v1/client.py` & `python-cyborgclient-2.2.0/cyborgclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/v1/deployables.py` & `python-cyborgclient-2.2.0/cyborgclient/v1/deployables.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/v1/shell.py` & `python-cyborgclient-2.2.0/cyborgclient/v1/shell.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/cyborgclient/version.py` & `python-cyborgclient-2.2.0/cyborgclient/version.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/doc/source/conf.py` & `python-cyborgclient-2.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/doc/source/contributor/contributing.rst` & `python-cyborgclient-2.2.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/doc/source/index.rst` & `python-cyborgclient-2.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/python_cyborgclient.egg-info/PKG-INFO` & `python-cyborgclient-2.2.0/python_cyborgclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-cyborgclient
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python client for cyborg API
 Home-page: https://docs.openstack.org/python-cyborgclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-cyborgclient-2.1.0/python_cyborgclient.egg-info/SOURCES.txt` & `python-cyborgclient-2.2.0/python_cyborgclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 cyborgclient/common/apiclient/exceptions.py
 cyborgclient/osc/__init__.py
 cyborgclient/osc/plugin.py
 cyborgclient/osc/v1/__init__.py
 cyborgclient/osc/v1/accelerator.py
 cyborgclient/osc/v2/__init__.py
 cyborgclient/osc/v2/accelerator_request.py
+cyborgclient/osc/v2/attribute.py
 cyborgclient/osc/v2/deployable.py
 cyborgclient/osc/v2/device.py
 cyborgclient/osc/v2/device_profile.py
 cyborgclient/tests/__init__.py
 cyborgclient/tests/base.py
 cyborgclient/tests/test_cyborgclient.py
 cyborgclient/tests/functional/__init__.py
@@ -49,14 +50,15 @@
 cyborgclient/tests/unit/common/test_utils.py
 cyborgclient/tests/unit/osc/__init__.py
 cyborgclient/tests/unit/osc/fakes.py
 cyborgclient/tests/unit/osc/test_plugin.py
 cyborgclient/tests/unit/osc/v2/__init__.py
 cyborgclient/tests/unit/osc/v2/fakes.py
 cyborgclient/tests/unit/osc/v2/test_accelerator_request.py
+cyborgclient/tests/unit/osc/v2/test_attribute.py
 cyborgclient/tests/unit/osc/v2/test_deployable.py
 cyborgclient/tests/unit/osc/v2/test_device.py
 cyborgclient/tests/unit/osc/v2/test_device_profile.py
 cyborgclient/tests/unit/v1/__init__.py
 cyborgclient/tests/unit/v1/shell_test_base.py
 cyborgclient/tests/unit/v1/test_accelerators.py
 cyborgclient/tests/unit/v1/test_accelerators_shell.py
```

### Comparing `python-cyborgclient-2.1.0/python_cyborgclient.egg-info/entry_points.txt` & `python-cyborgclient-2.2.0/python_cyborgclient.egg-info/entry_points.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 accelerator_arq_delete = cyborgclient.osc.v2.accelerator_request:DeleteAcceleratorRequest
 accelerator_arq_list = cyborgclient.osc.v2.accelerator_request:ListAcceleratorRequest
 accelerator_arq_show = cyborgclient.osc.v2.accelerator_request:ShowAcceleratorRequest
 accelerator_arq_unbind = cyborgclient.osc.v2.accelerator_request:UnbindAcceleratorRequest
 accelerator_deployable_list = cyborgclient.osc.v2.deployable:ListDeployable
 accelerator_deployable_program = cyborgclient.osc.v2.deployable:ProgramDeployable
 accelerator_deployable_show = cyborgclient.osc.v2.deployable:ShowDeployable
+accelerator_device_attribute_create = cyborgclient.osc.v2.attribute:CreateAttribute
+accelerator_device_attribute_delete = cyborgclient.osc.v2.attribute:DeleteAttribute
+accelerator_device_attribute_list = cyborgclient.osc.v2.attribute:ListAttribute
+accelerator_device_attribute_show = cyborgclient.osc.v2.attribute:ShowAttribute
 accelerator_device_list = cyborgclient.osc.v2.device:ListDevice
 accelerator_device_profile_create = cyborgclient.osc.v2.device_profile:CreateDeviceProfile
 accelerator_device_profile_delete = cyborgclient.osc.v2.device_profile:DeleteDeviceProfile
 accelerator_device_profile_list = cyborgclient.osc.v2.device_profile:ListDeviceProfile
 accelerator_device_profile_show = cyborgclient.osc.v2.device_profile:ShowDeviceProfile
 accelerator_device_show = cyborgclient.osc.v2.device:ShowDevice
```

### Comparing `python-cyborgclient-2.1.0/releasenotes/source/conf.py` & `python-cyborgclient-2.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/requirements.txt` & `python-cyborgclient-2.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/setup.cfg` & `python-cyborgclient-2.2.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -33,14 +33,18 @@
 	accelerator_list = cyborgclient.osc.v1.accelerator:ListAccelerator
 openstack.accelerator.v2 = 
 	accelerator_deployable_list = cyborgclient.osc.v2.deployable:ListDeployable
 	accelerator_deployable_program = cyborgclient.osc.v2.deployable:ProgramDeployable
 	accelerator_deployable_show = cyborgclient.osc.v2.deployable:ShowDeployable
 	accelerator_device_list = cyborgclient.osc.v2.device:ListDevice
 	accelerator_device_show = cyborgclient.osc.v2.device:ShowDevice
+	accelerator_device_attribute_list = cyborgclient.osc.v2.attribute:ListAttribute
+	accelerator_device_attribute_create = cyborgclient.osc.v2.attribute:CreateAttribute
+	accelerator_device_attribute_delete = cyborgclient.osc.v2.attribute:DeleteAttribute
+	accelerator_device_attribute_show = cyborgclient.osc.v2.attribute:ShowAttribute
 	accelerator_device_profile_list = cyborgclient.osc.v2.device_profile:ListDeviceProfile
 	accelerator_device_profile_create = cyborgclient.osc.v2.device_profile:CreateDeviceProfile
 	accelerator_device_profile_delete = cyborgclient.osc.v2.device_profile:DeleteDeviceProfile
 	accelerator_device_profile_show = cyborgclient.osc.v2.device_profile:ShowDeviceProfile
 	accelerator_arq_list = cyborgclient.osc.v2.accelerator_request:ListAcceleratorRequest
 	accelerator_arq_create = cyborgclient.osc.v2.accelerator_request:CreateAcceleratorRequest
 	accelerator_arq_delete = cyborgclient.osc.v2.accelerator_request:DeleteAcceleratorRequest
```

### Comparing `python-cyborgclient-2.1.0/setup.py` & `python-cyborgclient-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.1.0/tox.ini` & `python-cyborgclient-2.2.0/tox.ini`

 * *Files identical despite different names*

