# Comparing `tmp/cmomy-0.5.0.tar.gz` & `tmp/cmomy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmomy-0.5.0.tar", last modified: Wed Jun 14 12:51:38 2023, max compression
+gzip compressed data, was "cmomy-0.6.0.tar", last modified: Thu Jul  6 18:53:23 2023, max compression
```

## Comparing `cmomy-0.5.0.tar` & `cmomy-0.6.0.tar`

### file list

```diff
@@ -1,139 +1,146 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.872837 cmomy-0.5.0/
--rw-r--r--   0 wpk      (42033)    36681     1484 2023-06-14 12:50:26.000000 cmomy-0.5.0/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 04:51:37.000000 cmomy-0.5.0/.editorconfig
--rw-r--r--   0 wpk      (42033)    36681       31 2023-01-25 16:37:02.000000 cmomy-0.5.0/.gitattributes
--rw-r--r--   0 wpk      (42033)    36681     1360 2023-06-14 12:50:26.000000 cmomy-0.5.0/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-04-24 20:47:28.000000 cmomy-0.5.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3572 2023-06-14 12:50:26.000000 cmomy-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-04-24 20:47:28.000000 cmomy-0.5.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      339 2023-06-14 12:50:26.000000 cmomy-0.5.0/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-04-24 20:47:28.000000 cmomy-0.5.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681     2949 2023-06-14 12:50:26.000000 cmomy-0.5.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9775 2023-06-14 12:50:26.000000 cmomy-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-03-15 19:07:26.000000 cmomy-0.5.0/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      258 2023-04-24 20:47:28.000000 cmomy-0.5.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681     9368 2023-06-14 12:50:26.000000 cmomy-0.5.0/Makefile
--rw-r--r--   0 wpk      (42033)    36681    10494 2023-06-14 12:51:38.872347 cmomy-0.5.0/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     4723 2023-06-14 12:50:26.000000 cmomy-0.5.0/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.821306 cmomy-0.5.0/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-04-24 20:47:28.000000 cmomy-0.5.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.822016 cmomy-0.5.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.823234 cmomy-0.5.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-04-24 20:47:28.000000 cmomy-0.5.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-04-24 20:47:28.000000 cmomy-0.5.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-04-24 20:47:28.000000 cmomy-0.5.0/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0 wpk      (42033)    36681      404 2023-06-14 12:50:26.000000 cmomy-0.5.0/conftest.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.828431 cmomy-0.5.0/docs/
--rw-r--r--   0 wpk      (42033)    36681     1401 2023-05-02 13:41:37.000000 cmomy-0.5.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.801041 cmomy-0.5.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.829090 cmomy-0.5.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.829990 cmomy-0.5.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      767 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      706 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.832448 cmomy-0.5.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.835275 cmomy-0.5.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.836723 cmomy-0.5.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-03-22 20:26:04.000000 cmomy-0.5.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033)    36681       69 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033)    36681    14595 2023-06-14 01:24:25.000000 cmomy-0.5.0/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       74 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/contributing.md
--rw-r--r--   0 wpk      (42033)    36681      891 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/example_for_readme.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.837242 cmomy-0.5.0/docs/examples/
--rw-r--r--   0 wpk      (42033)    36681       84 2023-06-14 01:24:29.000000 cmomy-0.5.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.838355 cmomy-0.5.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681   156774 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/examples/usage/motivation.ipynb
--rw-r--r--   0 wpk      (42033)    36681   295212 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/examples/usage/usage_notebook.ipynb
--rw-r--r--   0 wpk      (42033)    36681      224 2023-06-14 01:24:29.000000 cmomy-0.5.0/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681     1030 2023-06-14 12:50:26.000000 cmomy-0.5.0/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       40 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-03-15 18:41:43.000000 cmomy-0.5.0/docs/make.bat
--rw-r--r--   0 wpk      (42033)    36681      169 2023-04-24 20:47:28.000000 cmomy-0.5.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.840352 cmomy-0.5.0/docs/reference/
--rw-r--r--   0 wpk      (42033)    36681      158 2023-04-06 00:58:31.000000 cmomy-0.5.0/docs/reference/api-baseclasses.rst
--rw-r--r--   0 wpk      (42033)    36681      122 2023-04-06 00:58:31.000000 cmomy-0.5.0/docs/reference/api-modules.rst
--rw-r--r--   0 wpk      (42033)    36681      398 2023-04-06 00:58:31.000000 cmomy-0.5.0/docs/reference/api-public.rst
--rw-r--r--   0 wpk      (42033)    36681      194 2023-06-14 02:39:04.000000 cmomy-0.5.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033)    36681      491 2023-06-14 02:39:06.000000 cmomy-0.5.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.844387 cmomy-0.5.0/environment/
--rw-r--r--   0 wpk      (42033)    36681      329 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/base.yaml
--rw-r--r--   0 wpk      (42033)    36681      521 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681      225 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      640 2023-04-24 20:47:28.000000 cmomy-0.5.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      520 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681      203 2023-05-02 04:51:37.000000 cmomy-0.5.0/environment/lint.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.846018 cmomy-0.5.0/environment/lock/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/lock/py310.yaml
--rw-r--r--   0 wpk      (42033)    36681       64 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/lock/py311.yaml
--rw-r--r--   0 wpk      (42033)    36681       63 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/lock/py38.yaml
--rw-r--r--   0 wpk      (42033)    36681       63 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/lock/py39.yaml
--rw-r--r--   0 wpk      (42033)    36681      389 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      398 2023-06-14 12:50:26.000000 cmomy-0.5.0/environment/typing.yaml
--rw-r--r--   0 wpk      (42033)    36681      187 2023-05-02 04:51:37.000000 cmomy-0.5.0/environment.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.846415 cmomy-0.5.0/examples/
--rw-r--r--   0 wpk      (42033)    36681      222 2023-04-24 20:47:28.000000 cmomy-0.5.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.850665 cmomy-0.5.0/examples/archived/
--rw-r--r--   0 wpk      (42033)    36681    70967 2023-04-24 20:47:28.000000 cmomy-0.5.0/examples/archived/bootstrap.ipynb
--rw-r--r--   0 wpk      (42033)    36681   136974 2023-04-24 20:47:28.000000 cmomy-0.5.0/examples/archived/central_moments.ipynb
--rw-r--r--   0 wpk      (42033)    36681    44856 2023-04-24 20:47:28.000000 cmomy-0.5.0/examples/archived/example_usage.ipynb
--rw-r--r--   0 wpk      (42033)    36681    12217 2023-04-24 20:47:28.000000 cmomy-0.5.0/examples/archived/parallel_test.ipynb
--rw-r--r--   0 wpk      (42033)    36681    58117 2023-04-24 20:47:28.000000 cmomy-0.5.0/examples/archived/test_accumulator.ipynb
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.853039 cmomy-0.5.0/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681   156774 2023-04-24 20:47:28.000000 cmomy-0.5.0/examples/usage/motivation.ipynb
--rw-r--r--   0 wpk      (42033)    36681   295212 2023-04-24 20:47:28.000000 cmomy-0.5.0/examples/usage/usage_notebook.ipynb
--rw-r--r--   0 wpk      (42033)    36681    27077 2023-06-14 12:50:26.000000 cmomy-0.5.0/noxfile.py
--rw-r--r--   0 wpk      (42033)    36681     7165 2023-06-14 12:50:26.000000 cmomy-0.5.0/pyproject.toml
--rw-r--r--   0 wpk      (42033)    36681       38 2023-06-14 12:51:38.872953 cmomy-0.5.0/setup.cfg
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.807222 cmomy-0.5.0/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.864815 cmomy-0.5.0/src/cmomy/
--rw-r--r--   0 wpk      (42033)    36681     1045 2023-03-29 00:12:57.000000 cmomy-0.5.0/src/cmomy/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     2736 2023-04-24 20:47:28.000000 cmomy-0.5.0/src/cmomy/_formatting.py
--rw-r--r--   0 wpk      (42033)    36681     6463 2023-03-22 20:26:04.000000 cmomy-0.5.0/src/cmomy/_resample.py
--rw-r--r--   0 wpk      (42033)    36681     2311 2023-01-25 16:37:02.000000 cmomy-0.5.0/src/cmomy/_testing.py
--rw-r--r--   0 wpk      (42033)    36681      658 2023-03-22 20:26:04.000000 cmomy-0.5.0/src/cmomy/_typing.py
--rw-r--r--   0 wpk      (42033)    36681    39729 2023-05-02 04:51:37.000000 cmomy-0.5.0/src/cmomy/abstract_central.py
--rw-r--r--   0 wpk      (42033)    36681    50419 2023-06-14 12:50:26.000000 cmomy-0.5.0/src/cmomy/central.py
--rw-r--r--   0 wpk      (42033)    36681      967 2023-01-25 16:37:02.000000 cmomy-0.5.0/src/cmomy/compile.py
--rw-r--r--   0 wpk      (42033)    36681    10920 2023-05-02 04:51:37.000000 cmomy-0.5.0/src/cmomy/convert.py
--rw-r--r--   0 wpk      (42033)    36681     3338 2023-05-02 04:51:37.000000 cmomy-0.5.0/src/cmomy/docstrings.py
--rw-r--r--   0 wpk      (42033)    36681     1834 2023-06-14 12:50:26.000000 cmomy-0.5.0/src/cmomy/options.py
--rw-r--r--   0 wpk      (42033)    36681     3122 2023-04-06 00:58:31.000000 cmomy-0.5.0/src/cmomy/pusher_interface.py
--rw-r--r--   0 wpk      (42033)    36681    14250 2023-01-25 16:37:02.000000 cmomy-0.5.0/src/cmomy/pushers.py
--rw-r--r--   0 wpk      (42033)    36681        0 2023-03-22 20:26:04.000000 cmomy-0.5.0/src/cmomy/py.typed
--rw-r--r--   0 wpk      (42033)    36681    13795 2023-04-24 20:47:28.000000 cmomy-0.5.0/src/cmomy/resample.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.871278 cmomy-0.5.0/src/cmomy/tests/
--rw-r--r--   0 wpk      (42033)    36681        0 2023-01-25 16:37:02.000000 cmomy-0.5.0/src/cmomy/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    11913 2023-05-02 04:51:37.000000 cmomy-0.5.0/src/cmomy/tests/conftest.py
--rw-r--r--   0 wpk      (42033)    36681     5427 2023-03-22 20:26:04.000000 cmomy-0.5.0/src/cmomy/tests/test_central.py
--rw-r--r--   0 wpk      (42033)    36681     9455 2023-05-02 04:51:37.000000 cmomy-0.5.0/src/cmomy/tests/test_central_2.py
--rw-r--r--   0 wpk      (42033)    36681     1085 2023-01-25 16:37:02.000000 cmomy-0.5.0/src/cmomy/tests/test_convert.py
--rw-r--r--   0 wpk      (42033)    36681     4085 2023-03-22 20:26:04.000000 cmomy-0.5.0/src/cmomy/tests/test_resample.py
--rw-r--r--   0 wpk      (42033)    36681     2354 2023-03-22 20:26:04.000000 cmomy-0.5.0/src/cmomy/tests/test_stability.py
--rw-r--r--   0 wpk      (42033)    36681     2682 2023-03-22 20:26:04.000000 cmomy-0.5.0/src/cmomy/tests/test_verify.py
--rw-r--r--   0 wpk      (42033)    36681     6183 2023-03-22 20:26:04.000000 cmomy-0.5.0/src/cmomy/tests/test_xcentral.py
--rw-r--r--   0 wpk      (42033)    36681     4879 2023-03-22 20:26:04.000000 cmomy-0.5.0/src/cmomy/tests/test_xcentral_constructors.py
--rw-r--r--   0 wpk      (42033)    36681     3190 2023-05-02 04:51:37.000000 cmomy-0.5.0/src/cmomy/utils.py
--rw-r--r--   0 wpk      (42033)    36681    61350 2023-06-14 12:50:26.000000 cmomy-0.5.0/src/cmomy/xcentral.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.867321 cmomy-0.5.0/src/cmomy.egg-info/
--rw-r--r--   0 wpk      (42033)    36681    10494 2023-06-14 12:51:38.000000 cmomy-0.5.0/src/cmomy.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2995 2023-06-14 12:51:38.000000 cmomy-0.5.0/src/cmomy.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-06-14 12:51:38.000000 cmomy-0.5.0/src/cmomy.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681      705 2023-06-14 12:51:38.000000 cmomy-0.5.0/src/cmomy.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681        6 2023-06-14 12:51:38.000000 cmomy-0.5.0/src/cmomy.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-05-04 19:42:47.000000 cmomy-0.5.0/src/cmomy.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-14 12:51:38.871687 cmomy-0.5.0/tools/
--rw-r--r--   0 wpk      (42033)    36681    20738 2023-06-14 12:50:26.000000 cmomy-0.5.0/tools/noxtools.py
--rw-r--r--   0 wpk      (42033)    36681     4081 2023-06-14 12:50:26.000000 cmomy-0.5.0/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.942524 cmomy-0.6.0/
+-rw-r--r--   0 wpk      (42033)    36681     1484 2023-07-06 18:49:10.000000 cmomy-0.6.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 04:51:37.000000 cmomy-0.6.0/.editorconfig
+-rw-r--r--   0 wpk      (42033)    36681       31 2023-01-25 16:37:02.000000 cmomy-0.6.0/.gitattributes
+-rw-r--r--   0 wpk      (42033)    36681     1398 2023-07-06 18:49:10.000000 cmomy-0.6.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-04-24 20:47:28.000000 cmomy-0.6.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3572 2023-06-14 12:50:26.000000 cmomy-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-04-24 20:47:28.000000 cmomy-0.6.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      339 2023-06-14 12:50:26.000000 cmomy-0.6.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-04-24 20:47:28.000000 cmomy-0.6.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681     2949 2023-06-14 20:21:01.000000 cmomy-0.6.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681    11044 2023-07-06 18:49:10.000000 cmomy-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-03-15 19:07:26.000000 cmomy-0.6.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      258 2023-04-24 20:47:28.000000 cmomy-0.6.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681     9597 2023-07-06 18:49:10.000000 cmomy-0.6.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681    10494 2023-07-06 18:53:23.941644 cmomy-0.6.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     4723 2023-06-14 20:22:16.000000 cmomy-0.6.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.886749 cmomy-0.6.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681      599 2023-07-06 18:49:10.000000 cmomy-0.6.0/changelog.d/20230706_144442_william.krekelberg.md
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-04-24 20:47:28.000000 cmomy-0.6.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.887123 cmomy-0.6.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.887845 cmomy-0.6.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-04-24 20:47:28.000000 cmomy-0.6.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-04-24 20:47:28.000000 cmomy-0.6.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-04-24 20:47:28.000000 cmomy-0.6.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033)    36681      404 2023-06-14 12:50:26.000000 cmomy-0.6.0/conftest.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.892906 cmomy-0.6.0/docs/
+-rw-r--r--   0 wpk      (42033)    36681     1401 2023-05-02 13:41:37.000000 cmomy-0.6.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.872937 cmomy-0.6.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.893519 cmomy-0.6.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-24 20:47:28.000000 cmomy-0.6.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.894521 cmomy-0.6.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-04-24 20:47:28.000000 cmomy-0.6.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033)    36681      706 2023-04-24 20:47:28.000000 cmomy-0.6.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.897066 cmomy-0.6.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.901160 cmomy-0.6.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033)    36681      289 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      249 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033)    36681      405 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      374 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.903425 cmomy-0.6.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033)    36681      106 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033)    36681     1119 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033)    36681     1418 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033)    36681     1177 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033)    36681     1071 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033)    36681     1179 2023-03-22 20:26:04.000000 cmomy-0.6.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681       69 2023-04-24 20:47:28.000000 cmomy-0.6.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-04-24 20:47:28.000000 cmomy-0.6.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033)    36681    14834 2023-07-06 18:49:10.000000 cmomy-0.6.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033)    36681       74 2023-04-24 20:47:28.000000 cmomy-0.6.0/docs/contributing.md
+-rw-r--r--   0 wpk      (42033)    36681      891 2023-04-24 20:47:28.000000 cmomy-0.6.0/docs/example_for_readme.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.904179 cmomy-0.6.0/docs/examples/
+-rw-r--r--   0 wpk      (42033)    36681       84 2023-06-14 20:22:29.000000 cmomy-0.6.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.905969 cmomy-0.6.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681   156783 2023-07-06 18:49:10.000000 cmomy-0.6.0/docs/examples/usage/motivation.ipynb
+-rw-r--r--   0 wpk      (42033)    36681   295212 2023-04-24 20:47:28.000000 cmomy-0.6.0/docs/examples/usage/usage_notebook.ipynb
+-rw-r--r--   0 wpk      (42033)    36681      224 2023-06-14 20:22:29.000000 cmomy-0.6.0/docs/index.md
+-rw-r--r--   0 wpk      (42033)    36681     1030 2023-06-14 20:22:29.000000 cmomy-0.6.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033)    36681       40 2023-04-24 20:47:28.000000 cmomy-0.6.0/docs/license.md
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-03-15 18:41:43.000000 cmomy-0.6.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033)    36681      169 2023-04-24 20:47:28.000000 cmomy-0.6.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.909458 cmomy-0.6.0/docs/reference/
+-rw-r--r--   0 wpk      (42033)    36681      158 2023-04-06 00:58:31.000000 cmomy-0.6.0/docs/reference/api-baseclasses.rst
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-04-06 00:58:31.000000 cmomy-0.6.0/docs/reference/api-modules.rst
+-rw-r--r--   0 wpk      (42033)    36681      398 2023-04-06 00:58:31.000000 cmomy-0.6.0/docs/reference/api-public.rst
+-rw-r--r--   0 wpk      (42033)    36681      194 2023-06-14 20:22:29.000000 cmomy-0.6.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033)    36681      491 2023-06-14 20:22:29.000000 cmomy-0.6.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.915660 cmomy-0.6.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      345 2023-07-06 18:53:13.000000 cmomy-0.6.0/environment/base.yaml
+-rw-r--r--   0 wpk      (42033)    36681      537 2023-07-06 18:53:14.000000 cmomy-0.6.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      280 2023-07-06 18:53:15.000000 cmomy-0.6.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-07-06 18:53:15.000000 cmomy-0.6.0/environment/dist-pypi.txt
+-rw-r--r--   0 wpk      (42033)    36681      225 2023-07-06 18:53:15.000000 cmomy-0.6.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      640 2023-04-24 20:47:28.000000 cmomy-0.6.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      517 2023-07-06 18:53:14.000000 cmomy-0.6.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681      203 2023-05-02 04:51:37.000000 cmomy-0.6.0/environment/lint.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.917334 cmomy-0.6.0/environment/lock/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-06-14 12:50:26.000000 cmomy-0.6.0/environment/lock/py310.yaml
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-06-14 12:50:26.000000 cmomy-0.6.0/environment/lock/py311.yaml
+-rw-r--r--   0 wpk      (42033)    36681       63 2023-06-14 12:50:26.000000 cmomy-0.6.0/environment/lock/py38.yaml
+-rw-r--r--   0 wpk      (42033)    36681       63 2023-06-14 12:50:26.000000 cmomy-0.6.0/environment/lock/py39.yaml
+-rw-r--r--   0 wpk      (42033)    36681      193 2023-07-06 18:53:16.000000 cmomy-0.6.0/environment/test-extras.txt
+-rw-r--r--   0 wpk      (42033)    36681      265 2023-07-06 18:53:16.000000 cmomy-0.6.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      405 2023-07-06 18:53:13.000000 cmomy-0.6.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      414 2023-07-06 18:53:14.000000 cmomy-0.6.0/environment/typing.yaml
+-rw-r--r--   0 wpk      (42033)    36681      187 2023-05-02 04:51:37.000000 cmomy-0.6.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.917796 cmomy-0.6.0/examples/
+-rw-r--r--   0 wpk      (42033)    36681      222 2023-04-24 20:47:28.000000 cmomy-0.6.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.921805 cmomy-0.6.0/examples/archived/
+-rw-r--r--   0 wpk      (42033)    36681    70967 2023-04-24 20:47:28.000000 cmomy-0.6.0/examples/archived/bootstrap.ipynb
+-rw-r--r--   0 wpk      (42033)    36681   136974 2023-04-24 20:47:28.000000 cmomy-0.6.0/examples/archived/central_moments.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    44856 2023-04-24 20:47:28.000000 cmomy-0.6.0/examples/archived/example_usage.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    12217 2023-04-24 20:47:28.000000 cmomy-0.6.0/examples/archived/parallel_test.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    58117 2023-04-24 20:47:28.000000 cmomy-0.6.0/examples/archived/test_accumulator.ipynb
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.922878 cmomy-0.6.0/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681   156783 2023-07-06 18:49:10.000000 cmomy-0.6.0/examples/usage/motivation.ipynb
+-rw-r--r--   0 wpk      (42033)    36681   295212 2023-04-24 20:47:28.000000 cmomy-0.6.0/examples/usage/usage_notebook.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    32065 2023-07-06 18:49:10.000000 cmomy-0.6.0/noxfile.py
+-rw-r--r--   0 wpk      (42033)    36681     7196 2023-07-06 18:49:10.000000 cmomy-0.6.0/pyproject.toml
+-rw-r--r--   0 wpk      (42033)    36681       38 2023-07-06 18:53:23.942741 cmomy-0.6.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.876411 cmomy-0.6.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.931104 cmomy-0.6.0/src/cmomy/
+-rw-r--r--   0 wpk      (42033)    36681      862 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     4206 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/_convert.py
+-rw-r--r--   0 wpk      (42033)    36681     2977 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/_formatting.py
+-rw-r--r--   0 wpk      (42033)    36681      219 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/_lazy_imports.py
+-rw-r--r--   0 wpk      (42033)    36681     7169 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/_resample.py
+-rw-r--r--   0 wpk      (42033)    36681     2322 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/_testing.py
+-rw-r--r--   0 wpk      (42033)    36681      653 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/_typing.py
+-rw-r--r--   0 wpk      (42033)    36681      160 2023-07-06 18:53:23.000000 cmomy-0.6.0/src/cmomy/_version.py
+-rw-r--r--   0 wpk      (42033)    36681    39835 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/abstract_central.py
+-rw-r--r--   0 wpk      (42033)    36681    50421 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/central.py
+-rw-r--r--   0 wpk      (42033)    36681      977 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/compile.py
+-rw-r--r--   0 wpk      (42033)    36681     6997 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/convert.py
+-rw-r--r--   0 wpk      (42033)    36681     3338 2023-05-02 04:51:37.000000 cmomy-0.6.0/src/cmomy/docstrings.py
+-rw-r--r--   0 wpk      (42033)    36681     1834 2023-06-14 12:50:26.000000 cmomy-0.6.0/src/cmomy/options.py
+-rw-r--r--   0 wpk      (42033)    36681     3133 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/pusher_interface.py
+-rw-r--r--   0 wpk      (42033)    36681    14250 2023-01-25 16:37:02.000000 cmomy-0.6.0/src/cmomy/pushers.py
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-03-22 20:26:04.000000 cmomy-0.6.0/src/cmomy/py.typed
+-rw-r--r--   0 wpk      (42033)    36681    13240 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/resample.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.939559 cmomy-0.6.0/src/cmomy/tests/
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-01-25 16:37:02.000000 cmomy-0.6.0/src/cmomy/tests/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681    11913 2023-05-02 04:51:37.000000 cmomy-0.6.0/src/cmomy/tests/conftest.py
+-rw-r--r--   0 wpk      (42033)    36681     5427 2023-07-06 18:35:59.000000 cmomy-0.6.0/src/cmomy/tests/test_central.py
+-rw-r--r--   0 wpk      (42033)    36681     9455 2023-05-02 04:51:37.000000 cmomy-0.6.0/src/cmomy/tests/test_central_2.py
+-rw-r--r--   0 wpk      (42033)    36681     1085 2023-01-25 16:37:02.000000 cmomy-0.6.0/src/cmomy/tests/test_convert.py
+-rw-r--r--   0 wpk      (42033)    36681     4085 2023-03-22 20:26:04.000000 cmomy-0.6.0/src/cmomy/tests/test_resample.py
+-rw-r--r--   0 wpk      (42033)    36681     2354 2023-03-22 20:26:04.000000 cmomy-0.6.0/src/cmomy/tests/test_stability.py
+-rw-r--r--   0 wpk      (42033)    36681     2682 2023-03-22 20:26:04.000000 cmomy-0.6.0/src/cmomy/tests/test_verify.py
+-rw-r--r--   0 wpk      (42033)    36681     6183 2023-03-22 20:26:04.000000 cmomy-0.6.0/src/cmomy/tests/test_xcentral.py
+-rw-r--r--   0 wpk      (42033)    36681     4879 2023-03-22 20:26:04.000000 cmomy-0.6.0/src/cmomy/tests/test_xcentral_constructors.py
+-rw-r--r--   0 wpk      (42033)    36681     3213 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/utils.py
+-rw-r--r--   0 wpk      (42033)    36681    61345 2023-07-06 18:49:10.000000 cmomy-0.6.0/src/cmomy/xcentral.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.934356 cmomy-0.6.0/src/cmomy.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681    10494 2023-07-06 18:53:23.000000 cmomy-0.6.0/src/cmomy.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     3199 2023-07-06 18:53:23.000000 cmomy-0.6.0/src/cmomy.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-07-06 18:53:23.000000 cmomy-0.6.0/src/cmomy.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681      687 2023-07-06 18:53:23.000000 cmomy-0.6.0/src/cmomy.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681        6 2023-07-06 18:53:23.000000 cmomy-0.6.0/src/cmomy.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-05-04 19:42:47.000000 cmomy-0.6.0/src/cmomy.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-07-06 18:53:23.940465 cmomy-0.6.0/tools/
+-rw-r--r--   0 wpk      (42033)    36681    24175 2023-07-06 18:49:10.000000 cmomy-0.6.0/tools/noxtools.py
+-rw-r--r--   0 wpk      (42033)    36681     4081 2023-06-14 12:50:26.000000 cmomy-0.6.0/tox.ini
```

### Comparing `cmomy-0.5.0/.cruft.json` & `cmomy-0.6.0/.cruft.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'commit'": "'9f90292d37d2ce2ad704f6e298125f29830b5480'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": "feature/nox",
-    "commit": "95a4ddeb3c55c50d43b4e9dd18c7137b1dfdf4f2",
+    "commit": "9f90292d37d2ce2ad704f6e298125f29830b5480",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
```

### Comparing `cmomy-0.5.0/.editorconfig` & `cmomy-0.6.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/.gitignore` & `cmomy-0.6.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -110,7 +110,9 @@
 .noxconfig.toml
 cruft.patch
 /docs/**/generated/
 /monkeytype.sqlite3
 /dist-conda/
 /tmp/
 /cmomy-feedstock*/
+/src/**/_version.py
+tuna-loadtime.log
```

### Comparing `cmomy-0.5.0/.pre-commit-config.yaml` & `cmomy-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/CHANGELOG.md` & `cmomy-0.6.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/CONTRIBUTING.md` & `cmomy-0.6.0/CONTRIBUTING.md`

 * *Files 14% similar despite different names*

```diff
@@ -380,21 +380,59 @@
 
 [setuptools_scm]: https://github.com/pypa/setuptools_scm
 
 Versioning is handled with [setuptools_scm].The package version is set by the
 git tag. For convenience, you can override the version with nox setting
 `--version ...`. This is useful for updating the docs, etc.
 
+We use the `write_to` option to [setuptools_scm]. This stores the current
+version in `_version.py`. Note that if you build the package (or, build docs
+with the `--version` flag), this will overwrite information in `_version.py` in
+the `src` directory. To refresh the version, run:
+
+```bash
+make version-scm
+```
+
+This scheme avoids having to install `setuptools-scm` (and `setuptools`) in each
+environment.
+
 ## Notes on [nox]
 
 One downside of using [tox] with this particular workflow is the need for
 multiple scripts/makefiles, while with [nox], most everything is self contained
 in the file `noxfile.py`. [nox] also is allows for a mix of conda and virtualenv
 environments.
 
+We use a mix of conda environments and virtualenv with nox. For example, for
+building the distribution, we use virtualenv, while for development, the default
+is to create a conda environment. To facilitate this, we need to let virtualenv
+know where different python interpreters are. I've had trouble mixing pyenv with
+conda. Instead, I use conda to create multiple invironments to hold different
+python version:
+
+```bash
+$ for version in 3.8 3.9 3.10 3.11; do
+    conda create -n test-3.8 python=3.8
+  done
+```
+
+To tell nox where these environments live, create the file `.noxconfig.toml`
+with the following:
+
+```toml
+[nox.python]
+paths = ["~/.conda/envs/test-3.*/bin"]
+
+```
+
+where `~/.conda/envs` should be replaced by whatever prefix you have setup on
+your machine. The noxfile will add this to the search path for python versions
+when creating virtualenvs.
+
 ## Serving the documentation
 
 To view to documentation with js headers/footers, you'll need to serve them:
 
 ```bash
 python -m http.server -d docs/_build/html
 ```
```

### Comparing `cmomy-0.5.0/LICENSE` & `cmomy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/Makefile` & `cmomy-0.6.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -129,19 +129,20 @@
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
-	python -c 'import cmomy; print(cmomy.__version__)'
+	-python -c 'import cmomy; print(cmomy.__version__)'
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
 .PHONY: environment-files-clean
@@ -266,7 +267,14 @@
 
 # Note that this requires `auto-changelog`, which can be installed with pip(x)
 auto-changelog: ## autogenerate changelog and print to stdout
 	auto-changelog -u -r usnistgov -v unreleased --tag-prefix v --stdout --template changelog.d/templates/auto-changelog/template.jinja2
 
 commitizen-changelog:
 	cz changelog --unreleased-version unreleased --dry-run --incremental
+
+# tuna analyze load time:
+.PHONY: tuna-analyze
+tuna-import: ## Analyze load time for module
+	python -X importtime -c 'import cmomy' 2> tuna-loadtime.log
+	tuna tuna-loadtime.log
+	rm tuna-loadtime.log
```

### Comparing `cmomy-0.5.0/PKG-INFO` & `cmomy-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmomy
-Version: 0.5.0
+Version: 0.6.0
 Summary: Central (co)moment calculation/manipulation
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/cmomy
 Project-URL: documentation, https://pages.nist.gov/cmomy/
 Keywords: cmomy
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cmomy-0.5.0/README.md` & `cmomy-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/changelog.d/templates/auto-changelog/template.jinja2` & `cmomy-0.6.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/Makefile` & `cmomy-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/_static/css/nist-combined.css` & `cmomy-0.6.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/_static/js/leave_notice.js` & `cmomy-0.6.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/_static/js/nist-header-footer.js` & `cmomy-0.6.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/_templates/autosummary/class.rst` & `cmomy-0.6.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/_templates/autosummary/module.rst` & `cmomy-0.6.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/_templates/class-individual-pages.rst` & `cmomy-0.6.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/_templates/module-custom.rst` & `cmomy-0.6.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/_templates/module-single.rst` & `cmomy-0.6.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/_templates/module-template.rst` & `cmomy-0.6.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/conf.py` & `cmomy-0.6.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,23 +232,36 @@
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 # versioning with scm with editable install has issues.
 # instead, try to use scm if available.
-try:
-    from setuptools_scm import get_version
+# try:
+#     from setuptools_scm import get_version
+
+#     version = get_version(root="..", relative_to=__file__)
+#     release = version
+# except ImportError:
+#     version = cmomy.__version__
+#     # The full version, including alpha/beta/rc tags.
+#     release = cmomy.__version__
+
+
+def _get_version():
+    import os
+
+    version = os.environ.get("SETUPTOOLS_SCM_PRETEND_VERSION", None)
+    if version is None:
+        version = cmomy.__version__
+    return version
+
+
+release = version = _get_version()
 
-    version = get_version(root="..", relative_to=__file__)
-    release = version
-except ImportError:
-    version = cmomy.__version__
-    # The full version, including alpha/beta/rc tags.
-    release = cmomy.__version__
 
 # if always want to print "latest"
 # release = "latest"
 # version = "latest"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
```

### Comparing `cmomy-0.5.0/docs/example_for_readme.md` & `cmomy-0.6.0/docs/example_for_readme.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/examples/usage/motivation.ipynb` & `cmomy-0.6.0/docs/examples/usage/motivation.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9890052702706768%*

 * *Differences: {"'cells'": "{5: {'execution_count': 4}, 7: {'execution_count': 5, 'outputs': {0: {'data': "*

 * *            '{\'text/html\': {insert: [(363, "</style><pre '*

 * *            "class='xr-text-repr-fallback'>array([1.0000e+03, 4.9592e-01, 8.4448e-02, "*

 * *            "1.5648e-03])</pre><div class='xr-wrap' style='display:none'><div "*

 * *            "class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul "*

 * *            "class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class "*

 * *         […]*

```diff
@@ -134,15 +134,15 @@
             "metadata": {},
             "source": [
                 "OK, great.  But what if we have unscaled data?  For example, setting $y = a x + b$ gives $\\ave{y} = a \\ave{x} + b$, but for central moments, $\\ave{(y - \\ave{y})^n} = \\ave{(a x - b - \\ave{a x - b})^n} = a^n \\ave{(\\delta x)^n}$"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 4,
             "id": "b2aad683",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -203,15 +203,15 @@
                 "\n",
                 "\n",
                 "The primary object for doing all this is {class}`~cmomy.CentralMoments`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 5,
             "id": "b50093e3",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -573,15 +573,15 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([1.0000e+03, 4.9592e-01, 8.4448e-02, 1.5648e-03])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-84ea3d45-e274-4d14-a832-78699b8b9fb8' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-84ea3d45-e274-4d14-a832-78699b8b9fb8' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-61e86f93-1179-4957-9811-171bb27416a2' class='xr-array-in' type='checkbox' checked><label for='section-61e86f93-1179-4957-9811-171bb27416a2' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>1e+03 0.4959 0.08445 0.001565</span></div><div class='xr-array-data'><pre>array([1.000000e+03, 4.959215e-01, 8.444769e-02, 1.564753e-03])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([1.0000e+03, 4.9592e-01, 8.4448e-02, 1.5648e-03])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-5c626096-5f8a-4f6e-ae33-2828bec413f0' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-5c626096-5f8a-4f6e-ae33-2828bec413f0' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-f462bc03-c896-4a54-b421-cef9c524f288' class='xr-array-in' type='checkbox' checked><label for='section-f462bc03-c896-4a54-b421-cef9c524f288' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>1e+03 0.4959 0.08445 0.001565</span></div><div class='xr-array-data'><pre>array([1.000000e+03, 4.959215e-01, 8.444769e-02, 1.564753e-03])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(3,))>\n",
                             "array([1.0000e+03, 4.9592e-01, 8.4448e-02, 1.5648e-03])"
                         ]
                     },
                     "metadata": {},
@@ -604,15 +604,15 @@
             "metadata": {},
             "source": [
                 "You can access the underlying data using the {attr}`cmomy.CentralMoments.values` or {attr}`cmomy.CentralMoments.data` attributes."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 9,
             "id": "0a64afad",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -630,15 +630,15 @@
             "metadata": {},
             "source": [
                 "Basically, the {class}`~cmomy.CentralMoments` object is just a collection of routines around {attr}`~cmomy.CentralMoments.data`, which is an array of central moments (with the convention that `data[..., 0]` is the total `weight`, `data[..., 1]` is the average, and `data[..., k > 1]` is the `kth` central moment).  It gives the same results as calculating central moments directly:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 10,
             "id": "c68b5deb",
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(cx.values, m1)\n",
                 "np.testing.assert_allclose(cy.values, m1_shift)"
             ]
@@ -650,29 +650,29 @@
             "source": [
                 "Nice!  But what can that's not all that special.  The real power comes in for multidimensional data.\n",
                 "Suppose that we have separate samples of the data $\\{x_a, x_b, ... \\}$, and want to get there central moments.  We can do the following."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 11,
             "id": "d9db01aa",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[ 1.0000e+02,  4.7485e-01,  8.4724e-02,  2.7697e-03,  1.3407e-02],\n",
                             "       [ 1.0000e+02,  4.8072e-01,  8.7882e-02,  8.1934e-04,  1.3999e-02],\n",
                             "       [ 1.0000e+02,  4.9077e-01,  9.2369e-02,  5.5313e-03,  1.5294e-02],\n",
                             "       [ 1.0000e+02,  5.4378e-01,  1.0249e-01, -5.3586e-03,  1.6396e-02],\n",
                             "       [ 1.0000e+02,  5.6677e-01,  8.0621e-02, -8.4636e-03,  1.3304e-02]])"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "x = np.random.rand(100, 5)\n",
                 "m1 = cmom_1(x, axis=0, mom=4)\n",
@@ -685,15 +685,15 @@
             "metadata": {},
             "source": [
                 "Wrapping the data in a central moments object gives"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 12,
             "id": "8caf651b",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -719,15 +719,15 @@
             "metadata": {},
             "source": [
                 "Excellent! We can use {class}`~cmomy.CentralMoments` to accumulate data on the go"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 14,
             "id": "54a71048",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -1089,15 +1089,15 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-5ceb1201-4b9a-4801-9fa9-4a6406e8fc58' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-5ceb1201-4b9a-4801-9fa9-4a6406e8fc58' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-3d45d097-8de1-4698-9b87-33c0de3fe359' class='xr-array-in' type='checkbox' checked><label for='section-3d45d097-8de1-4698-9b87-33c0de3fe359' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
+                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-c14610fa-b159-4fea-a537-caa5cb180619' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-c14610fa-b159-4fea-a537-caa5cb180619' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-6edbabb9-e2c4-4fd4-9002-9d18c15fb96a' class='xr-array-in' type='checkbox' checked><label for='section-6edbabb9-e2c4-4fd4-9002-9d18c15fb96a' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
                             "        1.448420e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])"
                         ]
                     },
@@ -1119,15 +1119,15 @@
             "metadata": {},
             "source": [
                 "Or, you can push all the values one at a time!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 15,
             "id": "e4857256",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -1489,23 +1489,23 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-ecbe12cf-9dc0-4886-874c-4c4a593b7468' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ecbe12cf-9dc0-4886-874c-4c4a593b7468' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-d34a2a8a-ec34-45cd-bb67-bdb2ce8107be' class='xr-array-in' type='checkbox' checked><label for='section-d34a2a8a-ec34-45cd-bb67-bdb2ce8107be' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
+                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-f154d33c-15a4-41fc-afaf-69444fd1cc87' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-f154d33c-15a4-41fc-afaf-69444fd1cc87' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-4a380ce5-48a9-41c8-af30-9a3272c8b1bf' class='xr-array-in' type='checkbox' checked><label for='section-4a380ce5-48a9-41c8-af30-9a3272c8b1bf' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
                             "        1.448420e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "c.zero()\n",
                 "for xx in x.reshape(-1):\n",
@@ -1521,15 +1521,15 @@
             "metadata": {},
             "source": [
                 "The values can even be differently weighted."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 16,
             "id": "bd188c32",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -1891,23 +1891,23 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-459d9aea-8b69-436c-b408-5dd23478d87e' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-459d9aea-8b69-436c-b408-5dd23478d87e' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-516c474c-340c-4cae-9779-44f9985f660f' class='xr-array-in' type='checkbox' checked><label for='section-516c474c-340c-4cae-9779-44f9985f660f' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
+                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-12357a5f-37b2-4237-9595-f0e4ede7f3a0' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-12357a5f-37b2-4237-9595-f0e4ede7f3a0' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-b3b7064a-3813-4090-a1ed-2f046524f074' class='xr-array-in' type='checkbox' checked><label for='section-b3b7064a-3813-4090-a1ed-2f046524f074' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
                             "        1.448420e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])"
                         ]
                     },
-                    "execution_count": 25,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "xs = np.split(x.reshape(-1), [50, 150, 300])\n",
                 "\n",
@@ -1923,15 +1923,15 @@
             "metadata": {},
             "source": [
                 "Alternatively, you can add objects together."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 17,
             "id": "74e8be73",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -2304,23 +2304,23 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-8191cda1-05be-4980-8e1a-e53f59577e07' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-8191cda1-05be-4980-8e1a-e53f59577e07' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-ec0b9318-47ce-40e9-b64b-bcd84208d21e' class='xr-array-in' type='checkbox' checked><label for='section-ec0b9318-47ce-40e9-b64b-bcd84208d21e' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
+                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-7e421a67-4e39-48b3-bc55-098e2814baac' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-7e421a67-4e39-48b3-bc55-098e2814baac' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-184c5dca-0f34-4db2-998c-83b98f486813' class='xr-array-in' type='checkbox' checked><label for='section-184c5dca-0f34-4db2-998c-83b98f486813' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
                             "        1.448420e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "cs = [cmomy.CentralMoments.from_vals(v, mom=4) for v in xs]\n",
                 "print(cs)\n",
@@ -2335,15 +2335,15 @@
             "metadata": {},
             "source": [
                 "Or more simply:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 18,
             "id": "39a9d1c8",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -2371,15 +2371,15 @@
                 "## weighted averages\n",
                 "\n",
                 "cmomy is setup to work with arbitrary weights.  We saw this work above when we considered unequal sample sizes.  For example,"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 19,
             "id": "b2ed66e7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def get_cmom_with_weights(x, w, axis=0, mom=3):\n",
                 "    \"\"\"Create central moments using stable method\"\"\"\n",
                 "    # output shape\n",
@@ -2400,15 +2400,15 @@
                 "    ).sum(axis=axis) * w_norm\n",
                 "\n",
                 "    return output"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 20,
             "id": "48a3fab7",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -2770,22 +2770,22 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([5.1503e+01, 4.9029e-01, 9.1092e-02, 5.3542e-09])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-c121a44f-59fb-437a-9a77-b17f2ea72d1a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-c121a44f-59fb-437a-9a77-b17f2ea72d1a' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-c27554c1-6a75-44a1-b845-47fe94469fb5' class='xr-array-in' type='checkbox' checked><label for='section-c27554c1-6a75-44a1-b845-47fe94469fb5' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>51.5 0.4903 0.09109 5.354e-09</span></div><div class='xr-array-data'><pre>array([5.150285e+01, 4.902857e-01, 9.109218e-02, 5.354191e-09])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([ 5.1337e+01,  5.4415e-01,  8.9238e-02, -6.9704e-03])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-ea34017f-fe34-4af9-a7ab-025ce68811b6' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ea34017f-fe34-4af9-a7ab-025ce68811b6' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-b8ed3002-fbcb-432c-b633-98892204a056' class='xr-array-in' type='checkbox' checked><label for='section-b8ed3002-fbcb-432c-b633-98892204a056' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>51.34 0.5442 0.08924 -0.00697</span></div><div class='xr-array-data'><pre>array([ 5.133746e+01,  5.441544e-01,  8.923830e-02, -6.970374e-03])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(3,))>\n",
-                            "array([5.1503e+01, 4.9029e-01, 9.1092e-02, 5.3542e-09])"
+                            "array([ 5.1337e+01,  5.4415e-01,  8.9238e-02, -6.9704e-03])"
                         ]
                     },
-                    "execution_count": 32,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "x = np.random.rand(100)\n",
                 "w = np.random.rand(100)\n",
@@ -2805,15 +2805,15 @@
                 "\n",
                 "cmomy can also handle comoments (covariance, etc), like the $\\ave{(\\delta x)^i (\\delta y)^j}$    \n",
                 "For example"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 22,
             "id": "88bf86b5",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -3175,28 +3175,28 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([[ 5.1503e+01,  4.7448e-01,  9.8409e-02],\n",
-                            "       [ 4.9029e-01,  2.3666e-02, -1.1773e-03],\n",
-                            "       [ 9.1092e-02,  1.0251e-04,  9.1080e-03]])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: (2, 2)</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-e63a1a0b-5345-4f82-b354-20e44d432b98' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-e63a1a0b-5345-4f82-b354-20e44d432b98' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-4fc2dc8b-9ad4-4d00-954c-d70c12ffa4e0' class='xr-array-in' type='checkbox' checked><label for='section-4fc2dc8b-9ad4-4d00-954c-d70c12ffa4e0' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>51.5 0.4745 0.09841 0.4903 ... -0.001177 0.09109 0.0001025 0.009108</span></div><div class='xr-array-data'><pre>array([[ 5.150285e+01,  4.744806e-01,  9.840866e-02],\n",
-                            "       [ 4.902857e-01,  2.366622e-02, -1.177349e-03],\n",
-                            "       [ 9.109218e-02,  1.025148e-04,  9.108013e-03]])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([[ 5.1337e+01,  5.3346e-01,  8.4150e-02],\n",
+                            "       [ 5.4415e-01, -8.0426e-03,  3.0820e-03],\n",
+                            "       [ 8.9238e-02, -8.2899e-04,  6.8269e-03]])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: (2, 2)</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-855eab1d-2dcd-4bff-82af-76cd059cb75a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-855eab1d-2dcd-4bff-82af-76cd059cb75a' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-d4979081-73a4-4223-ae33-58e48e932a90' class='xr-array-in' type='checkbox' checked><label for='section-d4979081-73a4-4223-ae33-58e48e932a90' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>51.34 0.5335 0.08415 0.5442 ... 0.003082 0.08924 -0.000829 0.006827</span></div><div class='xr-array-data'><pre>array([[ 5.133746e+01,  5.334590e-01,  8.414989e-02],\n",
+                            "       [ 5.441544e-01, -8.042619e-03,  3.081975e-03],\n",
+                            "       [ 8.923830e-02, -8.289860e-04,  6.826899e-03]])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(2, 2))>\n",
-                            "array([[ 5.1503e+01,  4.7448e-01,  9.8409e-02],\n",
-                            "       [ 4.9029e-01,  2.3666e-02, -1.1773e-03],\n",
-                            "       [ 9.1092e-02,  1.0251e-04,  9.1080e-03]])"
+                            "array([[ 5.1337e+01,  5.3346e-01,  8.4150e-02],\n",
+                            "       [ 5.4415e-01, -8.0426e-03,  3.0820e-03],\n",
+                            "       [ 8.9238e-02, -8.2899e-04,  6.8269e-03]])"
                         ]
                     },
-                    "execution_count": 33,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "y = np.random.rand(100)\n",
                 "\n",
@@ -3219,15 +3219,15 @@
                 "## xarray DataArray support\n",
                 "\n",
                 "cmomy also works with {class}`xarray.DataArray` objects.  For example"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 23,
             "id": "cc5e273d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -3590,45 +3590,45 @@
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (rec: 3, a: 2, b: 3)&gt;\n",
-                            "array([[[0.8115, 0.4761, 0.5232],\n",
-                            "        [0.2505, 0.605 , 0.3029]],\n",
+                            "array([[[0.8257, 0.7468, 0.5123],\n",
+                            "        [0.458 , 0.5494, 0.7046]],\n",
                             "\n",
-                            "       [[0.5773, 0.1697, 0.1595],\n",
-                            "        [0.417 , 0.4268, 0.2681]],\n",
+                            "       [[0.9229, 0.617 , 0.8878],\n",
+                            "        [0.7013, 0.0683, 0.5008]],\n",
                             "\n",
-                            "       [[0.1316, 0.0392, 0.0252],\n",
-                            "        [0.2716, 0.4619, 0.7262]]])\n",
-                            "Dimensions without coordinates: rec, a, b</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rec</span>: 3</li><li><span>a</span>: 2</li><li><span>b</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-67189007-b62b-48c2-9346-92b6524a177c' class='xr-array-in' type='checkbox' checked><label for='section-67189007-b62b-48c2-9346-92b6524a177c' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>0.8115 0.4761 0.5232 0.2505 0.605 ... 0.02523 0.2716 0.4619 0.7262</span></div><div class='xr-array-data'><pre>array([[[0.8115, 0.4761, 0.5232],\n",
-                            "        [0.2505, 0.605 , 0.3029]],\n",
+                            "       [[0.2865, 0.2852, 0.3559],\n",
+                            "        [0.3147, 0.5786, 0.6836]]])\n",
+                            "Dimensions without coordinates: rec, a, b</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rec</span>: 3</li><li><span>a</span>: 2</li><li><span>b</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-995e5b75-9260-4de3-b352-70f7917ff811' class='xr-array-in' type='checkbox' checked><label for='section-995e5b75-9260-4de3-b352-70f7917ff811' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>0.8257 0.7468 0.5123 0.458 0.5494 ... 0.3559 0.3147 0.5786 0.6836</span></div><div class='xr-array-data'><pre>array([[[0.8257, 0.7468, 0.5123],\n",
+                            "        [0.458 , 0.5494, 0.7046]],\n",
                             "\n",
-                            "       [[0.5773, 0.1697, 0.1595],\n",
-                            "        [0.417 , 0.4268, 0.2681]],\n",
+                            "       [[0.9229, 0.617 , 0.8878],\n",
+                            "        [0.7013, 0.0683, 0.5008]],\n",
                             "\n",
-                            "       [[0.1316, 0.0392, 0.0252],\n",
-                            "        [0.2716, 0.4619, 0.7262]]])</pre></div></div></li><li class='xr-section-item'><input id='section-f390945f-8166-4ddc-9701-233683252642' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-f390945f-8166-4ddc-9701-233683252642' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-ac861439-d4d0-4267-a906-ece0ba7e1eb9' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ac861439-d4d0-4267-a906-ece0ba7e1eb9' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-eb9bbbbc-0b4c-47ff-9c83-bb62d53251dc' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-eb9bbbbc-0b4c-47ff-9c83-bb62d53251dc' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "       [[0.2865, 0.2852, 0.3559],\n",
+                            "        [0.3147, 0.5786, 0.6836]]])</pre></div></div></li><li class='xr-section-item'><input id='section-ab659195-7680-4e7d-9bf5-1a4fe8888f6a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ab659195-7680-4e7d-9bf5-1a4fe8888f6a' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-9568ba27-c22b-4346-86f7-43ac3a39ea75' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-9568ba27-c22b-4346-86f7-43ac3a39ea75' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-84d6b7d4-2d22-4470-aa12-2b29fb407116' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-84d6b7d4-2d22-4470-aa12-2b29fb407116' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.DataArray (rec: 3, a: 2, b: 3)>\n",
-                            "array([[[0.8115, 0.4761, 0.5232],\n",
-                            "        [0.2505, 0.605 , 0.3029]],\n",
+                            "array([[[0.8257, 0.7468, 0.5123],\n",
+                            "        [0.458 , 0.5494, 0.7046]],\n",
                             "\n",
-                            "       [[0.5773, 0.1697, 0.1595],\n",
-                            "        [0.417 , 0.4268, 0.2681]],\n",
+                            "       [[0.9229, 0.617 , 0.8878],\n",
+                            "        [0.7013, 0.0683, 0.5008]],\n",
                             "\n",
-                            "       [[0.1316, 0.0392, 0.0252],\n",
-                            "        [0.2716, 0.4619, 0.7262]]])\n",
+                            "       [[0.2865, 0.2852, 0.3559],\n",
+                            "        [0.3147, 0.5786, 0.6836]]])\n",
                             "Dimensions without coordinates: rec, a, b"
                         ]
                     },
-                    "execution_count": 34,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import xarray as xr\n",
                 "\n",
@@ -3642,15 +3642,15 @@
             "metadata": {},
             "source": [
                 "To create a cmomy object wrapping a {class}`xarray.DataArray`, use {class}`~cmomy.xCentralMoments`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 24,
             "id": "38a244b6",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -4013,22 +4013,22 @@
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (a: 2, b: 3, mom_0: 4)&gt;\n",
-                            "array([[[ 1.0000e+02,  5.4290e-01,  7.7797e-02, -8.3022e-03],\n",
-                            "        [ 1.0000e+02,  5.0585e-01,  9.4957e-02,  7.6531e-04],\n",
-                            "        [ 1.0000e+02,  4.5853e-01,  8.5859e-02,  6.1346e-03]],\n",
-                            "\n",
-                            "       [[ 1.0000e+02,  5.0983e-01,  7.7844e-02,  2.2635e-03],\n",
-                            "        [ 1.0000e+02,  5.2817e-01,  8.4799e-02,  5.6189e-04],\n",
-                            "        [ 1.0000e+02,  4.8895e-01,  6.4305e-02, -1.0829e-04]]])\n",
-                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: (2, 3)</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-02121d9e-9620-4f6f-8185-5f43310a3f93' class='xr-section-summary-in' type='checkbox'  checked><label for='section-02121d9e-9620-4f6f-8185-5f43310a3f93' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>(a, b)</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
+                            "array([[[ 1.0000e+02,  4.6429e-01,  8.9723e-02,  4.5381e-03],\n",
+                            "        [ 1.0000e+02,  5.0233e-01,  8.0919e-02,  3.1135e-03],\n",
+                            "        [ 1.0000e+02,  5.2084e-01,  8.6462e-02, -1.6221e-03]],\n",
+                            "\n",
+                            "       [[ 1.0000e+02,  4.9178e-01,  6.4268e-02, -2.2615e-04],\n",
+                            "        [ 1.0000e+02,  5.0930e-01,  8.1505e-02, -4.6409e-03],\n",
+                            "        [ 1.0000e+02,  5.0885e-01,  9.2137e-02, -1.6572e-03]]])\n",
+                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: (2, 3)</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-40dedf1d-f740-4b71-8aa8-3ef78ce5037d' class='xr-section-summary-in' type='checkbox'  checked><label for='section-40dedf1d-f740-4b71-8aa8-3ef78ce5037d' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>(a, b)</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
                             "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
                             "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "</symbol>\n",
                             "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
@@ -4384,43 +4384,43 @@
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (a: 2, b: 3, mom_0: 4)&gt;\n",
-                            "array([[[ 1.0000e+02,  5.4290e-01,  7.7797e-02, -8.3022e-03],\n",
-                            "        [ 1.0000e+02,  5.0585e-01,  9.4957e-02,  7.6531e-04],\n",
-                            "        [ 1.0000e+02,  4.5853e-01,  8.5859e-02,  6.1346e-03]],\n",
-                            "\n",
-                            "       [[ 1.0000e+02,  5.0983e-01,  7.7844e-02,  2.2635e-03],\n",
-                            "        [ 1.0000e+02,  5.2817e-01,  8.4799e-02,  5.6189e-04],\n",
-                            "        [ 1.0000e+02,  4.8895e-01,  6.4305e-02, -1.0829e-04]]])\n",
-                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>a</span>: 2</li><li><span>b</span>: 3</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-c6c44a6f-53ba-490c-867d-1f8115fbe730' class='xr-array-in' type='checkbox' checked><label for='section-c6c44a6f-53ba-490c-867d-1f8115fbe730' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>100.0 0.5429 0.0778 -0.008302 ... 100.0 0.4889 0.06431 -0.0001083</span></div><div class='xr-array-data'><pre>array([[[ 1.0000e+02,  5.4290e-01,  7.7797e-02, -8.3022e-03],\n",
-                            "        [ 1.0000e+02,  5.0585e-01,  9.4957e-02,  7.6531e-04],\n",
-                            "        [ 1.0000e+02,  4.5853e-01,  8.5859e-02,  6.1346e-03]],\n",
-                            "\n",
-                            "       [[ 1.0000e+02,  5.0983e-01,  7.7844e-02,  2.2635e-03],\n",
-                            "        [ 1.0000e+02,  5.2817e-01,  8.4799e-02,  5.6189e-04],\n",
-                            "        [ 1.0000e+02,  4.8895e-01,  6.4305e-02, -1.0829e-04]]])</pre></div></div></li><li class='xr-section-item'><input id='section-1df705fa-ff6a-4128-9e62-26988df23d6e' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1df705fa-ff6a-4128-9e62-26988df23d6e' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-1861d6c1-cd0e-4c88-9c46-154b6aaa7e75' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1861d6c1-cd0e-4c88-9c46-154b6aaa7e75' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-572c7fe3-4d3b-4788-aa96-10ddb87b093a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-572c7fe3-4d3b-4788-aa96-10ddb87b093a' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "array([[[ 1.0000e+02,  4.6429e-01,  8.9723e-02,  4.5381e-03],\n",
+                            "        [ 1.0000e+02,  5.0233e-01,  8.0919e-02,  3.1135e-03],\n",
+                            "        [ 1.0000e+02,  5.2084e-01,  8.6462e-02, -1.6221e-03]],\n",
+                            "\n",
+                            "       [[ 1.0000e+02,  4.9178e-01,  6.4268e-02, -2.2615e-04],\n",
+                            "        [ 1.0000e+02,  5.0930e-01,  8.1505e-02, -4.6409e-03],\n",
+                            "        [ 1.0000e+02,  5.0885e-01,  9.2137e-02, -1.6572e-03]]])\n",
+                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>a</span>: 2</li><li><span>b</span>: 3</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-40560fd9-580a-47df-9ca0-250337a8a9e3' class='xr-array-in' type='checkbox' checked><label for='section-40560fd9-580a-47df-9ca0-250337a8a9e3' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>100.0 0.4643 0.08972 0.004538 100.0 ... 100.0 0.5089 0.09214 -0.001657</span></div><div class='xr-array-data'><pre>array([[[ 1.0000e+02,  4.6429e-01,  8.9723e-02,  4.5381e-03],\n",
+                            "        [ 1.0000e+02,  5.0233e-01,  8.0919e-02,  3.1135e-03],\n",
+                            "        [ 1.0000e+02,  5.2084e-01,  8.6462e-02, -1.6221e-03]],\n",
+                            "\n",
+                            "       [[ 1.0000e+02,  4.9178e-01,  6.4268e-02, -2.2615e-04],\n",
+                            "        [ 1.0000e+02,  5.0930e-01,  8.1505e-02, -4.6409e-03],\n",
+                            "        [ 1.0000e+02,  5.0885e-01,  9.2137e-02, -1.6572e-03]]])</pre></div></div></li><li class='xr-section-item'><input id='section-68044e2b-2e3c-4a6f-8bee-2fb27df11a3a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-68044e2b-2e3c-4a6f-8bee-2fb27df11a3a' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-e4c77ac9-16cb-4bca-b9d5-e44460fea2a6' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-e4c77ac9-16cb-4bca-b9d5-e44460fea2a6' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-d70728cf-e253-40f6-b5e2-191d8df923a3' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-d70728cf-e253-40f6-b5e2-191d8df923a3' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xCentralMoments(val_shape=(2, 3), mom=(3,))>\n",
                             "<xarray.DataArray (a: 2, b: 3, mom_0: 4)>\n",
-                            "array([[[ 1.0000e+02,  5.4290e-01,  7.7797e-02, -8.3022e-03],\n",
-                            "        [ 1.0000e+02,  5.0585e-01,  9.4957e-02,  7.6531e-04],\n",
-                            "        [ 1.0000e+02,  4.5853e-01,  8.5859e-02,  6.1346e-03]],\n",
-                            "\n",
-                            "       [[ 1.0000e+02,  5.0983e-01,  7.7844e-02,  2.2635e-03],\n",
-                            "        [ 1.0000e+02,  5.2817e-01,  8.4799e-02,  5.6189e-04],\n",
-                            "        [ 1.0000e+02,  4.8895e-01,  6.4305e-02, -1.0829e-04]]])\n",
+                            "array([[[ 1.0000e+02,  4.6429e-01,  8.9723e-02,  4.5381e-03],\n",
+                            "        [ 1.0000e+02,  5.0233e-01,  8.0919e-02,  3.1135e-03],\n",
+                            "        [ 1.0000e+02,  5.2084e-01,  8.6462e-02, -1.6221e-03]],\n",
+                            "\n",
+                            "       [[ 1.0000e+02,  4.9178e-01,  6.4268e-02, -2.2615e-04],\n",
+                            "        [ 1.0000e+02,  5.0930e-01,  8.1505e-02, -4.6409e-03],\n",
+                            "        [ 1.0000e+02,  5.0885e-01,  9.2137e-02, -1.6572e-03]]])\n",
                             "Dimensions without coordinates: a, b, mom_0"
                         ]
                     },
-                    "execution_count": 35,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "c = cmomy.xCentralMoments.from_vals(x, dim=\"rec\", mom=3)\n",
                 "c"
@@ -4434,29 +4434,29 @@
                 "Everything that {class}`~cmomy.CentralMoments` can do, {class}`~cmomy.xCentralMoments` can do."
             ]
         }
     ],
     "metadata": {
         "celltoolbar": "Tags",
         "kernelspec": {
-            "display_name": "Python [conda env:cmomy-env]",
+            "display_name": "cmomy-dev [conda env:dev-3]",
             "language": "python",
-            "name": "conda-env-cmomy-env-py"
+            "name": "conda-env-dev-3-py"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.10.11"
         },
         "toc": {
             "base_numbering": 1,
             "nav_menu": {},
             "number_sections": true,
             "sideBar": true,
             "skip_h1_title": false,
```

### Comparing `cmomy-0.5.0/docs/examples/usage/usage_notebook.ipynb` & `cmomy-0.6.0/docs/examples/usage/usage_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/installation.md` & `cmomy-0.6.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/docs/make.bat` & `cmomy-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/environment/dev.yaml` & `cmomy-0.6.0/environment/dev.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,17 @@
   - python>=3.8
   - numpy >= 1.21
   - numba >= 0.50
   - xarray >= 0.16
   - typing-extensions
   - custom-inherit
   - module-utilities >= 0.1
+  - lazy_loader
   - pytest
-  - python-xdist
+  - pytest-xdist
   - pytest-cov
   - pytest-sugar
   - mypy
   - setuptools-scm
   - ipython
   - ipykernel
   - nox
```

### Comparing `cmomy-0.5.0/environment/docs-extras.yaml` & `cmomy-0.6.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/environment/docs.yaml` & `cmomy-0.6.0/environment/docs.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   - python>=3.8
   - numpy >= 1.21
   - numba >= 0.50
   - xarray >= 0.16
   - typing-extensions
   - custom-inherit
   - module-utilities >= 0.1
-  - setuptools-scm
+  - lazy_loader
   - ipython
   - pyenchant
   - ghp-import
   - sphinx
   - sphinx-copybutton
   - sphinxcontrib-spelling
   - sphinx-autobuild
```

### Comparing `cmomy-0.5.0/examples/archived/bootstrap.ipynb` & `cmomy-0.6.0/examples/archived/bootstrap.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/examples/archived/central_moments.ipynb` & `cmomy-0.6.0/examples/archived/central_moments.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/examples/archived/example_usage.ipynb` & `cmomy-0.6.0/examples/archived/example_usage.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/examples/archived/parallel_test.ipynb` & `cmomy-0.6.0/examples/archived/parallel_test.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/examples/archived/test_accumulator.ipynb` & `cmomy-0.6.0/examples/archived/test_accumulator.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/examples/usage/motivation.ipynb` & `cmomy-0.6.0/examples/usage/motivation.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9890052702706768%*

 * *Differences: {"'cells'": "{5: {'execution_count': 4}, 7: {'execution_count': 5, 'outputs': {0: {'data': "*

 * *            '{\'text/html\': {insert: [(363, "</style><pre '*

 * *            "class='xr-text-repr-fallback'>array([1.0000e+03, 4.9592e-01, 8.4448e-02, "*

 * *            "1.5648e-03])</pre><div class='xr-wrap' style='display:none'><div "*

 * *            "class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul "*

 * *            "class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class "*

 * *         […]*

```diff
@@ -134,15 +134,15 @@
             "metadata": {},
             "source": [
                 "OK, great.  But what if we have unscaled data?  For example, setting $y = a x + b$ gives $\\ave{y} = a \\ave{x} + b$, but for central moments, $\\ave{(y - \\ave{y})^n} = \\ave{(a x - b - \\ave{a x - b})^n} = a^n \\ave{(\\delta x)^n}$"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 4,
             "id": "b2aad683",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -203,15 +203,15 @@
                 "\n",
                 "\n",
                 "The primary object for doing all this is {class}`~cmomy.CentralMoments`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 5,
             "id": "b50093e3",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -573,15 +573,15 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([1.0000e+03, 4.9592e-01, 8.4448e-02, 1.5648e-03])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-84ea3d45-e274-4d14-a832-78699b8b9fb8' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-84ea3d45-e274-4d14-a832-78699b8b9fb8' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-61e86f93-1179-4957-9811-171bb27416a2' class='xr-array-in' type='checkbox' checked><label for='section-61e86f93-1179-4957-9811-171bb27416a2' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>1e+03 0.4959 0.08445 0.001565</span></div><div class='xr-array-data'><pre>array([1.000000e+03, 4.959215e-01, 8.444769e-02, 1.564753e-03])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([1.0000e+03, 4.9592e-01, 8.4448e-02, 1.5648e-03])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-5c626096-5f8a-4f6e-ae33-2828bec413f0' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-5c626096-5f8a-4f6e-ae33-2828bec413f0' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-f462bc03-c896-4a54-b421-cef9c524f288' class='xr-array-in' type='checkbox' checked><label for='section-f462bc03-c896-4a54-b421-cef9c524f288' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>1e+03 0.4959 0.08445 0.001565</span></div><div class='xr-array-data'><pre>array([1.000000e+03, 4.959215e-01, 8.444769e-02, 1.564753e-03])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(3,))>\n",
                             "array([1.0000e+03, 4.9592e-01, 8.4448e-02, 1.5648e-03])"
                         ]
                     },
                     "metadata": {},
@@ -604,15 +604,15 @@
             "metadata": {},
             "source": [
                 "You can access the underlying data using the {attr}`cmomy.CentralMoments.values` or {attr}`cmomy.CentralMoments.data` attributes."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 9,
             "id": "0a64afad",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -630,15 +630,15 @@
             "metadata": {},
             "source": [
                 "Basically, the {class}`~cmomy.CentralMoments` object is just a collection of routines around {attr}`~cmomy.CentralMoments.data`, which is an array of central moments (with the convention that `data[..., 0]` is the total `weight`, `data[..., 1]` is the average, and `data[..., k > 1]` is the `kth` central moment).  It gives the same results as calculating central moments directly:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 10,
             "id": "c68b5deb",
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(cx.values, m1)\n",
                 "np.testing.assert_allclose(cy.values, m1_shift)"
             ]
@@ -650,29 +650,29 @@
             "source": [
                 "Nice!  But what can that's not all that special.  The real power comes in for multidimensional data.\n",
                 "Suppose that we have separate samples of the data $\\{x_a, x_b, ... \\}$, and want to get there central moments.  We can do the following."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 11,
             "id": "d9db01aa",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[ 1.0000e+02,  4.7485e-01,  8.4724e-02,  2.7697e-03,  1.3407e-02],\n",
                             "       [ 1.0000e+02,  4.8072e-01,  8.7882e-02,  8.1934e-04,  1.3999e-02],\n",
                             "       [ 1.0000e+02,  4.9077e-01,  9.2369e-02,  5.5313e-03,  1.5294e-02],\n",
                             "       [ 1.0000e+02,  5.4378e-01,  1.0249e-01, -5.3586e-03,  1.6396e-02],\n",
                             "       [ 1.0000e+02,  5.6677e-01,  8.0621e-02, -8.4636e-03,  1.3304e-02]])"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "x = np.random.rand(100, 5)\n",
                 "m1 = cmom_1(x, axis=0, mom=4)\n",
@@ -685,15 +685,15 @@
             "metadata": {},
             "source": [
                 "Wrapping the data in a central moments object gives"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 12,
             "id": "8caf651b",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -719,15 +719,15 @@
             "metadata": {},
             "source": [
                 "Excellent! We can use {class}`~cmomy.CentralMoments` to accumulate data on the go"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 14,
             "id": "54a71048",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -1089,15 +1089,15 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-5ceb1201-4b9a-4801-9fa9-4a6406e8fc58' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-5ceb1201-4b9a-4801-9fa9-4a6406e8fc58' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-3d45d097-8de1-4698-9b87-33c0de3fe359' class='xr-array-in' type='checkbox' checked><label for='section-3d45d097-8de1-4698-9b87-33c0de3fe359' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
+                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-c14610fa-b159-4fea-a537-caa5cb180619' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-c14610fa-b159-4fea-a537-caa5cb180619' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-6edbabb9-e2c4-4fd4-9002-9d18c15fb96a' class='xr-array-in' type='checkbox' checked><label for='section-6edbabb9-e2c4-4fd4-9002-9d18c15fb96a' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
                             "        1.448420e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])"
                         ]
                     },
@@ -1119,15 +1119,15 @@
             "metadata": {},
             "source": [
                 "Or, you can push all the values one at a time!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 15,
             "id": "e4857256",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -1489,23 +1489,23 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-ecbe12cf-9dc0-4886-874c-4c4a593b7468' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ecbe12cf-9dc0-4886-874c-4c4a593b7468' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-d34a2a8a-ec34-45cd-bb67-bdb2ce8107be' class='xr-array-in' type='checkbox' checked><label for='section-d34a2a8a-ec34-45cd-bb67-bdb2ce8107be' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
+                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-f154d33c-15a4-41fc-afaf-69444fd1cc87' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-f154d33c-15a4-41fc-afaf-69444fd1cc87' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-4a380ce5-48a9-41c8-af30-9a3272c8b1bf' class='xr-array-in' type='checkbox' checked><label for='section-4a380ce5-48a9-41c8-af30-9a3272c8b1bf' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
                             "        1.448420e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "c.zero()\n",
                 "for xx in x.reshape(-1):\n",
@@ -1521,15 +1521,15 @@
             "metadata": {},
             "source": [
                 "The values can even be differently weighted."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 16,
             "id": "bd188c32",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -1891,23 +1891,23 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-459d9aea-8b69-436c-b408-5dd23478d87e' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-459d9aea-8b69-436c-b408-5dd23478d87e' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-516c474c-340c-4cae-9779-44f9985f660f' class='xr-array-in' type='checkbox' checked><label for='section-516c474c-340c-4cae-9779-44f9985f660f' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
+                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-12357a5f-37b2-4237-9595-f0e4ede7f3a0' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-12357a5f-37b2-4237-9595-f0e4ede7f3a0' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-b3b7064a-3813-4090-a1ed-2f046524f074' class='xr-array-in' type='checkbox' checked><label for='section-b3b7064a-3813-4090-a1ed-2f046524f074' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
                             "        1.448420e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])"
                         ]
                     },
-                    "execution_count": 25,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "xs = np.split(x.reshape(-1), [50, 150, 300])\n",
                 "\n",
@@ -1923,15 +1923,15 @@
             "metadata": {},
             "source": [
                 "Alternatively, you can add objects together."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 17,
             "id": "74e8be73",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -2304,23 +2304,23 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-8191cda1-05be-4980-8e1a-e53f59577e07' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-8191cda1-05be-4980-8e1a-e53f59577e07' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-ec0b9318-47ce-40e9-b64b-bcd84208d21e' class='xr-array-in' type='checkbox' checked><label for='section-ec0b9318-47ce-40e9-b64b-bcd84208d21e' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
+                            "</style><pre class='xr-text-repr-fallback'>array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-7e421a67-4e39-48b3-bc55-098e2814baac' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-7e421a67-4e39-48b3-bc55-098e2814baac' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-184c5dca-0f34-4db2-998c-83b98f486813' class='xr-array-in' type='checkbox' checked><label for='section-184c5dca-0f34-4db2-998c-83b98f486813' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.5114 0.09098 -0.0008604 0.01448</span></div><div class='xr-array-data'><pre>array([ 5.000000e+02,  5.113782e-01,  9.098104e-02, -8.603719e-04,\n",
                             "        1.448420e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([ 5.0000e+02,  5.1138e-01,  9.0981e-02, -8.6037e-04,  1.4484e-02])"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "cs = [cmomy.CentralMoments.from_vals(v, mom=4) for v in xs]\n",
                 "print(cs)\n",
@@ -2335,15 +2335,15 @@
             "metadata": {},
             "source": [
                 "Or more simply:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 18,
             "id": "39a9d1c8",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -2371,15 +2371,15 @@
                 "## weighted averages\n",
                 "\n",
                 "cmomy is setup to work with arbitrary weights.  We saw this work above when we considered unequal sample sizes.  For example,"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 19,
             "id": "b2ed66e7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def get_cmom_with_weights(x, w, axis=0, mom=3):\n",
                 "    \"\"\"Create central moments using stable method\"\"\"\n",
                 "    # output shape\n",
@@ -2400,15 +2400,15 @@
                 "    ).sum(axis=axis) * w_norm\n",
                 "\n",
                 "    return output"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 20,
             "id": "48a3fab7",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -2770,22 +2770,22 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([5.1503e+01, 4.9029e-01, 9.1092e-02, 5.3542e-09])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-c121a44f-59fb-437a-9a77-b17f2ea72d1a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-c121a44f-59fb-437a-9a77-b17f2ea72d1a' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-c27554c1-6a75-44a1-b845-47fe94469fb5' class='xr-array-in' type='checkbox' checked><label for='section-c27554c1-6a75-44a1-b845-47fe94469fb5' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>51.5 0.4903 0.09109 5.354e-09</span></div><div class='xr-array-data'><pre>array([5.150285e+01, 4.902857e-01, 9.109218e-02, 5.354191e-09])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([ 5.1337e+01,  5.4415e-01,  8.9238e-02, -6.9704e-03])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-ea34017f-fe34-4af9-a7ab-025ce68811b6' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ea34017f-fe34-4af9-a7ab-025ce68811b6' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-b8ed3002-fbcb-432c-b633-98892204a056' class='xr-array-in' type='checkbox' checked><label for='section-b8ed3002-fbcb-432c-b633-98892204a056' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>51.34 0.5442 0.08924 -0.00697</span></div><div class='xr-array-data'><pre>array([ 5.133746e+01,  5.441544e-01,  8.923830e-02, -6.970374e-03])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(3,))>\n",
-                            "array([5.1503e+01, 4.9029e-01, 9.1092e-02, 5.3542e-09])"
+                            "array([ 5.1337e+01,  5.4415e-01,  8.9238e-02, -6.9704e-03])"
                         ]
                     },
-                    "execution_count": 32,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "x = np.random.rand(100)\n",
                 "w = np.random.rand(100)\n",
@@ -2805,15 +2805,15 @@
                 "\n",
                 "cmomy can also handle comoments (covariance, etc), like the $\\ave{(\\delta x)^i (\\delta y)^j}$    \n",
                 "For example"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 22,
             "id": "88bf86b5",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -3175,28 +3175,28 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([[ 5.1503e+01,  4.7448e-01,  9.8409e-02],\n",
-                            "       [ 4.9029e-01,  2.3666e-02, -1.1773e-03],\n",
-                            "       [ 9.1092e-02,  1.0251e-04,  9.1080e-03]])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: (2, 2)</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-e63a1a0b-5345-4f82-b354-20e44d432b98' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-e63a1a0b-5345-4f82-b354-20e44d432b98' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-4fc2dc8b-9ad4-4d00-954c-d70c12ffa4e0' class='xr-array-in' type='checkbox' checked><label for='section-4fc2dc8b-9ad4-4d00-954c-d70c12ffa4e0' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>51.5 0.4745 0.09841 0.4903 ... -0.001177 0.09109 0.0001025 0.009108</span></div><div class='xr-array-data'><pre>array([[ 5.150285e+01,  4.744806e-01,  9.840866e-02],\n",
-                            "       [ 4.902857e-01,  2.366622e-02, -1.177349e-03],\n",
-                            "       [ 9.109218e-02,  1.025148e-04,  9.108013e-03]])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([[ 5.1337e+01,  5.3346e-01,  8.4150e-02],\n",
+                            "       [ 5.4415e-01, -8.0426e-03,  3.0820e-03],\n",
+                            "       [ 8.9238e-02, -8.2899e-04,  6.8269e-03]])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: (2, 2)</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-855eab1d-2dcd-4bff-82af-76cd059cb75a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-855eab1d-2dcd-4bff-82af-76cd059cb75a' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-d4979081-73a4-4223-ae33-58e48e932a90' class='xr-array-in' type='checkbox' checked><label for='section-d4979081-73a4-4223-ae33-58e48e932a90' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>51.34 0.5335 0.08415 0.5442 ... 0.003082 0.08924 -0.000829 0.006827</span></div><div class='xr-array-data'><pre>array([[ 5.133746e+01,  5.334590e-01,  8.414989e-02],\n",
+                            "       [ 5.441544e-01, -8.042619e-03,  3.081975e-03],\n",
+                            "       [ 8.923830e-02, -8.289860e-04,  6.826899e-03]])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(2, 2))>\n",
-                            "array([[ 5.1503e+01,  4.7448e-01,  9.8409e-02],\n",
-                            "       [ 4.9029e-01,  2.3666e-02, -1.1773e-03],\n",
-                            "       [ 9.1092e-02,  1.0251e-04,  9.1080e-03]])"
+                            "array([[ 5.1337e+01,  5.3346e-01,  8.4150e-02],\n",
+                            "       [ 5.4415e-01, -8.0426e-03,  3.0820e-03],\n",
+                            "       [ 8.9238e-02, -8.2899e-04,  6.8269e-03]])"
                         ]
                     },
-                    "execution_count": 33,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "y = np.random.rand(100)\n",
                 "\n",
@@ -3219,15 +3219,15 @@
                 "## xarray DataArray support\n",
                 "\n",
                 "cmomy also works with {class}`xarray.DataArray` objects.  For example"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 23,
             "id": "cc5e273d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -3590,45 +3590,45 @@
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (rec: 3, a: 2, b: 3)&gt;\n",
-                            "array([[[0.8115, 0.4761, 0.5232],\n",
-                            "        [0.2505, 0.605 , 0.3029]],\n",
+                            "array([[[0.8257, 0.7468, 0.5123],\n",
+                            "        [0.458 , 0.5494, 0.7046]],\n",
                             "\n",
-                            "       [[0.5773, 0.1697, 0.1595],\n",
-                            "        [0.417 , 0.4268, 0.2681]],\n",
+                            "       [[0.9229, 0.617 , 0.8878],\n",
+                            "        [0.7013, 0.0683, 0.5008]],\n",
                             "\n",
-                            "       [[0.1316, 0.0392, 0.0252],\n",
-                            "        [0.2716, 0.4619, 0.7262]]])\n",
-                            "Dimensions without coordinates: rec, a, b</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rec</span>: 3</li><li><span>a</span>: 2</li><li><span>b</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-67189007-b62b-48c2-9346-92b6524a177c' class='xr-array-in' type='checkbox' checked><label for='section-67189007-b62b-48c2-9346-92b6524a177c' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>0.8115 0.4761 0.5232 0.2505 0.605 ... 0.02523 0.2716 0.4619 0.7262</span></div><div class='xr-array-data'><pre>array([[[0.8115, 0.4761, 0.5232],\n",
-                            "        [0.2505, 0.605 , 0.3029]],\n",
+                            "       [[0.2865, 0.2852, 0.3559],\n",
+                            "        [0.3147, 0.5786, 0.6836]]])\n",
+                            "Dimensions without coordinates: rec, a, b</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rec</span>: 3</li><li><span>a</span>: 2</li><li><span>b</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-995e5b75-9260-4de3-b352-70f7917ff811' class='xr-array-in' type='checkbox' checked><label for='section-995e5b75-9260-4de3-b352-70f7917ff811' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>0.8257 0.7468 0.5123 0.458 0.5494 ... 0.3559 0.3147 0.5786 0.6836</span></div><div class='xr-array-data'><pre>array([[[0.8257, 0.7468, 0.5123],\n",
+                            "        [0.458 , 0.5494, 0.7046]],\n",
                             "\n",
-                            "       [[0.5773, 0.1697, 0.1595],\n",
-                            "        [0.417 , 0.4268, 0.2681]],\n",
+                            "       [[0.9229, 0.617 , 0.8878],\n",
+                            "        [0.7013, 0.0683, 0.5008]],\n",
                             "\n",
-                            "       [[0.1316, 0.0392, 0.0252],\n",
-                            "        [0.2716, 0.4619, 0.7262]]])</pre></div></div></li><li class='xr-section-item'><input id='section-f390945f-8166-4ddc-9701-233683252642' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-f390945f-8166-4ddc-9701-233683252642' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-ac861439-d4d0-4267-a906-ece0ba7e1eb9' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ac861439-d4d0-4267-a906-ece0ba7e1eb9' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-eb9bbbbc-0b4c-47ff-9c83-bb62d53251dc' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-eb9bbbbc-0b4c-47ff-9c83-bb62d53251dc' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "       [[0.2865, 0.2852, 0.3559],\n",
+                            "        [0.3147, 0.5786, 0.6836]]])</pre></div></div></li><li class='xr-section-item'><input id='section-ab659195-7680-4e7d-9bf5-1a4fe8888f6a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ab659195-7680-4e7d-9bf5-1a4fe8888f6a' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-9568ba27-c22b-4346-86f7-43ac3a39ea75' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-9568ba27-c22b-4346-86f7-43ac3a39ea75' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-84d6b7d4-2d22-4470-aa12-2b29fb407116' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-84d6b7d4-2d22-4470-aa12-2b29fb407116' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.DataArray (rec: 3, a: 2, b: 3)>\n",
-                            "array([[[0.8115, 0.4761, 0.5232],\n",
-                            "        [0.2505, 0.605 , 0.3029]],\n",
+                            "array([[[0.8257, 0.7468, 0.5123],\n",
+                            "        [0.458 , 0.5494, 0.7046]],\n",
                             "\n",
-                            "       [[0.5773, 0.1697, 0.1595],\n",
-                            "        [0.417 , 0.4268, 0.2681]],\n",
+                            "       [[0.9229, 0.617 , 0.8878],\n",
+                            "        [0.7013, 0.0683, 0.5008]],\n",
                             "\n",
-                            "       [[0.1316, 0.0392, 0.0252],\n",
-                            "        [0.2716, 0.4619, 0.7262]]])\n",
+                            "       [[0.2865, 0.2852, 0.3559],\n",
+                            "        [0.3147, 0.5786, 0.6836]]])\n",
                             "Dimensions without coordinates: rec, a, b"
                         ]
                     },
-                    "execution_count": 34,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import xarray as xr\n",
                 "\n",
@@ -3642,15 +3642,15 @@
             "metadata": {},
             "source": [
                 "To create a cmomy object wrapping a {class}`xarray.DataArray`, use {class}`~cmomy.xCentralMoments`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 24,
             "id": "38a244b6",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -4013,22 +4013,22 @@
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (a: 2, b: 3, mom_0: 4)&gt;\n",
-                            "array([[[ 1.0000e+02,  5.4290e-01,  7.7797e-02, -8.3022e-03],\n",
-                            "        [ 1.0000e+02,  5.0585e-01,  9.4957e-02,  7.6531e-04],\n",
-                            "        [ 1.0000e+02,  4.5853e-01,  8.5859e-02,  6.1346e-03]],\n",
-                            "\n",
-                            "       [[ 1.0000e+02,  5.0983e-01,  7.7844e-02,  2.2635e-03],\n",
-                            "        [ 1.0000e+02,  5.2817e-01,  8.4799e-02,  5.6189e-04],\n",
-                            "        [ 1.0000e+02,  4.8895e-01,  6.4305e-02, -1.0829e-04]]])\n",
-                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: (2, 3)</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-02121d9e-9620-4f6f-8185-5f43310a3f93' class='xr-section-summary-in' type='checkbox'  checked><label for='section-02121d9e-9620-4f6f-8185-5f43310a3f93' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>(a, b)</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
+                            "array([[[ 1.0000e+02,  4.6429e-01,  8.9723e-02,  4.5381e-03],\n",
+                            "        [ 1.0000e+02,  5.0233e-01,  8.0919e-02,  3.1135e-03],\n",
+                            "        [ 1.0000e+02,  5.2084e-01,  8.6462e-02, -1.6221e-03]],\n",
+                            "\n",
+                            "       [[ 1.0000e+02,  4.9178e-01,  6.4268e-02, -2.2615e-04],\n",
+                            "        [ 1.0000e+02,  5.0930e-01,  8.1505e-02, -4.6409e-03],\n",
+                            "        [ 1.0000e+02,  5.0885e-01,  9.2137e-02, -1.6572e-03]]])\n",
+                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: (2, 3)</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-40dedf1d-f740-4b71-8aa8-3ef78ce5037d' class='xr-section-summary-in' type='checkbox'  checked><label for='section-40dedf1d-f740-4b71-8aa8-3ef78ce5037d' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>(a, b)</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
                             "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
                             "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "</symbol>\n",
                             "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
@@ -4384,43 +4384,43 @@
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (a: 2, b: 3, mom_0: 4)&gt;\n",
-                            "array([[[ 1.0000e+02,  5.4290e-01,  7.7797e-02, -8.3022e-03],\n",
-                            "        [ 1.0000e+02,  5.0585e-01,  9.4957e-02,  7.6531e-04],\n",
-                            "        [ 1.0000e+02,  4.5853e-01,  8.5859e-02,  6.1346e-03]],\n",
-                            "\n",
-                            "       [[ 1.0000e+02,  5.0983e-01,  7.7844e-02,  2.2635e-03],\n",
-                            "        [ 1.0000e+02,  5.2817e-01,  8.4799e-02,  5.6189e-04],\n",
-                            "        [ 1.0000e+02,  4.8895e-01,  6.4305e-02, -1.0829e-04]]])\n",
-                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>a</span>: 2</li><li><span>b</span>: 3</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-c6c44a6f-53ba-490c-867d-1f8115fbe730' class='xr-array-in' type='checkbox' checked><label for='section-c6c44a6f-53ba-490c-867d-1f8115fbe730' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>100.0 0.5429 0.0778 -0.008302 ... 100.0 0.4889 0.06431 -0.0001083</span></div><div class='xr-array-data'><pre>array([[[ 1.0000e+02,  5.4290e-01,  7.7797e-02, -8.3022e-03],\n",
-                            "        [ 1.0000e+02,  5.0585e-01,  9.4957e-02,  7.6531e-04],\n",
-                            "        [ 1.0000e+02,  4.5853e-01,  8.5859e-02,  6.1346e-03]],\n",
-                            "\n",
-                            "       [[ 1.0000e+02,  5.0983e-01,  7.7844e-02,  2.2635e-03],\n",
-                            "        [ 1.0000e+02,  5.2817e-01,  8.4799e-02,  5.6189e-04],\n",
-                            "        [ 1.0000e+02,  4.8895e-01,  6.4305e-02, -1.0829e-04]]])</pre></div></div></li><li class='xr-section-item'><input id='section-1df705fa-ff6a-4128-9e62-26988df23d6e' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1df705fa-ff6a-4128-9e62-26988df23d6e' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-1861d6c1-cd0e-4c88-9c46-154b6aaa7e75' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1861d6c1-cd0e-4c88-9c46-154b6aaa7e75' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-572c7fe3-4d3b-4788-aa96-10ddb87b093a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-572c7fe3-4d3b-4788-aa96-10ddb87b093a' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "array([[[ 1.0000e+02,  4.6429e-01,  8.9723e-02,  4.5381e-03],\n",
+                            "        [ 1.0000e+02,  5.0233e-01,  8.0919e-02,  3.1135e-03],\n",
+                            "        [ 1.0000e+02,  5.2084e-01,  8.6462e-02, -1.6221e-03]],\n",
+                            "\n",
+                            "       [[ 1.0000e+02,  4.9178e-01,  6.4268e-02, -2.2615e-04],\n",
+                            "        [ 1.0000e+02,  5.0930e-01,  8.1505e-02, -4.6409e-03],\n",
+                            "        [ 1.0000e+02,  5.0885e-01,  9.2137e-02, -1.6572e-03]]])\n",
+                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>a</span>: 2</li><li><span>b</span>: 3</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-40560fd9-580a-47df-9ca0-250337a8a9e3' class='xr-array-in' type='checkbox' checked><label for='section-40560fd9-580a-47df-9ca0-250337a8a9e3' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>100.0 0.4643 0.08972 0.004538 100.0 ... 100.0 0.5089 0.09214 -0.001657</span></div><div class='xr-array-data'><pre>array([[[ 1.0000e+02,  4.6429e-01,  8.9723e-02,  4.5381e-03],\n",
+                            "        [ 1.0000e+02,  5.0233e-01,  8.0919e-02,  3.1135e-03],\n",
+                            "        [ 1.0000e+02,  5.2084e-01,  8.6462e-02, -1.6221e-03]],\n",
+                            "\n",
+                            "       [[ 1.0000e+02,  4.9178e-01,  6.4268e-02, -2.2615e-04],\n",
+                            "        [ 1.0000e+02,  5.0930e-01,  8.1505e-02, -4.6409e-03],\n",
+                            "        [ 1.0000e+02,  5.0885e-01,  9.2137e-02, -1.6572e-03]]])</pre></div></div></li><li class='xr-section-item'><input id='section-68044e2b-2e3c-4a6f-8bee-2fb27df11a3a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-68044e2b-2e3c-4a6f-8bee-2fb27df11a3a' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-e4c77ac9-16cb-4bca-b9d5-e44460fea2a6' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-e4c77ac9-16cb-4bca-b9d5-e44460fea2a6' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-d70728cf-e253-40f6-b5e2-191d8df923a3' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-d70728cf-e253-40f6-b5e2-191d8df923a3' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xCentralMoments(val_shape=(2, 3), mom=(3,))>\n",
                             "<xarray.DataArray (a: 2, b: 3, mom_0: 4)>\n",
-                            "array([[[ 1.0000e+02,  5.4290e-01,  7.7797e-02, -8.3022e-03],\n",
-                            "        [ 1.0000e+02,  5.0585e-01,  9.4957e-02,  7.6531e-04],\n",
-                            "        [ 1.0000e+02,  4.5853e-01,  8.5859e-02,  6.1346e-03]],\n",
-                            "\n",
-                            "       [[ 1.0000e+02,  5.0983e-01,  7.7844e-02,  2.2635e-03],\n",
-                            "        [ 1.0000e+02,  5.2817e-01,  8.4799e-02,  5.6189e-04],\n",
-                            "        [ 1.0000e+02,  4.8895e-01,  6.4305e-02, -1.0829e-04]]])\n",
+                            "array([[[ 1.0000e+02,  4.6429e-01,  8.9723e-02,  4.5381e-03],\n",
+                            "        [ 1.0000e+02,  5.0233e-01,  8.0919e-02,  3.1135e-03],\n",
+                            "        [ 1.0000e+02,  5.2084e-01,  8.6462e-02, -1.6221e-03]],\n",
+                            "\n",
+                            "       [[ 1.0000e+02,  4.9178e-01,  6.4268e-02, -2.2615e-04],\n",
+                            "        [ 1.0000e+02,  5.0930e-01,  8.1505e-02, -4.6409e-03],\n",
+                            "        [ 1.0000e+02,  5.0885e-01,  9.2137e-02, -1.6572e-03]]])\n",
                             "Dimensions without coordinates: a, b, mom_0"
                         ]
                     },
-                    "execution_count": 35,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "c = cmomy.xCentralMoments.from_vals(x, dim=\"rec\", mom=3)\n",
                 "c"
@@ -4434,29 +4434,29 @@
                 "Everything that {class}`~cmomy.CentralMoments` can do, {class}`~cmomy.xCentralMoments` can do."
             ]
         }
     ],
     "metadata": {
         "celltoolbar": "Tags",
         "kernelspec": {
-            "display_name": "Python [conda env:cmomy-env]",
+            "display_name": "cmomy-dev [conda env:dev-3]",
             "language": "python",
-            "name": "conda-env-cmomy-env-py"
+            "name": "conda-env-dev-3-py"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.10.11"
         },
         "toc": {
             "base_numbering": 1,
             "nav_menu": {},
             "number_sections": true,
             "sideBar": true,
             "skip_h1_title": false,
```

### Comparing `cmomy-0.5.0/examples/usage/usage_notebook.ipynb` & `cmomy-0.6.0/examples/usage/usage_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/noxfile.py` & `cmomy-0.6.0/noxfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,78 @@
 """Config file for nox"""
 from __future__ import annotations
 
 import shutil
 from dataclasses import replace  # noqa
 from pathlib import Path
 from textwrap import dedent
-from typing import Annotated, Any, Callable, Collection, Literal, TypeVar, cast
+from typing import Annotated, Any, Callable, Collection, TypeVar, cast
 
 import nox
 from noxopt import NoxOpt, Option, Session
 
 from tools.noxtools import (
     combine_list_str,
+    load_nox_config,
+    open_webpage,
     prepend_flag,
     session_install_envs,
     session_install_envs_lock,
     # session_install_package,
     session_install_pip,
     session_run_commands,
-    # session_skip_install,
     sort_like,
     update_target,
 )
 
-# --- nox options ----------------------------------------------------------------------
+# * nox options ------------------------------------------------------------------------
 ROOT = Path(__file__).parent
 
 nox.options.reuse_existing_virtualenvs = True
 nox.options.sessions = ["test"]
 
-# --- Options --------------------------------------------------------------------------
+# * Options ----------------------------------------------------------------------------
 
 PACKAGE_NAME = "cmomy"
 IMPORT_NAME = "cmomy"
 KERNEL_BASE = "cmomy"
 
 PYTHON_ALL_VERSIONS = ["3.8", "3.9", "3.10", "3.11"]
 PYTHON_DEFAULT_VERSION = "3.10"
 
 # conda/mamba
 if shutil.which("mamba"):
     CONDA_BACKEND = "mamba"
 elif shutil.which("conda"):
     CONDA_BACKEND = "conda"
 else:
-    raise ValueError("neigher conda or mamba found")
+    raise ValueError("neither conda or mamba found")
 
 SESSION_DEFAULT_KWS = {"python": PYTHON_DEFAULT_VERSION, "venv_backend": CONDA_BACKEND}
 SESSION_ALL_KWS = {"python": PYTHON_ALL_VERSIONS, "venv_backend": CONDA_BACKEND}
 
 
-# --- Set PATH to find all python versions ---------------------------------------------
+# * User config ------------------------------------------------------------------------
 
-DEFAULTS: dict[str, Any] = {}
+CONFIG = load_nox_config()
 
-
-def load_nox_config():
-    path = Path(".") / ".noxconfig.toml"
-    if not path.exists():
-        return
-
-    import os
-    from glob import glob
-
-    import tomli
-
-    with path.open("rb") as f:
-        data = tomli.load(f)
-
-    # python paths
-    try:
-        paths = []
-        for p in data["nox"]["python"]["paths"]:
-            paths.extend(glob(os.path.expanduser(p)))
-
-        paths = ":".join(map(str, paths))
-        os.environ["PATH"] = paths + ":" + os.environ["PATH"]
-    except KeyError:
-        pass
-
-    # extras:
-    extras = {"dev": ["nox", "dev"]}
-    try:
-        for k, v in data["nox"]["extras"].items():
-            extras[k] = v
-    except KeyError:
-        pass
-
-    DEFAULTS["environment-extras"] = extras
-
-    # for py in PYTHON_ALL_VERSIONS:
-    #     print(f"which python{py}", shutil.which(f"python{py}"))
-
-    return
-
-
-load_nox_config()
-
-
-# --- noxopt ---------------------------------------------------------------------------
+# * noxopt -----------------------------------------------------------------------------
 group = NoxOpt(auto_tag=True)
 
 F = TypeVar("F", bound=Callable[..., Any])
+C = Callable[[F], F]
+
+DEFAULT_SESSION = cast(C, group.session(**SESSION_DEFAULT_KWS))  # type: ignore
+ALL_SESSION = cast(C, group.session(**SESSION_ALL_KWS))  # type: ignore
 
-DEFAULT_SESSION = cast(Callable[[F], F], group.session(**SESSION_DEFAULT_KWS))  # type: ignore
-ALL_SESSION = cast(Callable[[F], F], group.session(**SESSION_ALL_KWS))  # type: ignore
+DEFAULT_SESSION_VENV = cast(C, group.session(python=PYTHON_DEFAULT_VERSION))  # type: ignore
+ALL_SESSION_VENV = cast(C, group.session(python=PYTHON_ALL_VERSIONS))  # type: ignore
 
 OPTS_OPT = Option(nargs="*", type=str)
-SET_KERNEL_OPT = Option(type=bool, help="If True, try to set the kernel name")
+# SET_KERNEL_OPT = Option(type=bool, help="If True, try to set the kernel name")
 RUN_OPT = Option(
     nargs="*",
     type=str,
     action="append",
     help="run passed command_demo using `external=True` flag",
 )
 
@@ -135,90 +96,106 @@
 RUN_CLI = Annotated[list[list[str]], RUN_OPT]
 TEST_OPTS_CLI = opts_annotated(help="extra arguments/flags to pytest")
 
 # CMD_CLI = Annotated[list[str], CMD_OPT]
 
 FORCE_REINSTALL_CLI = Annotated[
     bool,
-    Option(type=bool, help="If True, force reinstall even if environment unchanged"),
+    Option(
+        type=bool,
+        help="If True, force reinstall requirements and package even if environment unchanged",
+    ),
 ]
 
 VERSION_CLI = Annotated[
     str, Option(type=str, help="Version to substitute or check against")
 ]
 
 LOG_SESSION_CLI = Annotated[
     bool,
     Option(
         type=bool,
         help="If flag included, log python and package (if installed) version",
     ),
 ]
 
-# --- installer ------------------------------------------------------------------------
-
 
-def install_requirements(
+# * Installation command ---------------------------------------------------------------
+def pkg_install_condaenv(
     session: nox.Session,
     name: str,
-    style: Literal["conda", "conda-lock", "pip"] | None = None,
     lock: bool = False,
     display_name: str | None = None,
-    set_kernel: bool = True,
     install_package: bool = True,
     force_reinstall: bool = False,
     log_session: bool = False,
     deps: Collection[str] | None = None,
     reqs: Collection[str] | None = None,
-    extras: str | Collection[str] | None = None,
     channels: Collection[str] | None = None,
     **kwargs,
 ):
     """Install requirements.  If need fine control, do it in calling func"""
 
-    if display_name is None and set_kernel:
-        display_name = f"{KERNEL_BASE}-{name}"
-
-    style = style or ("conda-lock" if lock else "conda")
-
-    if style == "pip":
-        session_install_pip(
-            session=session,
-            extras=extras,
-            display_name=display_name,
-            force_reinstall=force_reinstall,
-            reqs=reqs,
-            install_package=install_package,
-            **kwargs,
-        )
-
-    elif style == "conda-lock":
+    if lock:
         py = session.python.replace(".", "")  # type: ignore
         session_install_envs_lock(
             session=session,
             lockfile=f"./environment/lock/py{py}-{name}-conda-lock.yml",
             display_name=display_name,
             force_reinstall=force_reinstall,
-            install_package=install_package**kwargs,
+            install_package=install_package,
+            **kwargs,
         )
 
-    elif style == "conda":
+    else:
         session_install_envs(
             session,
             f"./environment/{name}.yaml",
             display_name=display_name,
             force_reinstall=force_reinstall,
             deps=deps,
             reqs=reqs,
             channels=channels,
             install_package=install_package,
             **kwargs,
         )
+
+    if log_session:
+        session_log_session(session, install_package)
+
+
+def pkg_install_venv(
+    session: nox.Session,
+    name: str,
+    lock: bool = False,
+    requirement_paths: Collection[str] | None = None,
+    constraint_paths: Collection[str] | None = None,
+    extras: str | Collection[str] | None = None,
+    reqs: Collection[str] | None = None,
+    display_name: str | None = None,
+    force_reinstall: bool = False,
+    install_package: bool = False,
+    no_deps: bool = False,
+    log_session: bool = False,
+):
+    if lock:
+        raise ValueError("lock not yet supported for install_pip")
+
     else:
-        raise ValueError(f"style={style} not recognized")
+        session_install_pip(
+            session=session,
+            requirement_paths=requirement_paths,
+            constraint_paths=constraint_paths,
+            extras=extras,
+            reqs=reqs,
+            display_name=display_name,
+            force_reinstall=force_reinstall,
+            install_package=install_package,
+            no_deps=no_deps,
+        )
 
     if log_session:
         session_log_session(session, install_package)
 
 
 def session_log_session(session, has_package=False):
     session.run("python", "--version")
@@ -231,108 +208,144 @@
         import {IMPORT_NAME}
         print({IMPORT_NAME}.__version__)
         """
             ),
         )
 
 
+# * Environments------------------------------------------------------------------------
+# ** Development (conda)
 @DEFAULT_SESSION
 def dev(
     session: Session,
-    # set_kernel: SET_KERNEL_CLI = True,
     dev_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
 ):
     """Create dev env"""
     # using conda
 
-    install_requirements(
+    pkg_install_condaenv(
         session=session,
         name="dev",
         lock=lock,
-        set_kernel=True,
+        display_name=f"{PACKAGE_NAME}-dev",
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
     session_run_commands(session, dev_run)
 
 
-@group.session(python=PYTHON_DEFAULT_VERSION)
+@DEFAULT_SESSION_VENV
+def dev_venv(
+    session: Session,
+    dev_run: RUN_CLI = [],  # noqa
+    lock: LOCK_CLI = False,
+    force_reinstall: FORCE_REINSTALL_CLI = False,
+    log_session: bool = False,
+):
+    """Create dev env"""
+    # using conda
+
+    pkg_install_venv(
+        session=session,
+        name="dev-venv",
+        lock=lock,
+        extras=["dev"],
+        display_name=f"{PACKAGE_NAME}-dev-venv",
+        install_package=True,
+        force_reinstall=force_reinstall,
+        log_session=log_session,
+    )
+    session_run_commands(session, dev_run)
+
+
+# ** pyproject2conda (create environment.yaml and requirement.txt files)
+@DEFAULT_SESSION_VENV
 def pyproject2conda(
     session: Session,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     pyproject2conda_force: bool = False,
 ):
     """Create environment.yaml files from pyproject.toml using pyproject2conda."""
-    session_install_envs(
-        session,
+    pkg_install_venv(
+        session=session,
+        name="pyporject2conda",
         reqs=["pyproject2conda>=0.4.0"],
         force_reinstall=force_reinstall,
     )
 
-    def create_env(output, extras=None, python="get", base=True):
+    def create_env(output, extras=None, python="get", base=True, cmd="yaml"):
         def _to_args(flag, val):
             if val is None:
                 return []
             if isinstance(val, str):
                 val = [val]
             return prepend_flag(flag, val)
 
         if pyproject2conda_force or update_target(output, "pyproject.toml"):
-            args = ["yaml", "-o", output] + _to_args("-e", extras)
+            args = [cmd, "-o", output] + _to_args("-e", extras)
 
-            if python:
+            if python and cmd == "yaml":
                 args.extend(["--python-include", python])
 
             if not base:
                 args.append("--no-base")
 
             session.run("pyproject2conda", *args)
         else:
             session.log(
                 f"{output} up to data.  Pass --pyproject2conda-force to force recreation"
             )
 
     # create root environment
     create_env("environment/base.yaml")
 
-    extras = DEFAULTS["environment-extras"]
+    extras = CONFIG["environment-extras"]
     for k in ["test", "typing", "docs", "dev"]:
         create_env(f"environment/{k}.yaml", extras=extras.get(k, k), base=True)
 
     # isolated
     for k in ["dist-pypi", "dist-conda"]:
         create_env(f"environment/{k}.yaml", extras=k, base=False)
+        if k == "dist-pypi":
+            create_env(f"environment/{k}.txt", extras=k, base=False, cmd="requirements")
 
+    # need an isolated set of test requirements
+    create_env("environment/test-extras.yaml", extras="test", base=False)
+    create_env(
+        "environment/test-extras.txt", extras="test", base=False, cmd="requirements"
+    )
 
-@DEFAULT_SESSION
+
+# ** conda-lock
+@DEFAULT_SESSION_VENV
 def conda_lock(
     session: Session,
     force_reinstall: FORCE_REINSTALL_CLI = False,
-    conda_lock_channel: cmd_annotated(help="conda channels to use") = (),
-    conda_lock_platform: cmd_annotated(
+    conda_lock_channel: cmd_annotated(help="conda channels to use") = (),  # type: ignore
+    conda_lock_platform: cmd_annotated(  # type: ignore
         help="platforms to build lock files for",
         choices=["osx-64", "linux-64", "win-64", "all"],
     ) = (),
-    conda_lock_cmd: cmd_annotated(
+    conda_lock_cmd: cmd_annotated(  # type: ignore
         help="lock files to create",
         choices=["test", "typing", "dev", "dist-pypi", "dist-conda", "all"],
     ) = (),
     conda_lock_run: RUN_CLI = [],  # noqa
     conda_lock_mamba: bool = False,
     conda_lock_force: bool = False,
 ):
     """Create lock files using conda-lock"""
 
-    session_install_envs(
+    pkg_install_venv(
         session,
-        # reqs=["git+https://github.com/conda/conda-lock.git"],
+        name="conda-lock",
         reqs=["conda-lock>=2.0.0"],
         force_reinstall=force_reinstall,
     )
 
     session.run("conda-lock", "--version")
 
     platform = conda_lock_platform
@@ -400,128 +413,166 @@
         elif c == "dist-conda":
             create_lock(
                 PYTHON_DEFAULT_VERSION,
                 "dist-conda",
             )
 
 
+# ** testing
+def _test(session, run, test_no_pytest, test_opts, no_cov):
+    session_run_commands(session, run)
+    if not test_no_pytest:
+        opts = combine_list_str(test_opts)
+        if not no_cov:
+            session.env["COVERAGE_FILE"] = str(Path(session.create_tmp()) / ".coverage")
+            if "--cov" not in opts:
+                opts.append("--cov")
+        session.run("pytest", *opts)
+
+
 @ALL_SESSION
 def test(
     session: Session,
     test_no_pytest: bool = False,
-    test_opts: TEST_OPTS_CLI = (),
+    test_opts: TEST_OPTS_CLI = (),  # type: ignore
     test_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
     no_cov: bool = False,
 ):
     """Test environments with conda installs"""
 
-    install_requirements(
+    pkg_install_condaenv(
         session=session,
         name="test",
         lock=lock,
-        set_kernel=False,
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
 
-    run = test_run
-    session_run_commands(session, run)
-
-    if not test_no_pytest:
-        opts = combine_list_str(test_opts)
-
-        if not no_cov:
-            session.env["COVERAGE_FILE"] = str(Path(session.create_tmp()) / ".coverage")
-            if "--cov" not in opts:
-                opts.append("--cov")
-        session.run("pytest", *opts)
+    _test(
+        session=session,
+        run=test_run,
+        test_no_pytest=test_no_pytest,
+        test_opts=test_opts,
+        no_cov=no_cov,
+    )
 
 
-@group.session(python=PYTHON_ALL_VERSIONS)
-def test_pip(
+@ALL_SESSION_VENV
+def test_venv(
     session: Session,
     test_no_pytest: bool = False,
-    test_opts: TEST_OPTS_CLI = (),
+    test_opts: TEST_OPTS_CLI = (),  # type: ignore
     test_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
     no_cov: bool = False,
 ):
     """Test environments virtualenv and pip installs"""
 
-    install_requirements(
+    pkg_install_venv(
         session=session,
         name="test-pip",
         extras="test",
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
-        style="pip",
     )
 
-    run = test_run
+    _test(
+        session=session,
+        run=test_run,
+        test_no_pytest=test_no_pytest,
+        test_opts=test_opts,
+        no_cov=no_cov,
+    )
+
+
+# ** coverage
+def _coverage(session, run, cmd, run_internal):
     session_run_commands(session, run)
 
-    if not test_no_pytest:
-        opts = combine_list_str(test_opts)
+    if not cmd and not run and not run_internal:
+        cmd = ["combine", "report"]
 
-        if not no_cov:
-            session.env["COVERAGE_FILE"] = str(Path(session.create_tmp()) / ".coverage")
-            if "--cov" not in opts:
-                opts.append("--cov")
-        session.run("pytest", *opts)
+    session.log(f"{cmd}")
+
+    for c in cmd:
+        if c == "combine":
+            paths = list(Path(".nox").glob("test*/tmp/.coverage"))
+            if update_target(".coverage", *paths):
+                session.run("coverage", "combine", "--keep", "-a", *map(str, paths))
+        elif c == "open":
+            open_webpage(path="htmlcov/index.html")
+        else:
+            session.run("coverage", c)
 
+    session_run_commands(session, run_internal, external=False)
 
-@group.session(python=PYTHON_DEFAULT_VERSION)
+
+@DEFAULT_SESSION_VENV
 def coverage(
     session: Session,
-    coverage_cmd: cmd_annotated(
+    coverage_cmd: cmd_annotated(  # type: ignore
         choices=["erase", "combine", "report", "html", "open"]
     ) = (),
     coverage_run: RUN_CLI = [],  # noqa
-    coverage_run_internal: run_annotated(
+    coverage_run_internal: run_annotated(  # type: ignore
         help="Arbitrary commands to run within the session"
     ) = [],  # noqa
     force_reinstall: FORCE_REINSTALL_CLI = False,
 ):
-    session_install_envs(
+    pkg_install_venv(
         session,
+        name="coverage",
         reqs=["coverage[toml]"],
         force_reinstall=force_reinstall,
     )
-    session_run_commands(session, coverage_run)
 
-    if not coverage_cmd and not coverage_run and not coverage_run_internal:
-        coverage_cmd = ["combine", "report"]
+    _coverage(
+        session=session,
+        run=coverage_run,
+        cmd=coverage_cmd,
+        run_internal=coverage_run_internal,
+    )
 
-    session.log(f"{coverage_cmd}")
 
-    for cmd in coverage_cmd:
-        if cmd == "combine":
-            paths = list(Path(".nox").glob("test*/tmp/.coverage"))
-            if update_target(".coverage", *paths):
-                session.run("coverage", "combine", "--keep", "-a", *map(str, paths))
-        elif cmd == "open":
-            _open_webpage(path="htmlcov/index.html")
+# ** Docs
+def _docs(session, run, cmd, version):
+    if version:
+        session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = version
 
-        else:
-            session.run("coverage", cmd)
+    session_run_commands(session, run)
+
+    if not run and not cmd:
+        cmd = ["html"]
+
+    if "symlink" in cmd:
+        cmd.remove("symlink")
+        _create_doc_examples_symlinks(session)
+
+    if open_page := "open" in cmd:
+        cmd.remove("open")
 
-    session_run_commands(session, coverage_run_internal, external=False)
+    if cmd:
+        args = ["make", "-C", "docs"] + combine_list_str(cmd)
+        session.run(*args, external=True)
+
+    if open_page:
+        open_webpage(path="./docs/_build/html/index.html")
 
 
 @DEFAULT_SESSION
 def docs(
     session: nox.Session,
-    docs_cmd: cmd_annotated(
+    docs_cmd: cmd_annotated(  # type: ignore
         choices=[
             "html",
             "build",
             "symlink",
             "clean",
             "livehtml",
             "linkcheck",
@@ -535,87 +586,73 @@
     docs_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
     """Runs make in docs directory. For example, 'nox -s docs -- --docs-cmd html' -> 'make -C docs html'. With 'release' option, you can set the message with 'message=...' in posargs."""
-    install_requirements(
+    pkg_install_condaenv(
         session=session,
         name="docs",
         lock=lock,
-        set_kernel=True,
+        display_name=f"{PACKAGE_NAME}-docs",
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
 
-    if version:
-        session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = version
+    _docs(session=session, cmd=docs_cmd, run=docs_run, version=version)
 
-    cmd = docs_cmd
-    run = docs_run
-
-    session_run_commands(session, run)
 
-    if not run and not cmd:
-        cmd = ["html"]
-
-    if "symlink" in cmd:
-        cmd.remove("symlink")
-        _create_doc_examples_symlinks(session)
-
-    if open_page := "open" in cmd:
-        cmd.remove("open")
-
-    if cmd:
-        args = ["make", "-C", "docs"] + combine_list_str(cmd)
-        # if version:
-        #     args.append( f"SETUPTOOLS_SCM_PRETEND_VERSION={version}" )
-        session.run(*args, external=True)
-
-    if open_page:
-        _open_webpage(path="./docs/_build/html/index.html")
-
-
-@DEFAULT_SESSION
-def dist_pypi(
+@DEFAULT_SESSION_VENV
+def docs_venv(
     session: nox.Session,
-    dist_pypi_run: RUN_CLI = [],  # noqa
-    dist_pypi_cmd: cmd_annotated(
-        choices=["clean", "build", "testrelease", "release"],
-        flags=("--dist-pypi-cmd", "-p"),
+    docs_cmd: cmd_annotated(  # type: ignore
+        choices=[
+            "html",
+            "build",
+            "symlink",
+            "clean",
+            "livehtml",
+            "linkcheck",
+            "spelling",
+            "showlinks",
+            "release",
+            "open",
+        ],
+        flags=("--docs-cmd", "-d"),
     ) = (),
+    docs_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
-    """Run 'nox -s dist_pypi -- {clean, build, testrelease, release}'"""
-    # conda
-
-    install_requirements(
+    """Runs make in docs directory. For example, 'nox -s docs -- --docs-cmd html' -> 'make -C docs html'. With 'release' option, you can set the message with 'message=...' in posargs."""
+    pkg_install_venv(
         session=session,
-        name="dist-pypi",
-        set_kernel=False,
-        install_package=False,
+        name="docs-venv",
+        lock=lock,
+        display_name=f"{PACKAGE_NAME}-docs-venv",
+        install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
+        extras="docs",
     )
 
-    if version:
-        session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = version
+    _docs(session=session, cmd=docs_cmd, run=docs_run, version=version)
 
-    run, cmd = dist_pypi_run, dist_pypi_cmd
 
+# ** Dist pypi
+def _dist_pypi(session, run, cmd, version):
+    if version:
+        session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = version
     session_run_commands(session, run)
-
     if not run and not cmd:
         cmd = ["build"]
-
     if cmd:
         if "build" in cmd:
             cmd.append("clean")
         cmd = sort_like(cmd, ["clean", "build", "testrelease", "release"])
 
         session.log(f"cmd={cmd}")
 
@@ -628,32 +665,103 @@
             elif command == "testrelease":
                 session.run("twine", "upload", "--repository", "testpypi", "dist/*")
 
             elif command == "release":
                 session.run("twine", "upload", "dist/*")
 
 
+@DEFAULT_SESSION_VENV
+def dist_pypi(
+    session: nox.Session,
+    dist_pypi_run: RUN_CLI = [],  # noqa
+    dist_pypi_cmd: cmd_annotated(  # type: ignore
+        choices=["clean", "build", "testrelease", "release"],
+        flags=("--dist-pypi-cmd", "-p"),
+    ) = (),
+    lock: LOCK_CLI = False,
+    force_reinstall: FORCE_REINSTALL_CLI = False,
+    version: VERSION_CLI = "",
+    log_session: bool = False,
+):
+    """Run 'nox -s dist-pypi -- {clean, build, testrelease, release}'"""
+
+    pkg_install_venv(
+        session=session,
+        name="dist-pypi",
+        requirement_paths=["environment/dist-pypi.txt"],
+        force_reinstall=force_reinstall,
+        install_package=False,
+    )
+
+    _dist_pypi(
+        session=session,
+        run=dist_pypi_run,
+        cmd=dist_pypi_cmd,
+        version=version,
+    )
+
+
+@DEFAULT_SESSION
+def dist_pypi_condaenv(
+    session: nox.Session,
+    dist_pypi_run: RUN_CLI = [],  # noqa
+    dist_pypi_cmd: cmd_annotated(  # type: ignore
+        choices=["clean", "build", "testrelease", "release"],
+        flags=("--dist-pypi-cmd", "-p"),
+    ) = (),
+    lock: LOCK_CLI = False,
+    force_reinstall: FORCE_REINSTALL_CLI = False,
+    version: VERSION_CLI = "",
+    log_session: bool = False,
+):
+    """Run 'nox -s dist_pypi -- {clean, build, testrelease, release}'"""
+    # conda
+
+    pkg_install_condaenv(
+        session=session,
+        name="dist-pypi",
+        install_package=False,
+        force_reinstall=force_reinstall,
+        log_session=log_session,
+    )
+
+    _dist_pypi(
+        session=session,
+        run=dist_pypi_run,
+        cmd=dist_pypi_cmd,
+        version=version,
+    )
+
+
+# ** Dist conda
 @DEFAULT_SESSION
 def dist_conda(
     session: nox.Session,
     dist_conda_run: RUN_CLI = [],  # noqa
-    dist_conda_cmd: cmd_annotated(
-        choices=["recipe", "build", "clean", "clean-recipe", "clean-build"],
+    dist_conda_cmd: cmd_annotated(  # type: ignore
+        choices=[
+            "recipe",
+            "build",
+            "clean",
+            "clean-recipe",
+            "clean-build",
+            "recipe-cat-full",
+        ],
         flags=("--dist-conda-cmd", "-c"),
     ) = (),
-    lock: LOCK_CLI = False,
+    # lock: LOCK_CLI = False,
     sdist_path: str = "",
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
+    version: VERSION_CLI = "",
 ):
     """Runs make -C dist-conda posargs"""
-    install_requirements(
+    pkg_install_condaenv(
         session=session,
         name="dist-conda",
-        set_kernel=False,
         install_package=False,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
 
     run, cmd = dist_conda_run, dist_conda_cmd
     session_run_commands(session, run)
@@ -665,24 +773,29 @@
             cmd.append("clean-recipe")
         if "build" in cmd:
             cmd.append("clean-build")
         if "clean" in cmd:
             cmd.extend(["clean-recipe", "clean-build"])
             cmd.remove("clean")
 
-        cmd = sort_like(cmd, ["clean-recipe", "recipe", "clean-build", "build"])
+        cmd = sort_like(
+            cmd, ["recipe-cat-full", "clean-recipe", "recipe", "clean-build", "build"]
+        )
+
+        if not sdist_path:
+            sdist_path = PACKAGE_NAME
+            if version:
+                sdist_path = f"{sdist_path}=={version}"
 
         for command in cmd:
             if command == "clean-recipe":
                 session.run("rm", "-rf", f"dist-conda/{PACKAGE_NAME}", external=True)
             elif command == "clean-build":
                 session.run("rm", "-rf", "dist-conda/build", external=True)
             elif command == "recipe":
-                if sdist_path is None:
-                    sdist_path = PACKAGE_NAME
                 session.run(
                     "grayskull",
                     "pypi",
                     sdist_path,
                     "--sections",
                     "package",
                     "source",
@@ -693,14 +806,28 @@
                 )
                 _append_recipe(
                     f"dist-conda/{PACKAGE_NAME}/meta.yaml", ".recipe-append.yaml"
                 )
                 session.run(
                     "cat", f"dist-conda/{PACKAGE_NAME}/meta.yaml", external=True
                 )
+            elif command == "recipe-cat-full":
+                import tempfile
+
+                with tempfile.TemporaryDirectory() as d:
+                    session.run(
+                        "grayskull",
+                        "pypi",
+                        sdist_path,
+                        "-o",
+                        d,
+                    )
+                    session.run(
+                        "cat", str(Path(d) / PACKAGE_NAME / "meta.yaml"), external=True
+                    )
 
             elif command == "build":
                 session.run(
                     "conda",
                     "mambabuild",
                     "--output-folder=dist-conda/build",
                     "--no-anaconda-upload",
@@ -715,64 +842,104 @@
     with open(append_path) as f:
         append = f.readlines()
 
     with open(recipe_path, "w") as f:
         f.writelines(recipe + ["\n"] + append)
 
 
+# type checking
+def _typing(session, run, cmd, run_internal):
+    session_run_commands(session, run)
+    if not run and not run_internal and not cmd:
+        cmd = ["mypy"]
+    for c in cmd:
+        if c == "mypy":
+            session.run("mypy", "--color-output")
+        elif c == "pyright":
+            session.run("pyright", external=True)
+        elif c == "pytype":
+            session.run("pytype")
+    session_run_commands(session, run_internal, external=False)
+
+
 @ALL_SESSION
 def typing(
     session: nox.Session,
-    typing_cmd: cmd_annotated(
+    typing_cmd: cmd_annotated(  # type: ignore
         choices=["mypy", "pyright", "pytype"],
         flags=("--typing-cmd", "-m"),
     ) = (),
     typing_run: RUN_CLI = [],  # noqa
-    typing_run_internal: run_annotated(
+    typing_run_internal: run_annotated(  # type: ignore
         help="run arbitrary (internal) commands.  For example, --typing-run-internal 'mypy --some-option'",
     ) = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
 ):
     """Run type checkers (mypy, pyright, pytype)"""
 
-    install_requirements(
+    pkg_install_condaenv(
         session=session,
         name="typing",
         lock=lock,
-        set_kernel=False,
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
 
-    run, cmd = typing_run, typing_cmd
+    _typing(
+        session=session,
+        run=typing_run,
+        cmd=typing_cmd,
+        run_internal=typing_run_internal,
+    )
 
-    session_run_commands(session, run)
 
-    if not run and not typing_run_internal and not cmd:
-        cmd = ["mypy"]
+@ALL_SESSION_VENV
+def typing_venv(
+    session: nox.Session,
+    typing_cmd: cmd_annotated(  # type: ignore
+        choices=["mypy", "pyright", "pytype"],
+        flags=("--typing-cmd", "-m"),
+    ) = (),
+    typing_run: RUN_CLI = [],  # noqa
+    typing_run_internal: run_annotated(  # type: ignore
+        help="run arbitrary (internal) commands.  For example, --typing-run-internal 'mypy --some-option'",
+    ) = [],  # noqa
+    lock: LOCK_CLI = False,
+    force_reinstall: FORCE_REINSTALL_CLI = False,
+    log_session: bool = False,
+):
+    """Run type checkers (mypy, pyright, pytype)"""
 
-    for c in cmd:
-        if c == "mypy":
-            session.run("mypy", "--color-output")
-        elif c == "pyright":
-            session.run("pyright", external=True)
-        elif c == "pytype":
-            session.run("pytype")
+    pkg_install_venv(
+        session=session,
+        name="typing",
+        lock=lock,
+        install_package=True,
+        force_reinstall=force_reinstall,
+        log_session=log_session,
+        extras="typing",
+    )
 
-    session_run_commands(session, typing_run_internal, external=False)
+    _typing(
+        session=session,
+        run=typing_run,
+        cmd=typing_cmd,
+        run_internal=typing_run_internal,
+    )
 
 
+# ** testdist conda
 @ALL_SESSION
 def testdist_conda(
     session: Session,
     test_no_pytest: bool = False,
-    test_opts: TEST_OPTS_CLI = (),
+    test_opts: TEST_OPTS_CLI = (),  # type: ignore
     testdist_conda_run: RUN_CLI = [],  # noqa
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
     """Test conda distribution"""
 
@@ -782,33 +949,77 @@
 
     session_install_envs(
         session,
         "environment/test-extras.yaml",
         deps=[install_str],
         channels=["conda-forge"],
         force_reinstall=force_reinstall,
+        install_package=False,
     )
 
     if log_session:
         session_log_session(session, False)
 
     session_run_commands(session, testdist_conda_run)
 
     if not test_no_pytest:
         opts = combine_list_str(test_opts)
         session.run("pytest", *opts)
 
 
-@ALL_SESSION
+# ** testdist pypi
+@ALL_SESSION_VENV
 def testdist_pypi(
     session: Session,
     test_no_pytest: bool = False,
-    test_opts: TEST_OPTS_CLI = (),
+    test_opts: TEST_OPTS_CLI = (),  # type: ignore
     testdist_pypi_run: RUN_CLI = [],  # noqa
-    testdist_pypi_extras: cmd_annotated(help="extras to install") = (),
+    testdist_pypi_extras: cmd_annotated(help="extras to install") = (),  # type: ignore
+    force_reinstall: FORCE_REINSTALL_CLI = False,
+    version: VERSION_CLI = "",
+    log_session: bool = False,
+):
+    """Test pypi distribution"""
+    extras = testdist_pypi_extras
+    install_str = PACKAGE_NAME
+
+    if extras:
+        install_str = "{}[{}]".format(install_str, ",".join(extras))
+
+    if version:
+        install_str = f"{install_str}=={version}"
+
+    pkg_install_venv(
+        session=session,
+        name="testdist-pypi",
+        requirement_paths=["environment/test-extras.txt"],
+        reqs=[install_str],
+        force_reinstall=force_reinstall,
+        install_package=False,
+    )
+
+    if log_session:
+        session_log_session(session, False)
+
+    _test(
+        session=session,
+        run=testdist_pypi_run,
+        test_no_pytest=test_no_pytest,
+        test_opts=test_opts,
+        no_cov=True,
+    )
+
+
+@ALL_SESSION
+def testdist_pypi_condaenv(
+    session: Session,
+    test_no_pytest: bool = False,
+    test_opts: TEST_OPTS_CLI = (),  # type: ignore
+    testdist_pypi_run: RUN_CLI = [],  # noqa
+    testdist_pypi_extras: cmd_annotated(help="extras to install") = (),  # type: ignore
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
     """Test pypi distribution"""
     extras = testdist_pypi_extras
     install_str = PACKAGE_NAME
@@ -821,26 +1032,29 @@
 
     session_install_envs(
         session,
         "environment/test-extras.yaml",
         reqs=[install_str],
         channels=["conda-forge"],
         force_reinstall=force_reinstall,
+        install_package=False,
     )
-
     if log_session:
         session_log_session(session, False)
 
-    session_run_commands(session, testdist_pypi_run)
-    if not test_no_pytest:
-        opts = combine_list_str(test_opts)
-        session.run("pytest", *opts)
+    _test(
+        session=session,
+        run=testdist_pypi_run,
+        test_no_pytest=test_no_pytest,
+        test_opts=test_opts,
+        no_cov=True,
+    )
 
 
-# --- Utilities ------------------------------------------------------------------------
+# * Utilities --------------------------------------------------------------------------
 def _create_doc_examples_symlinks(session, clean=True):
     """Create symlinks from docs/examples/*.md files to /examples/usage/..."""
 
     import os
 
     def usage_paths(path):
         with path.open("r") as f:
@@ -883,71 +1097,37 @@
 
             target_rel = os.path.relpath(target, start=link.parent)
             session.log(f"linking {target_rel} -> {link}")
 
             os.symlink(target_rel, link)
 
 
-def _open_webpage(path=None, url=None):
-    import webbrowser
-    from urllib.request import pathname2url
-
-    if path:
-        url = "file://" + pathname2url(str(Path(path).absolute()))
-    if url:
-        webbrowser.open(url)
-
-
-# @group.session(python=PYTHON_DEFAULT_VERSION)
-# def conda_merge(
+# # If want seperate env for updating/reporting version with setuptools-scm
+# # We do this from dev environment.
+# # ** version report/update
+# @DEFAULT_SESSION_VENV
+# def version_scm(
 #     session: Session,
-#     conda_merge_force: bool = False,
+#     version: VERSION_CLI = "",
 #     force_reinstall: FORCE_REINSTALL_CLI = False,
 # ):
-#     """Merge environments using conda-merge."""
-#     import tempfile
-#     session_install_envs(
-#         session,
-#         reqs=["conda-merge", "ruamel.yaml"],
+#     """
+#     Get current version from setuptools-scm
+
+#     Note that the version of editable installs can get stale.
+#     This will show the actual current version.
+#     Avoids need to include setuptools-scm in develop/docs/etc.
+#     """
+
+#     pkg_install_venv(
+#         session=session,
+#         name="version-scm",
+#         install_package=True,
+#         reqs=["setuptools_scm"],
 #         force_reinstall=force_reinstall,
+#         no_deps=True,
 #     )
 
-#     env_base = ROOT / "environment.yaml"
-#     env_dir = ROOT / "environment"
-
-#     def create_env(*extras, others=None, name=None, base=True):
-#         if name is None:
-#             name = extras[0]
-#         env = env_dir / f"{name}.yaml"
-
-#         deps = []
-#         if base:
-#             deps.append(str(env_base))
-#         for extra in extras:
-#             deps.append(str(env_dir / f"{extra}-extras.yaml"))
-
-#         if conda_merge_force or update_target(env, *deps):
-#             session.log(f"creating {env}")
-
-#             args = ["conda-merge"] + deps
-#             with tempfile.TemporaryDirectory() as d:
-#                 tmp_path = Path(d) / "tmp_env.yaml"
-
-#                 with tmp_path.open("w") as f:
-#                     session.run(*args, stdout=f)
-
-#                 run_str = dedent(
-#                     f"""
-#                 from ruamel.yaml import YAML; from pathlib import Path;
-#                 pin, pout = Path("{tmp_path}"), Path("{env}")
-#                 y = YAML(); y.indent(mapping=2, sequence=4, offset=2)
-#                 y.dump(y.load(pin.open("r")), pout.open("w"))
-#                 """
-#                 )
-
-#                 session.run("python", "-c", run_str, silent=True)
-
-#     for extra in ["test", "docs"]:
-#         create_env(extra, base=True)
+#     if version:
+#         session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = version
 
-#     create_env("test", "typing", name="typing", base=True)
-#     create_env("dev", "test", "typing", "nox", name="dev", base=True)
+#     session.run("python", "-m", "setuptools_scm")
```

### Comparing `cmomy-0.5.0/pyproject.toml` & `cmomy-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,30 +28,31 @@
 dependencies = [
     "numpy >= 1.21",
     "numba >= 0.50",
     "xarray >= 0.16",
     "typing-extensions",
     "custom-inherit",
     "module-utilities >= 0.1",
+    "lazy_loader",
 ]
 
 [project.urls]
 homepage = "https://github.com/usnistgov/cmomy"
 documentation = "https://pages.nist.gov/cmomy/"
 
 [project.optional-dependencies]
 test = [
     "pytest", #
-    "python-xdist",
+    "pytest-xdist",
     "pytest-cov",
     "pytest-sugar",
 ]
 dev-extras = [
+    "setuptools-scm", #
     "pytest-accept", # p2c: -p
-    "setuptools-scm",
     "ipython",
     "ipykernel",
 ]
 typing-extras = [
     # "pytype; python_version < '3.11'",
     "mypy",
 ]
@@ -76,16 +77,15 @@
 ]
 dev-complete = [
     "cmomy[dev]", #
     "cmomy[tools]",
     "cmomy[nox]",
 ]
 docs = [
-    "setuptools-scm", #
-    "ipython",
+    "ipython", #
     "pyenchant",
     "ghp-import",
     "sphinx",
     "sphinx-copybutton",
     "sphinxcontrib-spelling",
     "sphinx-autobuild",
     "myst-nb",
@@ -96,15 +96,14 @@
 dist-pypi = ["twine", "build"]
 dist-conda = [
     "anaconda-client", #
     "grayskull",
     "conda-build",
     "conda-verify",
     "boa",
-    "setuptools-scm",
 ]
 
 [tool.pyproject2conda]
 channels = ["conda-forge"]
 
 ## grayskull still messes some things up, but use scripts/recipe-append.sh for this
 [tool.setuptools]
@@ -123,14 +122,15 @@
     "README.md",
     "CHANGELOG.md",
     "LICENSE"
 ], content-type = "text/markdown" }
 
 [tool.setuptools_scm]
 fallback_version = "999"
+write_to = "src/cmomy/_version.py"
 
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --doctest-glob='*.md'"
 testpaths = ["README.md", "src", "tests"]
@@ -291,28 +291,28 @@
 
 [tool.mypy]
 files = ["src/cmomy"]
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

### Comparing `cmomy-0.5.0/src/cmomy/_formatting.py` & `cmomy-0.6.0/src/cmomy/_formatting.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 """pretty formatting for notebook."""
 
-from functools import partial
+from typing import TYPE_CHECKING
 
-from xarray.core import formatting as ff
-from xarray.core import formatting_html as fm
-
-if hasattr(ff, "short_array_repr"):
-    short_numpy_repr = ff.short_array_repr
-elif hasattr(ff, "short_numpy_repr"):
-    short_numpy_repr = ff.short_numpy_repr
+if TYPE_CHECKING:
+    from xarray.core import formatting as ff
+    from xarray.core import formatting_html as fm
 else:
-    short_numpy_rerp = repr
+    import lazy_loader as lazy
+
+    ff = lazy.load("xarray.core.formatting")
+    fm = lazy.load("xarray.core.formatting_html")
+
+
+def short_numpy_repr(*args, **kwargs):
+    if hasattr(ff, "short_array_repr"):
+        f = ff.short_array_repr
+    elif hasattr(ff, "short_numpy_repr"):
+        f = ff.short_numpy_repr
+    else:
+        f = repr
+
+    return f(*args, **kwargs)
 
 
 def tuple_to_str(x):
     """Convert tuple to a string."""
     if len(x) == 0:
         return "*empty*"
 
@@ -22,23 +32,14 @@
 
     if len(x) > 1:
         out = f"({out})"
 
     return out
 
 
-cmomy_section = partial(
-    fm._mapping_section,
-    name="Info",
-    details_func=fm.summarize_attrs,
-    max_items_collapse=5,
-    expand_option_name="display_expand_attrs",
-)
-
-
 def numpy_section(x):
     """Create numpy array section."""
     # "unique" id to expand/collapse the section
     data_id = "section-" + str(fm.uuid.uuid4())
     collapsed = (
         "checked"
         if fm._get_boolean_with_default("display_expand_data", default=True)
@@ -82,15 +83,23 @@
     # dims = {k: attrs[k] for k in ["mom", "val_shape"] if k in attrs}
 
     header_components = [
         f"<div class='xr-obj-type'>{obj_type}</div>",
         fm.format_dims(dims, {}),
     ]
 
-    sections = [cmomy_section(attrs)]
+    sections = [
+        fm._mapping_section(
+            mapping=attrs,
+            name="Info",
+            details_func=fm.summarize_attrs,
+            max_items_collapse=5,
+            expand_option_name="display_expand_attrs",
+        )
+    ]
 
     if hasattr(x.values, "_repr_html_"):
         sections += []
 
         out = fm._obj_repr(
             x.values,
             header_components,
```

### Comparing `cmomy-0.5.0/src/cmomy/_resample.py` & `cmomy-0.6.0/src/cmomy/_resample.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,55 @@
 """Routines to perform resampling."""
 
 from typing import Any, Callable, Dict, Hashable
 
 from numba import njit, prange
 
+from ._lazy_imports import np
 from .options import OPTIONS
 from .pushers import (
     _push_datas_scale,
     _push_datas_scale_cov,
     _push_datas_scale_cov_vec,
     _push_datas_scale_vec,
     _push_vals_scale,
     _push_vals_scale_cov,
     _push_vals_scale_cov_vec,
     _push_vals_scale_vec,
 )
+from .utils import myjit
 
-# from functools import lru_cache
-# import numpy as np
+# --- * Utilities ------------------------------------------------------------------------
+# put these here to avoid slow load up
+
+
+@myjit
+def _numba_random_seed(seed):
+    """Set the random seed for numba functions."""
+    np.random.seed(seed)
+
+
+@myjit
+def _randsamp_freq_out(freq):
+    nrep = freq.shape[0]
+    ndat = freq.shape[1]
+    for i in range(nrep):
+        for j in range(ndat):
+            index = np.random.randint(0, ndat)
+            freq[i, index] += 1
+
+
+@myjit
+def _randsamp_freq_indices(indices, freq):
+    assert freq.shape == indices.shape
+    nrep, ndat = freq.shape
+    for r in range(nrep):
+        for d in range(ndat):
+            idx = indices[r, d]
+            freq[r, idx] += 1
 
 
 def jitter(parallel):
     """Perform jitting."""
     return njit(fastmath=OPTIONS["fastmath"], cache=OPTIONS["cache"], parallel=parallel)
```

### Comparing `cmomy-0.5.0/src/cmomy/_testing.py` & `cmomy-0.6.0/src/cmomy/_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Common routings used in testing."""
 
-import numpy as np
+from ._lazy_imports import np
 
 
 # Dumb calculations
 def _get_cmom(w, x, moments, axis=0, last=True):
     if w is None:
         w = np.array(1.0)
```

### Comparing `cmomy-0.5.0/src/cmomy/_typing.py` & `cmomy-0.6.0/src/cmomy/_typing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Useful typing stuff."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Hashable, Literal, Tuple, TypeVar, Union
 
-import numpy as np
-import xarray as xr
+from ._lazy_imports import np, xr
 
 if TYPE_CHECKING:
     from .abstract_central import CentralMomentsABC  # type: ignore
 
 
 Moments = Union[int, Tuple[int], Tuple[int, int]]
 XvalStrict = Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]
```

### Comparing `cmomy-0.5.0/src/cmomy/abstract_central.py` & `cmomy-0.6.0/src/cmomy/abstract_central.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,25 +14,23 @@
     Mapping,
     Tuple,
     Union,
     cast,
     no_type_check,
 )
 
-import numpy as np
 from custom_inherit import DocInheritMeta
 from module_utilities import cached
-from numpy.core.numeric import normalize_axis_index  # type: ignore
 
 from . import convert
 from ._formatting import repr_html
+from ._lazy_imports import np
 from ._typing import Moments, T_Array, T_CentralMoments
 from .docstrings import docfiller_decorate
 from .options import DOC_SUB
-from .pushers import factory_pushers
 
 if TYPE_CHECKING:
     import xarray as xr
     from numpy.typing import ArrayLike, DTypeLike
 
 # * TODO Main
 # TODO: Total rework is called for to handle typing correctly.
@@ -190,14 +188,16 @@
     @property
     def shape_flat_var(self) -> tuple[int, ...]:
         """Shape of flat variance."""
         return self.val_shape_flat + self.mom_shape_var
 
     @cached.prop
     def _push(self):
+        from .pushers import factory_pushers
+
         vec = len(self.val_shape) > 0
         cov = self.mom_ndim == 2
         return factory_pushers(cov=cov, vec=vec)
 
     def __repr__(self):
         """Repr for class."""
         name = self.__class__.__name__
@@ -948,23 +948,27 @@
         """Move axis to first first position."""
         # NOTE: removinvg this. should be handles elsewhere
         # datas = np.asarray(datas)
         # ndim = datas.ndim - mom_ndim
         # if axis < 0:
         #     axis += ndim
         # assert 0 <= axis < ndim
+        from numpy.core.numeric import normalize_axis_index  # type: ignore
+
         axis = normalize_axis_index(axis, datas.ndim - mom_ndim)
         if axis != 0:
             datas = np.moveaxis(datas, axis, 0)
         return datas, axis
 
     def _wrap_axis(
         self, axis: int | None, default: int = 0, ndim: int | None = None, **kws
     ) -> int:
         """Wrap axis to positive value and check."""
+        from numpy.core.numeric import normalize_axis_index  # type: ignore
+
         if axis is None:
             axis = default
         if ndim is None:
             ndim = self.val_ndim
 
         return cast(int, normalize_axis_index(axis, ndim))
```

### Comparing `cmomy-0.5.0/src/cmomy/central.py` & `cmomy-0.6.0/src/cmomy/central.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 Central moments/comoments routines from :class:`np.ndarray` objects
 -------------------------------------------------------------------.
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Hashable, Literal, Mapping, Sequence, cast
 
-import numpy as np
-import xarray as xr
-from numpy.core.numeric import normalize_axis_index  # type: ignore
-
 from . import convert
+from ._lazy_imports import np, xr
 from .docstrings import docfiller_decorate
 from .resample import randsamp_freq, resample_data, resample_vals
 from .utils import _axis_expand_broadcast, _shape_insert_axis, _shape_reduce
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike, DTypeLike
 
@@ -572,14 +569,15 @@
         target : tuple or array
             If tuple, this is the target shape to be used to Make target.
             If array, this is the target array
         Optional target that has already been rolled.  If this is passed, and
         x will be broadcast/expanded, can expand to this shape without the need
         to reorder,
         """
+        from numpy.core.numeric import normalize_axis_index  # type: ignore
 
         x = np.asarray(x, dtype=self.dtype)
 
         if isinstance(target, str):
             if target == "val":
                 target_shape = self.val_shape
             elif target == "vals":
```

### Comparing `cmomy-0.5.0/src/cmomy/compile.py` & `cmomy-0.6.0/src/cmomy/compile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Set of routines to call most cases to pre-compile numba functions."""
 
 
-import numpy as np
-
+from ._lazy_imports import np
 from .central import CentralMoments
 
 
 def compile_numba_funcs():
     """Attempt at function to compile all funcs."""
     dtype = float
     for val_shape in [(), (1,), (1, 1)]:
```

### Comparing `cmomy-0.5.0/src/cmomy/docstrings.py` & `cmomy-0.6.0/src/cmomy/docstrings.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/options.py` & `cmomy-0.6.0/src/cmomy/options.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/pusher_interface.py` & `cmomy-0.6.0/src/cmomy/pusher_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Interface to numba push functions."""
 
 from __future__ import annotations
 
-import numpy as np
+from ._lazy_imports import np
 
 # from .pushers import factory_pushers
 
 
 def verify_value(
     x,
     val_shape,
```

### Comparing `cmomy-0.5.0/src/cmomy/pushers.py` & `cmomy-0.6.0/src/cmomy/pushers.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/resample.py` & `cmomy-0.6.0/src/cmomy/resample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,90 +1,54 @@
 """
 Routine to perform resampling (:mod:`cmomy.resample`)
 =====================================================
 
 
 """
 
-
-# .. automodule:: cmomy.resample
-#     :members:
-
-# .. autosummary::
-#     :toctree: generated/
-
-#     freq_to_indices
-#     indices_to_freq
-#     randsamp_freq
-#     resample_data
-#     resample_vals
-#     bootstrap_confidence_interval
-#     xbootstrap_confidence_interval
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Hashable, Literal, Sequence, Tuple, cast
 
-import numpy as np
-import xarray as xr
-
-from ._resample import factory_resample_data, factory_resample_vals
-from .utils import _axis_expand_broadcast, myjit
+from ._lazy_imports import np, xr
+from .utils import _axis_expand_broadcast
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike, DTypeLike
 
     from ._typing import ArrayOrder, Moments, XvalStrict
 
 ##############################################################################
 # resampling
 ###############################################################################
 
 
-@myjit
 def numba_random_seed(seed):
     """Set the random seed for numba functions."""
-    np.random.seed(seed)
+    from ._resample import _numba_random_seed
 
-
-@myjit
-def _randsamp_freq_out(freq):
-    nrep = freq.shape[0]
-    ndat = freq.shape[1]
-    for i in range(nrep):
-        for j in range(ndat):
-            index = np.random.randint(0, ndat)
-            freq[i, index] += 1
-
-
-@myjit
-def _randsamp_freq_indices(indices, freq):
-    assert freq.shape == indices.shape
-    nrep, ndat = freq.shape
-    for r in range(nrep):
-        for d in range(ndat):
-            idx = indices[r, d]
-            freq[r, idx] += 1
+    _numba_random_seed(seed)
 
 
 def freq_to_indices(freq):
     """Convert a frequency array to indices array."""
 
     indices_all = []
 
     for f in freq:
         indices = np.concatenate([np.repeat(i, count) for i, count in enumerate(f)])
-
         indices_all.append(indices)
 
     return np.array(indices_all)
 
 
 def indices_to_freq(indices):
     """Convert indices to frequency array."""
+    from ._resample import _randsamp_freq_indices
+
     freq = np.zeros_like(indices)
     _randsamp_freq_indices(indices, freq)
 
     return freq
 
 
 def randsamp_freq(
@@ -128,14 +92,16 @@
     -------
     output : ndarray
         Frequency table.
         if not transpose: output.shape == (nrep, size)
         if transpose, output.shape = (size, nrep)
     """
 
+    from ._resample import _randsamp_freq_indices, _randsamp_freq_out
+
     def _array_check(x: ArrayLike, name="") -> np.ndarray:
         x = np.asarray(x, dtype=np.int64)
         if check:
             if nrep is not None:
                 if x.shape[0] != nrep:
                     raise ValueError(f"{name} has wrong nrep")
 
@@ -197,14 +163,15 @@
 
     Returns
     -------
     output : array
         output shape is `(nrep,) + shape + mom`, where shape is
         the shape of data less axis, and mom is the shape of the resulting mom.
     """
+    from ._resample import factory_resample_data
 
     if isinstance(mom, int):
         mom = (mom,)
 
     # check inputs
     data = np.asarray(data, dtype=dtype, order=order)
     freq = np.asarray(freq, dtype=np.int64, order=order)
@@ -267,14 +234,15 @@
     broadcast: bool = False,
     dtype: DTypeLike | None = None,
     order: ArrayOrder = None,
     parallel: bool = True,
     out: np.ndarray | None = None,
 ) -> np.ndarray:
     """Resample data according to frequency table."""
+    from ._resample import factory_resample_vals
 
     if isinstance(mom, int):
         mom = (mom,) * 1
     assert isinstance(mom, tuple)
 
     if mom_ndim is None:
         mom_ndim = len(mom)
```

### Comparing `cmomy-0.5.0/src/cmomy/tests/conftest.py` & `cmomy-0.6.0/src/cmomy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/tests/test_central.py` & `cmomy-0.6.0/src/cmomy/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/tests/test_central_2.py` & `cmomy-0.6.0/src/cmomy/tests/test_central_2.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/tests/test_convert.py` & `cmomy-0.6.0/src/cmomy/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/tests/test_resample.py` & `cmomy-0.6.0/src/cmomy/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/tests/test_stability.py` & `cmomy-0.6.0/src/cmomy/tests/test_stability.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/tests/test_verify.py` & `cmomy-0.6.0/src/cmomy/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/tests/test_xcentral.py` & `cmomy-0.6.0/src/cmomy/tests/test_xcentral.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/tests/test_xcentral_constructors.py` & `cmomy-0.6.0/src/cmomy/tests/test_xcentral_constructors.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.5.0/src/cmomy/utils.py` & `cmomy-0.6.0/src/cmomy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 """Utilities."""
 from __future__ import annotations
 
 from functools import lru_cache
 from typing import TYPE_CHECKING, Sequence
 
-import numpy as np
-from numba import njit
-
+from ._lazy_imports import np
 from .options import OPTIONS
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike, DTypeLike
 
     from ._typing import ArrayOrder
 
 
 def myjit(func):
     """Jitter with option inline='always', fastmath=True."""
+    from numba import njit
+
     return njit(inline="always", fastmath=OPTIONS["fastmath"], cache=OPTIONS["cache"])(
         func
     )
 
 
 # from scipy.special import binom
 # def factory_binomial(order):
 #     irange = np.arange(order + 1)
 #     bfac = np.array([binom(i, irange) for i in irange])
 #     return bfac
 
 
 def _binom(n, k):
+    import math
+
     if n > k:
-        return np.math.factorial(n) / (np.math.factorial(k) * np.math.factorial(n - k))
+        return math.factorial(n) / (math.factorial(k) * math.factorial(n - k))
     elif n == k:
         return 1.0
     else:
         # n < k
         return 0.0
```

### Comparing `cmomy-0.5.0/src/cmomy/xcentral.py` & `cmomy-0.6.0/src/cmomy/xcentral.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,18 @@
     Mapping,
     Sequence,
     cast,
     no_type_check,
 )
 from warnings import warn
 
-import numpy as np
-import xarray as xr
 from module_utilities import cached
 
 from . import convert
+from ._lazy_imports import np, xr
 from .abstract_central import CentralMomentsABC
 from .central import CentralMoments
 from .docstrings import docfiller_decorate
 from .utils import _shape_reduce
 
 if TYPE_CHECKING:
     from numpy.typing import DTypeLike
```

### Comparing `cmomy-0.5.0/src/cmomy.egg-info/PKG-INFO` & `cmomy-0.6.0/src/cmomy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmomy
-Version: 0.5.0
+Version: 0.6.0
 Summary: Central (co)moment calculation/manipulation
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/cmomy
 Project-URL: documentation, https://pages.nist.gov/cmomy/
 Keywords: cmomy
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cmomy-0.5.0/src/cmomy.egg-info/SOURCES.txt` & `cmomy-0.6.0/src/cmomy.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 Makefile
 README.md
 conftest.py
 environment.yaml
 noxfile.py
 pyproject.toml
 tox.ini
+changelog.d/20230706_144442_william.krekelberg.md
 changelog.d/README.txt
 changelog.d/templates/new_fragment.md.j2
 changelog.d/templates/auto-changelog/macros.jinja2
 changelog.d/templates/auto-changelog/template.jinja2
 docs/Makefile
 docs/authors.md
 docs/changelog.md
@@ -55,18 +56,21 @@
 docs/reference/api-baseclasses.rst
 docs/reference/api-modules.rst
 docs/reference/api-public.rst
 docs/reference/index.md
 environment/base.yaml
 environment/dev.yaml
 environment/dist-conda.yaml
+environment/dist-pypi.txt
 environment/dist-pypi.yaml
 environment/docs-extras.yaml
 environment/docs.yaml
 environment/lint.yaml
+environment/test-extras.txt
+environment/test-extras.yaml
 environment/test.yaml
 environment/typing.yaml
 environment/lock/py310.yaml
 environment/lock/py311.yaml
 environment/lock/py38.yaml
 environment/lock/py39.yaml
 examples/README.md
@@ -74,18 +78,21 @@
 examples/archived/central_moments.ipynb
 examples/archived/example_usage.ipynb
 examples/archived/parallel_test.ipynb
 examples/archived/test_accumulator.ipynb
 examples/usage/motivation.ipynb
 examples/usage/usage_notebook.ipynb
 src/cmomy/__init__.py
+src/cmomy/_convert.py
 src/cmomy/_formatting.py
+src/cmomy/_lazy_imports.py
 src/cmomy/_resample.py
 src/cmomy/_testing.py
 src/cmomy/_typing.py
+src/cmomy/_version.py
 src/cmomy/abstract_central.py
 src/cmomy/central.py
 src/cmomy/compile.py
 src/cmomy/convert.py
 src/cmomy/docstrings.py
 src/cmomy/options.py
 src/cmomy/pusher_interface.py
```

### Comparing `cmomy-0.5.0/src/cmomy.egg-info/requires.txt` & `cmomy-0.6.0/src/cmomy.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 numpy>=1.21
 numba>=0.50
 xarray>=0.16
 typing-extensions
 custom-inherit
 module-utilities>=0.1
+lazy_loader
 
 [dev]
 cmomy[test]
 cmomy[typing-extras]
 cmomy[dev-extras]
 
 [dev-complete]
 cmomy[dev]
 cmomy[tools]
 cmomy[nox]
 
 [dev-extras]
-pytest-accept
 setuptools-scm
+pytest-accept
 ipython
 ipykernel
 
 [dist-conda]
 anaconda-client
 grayskull
 conda-build
 conda-verify
 boa
-setuptools-scm
 
 [dist-pypi]
 twine
 build
 
 [docs]
-setuptools-scm
 ipython
 pyenchant
 ghp-import
 sphinx
 sphinx-copybutton
 sphinxcontrib-spelling
 sphinx-autobuild
@@ -49,15 +48,15 @@
 [nox]
 nox
 noxopt
 ruamel.yaml
 
 [test]
 pytest
-python-xdist
+pytest-xdist
 pytest-cov
 pytest-sugar
 
 [tools]
 pre-commit
 cruft
 scriv
```

### Comparing `cmomy-0.5.0/tools/noxtools.py` & `cmomy-0.6.0/tools/noxtools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Utilities to work with nox"""
 
 from __future__ import annotations
 
 import shlex
-import tempfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable, Literal, cast
 
 from ruamel.yaml import safe_load
 
 if TYPE_CHECKING:
     from collections.abc import Collection, Sequence
@@ -32,17 +31,15 @@
     # only unique
     sorter = {k: i for i, k in enumerate(like)}
     return sorted(set(values), key=lambda k: sorter[k])
 
 
 def update_target(target: str | Path, *deps: str | Path) -> bool:
     """Check if target is older than deps:"""
-
     target_path = Path(target)
-
     deps_path = tuple(map(Path, deps))
 
     for d in deps_path:
         if not d.exists():
             raise ValueError(f"dependency {d} does not exist")
 
     if not target_path.exists():
@@ -66,14 +63,87 @@
 
     if len(args) == 1 and not isinstance(args[0], str):
         args = args[0]
 
     return sum([[flag, _] for _ in args], [])
 
 
+def open_webpage(path: str | Path | None = None, url: str | None = None):
+    """
+    Open webpage from path or url.
+
+    Useful if want to view webpage with javascript, etc., as well as static html.
+    """
+    import webbrowser
+    from urllib.request import pathname2url
+
+    if path:
+        url = "file://" + pathname2url(str(Path(path).absolute()))
+    if url:
+        webbrowser.open(url)
+
+
+# --- Load user configuration ----------------------------------------------------------
+def load_nox_config(path: str | Path = "./.noxconfig.toml") -> dict[str, Any]:
+    """
+    Load user toml config file.
+
+    File should look something like:
+
+    [nox.python]
+    paths = ["~/.conda/envs/test-3.*/bin"]
+
+    # Extras for environments
+    # for example, could have
+    # dev = ["dev", "nox", "tools"]
+    [nox.extras]
+    dev = ["dev", "nox"]
+
+    """
+    import os
+    from glob import glob
+
+    import tomli
+
+    config = {}
+
+    path = Path(path)
+    if not path.exists():
+        return config
+
+    with path.open("rb") as f:
+        data = tomli.load(f)
+
+    # Python paths
+    try:
+        paths = []
+        for p in data["nox"]["python"]["paths"]:
+            paths.extend(glob(os.path.expanduser(p)))
+
+        paths_str = ":".join(map(str, paths))
+        os.environ["PATH"] = paths_str + ":" + os.environ["PATH"]
+    except KeyError:
+        pass
+
+    # extras:
+    extras = {"dev": ["nox", "dev"]}
+    try:
+        for k, v in data["nox"]["extras"].items():
+            extras[k] = v
+    except KeyError:
+        pass
+
+    config["environment-extras"] = extras
+
+    # for py in PYTHON_ALL_VERSIONS:
+    #     print(f"which python{py}", shutil.which(f"python{py}"))
+
+    return config
+
+
 # --- Nox session utilities ------------------------------------------------------------
 def session_skip_install(session: nox.Session) -> bool:
     """
     Utility to check if we're skipping install and reusing existing venv
     This is a hack and may need to change if upstream changes.
     """
     return session._runner.global_config.no_install and session._runner.venv._reused  # type: ignore
@@ -125,16 +195,14 @@
     if no_deps:
         command.append("--no-deps")
 
     session.install(*command, *args, **kwargs)
 
 
 # --- Create env from lock -------------------------------------------------------------
-
-
 def session_install_envs_lock(
     session: nox.Session,
     lockfile: str | Path,
     extras: str | list[str] | None = None,
     display_name: str | None = None,
     force_reinstall: bool = False,
     install_package: bool = False,
@@ -176,37 +244,38 @@
 
     write_hashfile(hashes, session=session, prefix="lock")
 
     return unchanged
 
 
 # --- create env from yaml -------------------------------------------------------------
-
-
 def parse_envs(
     *paths: str | Path,
     remove_python: bool = True,
     deps: Collection[str] | None = None,
     reqs: Collection[str] | None = None,
     channels: Collection[str] | None = None,
 ) -> tuple[set[str], set[str], set[str], str | None]:
     """Parse an `environment.yaml` file."""
+    import re
 
     def _default(x) -> set[str]:
         if x is None:
             return set()
         elif isinstance(x, str):
             x = [x]
         return set(x)
 
     channels = _default(channels)
     deps = _default(deps)
     reqs = _default(reqs)
     name = None
 
+    python_match = re.compile(r"\s*(python)\s*[~<=>].*")
+
     def _get_context(path):
         if hasattr(path, "readline"):
             from contextlib import nullcontext
 
             return nullcontext(path)
         else:
             return Path(path).open("r")
@@ -219,15 +288,15 @@
         name = data.get("name", name)
 
         # check dependencies for pip
         for d in data.get("dependencies", []):
             if isinstance(d, dict):
                 reqs.update(cast(list[str], d.get("pip")))
             else:
-                if remove_python and d[: len("python")] != "python":
+                if remove_python and not python_match.match(d):
                     deps.add(d)
 
     return channels, deps, reqs, name
 
 
 def session_install_envs(
     session: nox.Session,
@@ -243,33 +312,35 @@
     install_package: bool = False,
 ) -> bool:
     """Parse and install everything. Pass an already merged yaml file."""
 
     if session_skip_install(session):
         return True
 
+    channels, deps, reqs, name = parse_envs(
+        *paths,
+        remove_python=remove_python,
+        deps=deps,
+        reqs=reqs,
+        channels=channels,
+    )
+
     unchanged, hashes = env_unchanged(
         session,
-        *paths,
         prefix="env",
         other=dict(
-            deps=deps, reqs=reqs, channels=channels, install_package=install_package
+            deps=deps,
+            reqs=reqs,
+            channels=channels,
+            install_package=install_package,
         ),
     )
     if unchanged and not force_reinstall:
         return unchanged
 
-    channels, deps, reqs, name = parse_envs(
-        *paths,
-        remove_python=remove_python,
-        deps=deps,
-        reqs=reqs,
-        channels=channels,
-    )
-
     if not channels:
         channels = ""
     if deps:
         conda_install_kws = conda_install_kws or {}
         conda_install_kws.update(channel=channels)
         session.conda_install(*deps, **(conda_install_kws or {}))
 
@@ -284,41 +355,49 @@
     write_hashfile(hashes, session=session, prefix="env")
 
     return unchanged
 
 
 def session_install_pip(
     session: nox.Session,
-    requirement_paths: Collection[str] | None = None,
-    constraint_paths: Collection[str] | None = None,
+    requirement_paths: str | Collection[str] | None = None,
+    constraint_paths: str | Collection[str] | None = None,
     extras: str | Collection[str] | None = None,
-    reqs: Collection[str] | None = None,
+    reqs: str | Collection[str] | None = None,
     display_name: str | None = None,
     force_reinstall: bool = False,
     install_package: bool = False,
     no_deps: bool = False,
 ):
     if session_skip_install(session):
         return True
 
+    def _check_param(x):
+        if x is None:
+            return []
+        elif isinstance(x, str):
+            return [x]
+        else:
+            return x
+
+    extras = _check_param(extras)
     if extras:
         install_package = True
-        if not isinstance(extras, str):
-            extras = ",".join(extras)
+        extras = ",".join(extras)
         install_package_args = ["-e", f".[{extras}]"]
     elif install_package:
         install_package_args = ["-e", "."]
 
     if install_package and no_deps:
         install_package_args.append("--no-deps")
 
-    requirement_paths = requirement_paths or ()
-    constraint_paths = constraint_paths or ()
-    reqs = reqs or ()
-    paths = requirement_paths + constraint_paths
+    requirement_paths = _check_param(requirement_paths)
+    constraint_paths = _check_param(constraint_paths)
+    reqs = _check_param(reqs)
+    paths = list(requirement_paths) + list(constraint_paths)
 
     unchanged, hashes = env_unchanged(
         session,
         *paths,
         prefix="pip",
         other=dict(
             reqs=reqs, extras=extras, install_package=install_package, no_deps=no_deps
@@ -337,82 +416,29 @@
     if install_args:
         session.install(*install_args)
 
     if install_package:
         session.install(*install_package_args)
 
     session_set_ipykernel_display_name(session, display_name)
-
     write_hashfile(hashes, session=session, prefix="pip")
 
 
-def session_install_envs_merge(
-    session,
-    *paths,
-    remove_python=True,
-    deps=None,
-    reqs=None,
-    channels=None,
-    conda_install_kws=None,
-    install_kws=None,
-    display_name=None,
-    force_reinstall=False,
-) -> bool:
-    """Merge files (using conda-merge) and then create env"""
-
-    if session_skip_install(session):
-        return True
-
-    unchanged, hashes = env_unchanged(
-        session, *paths, prefix="env", other=dict(deps=deps, reqs=reqs)
-    )
-    if unchanged and not force_reinstall:
-        return unchanged
-
-    # first create a temporary file for the environment
-    with tempfile.TemporaryDirectory() as d:
-        yaml = Path(d) / "tmp_env.yaml"
-        with yaml.open("w") as f:
-            session.run("conda-merge", *paths, stdout=f, external=True)
-        session.run("cat", str(yaml), external=True, silent=True)
-
-        channels, deps, reqs, _ = parse_envs(
-            yaml, remove_python=remove_python, deps=deps, reqs=reqs, channels=channels
-        )
-
-    if deps:
-        if conda_install_kws is None:
-            conda_install_kws = {}
-        conda_install_kws.update(channel=channels)
-        session.conda_install(*deps, **conda_install_kws)
-
-    if reqs:
-        if install_kws is None:
-            install_kws = {}
-        session.install(*reqs, **install_kws)
-
-    session_set_ipykernel_display_name(session, display_name)
-
-    write_hashfile(hashes, session=session, prefix="env")
-
-    return unchanged
-
-
 # --- Hash environment -----------------------------------------------------------------
 
 PREFIX_HASH_EXTS = Literal["env", "lock", "pip"]
 
 
 def env_unchanged(
     session: nox.Session,
     *paths: str | Path,
     prefix: PREFIX_HASH_EXTS,
     verbose: bool = True,
     hashes: dict[str, str] | None = None,
-    other: Any | None = None,
+    other: dict[str, Any] | None = None,
 ) -> tuple[bool, dict[str, str]]:
     hashfile = hashfile_path(session, prefix)
 
     if hashes is None:
         hashes = get_hashes(*paths, other=other)
 
     if hashfile.exists():
@@ -428,23 +454,36 @@
         session.log(f"session {session.name} changed")
 
     return unchanged, hashes
 
 
 def get_hashes(
     *paths: str | Path,
-    other: str | None = None,
+    other: dict[str, Any] | None = None,
 ) -> dict[str, str]:
     """Get md5 hashes for paths"""
-    out = {str(path): _get_file_hash(path) for path in paths}
+
+    out = {"path": {str(path): _get_file_hash(path) for path in paths}}
 
     if other:
         import hashlib
 
-        out["other"] = hashlib.md5(str(other).encode("utf-8")).hexdigest()
+        other_hashes = {}
+        for k, v in other.items():
+            if isinstance(v, str):
+                s = v
+            else:
+                try:
+                    s = str(sorted(v))
+                except Exception:
+                    s = str(v)
+            other_hashes[k] = hashlib.md5(s.encode("utf-8")).hexdigest()
+
+        out["other"] = other_hashes
+
     return out
 
 
 def hashfile_path(session: nox.Session, prefix: PREFIX_HASH_EXTS) -> Path:
     """Path for hashfile for this session"""
     return Path(session.create_tmp()) / f"{prefix}.json"
 
@@ -481,40 +520,65 @@
             data = f.read(buff_size)
             if not data:
                 break
             md5.update(data)
     return md5.hexdigest()
 
 
-# from contextlib import contextmanager
-# @contextmanager
-# def check_hashed_env(
-#         session: nox.Session,
-#         *paths: str | Path,
-#         prefix: Literal["env", "lock"],
-#         verbose: bool=True,
-#         recreate_session=False,
-# ):
+# --- Old stuff ------------------------------------------------------------------------
+# def session_install_envs_merge(
+#     session,
+#     *paths,
+#     remove_python=True,
+#     deps=None,
+#     reqs=None,
+#     channels=None,
+#     conda_install_kws=None,
+#     install_kws=None,
+#     display_name=None,
+#     force_reinstall=False,
+# ) -> bool:
+#     """Merge files (using conda-merge) and then create env"""
+
+#     if session_skip_install(session):
+#         return True
+
+#     unchanged, hashes = env_unchanged(
+#         session, *paths, prefix="env", other=dict(deps=deps, reqs=reqs)
+#     )
+#     if unchanged and not force_reinstall:
+#         return unchanged
 
-#     changed, hashes = env_hashes_changed(session, *paths, prefix, verbose=verbose, return_hashes=True)
+#     # first create a temporary file for the environment
+#     with tempfile.TemporaryDirectory() as d:
+#         yaml = Path(d) / "tmp_env.yaml"
+#         with yaml.open("w") as f:
+#             session.run("conda-merge", *paths, stdout=f, external=True)
+#         session.run("cat", str(yaml), external=True, silent=True)
 
+#         channels, deps, reqs, _ = parse_envs(
+#             yaml, remove_python=remove_python, deps=deps, reqs=reqs, channels=channels
+#         )
 
-#     if changed and recreate_session:
-#         if verbose:
-#             session.log("env changed.  Recreating {session.virtualenv.location_name}")
-#             _reuse_original = session.virtualenv.reuse_existing
-#             _no_install_original = session._runner.global_config.no_install
+#     if deps:
+#         if conda_install_kws is None:
+#             conda_install_kws = {}
+#         conda_install_kws.update(channel=channels)
+#         session.conda_install(*deps, **conda_install_kws)
+
+#     if reqs:
+#         if install_kws is None:
+#             install_kws = {}
+#         session.install(*reqs, **install_kws)
 
-#             session.virtualenv.reuse_existing = False
-#             session._runner.global_config.no_install = False
+#     session_set_ipykernel_display_name(session, display_name)
 
-#             session.virtualenv.create()
-#             env_hashes_changed(session, *paths, prefix, verbose=verbose, hashes=hashes)
+#     write_hashfile(hashes, session=session, prefix="env")
 
-#             session.virtualenv.reuse_existing = _reuse_original
+#     return unchanged
 
 
 # def _remove_python_from_yaml(path):
 #     from yaml import safe_dump
 
 #     path = Path(path)
 
@@ -763,7 +827,65 @@
 #         external = False
 
 #     args = check_args_with_default(args, default=default)
 
 # #     session.log(f"args {args}")
 # #     session.log(f"external {external}")
 # #     session.run(*args, external=external, **kws)
+
+
+## This should actually go in the noxfile.  Keeping here
+## incase want it again in the future.
+# @group.session(python=PYTHON_DEFAULT_VERSION)
+# def conda_merge(
+#     session: Session,
+#     conda_merge_force: bool = False,
+#     force_reinstall: FORCE_REINSTALL_CLI = False,
+# ):
+#     """Merge environments using conda-merge."""
+#     import tempfile
+#     session_install_envs(
+#         session,
+#         reqs=["conda-merge", "ruamel.yaml"],
+#         force_reinstall=force_reinstall,
+#     )
+
+#     env_base = ROOT / "environment.yaml"
+#     env_dir = ROOT / "environment"
+
+#     def create_env(*extras, others=None, name=None, base=True):
+#         if name is None:
+#             name = extras[0]
+#         env = env_dir / f"{name}.yaml"
+
+#         deps = []
+#         if base:
+#             deps.append(str(env_base))
+#         for extra in extras:
+#             deps.append(str(env_dir / f"{extra}-extras.yaml"))
+
+#         if conda_merge_force or update_target(env, *deps):
+#             session.log(f"creating {env}")
+
+#             args = ["conda-merge"] + deps
+#             with tempfile.TemporaryDirectory() as d:
+#                 tmp_path = Path(d) / "tmp_env.yaml"
+
+#                 with tmp_path.open("w") as f:
+#                     session.run(*args, stdout=f)
+
+#                 run_str = dedent(
+#                     f"""
+#                 from ruamel.yaml import YAML; from pathlib import Path;
+#                 pin, pout = Path("{tmp_path}"), Path("{env}")
+#                 y = YAML(); y.indent(mapping=2, sequence=4, offset=2)
+#                 y.dump(y.load(pin.open("r")), pout.open("w"))
+#                 """
+#                 )
+
+#                 session.run("python", "-c", run_str, silent=True)
+
+#     for extra in ["test", "docs"]:
+#         create_env(extra, base=True)
+
+#     create_env("test", "typing", name="typing", base=True)
+#     create_env("dev", "test", "typing", "nox", name="dev", base=True)
```

### Comparing `cmomy-0.5.0/tox.ini` & `cmomy-0.6.0/tox.ini`

 * *Files identical despite different names*

