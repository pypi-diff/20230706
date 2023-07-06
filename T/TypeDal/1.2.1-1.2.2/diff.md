# Comparing `tmp/typedal-1.2.1.tar.gz` & `tmp/typedal-1.2.2.tar.gz`

## Comparing `typedal-1.2.1.tar` & `typedal-1.2.2.tar`

### file list

```diff
@@ -1,354 +1,354 @@
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 typedal-1.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 typedal-1.2.1/coverage.svg
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 typedal-1.2.1/example_new.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 typedal-1.2.1/example_old.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 typedal-1.2.1/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0   177667 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   170960 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1054992 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   123328 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   104160 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    57612 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   142044 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    85348 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0    88278 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    75208 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   167175 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    49442 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   168498 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   146267 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   228230 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   416965 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407999 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   128994 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    79298 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70175 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    90277 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350178 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/__init__.data.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/__init__.meta.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/__about__.data.json
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/__init__.data.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/__init__.meta.json
--rw-r--r--   0        0        0    33347 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/core.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/core.meta.json
--rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/fields.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/fields.meta.json
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/pydal_objects.data.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180368 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171931 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0    23336 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60676 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1130454 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123317 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109204 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57745 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142208 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    90123 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    27481 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/example_new.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/example_new.meta.json
--rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    85337 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    28767 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0    87488 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75197 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167545 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src.data.json
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src.meta.json
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28480 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49741 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   172768 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239632 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432234 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57845 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    89054 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407988 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128983 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79287 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70579 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91119 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350743 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/__init__.data.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/__init__.meta.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/__about__.data.json
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/__init__.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/__init__.meta.json
--rw-r--r--   0        0        0    43623 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/core.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/core.meta.json
--rw-r--r--   0        0        0    28504 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/fields.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/fields.meta.json
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/__about__.data.json
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/__init__.data.json
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/__init__.meta.json
--rw-r--r--   0        0        0    42844 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/core.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/core.meta.json
--rw-r--r--   0        0        0    28193 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/fields.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/fields.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/README.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1215429078721865123
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/121ed75fe9fe5f8e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/19309938546e93ab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/197f3188bc94f91f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1aa1390b5bde1004
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1b34455c399f0006
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1bd1a229a4f4ee7f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1c46d1f378d28fbb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1ca71ee291d82018
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1d6bb777df44b8ec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1dc8423cfb79eaa4
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/20585cf790eae81e
--rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/221af82ae72a7f27
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/2282e801459c52a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/248c4e1a32c704cb
--rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/24e1b4aab386ebc8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/28b1d8ac7e2aab6b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/2b7f7d266c8efaad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/2bb6610cadf18e18
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/2dac345be8527adf
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/2f3396c610fd7095
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/31731f8e74291475
--rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/322af04e6d059ce5
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/3826106cf4494de8
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/38d5fd55b14a9d6c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/3afc55a04b8f8bb2
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/4022ee8774ccd98a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/42f9a2406e74c24f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/4696b157ff786f22
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/46a88ce266f1ad94
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/4a6edd5010cb9700
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/4d0230e9a81a468
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/52018ba3989fcaf7
--rw-r--r--   0        0        0    13679 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/5491563776466765346
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/54e6ba8c25a22ffc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/566d94db91d23339
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/5a67aed8f6b70cd5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/5b076d769fa5cacd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/5ceb1580c62ee794
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/6bc90dbb56504f96
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/6c52d14716eee431
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/6f0c8f98e4da1d48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/74e52af774eebdbd
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/75bd1769f6e29ed7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/815ba2cfea236769
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/876d9a8d302e1c46
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/88e2927df9448936
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/8c4d3f5ef14b0167
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/8f8ec552e76f3eab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/95c82d8566c6704c
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/a0739889bf9412e8
--rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/a225e4df39be9b29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/a2340fd4c9aa1141
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/a513d558646cd439
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/b121e2b70fd66eb8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/b218ff88bc22b626
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/b419496fa9e72887
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/b886c97e4d4117f0
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/bdcdf5c7bbc1d738
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/c06de16f3c7a64cc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/c635f255374598c5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/c671ae94ff3d3e2e
--rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/cdfecbca581311ee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/ce44121ca4091b64
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/ced49ec87d10bcb0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/cfc06a1f13c8ab47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/d16c5d29763a704e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/d225ad4c14b8ca60
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/d379b35d5e80b789
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/d3a95555c0919160
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/d655bee8ff0a59f2
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/da4811a7730a562a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/dca573767bc8be7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/e3e29f9eacb7027f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/e46ab4b61bb5d446
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/e5e0cc178d5c9df5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/eb564f7989641958
--rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/eee2f3c667de6c7a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/f04d0d78a00adfd6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/f2ddc22a4b221f54
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/f879e8c947a6b7a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/fa45ef3c3166e02d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/faa51a5044a3c279
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c___about___py.html
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c___init___py.html
--rw-r--r--   0        0        0   127189 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c_core_py.html
--rw-r--r--   0        0        0    60671 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c_fields_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/style.css
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 typedal-1.2.1/src/typedal/__about__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 typedal-1.2.1/src/typedal/__init__.py
--rw-r--r--   0        0        0    15559 2020-02-02 00:00:00.000000 typedal-1.2.1/src/typedal/core.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 typedal-1.2.1/src/typedal/fields.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedal-1.2.1/src/typedal/py.typed
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 typedal-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0     9736 2020-02-02 00:00:00.000000 typedal-1.2.1/tests/test_main.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 typedal-1.2.1/tests/test_mypy.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 typedal-1.2.1/.gitignore
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 typedal-1.2.1/README.md
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 typedal-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 typedal-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 typedal-1.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 typedal-1.2.2/coverage.svg
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 typedal-1.2.2/example_new.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 typedal-1.2.2/example_old.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 typedal-1.2.2/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0   177667 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0   170960 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_decimal.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_decimal.meta.json
+-rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0  1054992 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   123328 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   104160 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    57612 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   142044 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/decimal.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/decimal.meta.json
+-rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    85348 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/numbers.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/numbers.meta.json
+-rw-r--r--   0        0        0    88278 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    75208 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   167175 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    49442 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   168498 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   146267 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   228230 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   416965 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407999 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   128994 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    79298 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70175 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    90277 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350178 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/__init__.data.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/__init__.meta.json
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    33347 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/typedal/core.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/typedal/core.meta.json
+-rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/typedal/fields.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/typedal/fields.meta.json
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/typedal/pydal_objects.data.json
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180368 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171931 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0    23336 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60676 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1130454 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123317 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109204 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57745 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142208 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    90123 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27481 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/example_new.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/example_new.meta.json
+-rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    85337 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    28767 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0    87488 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75197 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167545 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src.data.json
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src.meta.json
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28480 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49741 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   172768 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   239632 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432234 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57845 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89054 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407988 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128983 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79287 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70579 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91119 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350743 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src/__init__.data.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src/__init__.meta.json
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    43623 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src/typedal/core.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src/typedal/core.meta.json
+-rw-r--r--   0        0        0    28504 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src/typedal/fields.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/src/typedal/fields.meta.json
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    44614 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typedal/core.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typedal/core.meta.json
+-rw-r--r--   0        0        0    28193 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typedal/fields.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-1.2.2/.mypy_cache/3.11/typedal/fields.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 typedal-1.2.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 typedal-1.2.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 typedal-1.2.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 typedal-1.2.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 typedal-1.2.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/1215429078721865123
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/121ed75fe9fe5f8e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/19309938546e93ab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/197f3188bc94f91f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/1aa1390b5bde1004
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/1b34455c399f0006
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/1bd1a229a4f4ee7f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/1c46d1f378d28fbb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/1ca71ee291d82018
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/1d6bb777df44b8ec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/1dc8423cfb79eaa4
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/20585cf790eae81e
+-rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/221af82ae72a7f27
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/2282e801459c52a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/248c4e1a32c704cb
+-rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/24e1b4aab386ebc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/28b1d8ac7e2aab6b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/2b7f7d266c8efaad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/2bb6610cadf18e18
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/2dac345be8527adf
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/2f3396c610fd7095
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/31731f8e74291475
+-rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/322af04e6d059ce5
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/3826106cf4494de8
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/38d5fd55b14a9d6c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/3afc55a04b8f8bb2
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/4022ee8774ccd98a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/42f9a2406e74c24f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/4696b157ff786f22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/46a88ce266f1ad94
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/4a6edd5010cb9700
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/4d0230e9a81a468
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/52018ba3989fcaf7
+-rw-r--r--   0        0        0    13679 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/5491563776466765346
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/54e6ba8c25a22ffc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/566d94db91d23339
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/5a67aed8f6b70cd5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/5b076d769fa5cacd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/5ceb1580c62ee794
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/6bc90dbb56504f96
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/6c52d14716eee431
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/6f0c8f98e4da1d48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/74e52af774eebdbd
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/75bd1769f6e29ed7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/815ba2cfea236769
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/876d9a8d302e1c46
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/88e2927df9448936
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/8c4d3f5ef14b0167
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/8f8ec552e76f3eab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/95c82d8566c6704c
+-rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/a0739889bf9412e8
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/a225e4df39be9b29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/a2340fd4c9aa1141
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/a513d558646cd439
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/b121e2b70fd66eb8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/b218ff88bc22b626
+-rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/b419496fa9e72887
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/b886c97e4d4117f0
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/bdcdf5c7bbc1d738
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/c06de16f3c7a64cc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/c635f255374598c5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/c671ae94ff3d3e2e
+-rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/cdfecbca581311ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/ce44121ca4091b64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/ced49ec87d10bcb0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/cfc06a1f13c8ab47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/d16c5d29763a704e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/d225ad4c14b8ca60
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/d379b35d5e80b789
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/d3a95555c0919160
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/d655bee8ff0a59f2
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/da4811a7730a562a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/dca573767bc8be7e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/e3e29f9eacb7027f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/e46ab4b61bb5d446
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/e5e0cc178d5c9df5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/eb564f7989641958
+-rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/eee2f3c667de6c7a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/f04d0d78a00adfd6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/f2ddc22a4b221f54
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/f879e8c947a6b7a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/fa45ef3c3166e02d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.2/.ruff_cache/content/faa51a5044a3c279
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/d_0ccc93afd6526b6c___about___py.html
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/d_0ccc93afd6526b6c___init___py.html
+-rw-r--r--   0        0        0   127189 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/d_0ccc93afd6526b6c_core_py.html
+-rw-r--r--   0        0        0    60671 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/d_0ccc93afd6526b6c_fields_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 typedal-1.2.2/htmlcov/style.css
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 typedal-1.2.2/src/typedal/__about__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 typedal-1.2.2/src/typedal/__init__.py
+-rw-r--r--   0        0        0    15998 2020-02-02 00:00:00.000000 typedal-1.2.2/src/typedal/core.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 typedal-1.2.2/src/typedal/fields.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedal-1.2.2/src/typedal/py.typed
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 typedal-1.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 typedal-1.2.2/tests/test_main.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 typedal-1.2.2/tests/test_mypy.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 typedal-1.2.2/.gitignore
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 typedal-1.2.2/README.md
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 typedal-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 typedal-1.2.2/PKG-INFO
```

### Comparing `typedal-1.2.1/CHANGELOG.md` & `typedal-1.2.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.2.2 (2023-07-06)
+### Fix
+
+* Allow using `TypedFieldType`s in .select() ([`2945d15`](https://github.com/trialandsuccess/TypeDAL/commit/2945d15b3856f4881d27bd00504b3a2b7363b7ed))
+
 ## v1.2.1 (2023-06-27)
 ### Fix
 
 * Typehint query options for db() and update_or_insert() ([`2b65f58`](https://github.com/trialandsuccess/TypeDAL/commit/2b65f58ccf93f12713877fd420ec43454911efe9))
 
 ## v1.2.0 (2023-06-27)
 ### Feature
```

### Comparing `typedal-1.2.1/coverage.svg` & `typedal-1.2.2/coverage.svg`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/example_new.py` & `typedal-1.2.2/example_new.py`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/example_old.py` & `typedal-1.2.2/example_old.py`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_ast.data.json` & `typedal-1.2.2/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_ast.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_codecs.data.json` & `typedal-1.2.2/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_codecs.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_collections_abc.data.json` & `typedal-1.2.2/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_collections_abc.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_ctypes.data.json` & `typedal-1.2.2/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_ctypes.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_decimal.data.json` & `typedal-1.2.2/.mypy_cache/3.10/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_decimal.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/abc.data.json` & `typedal-1.2.2/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/abc.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/array.data.json` & `typedal-1.2.2/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/array.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/builtins.data.json` & `typedal-1.2.2/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/builtins.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/codecs.data.json` & `typedal-1.2.2/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/codecs.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/contextlib.data.json` & `typedal-1.2.2/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/contextlib.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/dataclasses.data.json` & `typedal-1.2.2/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/dataclasses.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/datetime.data.json` & `typedal-1.2.2/.mypy_cache/3.10/datetime.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/datetime.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/decimal.data.json` & `typedal-1.2.2/.mypy_cache/3.10/decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/decimal.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/enum.data.json` & `typedal-1.2.2/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/enum.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/genericpath.data.json` & `typedal-1.2.2/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/genericpath.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/io.data.json` & `typedal-1.2.2/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/io.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/mmap.data.json` & `typedal-1.2.2/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/mmap.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/numbers.data.json` & `typedal-1.2.2/.mypy_cache/3.10/numbers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/numbers.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/pathlib.data.json` & `typedal-1.2.2/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/pathlib.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/pickle.data.json` & `typedal-1.2.2/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/pickle.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/posixpath.data.json` & `typedal-1.2.2/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/posixpath.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/re.data.json` & `typedal-1.2.2/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/re.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/sre_compile.data.json` & `typedal-1.2.2/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/sre_compile.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/sre_constants.data.json` & `typedal-1.2.2/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/sre_constants.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/sre_parse.data.json` & `typedal-1.2.2/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/sre_parse.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/subprocess.data.json` & `typedal-1.2.2/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/subprocess.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/sys.data.json` & `typedal-1.2.2/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/sys.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/time.data.json` & `typedal-1.2.2/.mypy_cache/3.10/time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/time.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/types.data.json` & `typedal-1.2.2/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/types.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/typing.data.json` & `typedal-1.2.2/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/typing.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/typing_extensions.data.json` & `typedal-1.2.2/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/typing_extensions.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_typeshed/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/collections/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/collections/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/collections/abc.data.json` & `typedal-1.2.2/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/collections/abc.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/ctypes/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/ctypes/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/charset.data.json` & `typedal-1.2.2/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/charset.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/contentmanager.data.json` & `typedal-1.2.2/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/contentmanager.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/errors.data.json` & `typedal-1.2.2/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/errors.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/header.data.json` & `typedal-1.2.2/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/header.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/message.data.json` & `typedal-1.2.2/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/message.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/policy.data.json` & `typedal-1.2.2/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/email/policy.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/importlib/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/importlib/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/importlib/abc.data.json` & `typedal-1.2.2/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/importlib/abc.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/importlib/machinery.data.json` & `typedal-1.2.2/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/importlib/machinery.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `typedal-1.2.2/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/os/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/os/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/os/path.data.json` & `typedal-1.2.2/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/os/path.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.10/src/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/src/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/typedal/__about__.data.json` & `typedal-1.2.2/.mypy_cache/3.10/src/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/typedal/__about__.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/src/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/typedal/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.10/src/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/typedal/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/src/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/typedal/core.data.json` & `typedal-1.2.2/.mypy_cache/3.10/src/typedal/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/typedal/core.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/src/typedal/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/typedal/fields.data.json` & `typedal-1.2.2/.mypy_cache/3.10/src/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/typedal/fields.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/src/typedal/fields.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/typedal/pydal_objects.data.json` & `typedal-1.2.2/.mypy_cache/3.10/src/typedal/pydal_objects.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json` & `typedal-1.2.2/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_ast.data.json` & `typedal-1.2.2/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_ast.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_codecs.data.json` & `typedal-1.2.2/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_codecs.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_collections_abc.data.json` & `typedal-1.2.2/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_collections_abc.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_ctypes.data.json` & `typedal-1.2.2/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_ctypes.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_decimal.data.json` & `typedal-1.2.2/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_decimal.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/abc.data.json` & `typedal-1.2.2/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/abc.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/array.data.json` & `typedal-1.2.2/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/array.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/builtins.data.json` & `typedal-1.2.2/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/builtins.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/codecs.data.json` & `typedal-1.2.2/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/codecs.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/contextlib.data.json` & `typedal-1.2.2/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/contextlib.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/dataclasses.data.json` & `typedal-1.2.2/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/dataclasses.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/datetime.data.json` & `typedal-1.2.2/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/datetime.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/decimal.data.json` & `typedal-1.2.2/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/decimal.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/enum.data.json` & `typedal-1.2.2/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/enum.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/example_new.data.json` & `typedal-1.2.2/.mypy_cache/3.11/example_new.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/example_new.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/example_new.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/genericpath.data.json` & `typedal-1.2.2/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/genericpath.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/io.data.json` & `typedal-1.2.2/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/io.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/mmap.data.json` & `typedal-1.2.2/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/mmap.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/numbers.data.json` & `typedal-1.2.2/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/numbers.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/pathlib.data.json` & `typedal-1.2.2/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/pathlib.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/pickle.data.json` & `typedal-1.2.2/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/pickle.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/posixpath.data.json` & `typedal-1.2.2/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/posixpath.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/re.data.json` & `typedal-1.2.2/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/re.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src.data.json` & `typedal-1.2.2/.mypy_cache/3.11/src.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/src.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/sre_compile.data.json` & `typedal-1.2.2/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/sre_compile.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/sre_constants.data.json` & `typedal-1.2.2/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/sre_constants.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/sre_parse.data.json` & `typedal-1.2.2/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/sre_parse.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/subprocess.data.json` & `typedal-1.2.2/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/subprocess.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/sys.data.json` & `typedal-1.2.2/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/sys.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/time.data.json` & `typedal-1.2.2/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/time.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/types.data.json` & `typedal-1.2.2/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/types.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typing.data.json` & `typedal-1.2.2/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typing.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typing_extensions.data.json` & `typedal-1.2.2/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typing_extensions.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_typeshed/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/collections/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/collections/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/collections/abc.data.json` & `typedal-1.2.2/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/collections/abc.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/ctypes/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/ctypes/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/charset.data.json` & `typedal-1.2.2/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/charset.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/contentmanager.data.json` & `typedal-1.2.2/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/contentmanager.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/errors.data.json` & `typedal-1.2.2/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/errors.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/header.data.json` & `typedal-1.2.2/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/header.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/message.data.json` & `typedal-1.2.2/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/message.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/policy.data.json` & `typedal-1.2.2/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/email/policy.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/importlib/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/importlib/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/importlib/abc.data.json` & `typedal-1.2.2/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/importlib/abc.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/importlib/machinery.data.json` & `typedal-1.2.2/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/importlib/machinery.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `typedal-1.2.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/os/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/os/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/os/path.data.json` & `typedal-1.2.2/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/os/path.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/src/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/src/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src/typedal/__about__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/src/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src/typedal/__about__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/src/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src/typedal/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/src/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src/typedal/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/src/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src/typedal/core.data.json` & `typedal-1.2.2/.mypy_cache/3.11/src/typedal/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src/typedal/core.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/src/typedal/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src/typedal/fields.data.json` & `typedal-1.2.2/.mypy_cache/3.11/src/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/src/typedal/fields.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/src/typedal/fields.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typedal/__about__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typedal/__about__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/typedal/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7266666666666667%*

 * *Differences: {"'data_mtime'": '1688650846',*

 * * "'dep_lines'": '{insert: [(0, 5), (1, 6)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'typedal.fields'), (1, 'typedal.core')]}",*

 * * "'hash'": "'86d37918830825d489c752ba036279764d920eb61960613df7edd1ea97ababeb'",*

 * * "'id'": "'typedal'",*

 * * "'interface_hash'": "'02445b61c73d58f2edb445e4d531ec93da432ca9e7dd8ca09bbc5336f30bdf07'",*

 * * "'mtime'": '1687424172',*

 * * "'path'": "'src/typedal/__init__.py'",*

 * * "'size'": '201'}*

```diff
@@ -1,29 +1,35 @@
 {
-    "data_mtime": 1685969397,
+    "data_mtime": 1688650846,
     "dep_lines": [
+        5,
+        6,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        5,
         30,
         30
     ],
     "dependencies": [
+        "typedal.fields",
+        "typedal.core",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "715b564c762b0d7a05435d3d89098ff8e0731a48bf0ce68da91aeda6c4af1a60",
-    "id": "typedal.__about__",
+    "hash": "86d37918830825d489c752ba036279764d920eb61960613df7edd1ea97ababeb",
+    "id": "typedal",
     "ignore_all": false,
-    "interface_hash": "78ab11aa8e8cfd1f5fac091f83a1f2c46aac46f2e8973053a728baf5854e8af9",
-    "mtime": 1687881086,
+    "interface_hash": "02445b61c73d58f2edb445e4d531ec93da432ca9e7dd8ca09bbc5336f30bdf07",
+    "mtime": 1687424172,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/typedal/__about__.py",
+    "path": "src/typedal/__init__.py",
     "plugin_data": null,
-    "size": 206,
+    "size": 201,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typedal/__init__.data.json` & `typedal-1.2.2/.mypy_cache/3.11/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typedal/__init__.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/typedal/core.meta.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6543859649122807%*

 * *Differences: {"'data_mtime'": '1688650846',*

 * * "'dep_lines'": '{insert: [(0, 4), (3, 7), (4, 8), (5, 9), (6, 1), (7, 1), (8, 1), (9, 1), (10, '*

 * *                '1), (11, 1), (12, 1), (16, 13), (17, 14), (18, 12)]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 10), (2, 10), (3, 5), (7, 30), (8, 30), (9, 30), (10, 30), '*

 * *                '(11, 30), (12, 30), (13, 30), (16, 5), (17, 5), (18, 10)]}',*

 * * "'dependencies'": "{insert: [(0, 'contextlib'), (1, 'datetime'), (2, 'types'), (3, 'typing'), (4, "*

 * *                   "'collection […]*

```diff
@@ -1,35 +1,74 @@
 {
-    "data_mtime": 1687879747,
+    "data_mtime": 1688650846,
     "dep_lines": [
+        4,
         5,
         6,
+        7,
+        8,
+        9,
         1,
         1,
-        1
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        13,
+        14,
+        12
     ],
     "dep_prios": [
+        10,
+        10,
+        10,
         5,
         5,
         5,
+        5,
+        30,
         30,
-        30
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        5,
+        5,
+        10
     ],
     "dependencies": [
-        "typedal.fields",
-        "typedal.core",
+        "contextlib",
+        "datetime",
+        "types",
+        "typing",
+        "collections",
+        "decimal",
         "builtins",
+        "_collections_abc",
+        "_decimal",
+        "_typeshed",
         "abc",
-        "typing"
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle",
+        "typing_extensions"
     ],
-    "hash": "86d37918830825d489c752ba036279764d920eb61960613df7edd1ea97ababeb",
-    "id": "typedal",
+    "hash": "9f25929dda020b46a9c396b3b1a9a66678d278a2991eefe0c6af7cb1ebdb8d12",
+    "id": "typedal.core",
     "ignore_all": false,
-    "interface_hash": "02445b61c73d58f2edb445e4d531ec93da432ca9e7dd8ca09bbc5336f30bdf07",
-    "mtime": 1687424172,
+    "interface_hash": "656067d89d1a4de189f7ffe696fe8ec67e648a6067a1e02421c7a8fa389261b1",
+    "mtime": 1688650869,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +102,17 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/typedal/__init__.py",
+    "path": "src/typedal/core.py",
     "plugin_data": null,
-    "size": 201,
-    "suppressed": [],
+    "size": 15998,
+    "suppressed": [
+        "pydal._globals",
+        "pydal.objects",
+        "pydal"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typedal/core.data.json` & `typedal-1.2.2/.mypy_cache/3.11/typedal/core.data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946144885659046%*

 * *Differences: {"'names'": "{'T_Query': {'node': {'line': 18}}, 'T_annotation': {'node': {'line': 17}}, "*

 * *            "'TypedFieldType': {'node': {'names': {'_db': {'node': {'flags': {insert: [(1, "*

 * *            "'is_ready')], delete: [1]}, 'type': {'.class': 'UnionType', 'items': "*

 * *            "[OrderedDict([('.class', 'AnyType'), ('missing_import_name', 'typedal.core.pydal'), "*

 * *            "('source_any', None), ('type_of_any', 3)]), OrderedDict([('.class', "*

 * *            "'NoneType')])]}}}, '_rname': {'node': {'flags': { […]*

```diff
@@ -92,14 +92,21 @@
                 "self_type": null,
                 "slots": null,
                 "tuple_type": null,
                 "type_vars": [],
                 "typeddict_type": null
             }
         },
+        "Any": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.Any",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "BASIC_MAPPINGS": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready",
@@ -175,14 +182,21 @@
                     ".class": "AnyType",
                     "missing_import_name": "typedal.core.Field",
                     "source_any": null,
                     "type_of_any": 3
                 }
             }
         },
+        "Optional": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.Optional",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "Query": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false,
             "node": {
                 ".class": "Var",
@@ -287,15 +301,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "typedal.core.T_Query",
-                "line": 16,
+                "line": 18,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         {
                             ".class": "AnyType",
@@ -343,15 +357,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "typedal.core.T_annotation",
-                "line": 15,
+                "line": 17,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         {
                             ".class": "TypeType",
@@ -1203,14 +1217,67 @@
                 "module_name": "typedal.core",
                 "mro": [
                     "typedal.core.TypedFieldType",
                     "builtins.object"
                 ],
                 "names": {
                     ".class": "SymbolTable",
+                    "__getattr__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                null,
+                                null
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "typedal.core.TypedFieldType.__getattr__",
+                            "name": "__getattr__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    null,
+                                    null
+                                ],
+                                "arg_types": [
+                                    "typedal.core.TypedFieldType",
+                                    "builtins.str"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__getattr__ of TypedFieldType",
+                                "ret_type": {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 2
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
                     "__init__": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
@@ -1360,55 +1427,111 @@
                     "_db": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
                                 "is_initialized_in_class",
-                                "is_inferred",
+                                "is_ready",
                                 "has_explicit_value"
                             ],
                             "fullname": "typedal.core.TypedFieldType._db",
                             "name": "_db",
                             "type": {
-                                ".class": "NoneType"
+                                ".class": "UnionType",
+                                "items": [
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": "typedal.core.pydal",
+                                        "source_any": null,
+                                        "type_of_any": 3
+                                    },
+                                    {
+                                        ".class": "NoneType"
+                                    }
+                                ]
+                            }
+                        }
+                    },
+                    "_field": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready",
+                                "has_explicit_value"
+                            ],
+                            "fullname": "typedal.core.TypedFieldType._field",
+                            "name": "_field",
+                            "type": {
+                                ".class": "UnionType",
+                                "items": [
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": "typedal.core.Table",
+                                        "source_any": null,
+                                        "type_of_any": 3
+                                    },
+                                    {
+                                        ".class": "NoneType"
+                                    }
+                                ]
                             }
                         }
                     },
                     "_rname": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
                                 "is_initialized_in_class",
-                                "is_inferred",
+                                "is_ready",
                                 "has_explicit_value"
                             ],
                             "fullname": "typedal.core.TypedFieldType._rname",
                             "name": "_rname",
                             "type": {
-                                ".class": "NoneType"
+                                ".class": "UnionType",
+                                "items": [
+                                    "builtins.str",
+                                    {
+                                        ".class": "NoneType"
+                                    }
+                                ]
                             }
                         }
                     },
                     "_table": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
                                 "is_initialized_in_class",
-                                "is_inferred",
+                                "is_ready",
                                 "has_explicit_value"
                             ],
                             "fullname": "typedal.core.TypedFieldType._table",
                             "name": "_table",
                             "type": {
-                                ".class": "NoneType"
+                                ".class": "UnionType",
+                                "items": [
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": "typedal.core.Table",
+                                        "source_any": null,
+                                        "type_of_any": 3
+                                    },
+                                    {
+                                        ".class": "NoneType"
+                                    }
+                                ]
                             }
                         }
                     },
                     "_to_field": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
@@ -1630,15 +1753,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "typedal.core.TypedRow",
-                "line": 349,
+                "line": 351,
                 "no_args": true,
                 "normalized": false,
                 "target": "typedal.core.TypedTable"
             }
         },
         "TypedRows": {
             ".class": "SymbolTableNode",
@@ -2751,15 +2874,15 @@
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "TypeAlias",
                             "alias_tvars": [],
                             "column": 4,
                             "fullname": "typedal.core._Types.NONETYPE",
-                            "line": 37,
+                            "line": 39,
                             "no_args": false,
                             "normalized": false,
                             "target": {
                                 ".class": "NoneType"
                             }
                         }
                     }
@@ -2963,14 +3086,21 @@
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
+        "contextlib": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "contextlib",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "dt": {
             ".class": "SymbolTableNode",
             "cross_ref": "datetime",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
```

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typedal/core.meta.json` & `typedal-1.2.2/.mypy_cache/3.11/typedal/fields.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7142019263845889%*

 * *Differences: {"'data_mtime'": '1688650846',*

 * * "'dep_lines'": '{insert: [(0, 12)], delete: [16, 15, 5, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (4, 10)], delete: [17, 15, 6, 4, 3]}',*

 * * "'dependencies'": "{insert: [(0, 'typedal.core'), (2, 'decimal')], delete: [6, 4, 3]}",*

 * * "'hash'": "'2da5da10836f40ec000f32c64446f28df3e5081a9e14d5473684770659627369'",*

 * * "'id'": "'typedal.fields'",*

 * * "'interface_hash'": "'7f52734fa267868275c2d07b23b14504cf86d84ca8ba75738eacb85b5ff41a00'",*

 * * "'mtime'": '1687423422',*

 * * "'path'": "'src/typedal/fie […]*

```diff
@@ -1,71 +1,64 @@
 {
-    "data_mtime": 1687882472,
+    "data_mtime": 1688650846,
     "dep_lines": [
-        4,
+        12,
         5,
         6,
         7,
         8,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1,
-        11,
-        12,
         10
     ],
     "dep_prios": [
+        5,
+        10,
         10,
         10,
         10,
-        5,
-        5,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        5,
-        5,
-        10
+        5
     ],
     "dependencies": [
+        "typedal.core",
         "datetime",
+        "decimal",
         "types",
         "typing",
-        "collections",
-        "decimal",
         "builtins",
-        "_collections_abc",
         "_decimal",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
         "pickle",
         "typing_extensions"
     ],
-    "hash": "14e567a449e281cd42f7beb83cf9625a9f4fa46929fd5aee437f19cc7fb7505c",
-    "id": "typedal.core",
+    "hash": "2da5da10836f40ec000f32c64446f28df3e5081a9e14d5473684770659627369",
+    "id": "typedal.fields",
     "ignore_all": false,
-    "interface_hash": "2a8637fd7039de29c861d95cfdb6fdf32577902c31ebc2db1a4c65341d866760",
-    "mtime": 1687882471,
+    "interface_hash": "7f52734fa267868275c2d07b23b14504cf86d84ca8ba75738eacb85b5ff41a00",
+    "mtime": 1687423422,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -99,17 +92,15 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/typedal/core.py",
+    "path": "src/typedal/fields.py",
     "plugin_data": null,
-    "size": 15559,
+    "size": 4949,
     "suppressed": [
-        "pydal._globals",
-        "pydal.objects",
-        "pydal"
+        "pydal.objects"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `typedal-1.2.1/.mypy_cache/3.11/typedal/fields.data.json` & `typedal-1.2.2/.mypy_cache/3.11/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.pytest_cache/v/cache/nodeids` & `typedal-1.2.2/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/1b34455c399f0006` & `typedal-1.2.2/.ruff_cache/content/1b34455c399f0006`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/20585cf790eae81e` & `typedal-1.2.2/.ruff_cache/content/20585cf790eae81e`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/221af82ae72a7f27` & `typedal-1.2.2/.ruff_cache/content/221af82ae72a7f27`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/24e1b4aab386ebc8` & `typedal-1.2.2/.ruff_cache/content/24e1b4aab386ebc8`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/2f3396c610fd7095` & `typedal-1.2.2/.ruff_cache/content/2f3396c610fd7095`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/322af04e6d059ce5` & `typedal-1.2.2/.ruff_cache/content/322af04e6d059ce5`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/3826106cf4494de8` & `typedal-1.2.2/.ruff_cache/content/3826106cf4494de8`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/38d5fd55b14a9d6c` & `typedal-1.2.2/.ruff_cache/content/38d5fd55b14a9d6c`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/4022ee8774ccd98a` & `typedal-1.2.2/.ruff_cache/content/4022ee8774ccd98a`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/5491563776466765346` & `typedal-1.2.2/.ruff_cache/content/5491563776466765346`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/75bd1769f6e29ed7` & `typedal-1.2.2/.ruff_cache/content/75bd1769f6e29ed7`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/a0739889bf9412e8` & `typedal-1.2.2/.ruff_cache/content/a0739889bf9412e8`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/a225e4df39be9b29` & `typedal-1.2.2/.ruff_cache/content/a225e4df39be9b29`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/b419496fa9e72887` & `typedal-1.2.2/.ruff_cache/content/b419496fa9e72887`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/bdcdf5c7bbc1d738` & `typedal-1.2.2/.ruff_cache/content/bdcdf5c7bbc1d738`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/c06de16f3c7a64cc` & `typedal-1.2.2/.ruff_cache/content/c06de16f3c7a64cc`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/cdfecbca581311ee` & `typedal-1.2.2/.ruff_cache/content/cdfecbca581311ee`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/da4811a7730a562a` & `typedal-1.2.2/.ruff_cache/content/da4811a7730a562a`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/.ruff_cache/content/eee2f3c667de6c7a` & `typedal-1.2.2/.ruff_cache/content/eee2f3c667de6c7a`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/coverage_html.js` & `typedal-1.2.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c___about___py.html` & `typedal-1.2.2/htmlcov/d_0ccc93afd6526b6c___about___py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c___init___py.html` & `typedal-1.2.2/htmlcov/d_0ccc93afd6526b6c___init___py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c_core_py.html` & `typedal-1.2.2/htmlcov/d_0ccc93afd6526b6c_core_py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c_fields_py.html` & `typedal-1.2.2/htmlcov/d_0ccc93afd6526b6c_fields_py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/favicon_32.png` & `typedal-1.2.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/index.html` & `typedal-1.2.2/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/keybd_closed.png` & `typedal-1.2.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/keybd_open.png` & `typedal-1.2.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/status.json` & `typedal-1.2.2/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/htmlcov/style.css` & `typedal-1.2.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/src/typedal/core.py` & `typedal-1.2.2/src/typedal/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 Core functionality of TypeDAL.
 """
+import contextlib
 import datetime as dt
 import types
 import typing
 from collections import ChainMap
 from decimal import Decimal
+from typing import Any, Optional
 
 import pydal
 from pydal._globals import DEFAULT
 from pydal.objects import Field, Query, Row, Rows, Table
 
 # use typing.cast(type, ...) to make mypy happy with unions
-T_annotation = typing.Type[typing.Any] | types.UnionType
-T_Query = typing.Union["Table", "Query", "bool", "None", "TypedTable", typing.Type["TypedTable"]]
+T_annotation = typing.Type[Any] | types.UnionType
+T_Query = typing.Union[Table, Query, bool, None, "TypedTable", typing.Type["TypedTable"]]
 
 BASIC_MAPPINGS: dict[T_annotation, str] = {
     str: "string",
     int: "integer",
     bool: "boolean",
     bytes: "blob",
     float: "double",
@@ -173,15 +175,15 @@
     @classmethod
     def _build_field(cls, name: str, _type: str, **kw: typing.Any) -> Field:
         return Field(name, _type, **{**cls.default_kwargs, **kw})
 
     @classmethod
     def _annotation_to_pydal_fieldtype(
         cls, _ftype: T_annotation, mut_kw: typing.MutableMapping[str, typing.Any]
-    ) -> typing.Optional[str]:
+    ) -> Optional[str]:
         # ftype can be a union or type. typing.cast is sometimes used to tell mypy when it's not a union.
         ftype = typing.cast(type, _ftype)  # cast from typing.Type to type to make mypy happy)
 
         if mapping := BASIC_MAPPINGS.get(ftype):
             # basi types
             return mapping
         elif isinstance(ftype, Table):
@@ -199,15 +201,15 @@
             _child_type = typing.get_args(ftype)[0]
             _child_type = cls._annotation_to_pydal_fieldtype(_child_type, mut_kw)
             return f"list:{_child_type}"
         elif is_union(ftype):
             # str | int -> UnionType
             # typing.Union[str | int] -> typing._UnionGenericAlias
 
-            # typing.Optional[type] == type | None
+            # Optional[type] == type | None
 
             match typing.get_args(ftype):
                 case (_child_type, _Types.NONETYPE):
                     # good union of Nullable
 
                     # if a field is optional, it is nullable:
                     mut_kw["notnull"] = False
@@ -330,15 +332,15 @@
             raise EnvironmentError("@define or db.define is not called on this class yet!")
 
         result = super().insert(cls.__table, **fields)
         # it already is an int but mypy doesn't understand that
         return typing.cast(int, result)
 
     @classmethod
-    def update_or_insert(cls, query: T_Query = DEFAULT, **values: typing.Any) -> typing.Optional[int]:
+    def update_or_insert(cls, query: T_Query = DEFAULT, **values: typing.Any) -> Optional[int]:
         """
         Add typing to pydal's update_or_insert.
         """
         result = super().update_or_insert(cls, _key=query, **values)
         if result is None:
             return None
         else:
@@ -354,17 +356,18 @@
     Typed version of pydal.Field, which will be converted to a normal Field in the background.
     """
 
     # todo: .bind
 
     # will be set by .bind on db.define
     name = ""
-    _db = None
-    _rname = None
-    _table = None
+    _db: Optional[pydal.DAL] = None
+    _rname: Optional[str] = None
+    _table: Optional[Table] = None
+    _field: Optional[Table] = None
 
     _type: T_annotation
     kwargs: typing.Any
 
     def __init__(self, _type: T_annotation, **kwargs: typing.Any) -> None:
         """
         A TypedFieldType should not be inited manually, but TypedField (from `fields.py`) should be used!
@@ -400,33 +403,44 @@
         Uses __str__ and adds the provided extra options (kwargs) in the representation.
         """
         s = self.__str__()
         kw = self.kwargs.copy()
         kw.pop("type", None)
         return f"<{s} with options {kw}>"
 
-    def _to_field(self, extra_kwargs: typing.MutableMapping[str, typing.Any]) -> typing.Optional[str]:
+    def _to_field(self, extra_kwargs: typing.MutableMapping[str, typing.Any]) -> Optional[str]:
         """
         Convert a Typed Field instance to a pydal.Field.
         """
         other_kwargs = self.kwargs.copy()
         extra_kwargs.update(other_kwargs)
         return extra_kwargs.pop("type", False) or TypeDAL._annotation_to_pydal_fieldtype(self._type, extra_kwargs)
 
     def bind(self, field: Field, table: Table) -> None:
         """
         Bind the right db/table/field info to this class, so queries can be made using `Class.field == ...`.
         """
+        self._field = field
         self.name = field.name
         self.type = field.type
+        # ._itype etc via getattrs
         super().bind(table)
 
     # def __eq__(self, value):
     #     return Query(self.db, self._dialect.eq, self, value)
 
+    def __getattr__(self, key: str) -> Any:
+        """
+        If the regular getattribute does not work, try to get info from the related Field.
+        """
+        with contextlib.suppress(AttributeError):
+            return super().__getattribute__(key)
+
+        return getattr(self._field, key)
+
 
 S = typing.TypeVar("S")
 
 
 class TypedRows(typing.Collection[S], Rows):  # type: ignore
     """
     Can be used as the return type of a .select().
@@ -442,22 +456,22 @@
 class TypedSet(pydal.objects.Set):  # type: ignore # pragma: no cover
     """
     Used to make pydal Set more typed.
 
     This class is not actually used, only 'cast' by TypeDAL.__call__
     """
 
-    def count(self, distinct: bool = None, cache: dict[str, typing.Any] = None) -> int:
+    def count(self, distinct: bool = None, cache: dict[str, Any] = None) -> int:
         """
         Count returns an int.
         """
         result = super().count(distinct, cache)
         return typing.cast(int, result)
 
-    def select(self, *fields: typing.Any, **attributes: typing.Any) -> TypedRows[T_Table]:
+    def select(self, *fields: Any, **attributes: Any) -> TypedRows[T_Table]:
         """
         Select returns a TypedRows of a user defined table.
 
         Example:
             result: TypedRows[MyTable] = db(MyTable.id > 0).select()
 
             for row in result:
```

### Comparing `typedal-1.2.1/src/typedal/fields.py` & `typedal-1.2.2/src/typedal/fields.py`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/tests/test_main.py` & `typedal-1.2.2/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,15 @@
             third = TypedField(dict[str, int])  # not supported
 
 
 def test_fields():
     @db.define
     class SomeNewTable(TypedTable):
         name: str
+        name_alt = TypedField(str)
 
     class OtherNewTable(TypedTable):
         name: str
 
     db.define(OtherNewTable)
 
     assert str(StringField()) == "TypedField.string"
@@ -261,22 +262,23 @@
     # test typedset:
     counted1 = db(SomeNewTable).count()
     counted2 = db(OtherNewTable).count()
     counted3 = db(db.some_new_table).count()
 
     assert counted1 == counted2 == counted3 == 0
 
-    select2: TypedRows[SomeNewTable] = db(SomeNewTable).select()
+    select2: TypedRows[SomeNewTable] = db(SomeNewTable.id > 0).select(SomeNewTable.name, SomeNewTable.name_alt)
 
     for row in select2:
         raise ValueError("no rows should exist")
 
     SomeNewTable.update_or_insert(
         SomeNewTable.name == "Hendrik",
         name="Hendrik 2",
+        name_alt="Hendrik II"
     )
 
     idx = OtherNewTable.update_or_insert(
         OtherNewTable.name == "Hendrik",
         name="Hendrik 2",
     )
     assert idx
```

### Comparing `typedal-1.2.1/tests/test_mypy.py` & `typedal-1.2.2/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/README.md` & `typedal-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/pyproject.toml` & `typedal-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedal-1.2.1/PKG-INFO` & `typedal-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TypeDal
-Version: 1.2.1
+Version: 1.2.2
 Summary: Typing support for PyDAL
 Project-URL: Documentation, https://github.com/trialandsuccess/TypeDAL#readme
 Project-URL: Issues, https://github.com/trialandsuccess/TypeDAL/issues
 Project-URL: Source, https://github.com/trialandsuccess/TypeDAL
 Author-email: Robin van der Noord <contact@trialandsuccess.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

