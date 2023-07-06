# Comparing `tmp/pydash-7.0.4.tar.gz` & `tmp/pydash-7.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash-7.0.4.tar", last modified: Fri Jun  2 14:03:15 2023, max compression
+gzip compressed data, was "pydash-7.0.5.tar", last modified: Thu Jul  6 13:57:26 2023, max compression
```

## Comparing `pydash-7.0.4.tar` & `pydash-7.0.5.tar`

### file list

```diff
@@ -1,633 +1,630 @@
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.498645 pydash-7.0.4/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.446816 pydash-7.0.4/.tox/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.432870 pydash-7.0.4/.tox/.package/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.432916 pydash-7.0.4/.tox/.package/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.432956 pydash-7.0.4/.tox/.package/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.432995 pydash-7.0.4/.tox/.package/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.453302 pydash-7.0.4/.tox/.package/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.4/.tox/.package/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433102 pydash-7.0.4/.tox/.pkg/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433144 pydash-7.0.4/.tox/.pkg/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433184 pydash-7.0.4/.tox/.pkg/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433224 pydash-7.0.4/.tox/.pkg/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.453573 pydash-7.0.4/.tox/.pkg/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.4/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433329 pydash-7.0.4/.tox/3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433371 pydash-7.0.4/.tox/3.11/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.433420 pydash-7.0.4/.tox/3.11/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.435972 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.453838 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.453937 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454021 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454109 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454395 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454484 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454581 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454675 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454772 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454872 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.454974 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455267 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455367 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455470 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455558 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455643 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.434504 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.455743 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456011 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456087 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456165 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456374 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456469 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456709 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.456802 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457049 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457129 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457346 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457552 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457633 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457731 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457828 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.457926 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458022 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458270 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458348 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458427 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458506 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458588 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458673 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458766 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.4/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.436064 pydash-7.0.4/.tox/py310/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.436101 pydash-7.0.4/.tox/py310/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.436138 pydash-7.0.4/.tox/py310/lib/python3.10/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.438506 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458860 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.458938 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459028 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459124 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459371 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459455 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459534 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459608 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459689 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459769 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.459867 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460099 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460175 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460252 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460332 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460408 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460494 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.437195 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460587 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460844 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.460923 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461005 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461205 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461281 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461504 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461596 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461823 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.461908 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462128 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462346 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462430 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462510 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462594 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462677 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.462767 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463092 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463205 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463313 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463417 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463518 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463791 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463885 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.463978 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.4/.tox/py310/lib/python3.10/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.438600 pydash-7.0.4/.tox/py311/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.438636 pydash-7.0.4/.tox/py311/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.438672 pydash-7.0.4/.tox/py311/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.441148 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464085 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464183 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464285 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464390 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464671 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464773 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464873 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.464965 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465052 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465142 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465225 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465551 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465666 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465777 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465876 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.465968 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.439678 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466056 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466334 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466412 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466495 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466764 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.466849 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467089 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467173 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467378 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467462 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467716 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.467926 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468010 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468159 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468288 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468387 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468491 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468748 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468855 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.468944 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469031 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469118 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469206 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469296 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.4/.tox/py311/lib/python3.11/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.441270 pydash-7.0.4/.tox/py37/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.441321 pydash-7.0.4/.tox/py37/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.441370 pydash-7.0.4/.tox/py37/lib/python3.7/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.443706 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469383 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469467 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469550 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469634 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469869 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.469964 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470049 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470135 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470214 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470294 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470545 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470628 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470720 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470825 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.470925 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471020 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.442412 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471114 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471349 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471439 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471526 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471775 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.471850 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472085 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472178 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472389 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472482 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472680 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472885 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.472965 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473044 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/py/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.443162 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473126 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/py/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473208 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473296 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473386 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473624 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473725 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473815 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.473908 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474025 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474301 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474417 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.4/.tox/py37/lib/python3.7/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.443799 pydash-7.0.4/.tox/py38/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.443836 pydash-7.0.4/.tox/py38/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.443874 pydash-7.0.4/.tox/py38/lib/python3.8/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.446715 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474531 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474640 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474746 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.474857 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475153 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475254 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475357 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475467 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475571 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475658 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.475760 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476049 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476211 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476307 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476419 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476523 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/importlib_resources/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476634 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476740 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.445199 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.476849 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477128 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477239 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477358 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477625 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477732 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.477990 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.478092 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.478311 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.478412 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.478668 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.478924 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479028 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479121 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479219 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479307 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479409 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479675 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479781 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479894 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.479996 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480106 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480352 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480464 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480578 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.4/.tox/py38/lib/python3.8/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.446870 pydash-7.0.4/.tox/py39/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.446923 pydash-7.0.4/.tox/py39/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.446976 pydash-7.0.4/.tox/py39/lib/python3.9/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.450126 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480687 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480796 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.480901 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481009 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481270 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481373 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481474 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481572 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481674 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481775 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.481877 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482144 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482253 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482358 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482452 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482545 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482636 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.448391 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.482745 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483007 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483109 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483209 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483425 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483509 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483704 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483781 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.483972 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484065 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484298 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484486 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484562 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484638 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484716 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484829 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.484923 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485170 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485257 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485335 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485416 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485510 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485725 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485820 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.485898 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.4/.tox/py39/lib/python3.9/site-packages/twine/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)     1396 2023-06-02 13:53:01.000000 pydash-7.0.4/AUTHORS.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    40727 2023-06-02 13:50:44.000000 pydash-7.0.4/CHANGELOG.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.4/CONTRIBUTING.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.4/LICENSE.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.4/MANIFEST.in
--rw-r--r--   0 dgilland   (501) staff       (20)    44202 2023-06-02 14:03:15.498748 pydash-7.0.4/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.4/README.rst
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.488634 pydash-7.0.4/docs/
--rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/Makefile
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.488880 pydash-7.0.4/docs/_static/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.4/docs/_static/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)      137 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/_static/theme_override.css
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.489010 pydash-7.0.4/docs/_templates/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.4/docs/_templates/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/api.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.4/docs/authors.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/callbacks.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.4/docs/chaining.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/changelog.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     5733 2022-09-23 13:07:13.000000 pydash-7.0.4/docs/conf.py
--rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.4/docs/contributing.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/deeppath.rst
--rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.4/docs/devguide.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/differences.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.4/docs/index.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.4/docs/installation.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/kudos.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.4/docs/license.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/quickstart.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/templating.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.4/docs/upgrading.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.4/docs/versioning.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.4/pylintrc
--rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.4/pyproject.toml
--rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.4/requirements.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     2536 2023-06-02 14:03:15.499134 pydash-7.0.4/setup.cfg
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.450516 pydash-7.0.4/src/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.492402 pydash-7.0.4/src/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)    11148 2023-06-02 13:50:23.000000 pydash-7.0.4/src/pydash/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    69733 2023-05-04 14:12:08.000000 pydash-7.0.4/src/pydash/arrays.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.493676 pydash-7.0.4/src/pydash/chaining/
--rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.4/src/pydash/chaining/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.4/src/pydash/chaining/all_funcs.py
--rw-r--r--   0 dgilland   (501) staff       (20)   123215 2023-05-04 14:12:08.000000 pydash-7.0.4/src/pydash/chaining/all_funcs.pyi
--rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.4/src/pydash/chaining/chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.4/src/pydash/exceptions.py
--rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/helpers.py
--rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.4/src/pydash/predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.4/src/pydash/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)      690 2023-04-27 16:14:56.000000 pydash-7.0.4/src/pydash/types.py
--rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.4/src/pydash/utilities.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.492982 pydash-7.0.4/src/pydash.egg-info/
--rw-r--r--   0 dgilland   (501) staff       (20)    44202 2023-06-02 14:03:13.000000 pydash-7.0.4/src/pydash.egg-info/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)    16310 2023-06-02 14:03:15.000000 pydash-7.0.4/src/pydash.egg-info/SOURCES.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-06-02 14:03:13.000000 pydash-7.0.4/src/pydash.egg-info/dependency_links.txt
--rw-r--r--   0 dgilland   (501) staff       (20)      301 2023-06-02 14:03:13.000000 pydash-7.0.4/src/pydash.egg-info/requires.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-06-02 14:03:13.000000 pydash-7.0.4/src/pydash.egg-info/top_level.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.4/tasks.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.496277 pydash-7.0.4/tests/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.4/tests/__init__.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.450764 pydash-7.0.4/tests/build/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.496439 pydash-7.0.4/tests/build/testresults/
--rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.4/tests/build/testresults/junit.xml
--rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.4/tests/conftest.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.4/tests/helpers.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-06-02 14:03:15.498515 pydash-7.0.4/tests/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.4/tests/pytest_mypy_testing/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    16882 2023-05-04 14:12:08.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.4/tests/pytest_mypy_testing/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.4/tests/test_annotations.py
--rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.4/tests/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.4/tests/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.4/tests/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.4/tests/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.4/tests/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.4/tests/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.4/tests/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.4/tests/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.4/tests/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.4/tox.ini
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.260303 pydash-7.0.5/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.205446 pydash-7.0.5/.tox/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.189874 pydash-7.0.5/.tox/.package/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.189941 pydash-7.0.5/.tox/.package/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.189989 pydash-7.0.5/.tox/.package/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190038 pydash-7.0.5/.tox/.package/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212134 pydash-7.0.5/.tox/.package/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.5/.tox/.package/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190170 pydash-7.0.5/.tox/.pkg/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190218 pydash-7.0.5/.tox/.pkg/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190273 pydash-7.0.5/.tox/.pkg/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190324 pydash-7.0.5/.tox/.pkg/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212401 pydash-7.0.5/.tox/.pkg/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.5/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190448 pydash-7.0.5/.tox/3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190500 pydash-7.0.5/.tox/3.11/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190557 pydash-7.0.5/.tox/3.11/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.193353 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212635 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212726 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212819 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212915 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213173 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213260 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213361 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213458 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213556 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213669 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213774 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214124 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214239 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214347 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214451 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214552 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.191785 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214656 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214939 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215028 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215117 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215432 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215541 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215799 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215902 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216156 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216259 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216514 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216774 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216864 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216958 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217042 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217127 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217216 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217490 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217581 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217667 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217750 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217843 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217937 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218028 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.193481 pydash-7.0.5/.tox/py310/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.193529 pydash-7.0.5/.tox/py310/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.193576 pydash-7.0.5/.tox/py310/lib/python3.10/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.196082 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218130 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218242 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218344 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218433 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218700 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218784 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218874 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218959 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219049 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219133 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219216 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219462 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219564 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219663 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219752 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219855 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219951 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.194594 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220039 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220288 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220399 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220508 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220734 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220826 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221074 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221180 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221422 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221508 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221705 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221935 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222030 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222130 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222233 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222338 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222443 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222667 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222760 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222844 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222939 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223028 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223281 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223372 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223474 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.196187 pydash-7.0.5/.tox/py311/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.196227 pydash-7.0.5/.tox/py311/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.196273 pydash-7.0.5/.tox/py311/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.199110 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223572 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223669 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223775 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223881 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224120 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224206 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224302 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224390 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224474 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224568 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224675 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224943 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225033 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225124 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225222 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225318 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.197430 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225410 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225639 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225726 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225812 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226080 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226174 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226417 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226507 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226744 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226829 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227068 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227288 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227387 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227484 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227588 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227688 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227791 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228035 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228135 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228222 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228309 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228397 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228487 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228590 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.199244 pydash-7.0.5/.tox/py37/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.199304 pydash-7.0.5/.tox/py37/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.199366 pydash-7.0.5/.tox/py37/lib/python3.7/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.202250 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228693 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228790 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228887 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228990 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229236 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229327 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229413 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229506 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229596 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229691 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229963 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230055 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230149 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230247 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230340 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230425 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.200646 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230512 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230778 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230887 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231002 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231268 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231359 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231593 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231683 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231890 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231976 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232192 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232437 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232543 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232663 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.201620 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232781 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/py/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232893 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233007 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233128 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233417 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233537 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233664 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233786 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233907 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234202 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234379 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.202360 pydash-7.0.5/.tox/py38/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.202411 pydash-7.0.5/.tox/py38/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.202465 pydash-7.0.5/.tox/py38/lib/python3.8/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.205355 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234517 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234648 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234766 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234877 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235143 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235265 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235386 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235505 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235624 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235745 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235871 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236152 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236268 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236389 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236504 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236658 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236777 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236905 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.203711 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237031 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237341 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237457 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237570 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237865 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237973 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.238230 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.238348 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.238602 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.238712 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.238963 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239220 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239339 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239452 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239566 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239669 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239788 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240069 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240176 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240283 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240402 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240516 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240789 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240901 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241014 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.205505 pydash-7.0.5/.tox/py39/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.205558 pydash-7.0.5/.tox/py39/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.205613 pydash-7.0.5/.tox/py39/lib/python3.9/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.208903 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241132 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241254 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241371 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241485 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241757 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241871 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241983 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242093 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242210 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242327 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242448 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242726 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242841 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242953 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243070 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243246 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243365 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.207067 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243482 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243746 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243850 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243955 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244220 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244320 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244526 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244625 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244860 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244957 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245205 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245420 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245522 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245629 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245753 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245863 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245979 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246245 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246348 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246450 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246561 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246662 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246930 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.247023 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.247122 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/twine/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)     1396 2023-06-02 13:53:01.000000 pydash-7.0.5/AUTHORS.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    40894 2023-07-06 13:44:03.000000 pydash-7.0.5/CHANGELOG.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.5/LICENSE.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.5/MANIFEST.in
+-rw-r--r--   0 dgilland   (501) staff       (20)    44369 2023-07-06 13:57:26.260416 pydash-7.0.5/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.5/README.rst
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.249857 pydash-7.0.5/docs/
+-rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/Makefile
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.249987 pydash-7.0.5/docs/_templates/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.5/docs/_templates/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/api.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.5/docs/authors.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/callbacks.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.5/docs/chaining.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/changelog.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     5356 2023-06-24 16:30:19.000000 pydash-7.0.5/docs/conf.py
+-rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.5/docs/contributing.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/deeppath.rst
+-rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.5/docs/devguide.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/differences.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.5/docs/index.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.5/docs/installation.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/kudos.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.5/docs/license.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/quickstart.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/templating.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/upgrading.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.5/docs/versioning.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.5/pylintrc
+-rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.5/pyproject.toml
+-rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.5/requirements.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     2524 2023-07-06 13:57:26.260824 pydash-7.0.5/setup.cfg
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.209270 pydash-7.0.5/src/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.253259 pydash-7.0.5/src/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)    11148 2023-07-06 13:44:11.000000 pydash-7.0.5/src/pydash/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    69930 2023-07-06 13:41:49.000000 pydash-7.0.5/src/pydash/arrays.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.254793 pydash-7.0.5/src/pydash/chaining/
+-rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.5/src/pydash/chaining/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.5/src/pydash/chaining/all_funcs.py
+-rw-r--r--   0 dgilland   (501) staff       (20)   123464 2023-07-06 13:41:49.000000 pydash-7.0.5/src/pydash/chaining/all_funcs.pyi
+-rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.5/src/pydash/chaining/chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.5/src/pydash/exceptions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/helpers.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.5/src/pydash/predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.5/src/pydash/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      690 2023-04-27 16:14:56.000000 pydash-7.0.5/src/pydash/types.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/utilities.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.254120 pydash-7.0.5/src/pydash.egg-info/
+-rw-r--r--   0 dgilland   (501) staff       (20)    44369 2023-07-06 13:57:24.000000 pydash-7.0.5/src/pydash.egg-info/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)    16254 2023-07-06 13:57:26.000000 pydash-7.0.5/src/pydash.egg-info/SOURCES.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-07-06 13:57:24.000000 pydash-7.0.5/src/pydash.egg-info/dependency_links.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)      289 2023-07-06 13:57:24.000000 pydash-7.0.5/src/pydash.egg-info/requires.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-07-06 13:57:24.000000 pydash-7.0.5/src/pydash.egg-info/top_level.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.5/tasks.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.257845 pydash-7.0.5/tests/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.5/tests/__init__.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.209558 pydash-7.0.5/tests/build/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.258019 pydash-7.0.5/tests/build/testresults/
+-rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.5/tests/build/testresults/junit.xml
+-rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.5/tests/conftest.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.5/tests/helpers.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.260157 pydash-7.0.5/tests/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.5/tests/pytest_mypy_testing/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    17085 2023-07-06 13:41:49.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.5/tests/test_annotations.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.5/tests/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.5/tests/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.5/tests/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.5/tests/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.5/tests/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.5/tests/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.5/tests/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.5/tests/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.5/tests/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.5/tox.ini
```

### Comparing `pydash-7.0.4/AUTHORS.rst` & `pydash-7.0.5/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/CHANGELOG.rst` & `pydash-7.0.5/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.5 (2023-07-06)
+-------------------
+
+- Fix typing for ``find_index`` and ``find_last_index`` by allowing ``predicate`` argument to be callback shorthand values.
+
+
 v7.0.4 (2023-06-02)
 -------------------
 
 - Exclude incompatible ``typing-extensions`` version ``4.6.0`` from install requirements. Incompatibility was fixed in ``4.6.1``.
 
 
 v7.0.3 (2023-05-04)
```

### Comparing `pydash-7.0.4/CONTRIBUTING.rst` & `pydash-7.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/LICENSE.rst` & `pydash-7.0.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/PKG-INFO` & `pydash-7.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 7.0.4
+Version: 7.0.5
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,14 +61,20 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.5 (2023-07-06)
+-------------------
+
+- Fix typing for ``find_index`` and ``find_last_index`` by allowing ``predicate`` argument to be callback shorthand values.
+
+
 v7.0.4 (2023-06-02)
 -------------------
 
 - Exclude incompatible ``typing-extensions`` version ``4.6.0`` from install requirements. Incompatibility was fixed in ``4.6.1``.
 
 
 v7.0.3 (2023-05-04)
```

### Comparing `pydash-7.0.4/README.rst` & `pydash-7.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/docs/Makefile` & `pydash-7.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/docs/api.rst` & `pydash-7.0.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/docs/callbacks.rst` & `pydash-7.0.5/docs/callbacks.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/docs/chaining.rst` & `pydash-7.0.5/docs/chaining.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/docs/conf.py` & `pydash-7.0.5/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,39 +93,26 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-# on_rtd is whether we are on readthedocs.org, this line of code grabbed from
-# docs.readthedocs.org.
-on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
-
-if on_rtd:
-    html_theme = 'default'
-else:
-    import sphinx_rtd_theme
-
-    html_theme = 'sphinx_rtd_theme'
-    html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
-
-    def setup(app):
-        app.add_css_file('theme_override.css')
+html_theme = 'furo'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 #html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+#html_static_path = ['_static']
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # The default sidebars (for documents that don't match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
 # default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
```

### Comparing `pydash-7.0.4/docs/deeppath.rst` & `pydash-7.0.5/docs/deeppath.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/docs/differences.rst` & `pydash-7.0.5/docs/differences.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/docs/index.rst` & `pydash-7.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/docs/quickstart.rst` & `pydash-7.0.5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/docs/templating.rst` & `pydash-7.0.5/docs/templating.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/docs/upgrading.rst` & `pydash-7.0.5/docs/upgrading.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/pylintrc` & `pydash-7.0.5/pylintrc`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/setup.cfg` & `pydash-7.0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -42,24 +42,24 @@
 	build
 	coverage
 	docformatter
 	flake8
 	flake8-black
 	flake8-bugbear
 	flake8-isort
+	furo
 	importlib_metadata<5; python_version=="3.7"
 	invoke
 	isort
 	mypy
 	pylint
 	pytest
 	pytest-mypy-testing
 	pytest-cov
 	Sphinx
-	sphinx-rtd-theme
 	tox
 	twine
 	wheel
 	sphinx-autodoc-typehints
 
 [bdist_wheel]
 python_tag = py3
```

### Comparing `pydash-7.0.4/src/pydash/__init__.py` & `pydash-7.0.5/src/pydash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python port of Lo-Dash."""
 
-__version__ = "7.0.4"
+__version__ = "7.0.5"
 
 from .arrays import (
     chunk,
     compact,
     concat,
     difference,
     difference_by,
```

### Comparing `pydash-7.0.4/src/pydash/arrays.py` & `pydash-7.0.5/src/pydash/arrays.py`

 * *Files 0% similar despite different names*

```diff
@@ -555,14 +555,19 @@
 
 @t.overload
 def find_index(array: t.Iterable[T], predicate: t.Callable[[T], t.Any]) -> int:
     ...
 
 
 @t.overload
+def find_index(array: t.Iterable[t.Any], predicate: IterateeObjT) -> int:
+    ...
+
+
+@t.overload
 def find_index(array: t.Iterable[t.Any], predicate: None = None) -> int:
     ...
 
 
 def find_index(array, predicate=None):
     """
     This method is similar to :func:`pydash.collections.find`, except that it returns the index of
@@ -600,14 +605,19 @@
 
 @t.overload
 def find_last_index(array: t.Iterable[T], predicate: t.Callable[[T], t.Any]) -> int:
     ...
 
 
 @t.overload
+def find_last_index(array: t.Iterable[t.Any], predicate: IterateeObjT) -> int:
+    ...
+
+
+@t.overload
 def find_last_index(array: t.Iterable[t.Any], predicate: None = None) -> int:
     ...
 
 
 def find_last_index(array, predicate=None):
     """
     This method is similar to :func:`find_index`, except that it iterates over elements from right
```

### Comparing `pydash-7.0.4/src/pydash/chaining/all_funcs.py` & `pydash-7.0.5/src/pydash/chaining/all_funcs.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash/chaining/all_funcs.pyi` & `pydash-7.0.5/src/pydash/chaining/all_funcs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -149,14 +149,16 @@
         self: "Chain[t.Iterable[T]]", predicate: t.Callable[[T, int], t.Any]
     ) -> "Chain[int]": ...
     @t.overload
     def find_index(
         self: "Chain[t.Iterable[T]]", predicate: t.Callable[[T], t.Any]
     ) -> "Chain[int]": ...
     @t.overload
+    def find_index(self: "Chain[t.Iterable[t.Any]]", predicate: IterateeObjT) -> "Chain[int]": ...
+    @t.overload
     def find_index(self: "Chain[t.Iterable[t.Any]]", predicate: None = None) -> "Chain[int]": ...
     def find_index(self, predicate=None):
         return self._wrap(pyd.find_index)(predicate)
     @t.overload
     def find_last_index(
         self: "Chain[t.Iterable[T]]", predicate: t.Callable[[T, int, t.List[T]], t.Any]
     ) -> "Chain[int]": ...
@@ -166,14 +168,18 @@
     ) -> "Chain[int]": ...
     @t.overload
     def find_last_index(
         self: "Chain[t.Iterable[T]]", predicate: t.Callable[[T], t.Any]
     ) -> "Chain[int]": ...
     @t.overload
     def find_last_index(
+        self: "Chain[t.Iterable[t.Any]]", predicate: IterateeObjT
+    ) -> "Chain[int]": ...
+    @t.overload
+    def find_last_index(
         self: "Chain[t.Iterable[t.Any]]", predicate: None = None
     ) -> "Chain[int]": ...
     def find_last_index(self, predicate=None):
         return self._wrap(pyd.find_last_index)(predicate)
     @t.overload
     def flatten(self: "Chain[t.Iterable[t.Iterable[T]]]") -> "Chain[t.List[T]]": ...
     @t.overload
```

### Comparing `pydash-7.0.4/src/pydash/chaining/chaining.py` & `pydash-7.0.5/src/pydash/chaining/chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash/collections.py` & `pydash-7.0.5/src/pydash/collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash/functions.py` & `pydash-7.0.5/src/pydash/functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash/helpers.py` & `pydash-7.0.5/src/pydash/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash/numerical.py` & `pydash-7.0.5/src/pydash/numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash/objects.py` & `pydash-7.0.5/src/pydash/objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash/predicates.py` & `pydash-7.0.5/src/pydash/predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash/strings.py` & `pydash-7.0.5/src/pydash/strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash/types.py` & `pydash-7.0.5/src/pydash/types.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash/utilities.py` & `pydash-7.0.5/src/pydash/utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/src/pydash.egg-info/PKG-INFO` & `pydash-7.0.5/src/pydash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 7.0.4
+Version: 7.0.5
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,14 +61,20 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.5 (2023-07-06)
+-------------------
+
+- Fix typing for ``find_index`` and ``find_last_index`` by allowing ``predicate`` argument to be callback shorthand values.
+
+
 v7.0.4 (2023-06-02)
 -------------------
 
 - Exclude incompatible ``typing-extensions`` version ``4.6.0`` from install requirements. Incompatibility was fixed in ``4.6.1``.
 
 
 v7.0.3 (2023-05-04)
```

### Comparing `pydash-7.0.4/src/pydash.egg-info/SOURCES.txt` & `pydash-7.0.5/src/pydash.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -275,16 +275,14 @@
 docs/installation.rst
 docs/kudos.rst
 docs/license.rst
 docs/quickstart.rst
 docs/templating.rst
 docs/upgrading.rst
 docs/versioning.rst
-docs/_static/.gitignore
-docs/_static/theme_override.css
 docs/_templates/.gitignore
 src/pydash/__init__.py
 src/pydash/arrays.py
 src/pydash/collections.py
 src/pydash/exceptions.py
 src/pydash/functions.py
 src/pydash/helpers.py
```

### Comparing `pydash-7.0.4/tasks.py` & `pydash-7.0.5/tasks.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/build/testresults/junit.xml` & `pydash-7.0.5/tests/build/testresults/junit.xml`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/helpers.py` & `pydash-7.0.5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/pytest_mypy_testing/test_arrays.py` & `pydash-7.0.5/tests/pytest_mypy_testing/test_arrays.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,20 +77,22 @@
     reveal_type(_.fill([1, 2, 3, 4, 5], 0, 0, 100))  # R: builtins.list[builtins.int]
 
 
 @pytest.mark.mypy_testing
 def test_mypy_find_index() -> None:
     reveal_type(_.find_index([1, 2, 3, 4], lambda x: x >= 3))  # R: builtins.int
     reveal_type(_.find_index([1, 2, 3, 4], lambda x: x > 4))  # R: builtins.int
+    reveal_type(_.find_index([{"a": 0, "b": 3}, {"a": "1", "c": 5}], {"a": 0}))  # R: builtins.int
 
 
 @pytest.mark.mypy_testing
 def test_mypy_find_last_index() -> None:
     reveal_type(_.find_last_index([1, 2, 3, 4], lambda x: x >= 3))  # R: builtins.int
     reveal_type(_.find_last_index([1, 2, 3, 4], lambda x: x > 4))  # R: builtins.int
+    reveal_type(_.find_last_index([{"a": 0, "b": 3}, {"a": "1", "c": 5}], {"a": 0}))  # R: builtins.int
 
 
 @pytest.mark.mypy_testing
 def test_mypy_flatten() -> None:
     my_list: t.List[t.List[t.Union[int, t.List[int]]]] = [[1], [2, [3]], [[4]]]
     reveal_type(_.flatten(my_list))  # R: builtins.list[Union[builtins.int, builtins.list[builtins.int]]]
```

### Comparing `pydash-7.0.4/tests/pytest_mypy_testing/test_chaining.py` & `pydash-7.0.5/tests/pytest_mypy_testing/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/pytest_mypy_testing/test_collections.py` & `pydash-7.0.5/tests/pytest_mypy_testing/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/pytest_mypy_testing/test_functions.py` & `pydash-7.0.5/tests/pytest_mypy_testing/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/pytest_mypy_testing/test_numerical.py` & `pydash-7.0.5/tests/pytest_mypy_testing/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/pytest_mypy_testing/test_objects.py` & `pydash-7.0.5/tests/pytest_mypy_testing/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/pytest_mypy_testing/test_predicates.py` & `pydash-7.0.5/tests/pytest_mypy_testing/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/pytest_mypy_testing/test_strings.py` & `pydash-7.0.5/tests/pytest_mypy_testing/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/pytest_mypy_testing/test_utilities.py` & `pydash-7.0.5/tests/pytest_mypy_testing/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/test_arrays.py` & `pydash-7.0.5/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/test_chaining.py` & `pydash-7.0.5/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/test_collections.py` & `pydash-7.0.5/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/test_functions.py` & `pydash-7.0.5/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/test_numerical.py` & `pydash-7.0.5/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/test_objects.py` & `pydash-7.0.5/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/test_predicates.py` & `pydash-7.0.5/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/test_strings.py` & `pydash-7.0.5/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.4/tests/test_utilities.py` & `pydash-7.0.5/tests/test_utilities.py`

 * *Files identical despite different names*

