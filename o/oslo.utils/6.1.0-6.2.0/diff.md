# Comparing `tmp/oslo.utils-6.1.0.tar.gz` & `tmp/oslo.utils-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslo.utils-6.1.0.tar", last modified: Thu Nov 17 10:05:08 2022, max compression
+gzip compressed data, was "oslo.utils-6.2.0.tar", last modified: Thu Jul  6 08:56:01 2023, max compression
```

## Comparing `oslo.utils-6.1.0.tar` & `oslo.utils-6.2.0.tar`

### file list

```diff
@@ -1,160 +1,163 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7047 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26838 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/dictutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/encodeutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/eventletutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/excutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/fileutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/fixture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/importutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/netutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/reflection.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/secretutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/specs_matcher.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/strutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/timeutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/units.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/uuidutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/versionutils.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/user/timeutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.778222 oslo.utils-6.1.0/oslo.utils.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4476 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.778222 oslo.utils-6.1.0/oslo_utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/dictutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6233 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/encodeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7090 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/eventletutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14561 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/excutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6098 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/fileutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3420 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8716 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/imageutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3743 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/importutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/oslo_utils/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/oslo_utils/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.778222 oslo.utils-6.1.0/oslo_utils/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2183 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/locale/de/LC_MESSAGES/oslo_utils.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/oslo_utils/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.778222 oslo.utils-6.1.0/oslo_utils/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3025 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/locale/en_GB/LC_MESSAGES/oslo_utils.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/oslo_utils/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.778222 oslo.utils-6.1.0/oslo_utils/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/locale/fr/LC_MESSAGES/oslo_utils.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16492 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/netutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8707 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/reflection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2198 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/secretutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/specs_matcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21500 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/strutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.782222 oslo.utils-6.1.0/oslo_utils/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1976 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.782222 oslo.utils-6.1.0/oslo_utils/tests/fake/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/fake/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.782222 oslo.utils-6.1.0/oslo_utils/tests/fake/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/fake/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/fake/v2/dummpy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_dictutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8513 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_eventletutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23309 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_excutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10716 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_fileutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3645 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11728 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_imageutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6728 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_importutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20171 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_netutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10996 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_reflection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4447 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_secretutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12430 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_specs_matcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42855 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_strutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21421 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_timeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2367 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_uuidutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3735 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_versionutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7016 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/tests_encodeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15755 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/timeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/units.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1572 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/uuidutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2870 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/versionutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/add-md5-wrapper-7bf81c2464a7a224.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/add-methods-for-json-yaml-file-check-746dca0a11c2f9c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/add-reno-350f5f34f794fb5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/allow-to-convert-ipv4-address-from-text-to-binary-8c46ad2d9989e8c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/bug-1942682-ea95d54b2587b32f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/bump-up-port-range-f774a16336158339.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/deprecate-fnmatch-057a092d434a0c53.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/drop-imageutils-human-format-support-a89101a36c4dd3cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/drop-python27-support-f97f680651693b47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/fix_mask_password_regex-c0661f95a23369a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/image-utils-handle-scientific-notation-6f65d46e9c8c8f8c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/introduce-keystoneidsentinel-16bf3e7f2ae7e9f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/mask-dict-passwords-99357ffb7972fb0b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/mask-password-pattern-c8c880098743de3e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/mask-password-patterns-f41524069b8ae488.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/netutils-get_mac_addr_by_ipv6-c3ce6a35a69f7c2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/remove-fnmatch-f227b54f237a02c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/remove-timeutils-deprecated-helpers-5de68c21dd281529.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8611 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10181 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2022-11-17 10:05:08.790223 oslo.utils-6.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/tools/perf_test_mask_password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.374003 oslo.utils-6.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7149 2023-07-06 08:56:01.000000 oslo.utils-6.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27319 2023-07-06 08:56:01.000000 oslo.utils-6.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2023-07-06 08:56:01.374003 oslo.utils-6.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.350003 oslo.utils-6.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.350003 oslo.utils-6.2.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.350003 oslo.utils-6.2.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.350003 oslo.utils-6.2.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.354003 oslo.utils-6.2.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/dictutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/encodeutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/eventletutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/excutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/fileutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/fixture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/importutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/netutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/reflection.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/secretutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/specs_matcher.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/strutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/timeutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/units.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/uuidutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/reference/versionutils.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.354003 oslo.utils-6.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/user/timeutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.358003 oslo.utils-6.2.0/oslo.utils.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2023-07-06 08:56:01.000000 oslo.utils-6.2.0/oslo.utils.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4644 2023-07-06 08:56:01.000000 oslo.utils-6.2.0/oslo.utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:56:01.000000 oslo.utils-6.2.0/oslo.utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:56:01.000000 oslo.utils-6.2.0/oslo.utils.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-06 08:56:01.000000 oslo.utils-6.2.0/oslo.utils.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-07-06 08:56:01.000000 oslo.utils-6.2.0/oslo.utils.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-07-06 08:56:01.000000 oslo.utils-6.2.0/oslo.utils.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.362003 oslo.utils-6.2.0/oslo_utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/dictutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6233 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/encodeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7090 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/eventletutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14561 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/excutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6098 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/fileutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3420 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8716 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/imageutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3743 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/importutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.346003 oslo.utils-6.2.0/oslo_utils/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.346003 oslo.utils-6.2.0/oslo_utils/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.362003 oslo.utils-6.2.0/oslo_utils/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2183 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/locale/de/LC_MESSAGES/oslo_utils.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.346003 oslo.utils-6.2.0/oslo_utils/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.362003 oslo.utils-6.2.0/oslo_utils/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3025 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/locale/en_GB/LC_MESSAGES/oslo_utils.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.346003 oslo.utils-6.2.0/oslo_utils/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.362003 oslo.utils-6.2.0/oslo_utils/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/locale/fr/LC_MESSAGES/oslo_utils.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18112 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/netutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8707 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/reflection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2198 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/secretutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/specs_matcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21941 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/strutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.366003 oslo.utils-6.2.0/oslo_utils/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1976 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.366003 oslo.utils-6.2.0/oslo_utils/tests/fake/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/fake/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.366003 oslo.utils-6.2.0/oslo_utils/tests/fake/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/fake/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/fake/v2/dummpy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_dictutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8513 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_eventletutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23309 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_excutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10716 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_fileutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3645 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11728 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_imageutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6728 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_importutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20917 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_netutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10996 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_reflection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4447 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_secretutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12430 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_specs_matcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43323 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_strutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21419 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_timeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2367 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_uuidutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3735 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/test_versionutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7016 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/tests/tests_encodeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16005 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/timeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1380 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/units.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1572 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/uuidutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2870 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/oslo_utils/versionutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.346003 oslo.utils-6.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.370003 oslo.utils-6.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/add-md5-wrapper-7bf81c2464a7a224.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/add-methods-for-json-yaml-file-check-746dca0a11c2f9c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/add-reno-350f5f34f794fb5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/allow-to-convert-ipv4-address-from-text-to-binary-8c46ad2d9989e8c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/bug-1942682-ea95d54b2587b32f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/bump-up-port-range-f774a16336158339.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/deprecate-fnmatch-057a092d434a0c53.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/drop-imageutils-human-format-support-a89101a36c4dd3cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/drop-python27-support-f97f680651693b47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/fix_mask_password_regex-c0661f95a23369a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/image-utils-handle-scientific-notation-6f65d46e9c8c8f8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/implement-zoneinfo-to-remove-pytz-fba6f70db09ecdb8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/introduce-keystoneidsentinel-16bf3e7f2ae7e9f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/mask-dict-passwords-99357ffb7972fb0b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/mask-password-pattern-c8c880098743de3e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/mask-password-patterns-f41524069b8ae488.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/netutils-get_mac_addr_by_ipv6-c3ce6a35a69f7c2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/netutils-get_my_ipv6-c9f124374655326b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/remove-fnmatch-f227b54f237a02c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/notes/remove-timeutils-deprecated-helpers-5de68c21dd281529.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.374003 oslo.utils-6.2.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.374003 oslo.utils-6.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.374003 oslo.utils-6.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8611 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.346003 oslo.utils-6.2.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.346003 oslo.utils-6.2.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.374003 oslo.utils-6.2.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10181 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2023-07-06 08:56:01.374003 oslo.utils-6.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:01.374003 oslo.utils-6.2.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/tools/perf_test_mask_password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2023-07-06 08:55:34.000000 oslo.utils-6.2.0/tox.ini
```

### Comparing `oslo.utils-6.1.0/.pre-commit-config.yaml` & `oslo.utils-6.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/AUTHORS` & `oslo.utils-6.2.0/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 Ann Kamyshnikova <akamyshnikova@mirantis.com>
 Balazs Gibizer <balazs.gibizer@est.tech>
 Ben Nemec <bnemec@redhat.com>
 Ben Nemec <bnemec@us.ibm.com>
 Bence Romsics <bence.romsics@gmail.com>
 Bin Zhou <zhou.bin9@zte.com.cn>
 Brant Knudson <bknudson@us.ibm.com>
+Brian Haley <haleyb.dev@gmail.com>
 Brian Rosmaita <rosmaita.fossdev@gmail.com>
 BubaVV <vmarkov@mirantis.com>
 Cedric Brandily <zzelle@gmail.com>
 Chang Bo Guo <guochbo@cn.ibm.com>
 ChangBo Guo(gcb) <eric.guo@easystack.cn>
 Christian Berendt <berendt@b1-systems.de>
 Chuck Short <chuck.short@canonical.com>
@@ -60,14 +61,15 @@
 Eoghan Glynn <eglynn@redhat.com>
 Eric Brown <browne@vmware.com>
 Eric Fried <efried@us.ibm.com>
 Eugene Kirpichov <ekirpichov@gmail.com>
 Flaper Fesp <flaper87@gmail.com>
 Flavio Percoco <flaper87@gmail.com>
 Gary Kotton <gkotton@redhat.com>
+Ghanshyam <gmann@ghanshyammann.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Ghe Rivero <ghe@debian.org>
 Guang Yee <guang.yee@hp.com>
 Hanxi Liu <hanxi.liu@easystack.cn>
 Hervé Beraud <hberaud@redhat.com>
 Ian Wienand <iwienand@redhat.com>
 Ihar Hrachyshka <ihrachys@redhat.com>
@@ -106,14 +108,15 @@
 Noorul Islam K M <noorul@noorul.com>
 Oleg Bondarev <obondarev@mirantis.com>
 Oleksii Chuprykov <ochuprykov@mirantis.com>
 Oleksii Zamiatin <ozamiatin@mirantis.com>
 Omar Shykhkerimov <oshykhkerimov@mirantis.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Paul Belanger <paul.belanger@polybeacon.com>
+Petr Vaněk <arkamar@atlas.cz>
 Pierre Riteau <pierre@stackhpc.com>
 Radomir Dopieralski <openstack@sheep.art.pl>
 Rahul Nair <rahulunair@gmail.com>
 Rajath Agasthya <rajathagasthya@gmail.com>
 Raymond Pekowski <pekowski@gmail.com>
 Rick Harris <rconradharris@gmail.com>
 Ronald Bradford <ronald.bradford@gmail.com>
```

### Comparing `oslo.utils-6.1.0/CONTRIBUTING.rst` & `oslo.utils-6.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/ChangeLog` & `oslo.utils-6.2.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 CHANGES
 =======
 
+6.2.0
+-----
+
+* Replace deprecated assertAlmostEquals method
+* strutils: update string\_to\_bytes
+* Add netutils.get\_my\_ipv6()
+* Bump bandit
+* Fix compatibility with Python 3.8
+* Revert "Moves supported python runtimes from version 3.8 to 3.10"
+* Moves supported python runtimes from version 3.8 to 3.10
+* Update units for current SI prefixes
+* Implement zoneinfo support to drop dependency to pytz
+* Use the new openstack-python3-jobs template
+* Update master for stable/2023.1
+
 6.1.0
 -----
 
 * [imageutils] Fix \_\_str\_\_ for QemuImgInfo
 * Imported Translations from Zanata
 * Add Python3 antelope unit tests
 * Update master for stable/zed
```

### Comparing `oslo.utils-6.1.0/LICENSE` & `oslo.utils-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/PKG-INFO` & `oslo.utils-6.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.utils
-Version: 6.1.0
+Version: 6.2.0
 Summary: Oslo Utility library
 Home-page: https://docs.openstack.org/oslo.utils/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -43,10 +43,11 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
```

### Comparing `oslo.utils-6.1.0/README.rst` & `oslo.utils-6.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/doc/source/conf.py` & `oslo.utils-6.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/doc/source/index.rst` & `oslo.utils-6.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/doc/source/user/timeutils.rst` & `oslo.utils-6.2.0/doc/source/user/timeutils.rst`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo.utils.egg-info/PKG-INFO` & `oslo.utils-6.2.0/oslo.utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.utils
-Version: 6.1.0
+Version: 6.2.0
 Summary: Oslo Utility library
 Home-page: https://docs.openstack.org/oslo.utils/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -43,10 +43,11 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
```

### Comparing `oslo.utils-6.1.0/oslo.utils.egg-info/SOURCES.txt` & `oslo.utils-6.2.0/oslo.utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -98,21 +98,24 @@
 releasenotes/notes/bug-1942682-ea95d54b2587b32f.yaml
 releasenotes/notes/bump-up-port-range-f774a16336158339.yaml
 releasenotes/notes/deprecate-fnmatch-057a092d434a0c53.yaml
 releasenotes/notes/drop-imageutils-human-format-support-a89101a36c4dd3cb.yaml
 releasenotes/notes/drop-python27-support-f97f680651693b47.yaml
 releasenotes/notes/fix_mask_password_regex-c0661f95a23369a4.yaml
 releasenotes/notes/image-utils-handle-scientific-notation-6f65d46e9c8c8f8c.yaml
+releasenotes/notes/implement-zoneinfo-to-remove-pytz-fba6f70db09ecdb8.yaml
 releasenotes/notes/introduce-keystoneidsentinel-16bf3e7f2ae7e9f3.yaml
 releasenotes/notes/mask-dict-passwords-99357ffb7972fb0b.yaml
 releasenotes/notes/mask-password-pattern-c8c880098743de3e.yaml
 releasenotes/notes/mask-password-patterns-f41524069b8ae488.yaml
 releasenotes/notes/netutils-get_mac_addr_by_ipv6-c3ce6a35a69f7c2b.yaml
+releasenotes/notes/netutils-get_my_ipv6-c9f124374655326b.yaml
 releasenotes/notes/remove-fnmatch-f227b54f237a02c2.yaml
 releasenotes/notes/remove-timeutils-deprecated-helpers-5de68c21dd281529.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
```

### Comparing `oslo.utils-6.1.0/oslo_utils/_i18n.py` & `oslo.utils-6.2.0/oslo_utils/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/dictutils.py` & `oslo.utils-6.2.0/oslo_utils/dictutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/encodeutils.py` & `oslo.utils-6.2.0/oslo_utils/encodeutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/eventletutils.py` & `oslo.utils-6.2.0/oslo_utils/eventletutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/excutils.py` & `oslo.utils-6.2.0/oslo_utils/excutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/fileutils.py` & `oslo.utils-6.2.0/oslo_utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/fixture.py` & `oslo.utils-6.2.0/oslo_utils/fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/imageutils.py` & `oslo.utils-6.2.0/oslo_utils/imageutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/importutils.py` & `oslo.utils-6.2.0/oslo_utils/importutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/locale/de/LC_MESSAGES/oslo_utils.po` & `oslo.utils-6.2.0/oslo_utils/locale/de/LC_MESSAGES/oslo_utils.po`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/locale/en_GB/LC_MESSAGES/oslo_utils.po` & `oslo.utils-6.2.0/oslo_utils/locale/en_GB/LC_MESSAGES/oslo_utils.po`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/locale/fr/LC_MESSAGES/oslo_utils.po` & `oslo.utils-6.2.0/oslo_utils/locale/fr/LC_MESSAGES/oslo_utils.po`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/netutils.py` & `oslo.utils-6.2.0/oslo_utils/netutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -410,14 +410,60 @@
     except Exception as e:
         LOG.info('Could not determine IPv4 address for '
                  'interface %(interface)s: %(error)s',
                  {'interface': interface, 'error': e})
     return LOCALHOST
 
 
+def get_my_ipv6():
+    """Returns the actual IPv6 address of the local machine.
+
+    This code figures out what source address would be used if some traffic
+    were to be sent out to some well known address on the Internet. In this
+    case, IPv6 from RFC3849 is used, but the specific address does not
+    matter much. No traffic is actually sent.
+
+    .. versionadded:: 6.1
+       Return ``'::1'`` if there is no default interface.
+    """
+    try:
+        csock = socket.socket(socket.AF_INET6, socket.SOCK_DGRAM)
+        csock.connect(('2001:db8::1', 80))
+        (addr, _, _, _) = csock.getsockname()
+        csock.close()
+        return addr
+    except socket.error:
+        return _get_my_ipv6_address()
+
+
+def _get_my_ipv6_address():
+    """Figure out the best IPv6 address
+    """
+    LOCALHOST = '::1'
+    gtw = netifaces.gateways()
+    try:
+        interface = gtw['default'][netifaces.AF_INET6][1]
+    except (KeyError, IndexError):
+        LOG.info('Could not determine default network interface, '
+                 'using %s for IPv6 address', LOCALHOST)
+        return LOCALHOST
+
+    try:
+        return netifaces.ifaddresses(interface)[netifaces.AF_INET6][0]['addr']
+    except (KeyError, IndexError):
+        LOG.info('Could not determine IPv6 address for interface '
+                 '%(interface)s, using %(address)s',
+                 {'interface': interface, 'address': LOCALHOST})
+    except Exception as e:
+        LOG.info('Could not determine IPv6 address for '
+                 'interface %(interface)s: %(error)s',
+                 {'interface': interface, 'error': e})
+    return LOCALHOST
+
+
 class _ModifiedSplitResult(parse.SplitResult):
     """Split results class for urlsplit."""
 
     def params(self, collapse=True):
         """Extracts the query parameters from the split urls components.
 
         This method will provide back as a dictionary the query parameter
```

### Comparing `oslo.utils-6.1.0/oslo_utils/reflection.py` & `oslo.utils-6.2.0/oslo_utils/reflection.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/secretutils.py` & `oslo.utils-6.2.0/oslo_utils/secretutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/specs_matcher.py` & `oslo.utils-6.2.0/oslo_utils/specs_matcher.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/strutils.py` & `oslo.utils-6.2.0/oslo_utils/strutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,19 +33,32 @@
     'Ki': 1,
     'M': 2,
     'Mi': 2,
     'G': 3,
     'Gi': 3,
     'T': 4,
     'Ti': 4,
+    'P': 5,
+    'Pi': 5,
+    'E': 6,
+    'Ei': 6,
+    'Z': 7,
+    'Zi': 7,
+    'Y': 8,
+    'Yi': 8,
+    'R': 9,
+    'Ri': 9,
+    'Q': 10,
+    'Qi': 10,
 }
 UNIT_SYSTEM_INFO = {
-    'IEC': (1024, re.compile(r'(^[-+]?\d*\.?\d+)([KMGT]i?)?(b|bit|B)$')),
-    'SI': (1000, re.compile(r'(^[-+]?\d*\.?\d+)([kMGT])?(b|bit|B)$')),
-    'mixed': (None, re.compile(r'(^[-+]?\d*\.?\d+)([kKMGT]i?)?(b|bit|B)$')),
+    'IEC': (1024, re.compile(r'(^[-+]?\d*\.?\d+)([KMGTPEZYRQ]i?)?(b|bit|B)$')),
+    'SI': (1000, re.compile(r'(^[-+]?\d*\.?\d+)([kMGTPEZYRQ])?(b|bit|B)$')),
+    'mixed': (None, re.compile(
+        r'(^[-+]?\d*\.?\d+)([kKMGTPEZYRQ]i?)?(b|bit|B)$')),
 }
 
 TRUE_STRINGS = ('1', 't', 'true', 'on', 'y', 'yes')
 FALSE_STRINGS = ('0', 'f', 'false', 'off', 'n', 'no')
 
 SLUGIFY_STRIP_RE = re.compile(r"[^\w\s-]")
 SLUGIFY_HYPHENATE_RE = re.compile(r"[-\s]+")
@@ -178,21 +191,27 @@
 
 
 def string_to_bytes(text, unit_system='IEC', return_int=False):
     """Converts a string into an float representation of bytes.
 
     The units supported for IEC / mixed::
 
-        Kb(it), Kib(it), Mb(it), Mib(it), Gb(it), Gib(it), Tb(it), Tib(it)
-        KB, KiB, MB, MiB, GB, GiB, TB, TiB
+        Kb(it), Kib(it), Mb(it), Mib(it), Gb(it), Gib(it), Tb(it), Tib(it),
+        Pb(it), Pib(it), Eb(it), Eib(it), Zb(it), Zib(it), Yb(it), Yib(it),
+        Rb(it), Rib(it), Qb(it), Qib(it)
+
+        KB, KiB, MB, MiB, GB, GiB, TB, TiB, PB, PiB, EB, EiB, ZB, ZiB,
+        YB, YiB, RB, RiB, QB, QiB
 
     The units supported for SI ::
 
-        kb(it), Mb(it), Gb(it), Tb(it)
-        kB, MB, GB, TB
+        kb(it), Mb(it), Gb(it), Tb(it), Pb(it), Eb(it), Zb(it), Yb(it),
+        Rb(it), Qb(it)
+
+        kB, MB, GB, TB, PB, EB, ZB, YB, RB, QB
 
     SI units are interpreted as power-of-ten (e.g. 1kb = 1000b).  Note
     that the SI unit system does not support capital letter 'K'
 
     IEC units are interpreted as power-of-two (e.g. 1MiB = 1MB =
     1024b)
```

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/__init__.py` & `oslo.utils-6.2.0/oslo_utils/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/base.py` & `oslo.utils-6.2.0/oslo_utils/tests/base.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/fake/__init__.py` & `oslo.utils-6.2.0/oslo_utils/tests/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/fake/v2/dummpy.py` & `oslo.utils-6.2.0/oslo_utils/tests/fake/v2/dummpy.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_dictutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_dictutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_eventletutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_eventletutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_excutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_excutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_fileutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_fileutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_fixture.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_imageutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_imageutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_importutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_importutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_netutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_netutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -272,21 +272,29 @@
 
     def test_valid_port_fail(self):
         invalid_inputs = ['-32768', '65536', 528491, '528491',
                           '528.491', 'thirty-seven', None]
         for input_str in invalid_inputs:
             self.assertFalse(netutils.is_valid_port(input_str))
 
-    def test_get_my_ip(self):
+    def test_get_my_ipv4(self):
         sock_attrs = {
             'return_value.getsockname.return_value': ['1.2.3.4', '']}
         with mock.patch('socket.socket', **sock_attrs):
             addr = netutils.get_my_ipv4()
         self.assertEqual(addr, '1.2.3.4')
 
+    def test_get_my_ipv6(self):
+        sock_attrs = {
+            'return_value.getsockname.return_value': ['2001:db8::2', '',
+                                                      '', '']}
+        with mock.patch('socket.socket', **sock_attrs):
+            addr = netutils.get_my_ipv6()
+        self.assertEqual(addr, '2001:db8::2')
+
     def test_is_int_in_range(self):
         valid_inputs = [(1, -100, 100),
                         ('1', -100, 100),
                         (100, -100, 100),
                         ('100', -100, 100),
                         (-100, -100, 100),
                         ('-100', -100, 100)]
@@ -319,45 +327,52 @@
     def test_invalid_icmp_code(self):
         invalid_inputs = [-1, '-1', 256, '256', 'None', 'zero']
         for input_value in invalid_inputs:
             self.assertFalse(netutils.is_valid_icmp_code(input_value))
 
     @mock.patch('socket.socket')
     @mock.patch('oslo_utils.netutils._get_my_ipv4_address')
-    def test_get_my_ip_socket_error(self, ip, mock_socket):
+    def test_get_my_ipv4_socket_error(self, ip, mock_socket):
         mock_socket.side_effect = socket.error
         ip.return_value = '1.2.3.4'
         addr = netutils.get_my_ipv4()
         self.assertEqual(addr, '1.2.3.4')
 
+    @mock.patch('socket.socket')
+    @mock.patch('oslo_utils.netutils._get_my_ipv6_address')
+    def test_get_my_ipv6_socket_error(self, ip, mock_socket):
+        mock_socket.side_effect = socket.error
+        ip.return_value = '2001:db8::2'
+        addr = netutils.get_my_ipv6()
+        self.assertEqual(addr, '2001:db8::2')
+
     @mock.patch('netifaces.gateways')
     @mock.patch('netifaces.ifaddresses')
-    def test_get_my_ipv4_address_with_default_route(
+    def test_get_my_ip_address_with_default_route(
             self, ifaddr, gateways):
-        with mock.patch.dict(netifaces.__dict__, {'AF_INET': '0'}):
-            ifaddr.return_value = {'0': [{'addr': '172.18.204.1'}]}
-            addr = netutils._get_my_ipv4_address()
-        self.assertEqual('172.18.204.1', addr)
+        ifaddr.return_value = {netifaces.AF_INET: [{'addr': '172.18.204.1'}],
+                               netifaces.AF_INET6: [{'addr': '2001:db8::2'}]}
+        self.assertEqual('172.18.204.1', netutils._get_my_ipv4_address())
+        self.assertEqual('2001:db8::2', netutils._get_my_ipv6_address())
 
     @mock.patch('netifaces.gateways')
     @mock.patch('netifaces.ifaddresses')
-    def test_get_my_ipv4_address_without_default_route(
+    def test_get_my_ip_address_without_default_route(
             self, ifaddr, gateways):
-        with mock.patch.dict(netifaces.__dict__, {'AF_INET': '0'}):
-            ifaddr.return_value = {}
-            addr = netutils._get_my_ipv4_address()
-        self.assertEqual('127.0.0.1', addr)
+        ifaddr.return_value = {}
+        self.assertEqual('127.0.0.1', netutils._get_my_ipv4_address())
+        self.assertEqual('::1', netutils._get_my_ipv6_address())
 
     @mock.patch('netifaces.gateways')
     @mock.patch('netifaces.ifaddresses')
     def test_get_my_ipv4_address_without_default_interface(
             self, ifaddr, gateways):
         gateways.return_value = {}
-        addr = netutils._get_my_ipv4_address()
-        self.assertEqual('127.0.0.1', addr)
+        self.assertEqual('127.0.0.1', netutils._get_my_ipv4_address())
+        self.assertEqual('::1', netutils._get_my_ipv6_address())
         self.assertFalse(ifaddr.called)
 
 
 class IPv6byEUI64TestCase(test_base.BaseTestCase):
     """Unit tests to generate IPv6 by EUI-64 operations."""
 
     def test_generate_IPv6_by_EUI64(self):
```

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_reflection.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_reflection.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_secretutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_secretutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_specs_matcher.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_specs_matcher.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_strutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_strutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,18 +203,30 @@
     _unit_prefix = [
         ('no_unit_prefix', dict(unit_prefix='')),
         ('k', dict(unit_prefix='k')),
         ('K', dict(unit_prefix='K')),
         ('M', dict(unit_prefix='M')),
         ('G', dict(unit_prefix='G')),
         ('T', dict(unit_prefix='T')),
+        ('P', dict(unit_prefix='P')),
+        ('E', dict(unit_prefix='E')),
+        ('Z', dict(unit_prefix='Z')),
+        ('Y', dict(unit_prefix='Y')),
+        ('R', dict(unit_prefix='R')),
+        ('Q', dict(unit_prefix='Q')),
         ('Ki', dict(unit_prefix='Ki')),
         ('Mi', dict(unit_prefix='Mi')),
         ('Gi', dict(unit_prefix='Gi')),
         ('Ti', dict(unit_prefix='Ti')),
+        ('Pi', dict(unit_prefix='Pi')),
+        ('Ei', dict(unit_prefix='Ei')),
+        ('Zi', dict(unit_prefix='Zi')),
+        ('Yi', dict(unit_prefix='Yi')),
+        ('Ri', dict(unit_prefix='Ri')),
+        ('Qi', dict(unit_prefix='Qi')),
         ('invalid_unit_prefix', dict(unit_prefix='B', assert_error=True)),
     ]
 
     _unit_suffix = [
         ('b', dict(unit_suffix='b')),
         ('bit', dict(unit_suffix='bit')),
         ('B', dict(unit_suffix='B')),
```

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_timeutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_timeutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,16 +188,16 @@
 
         self.assertEqual(expected, leap_time)
 
     def test_delta_seconds(self):
         before = timeutils.utcnow()
         after = before + datetime.timedelta(days=7, seconds=59,
                                             microseconds=123456)
-        self.assertAlmostEquals(604859.123456,
-                                timeutils.delta_seconds(before, after))
+        self.assertAlmostEqual(604859.123456,
+                               timeutils.delta_seconds(before, after))
 
     def test_is_soon(self):
         expires = timeutils.utcnow() + datetime.timedelta(minutes=5)
         self.assertFalse(timeutils.is_soon(expires, 120))
         self.assertTrue(timeutils.is_soon(expires, 300))
         self.assertTrue(timeutils.is_soon(expires, 600))
```

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_uuidutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_uuidutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/test_versionutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/test_versionutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/tests/tests_encodeutils.py` & `oslo.utils-6.2.0/oslo_utils/tests/tests_encodeutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/timeutils.py` & `oslo.utils-6.2.0/oslo_utils/timeutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,21 @@
 import calendar
 import datetime
 import functools
 import logging
 import time
 
 import iso8601
-import pytz
+
+try:
+    import zoneinfo
+except ImportError:
+    # zoneinfo is available in Python >= 3.9
+    import pytz
+    zoneinfo = None
 
 from oslo_utils import reflection
 
 # ISO 8601 extended time format with microseconds
 _ISO8601_TIME_FORMAT_SUBSECOND = '%Y-%m-%dT%H:%M:%S.%f'
 _ISO8601_TIME_FORMAT = '%Y-%m-%dT%H:%M:%S'
 PERFECT_TIME_FORMAT = _ISO8601_TIME_FORMAT_SUBSECOND
@@ -221,16 +227,22 @@
                            minute=tyme['minute'],
                            second=second,
                            microsecond=tyme['microsecond'])
     tzname = tyme.get('tzname')
     if tzname:
         # Need to handle either iso8601 or python UTC format
         tzname = 'UTC' if tzname == 'UTC+00:00' else tzname
-        tzinfo = pytz.timezone(tzname)
-        dt = tzinfo.localize(dt)
+
+        if zoneinfo:
+            tzinfo = zoneinfo.ZoneInfo(tzname)
+            dt = dt.replace(tzinfo=tzinfo)
+        else:
+            tzinfo = pytz.timezone(tzname)
+            dt = tzinfo.localize(dt)
+
     return dt
 
 
 def delta_seconds(before, after):
     """Return the difference between two timing objects.
 
     Compute the difference in seconds between two date, time, or
```

### Comparing `oslo.utils-6.1.0/oslo_utils/units.py` & `oslo.utils-6.2.0/oslo_utils/units.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 "Binary peta unit"
 Ei = 1024 ** 6
 "Binary exa unit"
 Zi = 1024 ** 7
 "Binary zetta unit"
 Yi = 1024 ** 8
 "Binary yotta unit"
+Ri = 1024 ** 9
+"Binary ronna unit"
+Qi = 1024 ** 10
+"Binary quetta unit"
 
 # Decimal unit constants.
 k = 1000
 "Decimal kilo unit"
 M = 1000 ** 2
 "Decimal mega unit"
 G = 1000 ** 3
@@ -48,7 +52,11 @@
 "Decimal peta unit"
 E = 1000 ** 6
 "Decimal exa unit"
 Z = 1000 ** 7
 "Decimal zetta unit"
 Y = 1000 ** 8
 "Decimal yotta unit"
+R = 1000 ** 9
+"Decimal ronna unit"
+Q = 1000 ** 10
+"Decimal quetta unit"
```

### Comparing `oslo.utils-6.1.0/oslo_utils/uuidutils.py` & `oslo.utils-6.2.0/oslo_utils/uuidutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/oslo_utils/versionutils.py` & `oslo.utils-6.2.0/oslo_utils/versionutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/releasenotes/notes/add-md5-wrapper-7bf81c2464a7a224.yaml` & `oslo.utils-6.2.0/releasenotes/notes/add-md5-wrapper-7bf81c2464a7a224.yaml`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/releasenotes/source/conf.py` & `oslo.utils-6.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `oslo.utils-6.2.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/setup.cfg` & `oslo.utils-6.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [files]
 packages = 
 	oslo_utils
```

### Comparing `oslo.utils-6.1.0/setup.py` & `oslo.utils-6.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/test-requirements.txt` & `oslo.utils-6.2.0/test-requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 #  deps = {[testenv]deps} coverage
 coverage!=4.4,>=4.0 # Apache-2.0
 
 # used for oslotest cross-testing scripts
 oslo.config>=5.2.0 # Apache-2.0
 
 # Bandit security code scanner
-bandit>=1.6.0,<1.7.0 # Apache-2.0
+bandit>=1.7.0,<1.8.0 # Apache-2.0
 
 pre-commit>=2.6.0 # MIT
```

### Comparing `oslo.utils-6.1.0/tools/perf_test_mask_password.py` & `oslo.utils-6.2.0/tools/perf_test_mask_password.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.1.0/tox.ini` & `oslo.utils-6.2.0/tox.ini`

 * *Files identical despite different names*

