# Comparing `tmp/click-8.1.3.tar.gz` & `tmp/click-8.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click-8.1.3.tar", last modified: Thu Apr 28 17:35:45 2022, max compression
+gzip compressed data, was "click-8.1.4.tar", last modified: Thu Jul  6 18:22:39 2023, max compression
```

## Comparing `click-8.1.3.tar` & `click-8.1.4.tar`

### file list

```diff
@@ -1,146 +1,147 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.383730 click-8.1.3/
--rw-r--r--   0 david     (1000) david     (1000)    44355 2022-04-28 17:35:17.000000 click-8.1.3/CHANGES.rst
--rw-r--r--   0 david     (1000) david     (1000)     1475 2021-03-04 00:26:07.000000 click-8.1.3/LICENSE.rst
--rw-r--r--   0 david     (1000) david     (1000)      181 2022-02-22 14:27:38.000000 click-8.1.3/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)     3133 2022-04-28 17:35:45.383730 click-8.1.3/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     2071 2022-02-22 14:27:38.000000 click-8.1.3/README.rst
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.377063 click-8.1.3/artwork/
--rw-r--r--   0 david     (1000) david     (1000)     8705 2019-09-07 13:32:47.000000 click-8.1.3/artwork/logo.svg
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/docs/
--rw-r--r--   0 david     (1000) david     (1000)      603 2020-08-13 00:50:56.000000 click-8.1.3/docs/Makefile
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/docs/_static/
--rw-r--r--   0 david     (1000) david     (1000)      625 2020-08-13 00:50:56.000000 click-8.1.3/docs/_static/click-icon.png
--rw-r--r--   0 david     (1000) david     (1000)     4246 2020-08-13 00:50:56.000000 click-8.1.3/docs/_static/click-logo-sidebar.png
--rw-r--r--   0 david     (1000) david     (1000)    26081 2020-08-13 00:50:56.000000 click-8.1.3/docs/_static/click-logo.png
--rw-r--r--   0 david     (1000) david     (1000)    17514 2022-02-22 14:27:38.000000 click-8.1.3/docs/advanced.rst
--rw-r--r--   0 david     (1000) david     (1000)     2828 2022-03-17 22:17:41.000000 click-8.1.3/docs/api.rst
--rw-r--r--   0 david     (1000) david     (1000)     8659 2021-10-08 16:57:05.000000 click-8.1.3/docs/arguments.rst
--rw-r--r--   0 david     (1000) david     (1000)       45 2022-02-22 14:27:38.000000 click-8.1.3/docs/changes.rst
--rw-r--r--   0 david     (1000) david     (1000)    18928 2022-02-22 14:27:38.000000 click-8.1.3/docs/commands.rst
--rw-r--r--   0 david     (1000) david     (1000)     7828 2020-08-13 00:50:56.000000 click-8.1.3/docs/complex.rst
--rw-r--r--   0 david     (1000) david     (1000)     2109 2022-02-22 14:27:38.000000 click-8.1.3/docs/conf.py
--rw-r--r--   0 david     (1000) david     (1000)     1193 2019-09-07 13:32:47.000000 click-8.1.3/docs/contrib.rst
--rw-r--r--   0 david     (1000) david     (1000)     5876 2021-10-08 16:57:05.000000 click-8.1.3/docs/documentation.rst
--rw-r--r--   0 david     (1000) david     (1000)     2924 2019-09-07 13:32:47.000000 click-8.1.3/docs/exceptions.rst
--rw-r--r--   0 david     (1000) david     (1000)     2271 2022-02-22 14:27:38.000000 click-8.1.3/docs/index.rst
--rw-r--r--   0 david     (1000) david     (1000)       71 2021-03-04 00:26:07.000000 click-8.1.3/docs/license.rst
--rw-r--r--   0 david     (1000) david     (1000)      773 2020-08-13 00:50:56.000000 click-8.1.3/docs/make.bat
--rw-r--r--   0 david     (1000) david     (1000)    26719 2022-03-17 22:17:41.000000 click-8.1.3/docs/options.rst
--rw-r--r--   0 david     (1000) david     (1000)     4875 2022-02-22 14:27:38.000000 click-8.1.3/docs/parameters.rst
--rw-r--r--   0 david     (1000) david     (1000)     1651 2019-09-07 13:32:47.000000 click-8.1.3/docs/prompts.rst
--rw-r--r--   0 david     (1000) david     (1000)     9347 2022-04-28 13:42:09.000000 click-8.1.3/docs/quickstart.rst
--rw-r--r--   0 david     (1000) david     (1000)     4392 2021-10-08 16:57:05.000000 click-8.1.3/docs/setuptools.rst
--rw-r--r--   0 david     (1000) david     (1000)     9508 2022-03-28 13:47:17.000000 click-8.1.3/docs/shell-completion.rst
--rw-r--r--   0 david     (1000) david     (1000)     4379 2022-02-22 14:27:38.000000 click-8.1.3/docs/testing.rst
--rw-r--r--   0 david     (1000) david     (1000)     4421 2021-10-08 16:57:05.000000 click-8.1.3/docs/unicode-support.rst
--rw-r--r--   0 david     (1000) david     (1000)     4705 2022-02-22 14:27:38.000000 click-8.1.3/docs/upgrading.rst
--rw-r--r--   0 david     (1000) david     (1000)    12792 2022-02-22 14:27:38.000000 click-8.1.3/docs/utils.rst
--rw-r--r--   0 david     (1000) david     (1000)     7164 2022-02-22 14:27:38.000000 click-8.1.3/docs/why.rst
--rw-r--r--   0 david     (1000) david     (1000)     3159 2021-10-08 16:57:05.000000 click-8.1.3/docs/wincmd.rst
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/
--rw-r--r--   0 david     (1000) david     (1000)      429 2022-03-17 22:17:41.000000 click-8.1.3/examples/README
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/aliases/
--rw-r--r--   0 david     (1000) david     (1000)      445 2019-09-07 13:32:47.000000 click-8.1.3/examples/aliases/README
--rw-r--r--   0 david     (1000) david     (1000)       20 2019-09-07 13:32:47.000000 click-8.1.3/examples/aliases/aliases.ini
--rw-r--r--   0 david     (1000) david     (1000)     4061 2022-02-22 14:27:38.000000 click-8.1.3/examples/aliases/aliases.py
--rw-r--r--   0 david     (1000) david     (1000)      267 2021-03-04 00:26:07.000000 click-8.1.3/examples/aliases/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/colors/
--rw-r--r--   0 david     (1000) david     (1000)      158 2022-02-22 14:27:38.000000 click-8.1.3/examples/colors/README
--rw-r--r--   0 david     (1000) david     (1000)      926 2022-02-22 14:27:38.000000 click-8.1.3/examples/colors/colors.py
--rw-r--r--   0 david     (1000) david     (1000)      263 2022-02-22 14:27:38.000000 click-8.1.3/examples/colors/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/completion/
--rw-r--r--   0 david     (1000) david     (1000)      472 2022-02-22 14:27:38.000000 click-8.1.3/examples/completion/README
--rw-r--r--   0 david     (1000) david     (1000)     1388 2022-02-22 14:27:38.000000 click-8.1.3/examples/completion/completion.py
--rw-r--r--   0 david     (1000) david     (1000)      279 2022-02-22 14:27:38.000000 click-8.1.3/examples/completion/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/complex/
--rw-r--r--   0 david     (1000) david     (1000)      452 2019-09-07 13:32:47.000000 click-8.1.3/examples/complex/README
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/complex/complex/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-09-07 13:32:47.000000 click-8.1.3/examples/complex/complex/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     1615 2021-10-08 16:57:05.000000 click-8.1.3/examples/complex/complex/cli.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/complex/complex/commands/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-09-07 13:32:47.000000 click-8.1.3/examples/complex/complex/commands/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      385 2021-10-08 16:57:05.000000 click-8.1.3/examples/complex/complex/commands/cmd_init.py
--rw-r--r--   0 david     (1000) david     (1000)      286 2021-03-04 00:26:07.000000 click-8.1.3/examples/complex/complex/commands/cmd_status.py
--rw-r--r--   0 david     (1000) david     (1000)      289 2021-03-04 00:26:07.000000 click-8.1.3/examples/complex/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/imagepipe/
--rw-r--r--   0 david     (1000) david     (1000)       12 2019-09-07 13:32:47.000000 click-8.1.3/examples/imagepipe/.gitignore
--rw-r--r--   0 david     (1000) david     (1000)      310 2019-09-07 13:32:47.000000 click-8.1.3/examples/imagepipe/README
--rw-r--r--   0 david     (1000) david     (1000)    51677 2019-09-07 13:32:47.000000 click-8.1.3/examples/imagepipe/example01.jpg
--rw-r--r--   0 david     (1000) david     (1000)    39106 2019-09-07 13:32:47.000000 click-8.1.3/examples/imagepipe/example02.jpg
--rw-r--r--   0 david     (1000) david     (1000)     8257 2022-02-22 14:27:38.000000 click-8.1.3/examples/imagepipe/imagepipe.py
--rw-r--r--   0 david     (1000) david     (1000)      285 2021-03-04 00:26:07.000000 click-8.1.3/examples/imagepipe/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/inout/
--rw-r--r--   0 david     (1000) david     (1000)      236 2019-09-07 13:32:47.000000 click-8.1.3/examples/inout/README
--rw-r--r--   0 david     (1000) david     (1000)      722 2021-03-04 00:26:07.000000 click-8.1.3/examples/inout/inout.py
--rw-r--r--   0 david     (1000) david     (1000)      259 2021-03-04 00:26:07.000000 click-8.1.3/examples/inout/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/naval/
--rw-r--r--   0 david     (1000) david     (1000)      354 2019-09-07 13:32:47.000000 click-8.1.3/examples/naval/README
--rw-r--r--   0 david     (1000) david     (1000)     1697 2021-10-08 16:57:05.000000 click-8.1.3/examples/naval/naval.py
--rw-r--r--   0 david     (1000) david     (1000)      259 2021-03-04 00:26:07.000000 click-8.1.3/examples/naval/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/repo/
--rw-r--r--   0 david     (1000) david     (1000)      153 2019-09-07 13:32:47.000000 click-8.1.3/examples/repo/README
--rw-r--r--   0 david     (1000) david     (1000)     4717 2021-10-08 16:57:05.000000 click-8.1.3/examples/repo/repo.py
--rw-r--r--   0 david     (1000) david     (1000)      255 2021-03-04 00:26:07.000000 click-8.1.3/examples/repo/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/termui/
--rw-r--r--   0 david     (1000) david     (1000)      143 2019-09-07 13:32:47.000000 click-8.1.3/examples/termui/README
--rw-r--r--   0 david     (1000) david     (1000)      263 2022-02-22 14:27:38.000000 click-8.1.3/examples/termui/setup.py
--rw-r--r--   0 david     (1000) david     (1000)     4150 2022-02-22 14:27:38.000000 click-8.1.3/examples/termui/termui.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/examples/validation/
--rw-r--r--   0 david     (1000) david     (1000)      241 2019-09-07 13:32:47.000000 click-8.1.3/examples/validation/README
--rw-r--r--   0 david     (1000) david     (1000)      279 2021-03-04 00:26:07.000000 click-8.1.3/examples/validation/setup.py
--rw-r--r--   0 david     (1000) david     (1000)     1407 2022-02-20 15:20:14.000000 click-8.1.3/examples/validation/validation.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.380397 click-8.1.3/requirements/
--rw-r--r--   0 david     (1000) david     (1000)     1100 2022-04-28 17:25:37.000000 click-8.1.3/requirements/dev.txt
--rw-r--r--   0 david     (1000) david     (1000)     1479 2022-04-28 17:25:33.000000 click-8.1.3/requirements/docs.txt
--rw-r--r--   0 david     (1000) david     (1000)      418 2022-04-28 17:25:34.000000 click-8.1.3/requirements/tests.txt
--rw-r--r--   0 david     (1000) david     (1000)      299 2022-04-28 17:25:34.000000 click-8.1.3/requirements/typing.txt
--rw-r--r--   0 david     (1000) david     (1000)     2020 2022-04-28 17:35:45.383730 click-8.1.3/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)      191 2022-02-22 14:27:38.000000 click-8.1.3/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.377063 click-8.1.3/src/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.383730 click-8.1.3/src/click/
--rw-r--r--   0 david     (1000) david     (1000)     3138 2022-04-28 17:35:17.000000 click-8.1.3/src/click/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)    18810 2022-02-22 14:27:38.000000 click-8.1.3/src/click/_compat.py
--rw-r--r--   0 david     (1000) david     (1000)    23451 2022-02-22 14:27:38.000000 click-8.1.3/src/click/_termui_impl.py
--rw-r--r--   0 david     (1000) david     (1000)     1353 2022-02-22 14:27:38.000000 click-8.1.3/src/click/_textwrap.py
--rw-r--r--   0 david     (1000) david     (1000)     7860 2022-02-22 14:27:38.000000 click-8.1.3/src/click/_winconsole.py
--rw-r--r--   0 david     (1000) david     (1000)   112782 2022-04-28 17:25:00.000000 click-8.1.3/src/click/core.py
--rw-r--r--   0 david     (1000) david     (1000)    16350 2022-04-28 13:42:09.000000 click-8.1.3/src/click/decorators.py
--rw-r--r--   0 david     (1000) david     (1000)     9167 2022-03-25 22:09:06.000000 click-8.1.3/src/click/exceptions.py
--rw-r--r--   0 david     (1000) david     (1000)     9706 2022-02-22 14:27:38.000000 click-8.1.3/src/click/formatting.py
--rw-r--r--   0 david     (1000) david     (1000)     1961 2022-02-22 14:27:38.000000 click-8.1.3/src/click/globals.py
--rw-r--r--   0 david     (1000) david     (1000)    19044 2022-03-28 15:04:22.000000 click-8.1.3/src/click/parser.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-02-22 14:27:38.000000 click-8.1.3/src/click/py.typed
--rw-r--r--   0 david     (1000) david     (1000)    18018 2022-03-28 15:10:16.000000 click-8.1.3/src/click/shell_completion.py
--rw-r--r--   0 david     (1000) david     (1000)    28355 2022-03-19 18:11:13.000000 click-8.1.3/src/click/termui.py
--rw-r--r--   0 david     (1000) david     (1000)    16063 2022-03-25 22:09:06.000000 click-8.1.3/src/click/testing.py
--rw-r--r--   0 david     (1000) david     (1000)    35805 2022-03-31 20:53:23.000000 click-8.1.3/src/click/types.py
--rw-r--r--   0 david     (1000) david     (1000)    18682 2022-03-25 22:08:09.000000 click-8.1.3/src/click/utils.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.383730 click-8.1.3/src/click.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)     3133 2022-04-28 17:35:45.000000 click-8.1.3/src/click.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     2859 2022-04-28 17:35:45.000000 click-8.1.3/src/click.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2022-04-28 17:35:45.000000 click-8.1.3/src/click.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       88 2022-04-28 17:35:45.000000 click-8.1.3/src/click.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)        6 2022-04-28 17:35:45.000000 click-8.1.3/src/click.egg-info/top_level.txt
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-04-28 17:35:45.383730 click-8.1.3/tests/
--rw-r--r--   0 david     (1000) david     (1000)      569 2022-02-22 14:27:38.000000 click-8.1.3/tests/conftest.py
--rw-r--r--   0 david     (1000) david     (1000)    10506 2022-03-25 22:09:06.000000 click-8.1.3/tests/test_arguments.py
--rw-r--r--   0 david     (1000) david     (1000)    15452 2022-03-25 22:09:06.000000 click-8.1.3/tests/test_basic.py
--rw-r--r--   0 david     (1000) david     (1000)     5800 2022-03-28 13:47:17.000000 click-8.1.3/tests/test_chain.py
--rw-r--r--   0 david     (1000) david     (1000)     1087 2022-03-19 18:11:13.000000 click-8.1.3/tests/test_command_decorators.py
--rw-r--r--   0 david     (1000) david     (1000)    11017 2022-03-28 15:10:16.000000 click-8.1.3/tests/test_commands.py
--rw-r--r--   0 david     (1000) david     (1000)      307 2022-02-22 14:27:38.000000 click-8.1.3/tests/test_compat.py
--rw-r--r--   0 david     (1000) david     (1000)     8680 2022-03-28 15:10:16.000000 click-8.1.3/tests/test_context.py
--rw-r--r--   0 david     (1000) david     (1000)     3022 2021-10-08 16:57:05.000000 click-8.1.3/tests/test_custom_classes.py
--rw-r--r--   0 david     (1000) david     (1000)     1079 2021-10-08 16:57:05.000000 click-8.1.3/tests/test_defaults.py
--rw-r--r--   0 david     (1000) david     (1000)     8968 2022-03-17 22:17:41.000000 click-8.1.3/tests/test_formatting.py
--rw-r--r--   0 david     (1000) david     (1000)     1374 2022-02-22 14:27:38.000000 click-8.1.3/tests/test_imports.py
--rw-r--r--   0 david     (1000) david     (1000)     7932 2022-03-28 13:47:17.000000 click-8.1.3/tests/test_info_dict.py
--rw-r--r--   0 david     (1000) david     (1000)      956 2021-03-04 00:26:07.000000 click-8.1.3/tests/test_normalization.py
--rw-r--r--   0 david     (1000) david     (1000)    28669 2022-04-28 17:25:00.000000 click-8.1.3/tests/test_options.py
--rw-r--r--   0 david     (1000) david     (1000)      902 2022-03-28 15:10:16.000000 click-8.1.3/tests/test_parser.py
--rw-r--r--   0 david     (1000) david     (1000)    11256 2022-03-28 15:10:16.000000 click-8.1.3/tests/test_shell_completion.py
--rw-r--r--   0 david     (1000) david     (1000)    13894 2022-03-19 18:11:13.000000 click-8.1.3/tests/test_termui.py
--rw-r--r--   0 david     (1000) david     (1000)    10762 2022-02-22 14:27:38.000000 click-8.1.3/tests/test_testing.py
--rw-r--r--   0 david     (1000) david     (1000)     4206 2022-03-19 18:26:07.000000 click-8.1.3/tests/test_types.py
--rw-r--r--   0 david     (1000) david     (1000)    15915 2022-03-25 22:08:09.000000 click-8.1.3/tests/test_utils.py
--rw-r--r--   0 david     (1000) david     (1000)      533 2022-03-17 22:17:41.000000 click-8.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.659953 click-8.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    46244 2023-07-06 18:22:30.000000 click-8.1.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-06 18:22:30.000000 click-8.1.4/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-06 18:22:30.000000 click-8.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-06 18:22:39.659953 click-8.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-06 18:22:30.000000 click-8.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.643953 click-8.1.4/artwork/
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-06 18:22:30.000000 click-8.1.4/artwork/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-06 18:22:30.000000 click-8.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-06 18:22:30.000000 click-8.1.4/docs/_static/click-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-06 18:22:30.000000 click-8.1.4/docs/_static/click-logo-sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26081 2023-07-06 18:22:30.000000 click-8.1.4/docs/_static/click-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-07-06 18:22:30.000000 click-8.1.4/docs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-06 18:22:30.000000 click-8.1.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-06 18:22:30.000000 click-8.1.4/docs/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 18:22:30.000000 click-8.1.4/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18928 2023-07-06 18:22:30.000000 click-8.1.4/docs/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-07-06 18:22:30.000000 click-8.1.4/docs/complex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-06 18:22:30.000000 click-8.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-06 18:22:30.000000 click-8.1.4/docs/contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-06 18:22:30.000000 click-8.1.4/docs/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-06 18:22:30.000000 click-8.1.4/docs/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-06 18:22:30.000000 click-8.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 18:22:30.000000 click-8.1.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 18:22:30.000000 click-8.1.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    26719 2023-07-06 18:22:30.000000 click-8.1.4/docs/options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-06 18:22:30.000000 click-8.1.4/docs/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-06 18:22:30.000000 click-8.1.4/docs/prompts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-06 18:22:30.000000 click-8.1.4/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-06 18:22:30.000000 click-8.1.4/docs/setuptools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-06 18:22:30.000000 click-8.1.4/docs/shell-completion.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-06 18:22:30.000000 click-8.1.4/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-06 18:22:30.000000 click-8.1.4/docs/unicode-support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-06 18:22:30.000000 click-8.1.4/docs/upgrading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-06 18:22:30.000000 click-8.1.4/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-07-06 18:22:30.000000 click-8.1.4/docs/why.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-06 18:22:30.000000 click-8.1.4/docs/wincmd.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 18:22:30.000000 click-8.1.4/examples/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/aliases/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 18:22:30.000000 click-8.1.4/examples/aliases/README
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 18:22:30.000000 click-8.1.4/examples/aliases/aliases.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-06 18:22:30.000000 click-8.1.4/examples/aliases/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-06 18:22:30.000000 click-8.1.4/examples/aliases/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-06 18:22:30.000000 click-8.1.4/examples/colors/README
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 18:22:30.000000 click-8.1.4/examples/colors/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-06 18:22:30.000000 click-8.1.4/examples/colors/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/completion/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 18:22:30.000000 click-8.1.4/examples/completion/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-06 18:22:30.000000 click-8.1.4/examples/completion/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-06 18:22:30.000000 click-8.1.4/examples/completion/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/complex/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/complex/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/complex/complex/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/complex/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/complex/commands/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/complex/commands/cmd_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/imagepipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/README
+-rw-r--r--   0 runner    (1001) docker     (123)    51677 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/example01.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39106 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/example02.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/imagepipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/inout/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 18:22:30.000000 click-8.1.4/examples/inout/README
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-06 18:22:30.000000 click-8.1.4/examples/inout/inout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-06 18:22:30.000000 click-8.1.4/examples/inout/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/naval/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 18:22:30.000000 click-8.1.4/examples/naval/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-06 18:22:30.000000 click-8.1.4/examples/naval/naval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-06 18:22:30.000000 click-8.1.4/examples/naval/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-06 18:22:30.000000 click-8.1.4/examples/repo/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-06 18:22:30.000000 click-8.1.4/examples/repo/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-06 18:22:30.000000 click-8.1.4/examples/repo/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/termui/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-06 18:22:30.000000 click-8.1.4/examples/termui/README
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-06 18:22:30.000000 click-8.1.4/examples/termui/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-06 18:22:30.000000 click-8.1.4/examples/termui/termui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-06 18:22:30.000000 click-8.1.4/examples/validation/README
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-06 18:22:30.000000 click-8.1.4/examples/validation/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-06 18:22:30.000000 click-8.1.4/examples/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-06 18:22:30.000000 click-8.1.4/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-06 18:22:30.000000 click-8.1.4/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-06 18:22:30.000000 click-8.1.4/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-06 18:22:30.000000 click-8.1.4/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-06 18:22:30.000000 click-8.1.4/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-06 18:22:39.659953 click-8.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 18:22:30.000000 click-8.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.643953 click-8.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.655953 click-8.1.4/src/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-06 18:22:30.000000 click-8.1.4/src/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-07-06 18:22:30.000000 click-8.1.4/src/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-07-06 18:22:30.000000 click-8.1.4/src/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-06 18:22:30.000000 click-8.1.4/src/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-06 18:22:30.000000 click-8.1.4/src/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114086 2023-07-06 18:22:30.000000 click-8.1.4/src/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-07-06 18:22:30.000000 click-8.1.4/src/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-07-06 18:22:30.000000 click-8.1.4/src/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-06 18:22:30.000000 click-8.1.4/src/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-06 18:22:30.000000 click-8.1.4/src/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-07-06 18:22:30.000000 click-8.1.4/src/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:30.000000 click-8.1.4/src/click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-07-06 18:22:30.000000 click-8.1.4/src/click/shell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28324 2023-07-06 18:22:30.000000 click-8.1.4/src/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-07-06 18:22:30.000000 click-8.1.4/src/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36391 2023-07-06 18:22:30.000000 click-8.1.4/src/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-07-06 18:22:30.000000 click-8.1.4/src/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.655953 click-8.1.4/src/click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-06 18:22:39.000000 click-8.1.4/src/click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-06 18:22:39.000000 click-8.1.4/src/click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:22:39.000000 click-8.1.4/src/click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 18:22:39.000000 click-8.1.4/src/click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 18:22:39.000000 click-8.1.4/src/click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.659953 click-8.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-06 18:22:30.000000 click-8.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_command_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_custom_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_info_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28531 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_shell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16173 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-06 18:22:30.000000 click-8.1.4/tox.ini
```

### Comparing `click-8.1.3/CHANGES.rst` & `click-8.1.4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,44 @@
 .. currentmodule:: click
 
+Version 8.1.4
+-------------
+
+Released 2023-07-06
+
+-   Replace all ``typing.Dict`` occurrences to ``typing.MutableMapping`` for
+    parameter hints. :issue:`2255`
+-   Improve type hinting for decorators and give all generic types parameters.
+    :issue:`2398`
+-   Fix return value and type signature of `shell_completion.add_completion_class`
+    function. :pr:`2421`
+-   Bash version detection doesn't fail on Windows. :issue:`2461`
+-   Completion works if there is a dot (``.``) in the program name. :issue:`2166`
+-   Improve type annotations for pyright type checker. :issue:`2268`
+-   Improve responsiveness of ``click.clear()``. :issue:`2284`
+-   Improve command name detection when using Shiv or PEX. :issue:`2332`
+-   Avoid showing empty lines if command help text is empty. :issue:`2368`
+-   ZSH completion script works when loaded from ``fpath``. :issue:`2344`.
+-   ``EOFError`` and ``KeyboardInterrupt`` tracebacks are not suppressed when
+    ``standalone_mode`` is disabled. :issue:`2380`
+-   ``@group.command`` does not fail if the group was created with a custom
+    ``command_class``. :issue:`2416`
+-   ``multiple=True`` is allowed for flag options again and does not require
+    setting ``default=()``. :issue:`2246, 2292, 2295`
+-   Make the decorators returned by ``@argument()`` and ``@option()`` reusable when the
+    ``cls`` parameter is used. :issue:`2294`
+-   Don't fail when writing filenames to streams with strict errors. Replace invalid
+    bytes with the replacement character (``�``). :issue:`2395`
+-   Remove unnecessary attempt to detect MSYS2 environment. :issue:`2355`
+-   Remove outdated and unnecessary detection of App Engine environment. :pr:`2554`
+-   ``echo()`` does not fail when no streams are attached, such as with ``pythonw`` on
+    Windows. :issue:`2415`
+-   Argument with ``expose_value=False`` do not cause completion to fail. :issue:`2336`
+
+
 Version 8.1.3
 -------------
 
 Released 2022-04-28
 
 -   Use verbose form of ``typing.Callable`` for ``@command`` and
     ``@group``. :issue:`2255`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `click-8.1.3/LICENSE.rst` & `click-8.1.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/PKG-INFO` & `click-8.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: click
-Version: 8.1.3
+Version: 8.1.4
 Summary: Composable command line interface toolkit
 Home-page: https://palletsprojects.com/p/click/
-Author: Armin Ronacher
-Author-email: armin.ronacher@active-4.com
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://click.palletsprojects.com/
 Project-URL: Changes, https://click.palletsprojects.com/changes/
 Project-URL: Source Code, https://github.com/pallets/click/
 Project-URL: Issue Tracker, https://github.com/pallets/click/issues/
-Project-URL: Twitter, https://twitter.com/PalletsTeam
 Project-URL: Chat, https://discord.gg/pallets
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -98,12 +94,8 @@
 -----
 
 -   Documentation: https://click.palletsprojects.com/
 -   Changes: https://click.palletsprojects.com/changes/
 -   PyPI Releases: https://pypi.org/project/click/
 -   Source Code: https://github.com/pallets/click
 -   Issue Tracker: https://github.com/pallets/click/issues
--   Website: https://palletsprojects.com/p/click
--   Twitter: https://twitter.com/PalletsTeam
 -   Chat: https://discord.gg/pallets
-
-
```

### Comparing `click-8.1.3/README.rst` & `click-8.1.4/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -71,10 +71,8 @@
 -----
 
 -   Documentation: https://click.palletsprojects.com/
 -   Changes: https://click.palletsprojects.com/changes/
 -   PyPI Releases: https://pypi.org/project/click/
 -   Source Code: https://github.com/pallets/click
 -   Issue Tracker: https://github.com/pallets/click/issues
--   Website: https://palletsprojects.com/p/click
--   Twitter: https://twitter.com/PalletsTeam
 -   Chat: https://discord.gg/pallets
```

### Comparing `click-8.1.3/artwork/logo.svg` & `click-8.1.4/artwork/logo.svg`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/Makefile` & `click-8.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/_static/click-icon.png` & `click-8.1.4/docs/_static/click-icon.png`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/_static/click-logo-sidebar.png` & `click-8.1.4/docs/_static/click-logo-sidebar.png`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/_static/click-logo.png` & `click-8.1.4/docs/_static/click-logo.png`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/advanced.rst` & `click-8.1.4/docs/advanced.rst`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 as you have seen.  One common way to prevent a parameter from being passed
 to the callback is the `expose_value` argument to a parameter which hides
 the parameter entirely.  The way this works is that the :class:`Context`
 object has a :attr:`~Context.params` attribute which is a dictionary of
 all parameters.  Whatever is in that dictionary is being passed to the
 callbacks.
 
-This can be used to make up addition parameters.  Generally this pattern
+This can be used to make up additional parameters.  Generally this pattern
 is not recommended but in some cases it can be useful.  At the very least
 it's good to know that the system works this way.
 
 .. click:example::
 
     import urllib
 
@@ -278,15 +278,15 @@
 
 1.  You can use :func:`pass_context` to get the context passed.  This will
     only work if in addition to :attr:`~Context.ignore_unknown_options`
     you also set :attr:`~Context.allow_extra_args` as otherwise the
     command will abort with an error that there are leftover arguments.
     If you go with this solution, the extra arguments will be collected in
     :attr:`Context.args`.
-2.  You can attach a :func:`argument` with ``nargs`` set to `-1` which
+2.  You can attach an :func:`argument` with ``nargs`` set to `-1` which
     will eat up all leftover arguments.  In this case it's recommended to
     set the `type` to :data:`UNPROCESSED` to avoid any string processing
     on those arguments as otherwise they are forced into unicode strings
     automatically which is often not what you want.
 
 In the end you end up with something like this:
 
@@ -335,15 +335,15 @@
     for further processing.
 *   Depending on what you plan on doing you might have some success by
     disabling interspersed arguments
     (:attr:`~Context.allow_interspersed_args`) which instructs the parser
     to not allow arguments and options to be mixed.  Depending on your
     situation this might improve your results.
 
-Generally though the combinated handling of options and arguments from
+Generally though the combined handling of options and arguments from
 your own commands and commands from another application are discouraged
 and if you can avoid it, you should.  It's a much better idea to have
 everything below a subcommand be forwarded to another application than to
 handle some arguments yourself.
 
 
 Global Context Access
```

### Comparing `click-8.1.3/docs/api.rst` & `click-8.1.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/arguments.rst` & `click-8.1.4/docs/arguments.rst`

 * *Files 2% similar despite different names*

```diff
@@ -120,23 +120,17 @@
         invoke(inout, args=['hello.txt', '-'])
 
 File Path Arguments
 -------------------
 
 In the previous example, the files were opened immediately.  But what if
 we just want the filename?  The naïve way is to use the default string
-argument type.  However, remember that Click is Unicode-based, so the string
-will always be a Unicode value.  Unfortunately, filenames can be Unicode or
-bytes depending on which operating system is being used.  As such, the type
-is insufficient.
-
-Instead, you should be using the :class:`Path` type, which automatically
-handles this ambiguity.  Not only will it return either bytes or Unicode
-depending on what makes more sense, but it will also be able to do some
-basic checks for you such as existence checks.
+argument type. The :class:`Path` type has several checks available which raise nice
+errors if they fail, such as existence. Filenames in these error messages are formatted
+with :func:`format_filename`, so any undecodable bytes will be printed nicely.
 
 Example:
 
 .. click:example::
 
     @click.command()
     @click.argument('filename', type=click.Path(exists=True))
```

### Comparing `click-8.1.3/docs/commands.rst` & `click-8.1.4/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/conf.py` & `click-8.1.4/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 from pallets_sphinx_themes import get_version
 from pallets_sphinx_themes import ProjectLink
 
-import click._compat
-
-# compat until pallets-sphinx-themes is updated
-click._compat.text_type = str
-
 # Project --------------------------------------------------------------
 
 project = "Click"
 copyright = "2014 Pallets"
 author = "Pallets"
 release, version = get_version("Click")
 
@@ -34,16 +29,14 @@
 html_theme_options = {"index_sidebar_logo": False}
 html_context = {
     "project_links": [
         ProjectLink("Donate", "https://palletsprojects.com/donate"),
         ProjectLink("PyPI Releases", "https://pypi.org/project/click/"),
         ProjectLink("Source Code", "https://github.com/pallets/click/"),
         ProjectLink("Issue Tracker", "https://github.com/pallets/click/issues/"),
-        ProjectLink("Website", "https://palletsprojects.com/p/click"),
-        ProjectLink("Twitter", "https://twitter.com/PalletsTeam"),
         ProjectLink("Chat", "https://discord.gg/pallets"),
     ]
 }
 html_sidebars = {
     "index": ["project.html", "localtoc.html", "searchbox.html", "ethicalads.html"],
     "**": ["localtoc.html", "relations.html", "searchbox.html", "ethicalads.html"],
 }
```

### Comparing `click-8.1.3/docs/documentation.rst` & `click-8.1.4/docs/documentation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -81,16 +81,17 @@
 For more examples, see the examples in :doc:`/arguments`.
 
 
 Preventing Rewrapping
 ---------------------
 
 The default behavior of Click is to rewrap text based on the width of the
-terminal.  In some circumstances, this can become a problem. The main issue
-is when showing code examples, where newlines are significant.
+terminal, to a maximum 80 characters. In some circumstances, this can become
+a problem. The main issue is when showing code examples, where newlines are
+significant.
 
 Rewrapping can be disabled on a per-paragraph basis by adding a line with
 solely the ``\b`` escape marker in it.  This line will be removed from the
 help text and rewrapping will be disabled.
 
 Example:
 
@@ -116,14 +117,21 @@
 
 And what it looks like:
 
 .. click:run::
 
     invoke(cli, args=['--help'])
 
+To change the maximum width, pass ``max_content_width`` when calling the command.
+
+.. code-block:: python
+
+    cli(max_content_width=120)
+
+
 .. _doc-meta-variables:
 
 Truncating Help Texts
 ---------------------
 
 Click gets command help text from function docstrings.  However if you
 already use docstrings to document function arguments you may not want
@@ -205,14 +213,32 @@
 
 And what it looks like:
 
 .. click:run::
 
     invoke(cli, prog_name='repo.py')
 
+Command Epilog Help
+-------------------
+
+The help epilog is like the help string but it's printed at the end of the help
+page after everything else. Useful for showing example command usages or
+referencing additional help resources.
+
+.. click:example::
+
+    @click.command(epilog='Check out our docs at https://click.palletsprojects.com/ for more details')
+    def init():
+        """Initializes the repository."""
+
+And what it looks like:
+
+.. click:run::
+
+    invoke(init, prog_name='repo.py', args=['--help'])
 
 Help Parameter Customization
 ----------------------------
 
 .. versionadded:: 2.0
 
 The help parameter is implemented in Click in a very special manner.
```

### Comparing `click-8.1.3/docs/exceptions.rst` & `click-8.1.4/docs/exceptions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 Where are Errors Handled?
 -------------------------
 
 Click's main error handling is happening in :meth:`BaseCommand.main`.  In
 there it handles all subclasses of :exc:`ClickException` as well as the
 standard :exc:`EOFError` and :exc:`KeyboardInterrupt` exceptions.  The
-latter are internally translated into a :exc:`Abort`.
+latter are internally translated into an :exc:`Abort`.
 
 The logic applied is the following:
 
 1.  If an :exc:`EOFError` or :exc:`KeyboardInterrupt` happens, reraise it
     as :exc:`Abort`.
-2.  If an :exc:`ClickException` is raised, invoke the
+2.  If a :exc:`ClickException` is raised, invoke the
     :meth:`ClickException.show` method on it to display it and then exit
     the program with :attr:`ClickException.exit_code`.
 3.  If an :exc:`Abort` exception is raised print the string ``Aborted!``
     to standard error and exit the program with exit code ``1``.
-4.  if it goes through well, exit the program with exit code ``0``.
+4.  If it goes through well, exit the program with exit code ``0``.
 
 What if I don't want that?
 --------------------------
 
 Generally you always have the option to invoke the :meth:`invoke` method
 yourself.  For instance if you have a :class:`Command` you can invoke it
 manually like this::
```

### Comparing `click-8.1.3/docs/index.rst` & `click-8.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/make.bat` & `click-8.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/options.rst` & `click-8.1.4/docs/options.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/parameters.rst` & `click-8.1.4/docs/parameters.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/prompts.rst` & `click-8.1.4/docs/prompts.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/quickstart.rst` & `click-8.1.4/docs/quickstart.rst`

 * *Files 5% similar despite different names*

```diff
@@ -25,56 +25,37 @@
 compatibility, and it's unlikely that any serious application will have
 zero dependencies.  So what do you do if two or more of your projects have
 conflicting dependencies?
 
 Virtualenv to the rescue!  Virtualenv enables multiple side-by-side
 installations of Python, one for each project.  It doesn't actually
 install separate copies of Python, but it does provide a clever way to
-keep different project environments isolated.  Let's see how virtualenv
-works.
+keep different project environments isolated.
 
-If you are on Mac OS X or Linux::
-
-    $ pip install virtualenv --user
-
-One of these will probably install virtualenv on your system.  Maybe it's even
-in your package manager.  If you use Ubuntu, try::
-
-    $ sudo apt-get install python-virtualenv
-
-If you are on Windows (or none of the above methods worked) you must install
-``pip`` first.  For more information about this, see `installing pip`_.
-Once you have it installed, run the ``pip`` command from above, but without
-the `sudo` prefix.
-
-.. _installing pip: https://pip.readthedocs.io/en/latest/installing/
-
-Once you have virtualenv installed, just fire up a shell and create
-your own environment.  I usually create a project folder and a `venv`
-folder within::
+Create your project folder, then a virtualenv within it::
 
     $ mkdir myproject
     $ cd myproject
-    $ virtualenv venv
-    New python executable in venv/bin/python
-    Installing setuptools, pip............done.
+    $ python3 -m venv .venv
 
 Now, whenever you want to work on a project, you only have to activate the
 corresponding environment.  On OS X and Linux, do the following::
 
-    $ . venv/bin/activate
+    $ . .venv/bin/activate
+    (venv) $
 
 If you are a Windows user, the following command is for you::
 
-    $ venv\scripts\activate
+    > .venv\scripts\activate
+    (venv) >
 
 Either way, you should now be using your virtualenv (notice how the prompt of
 your shell has changed to show the active environment).
 
-And if you want to go back to the real world, use the following command::
+And if you want to stop using the virtualenv, use the following command::
 
     $ deactivate
 
 After doing this, the prompt of your shell should be as familiar as before.
 
 Now, let's move on. Enter the following command to get Click activated in your
 virtualenv::
```

### Comparing `click-8.1.3/docs/setuptools.rst` & `click-8.1.4/docs/setuptools.rst`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 ------------------
 
 To test the script, you can make a new virtualenv and then install your
 package:
 
 .. code-block:: console
 
-    $ virtualenv venv
-    $ . venv/bin/activate
+    $ python3 -m venv .venv
+    $ . .venv/bin/activate
     $ pip install --editable .
 
 Afterwards, your command should be available:
 
 .. click:run::
 
     invoke(cli, prog_name='yourscript')
```

### Comparing `click-8.1.3/docs/shell-completion.rst` & `click-8.1.4/docs/shell-completion.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/testing.rst` & `click-8.1.4/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/unicode-support.rst` & `click-8.1.4/docs/unicode-support.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/upgrading.rst` & `click-8.1.4/docs/upgrading.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/utils.rst` & `click-8.1.4/docs/utils.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/why.rst` & `click-8.1.4/docs/why.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/docs/wincmd.rst` & `click-8.1.4/docs/wincmd.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/aliases/aliases.py` & `click-8.1.4/examples/aliases/aliases.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/colors/colors.py` & `click-8.1.4/examples/colors/colors.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/completion/completion.py` & `click-8.1.4/examples/completion/completion.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/complex/complex/cli.py` & `click-8.1.4/examples/complex/complex/cli.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/imagepipe/example01.jpg` & `click-8.1.4/examples/imagepipe/example01.jpg`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/imagepipe/example02.jpg` & `click-8.1.4/examples/imagepipe/example02.jpg`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/imagepipe/imagepipe.py` & `click-8.1.4/examples/imagepipe/imagepipe.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/inout/inout.py` & `click-8.1.4/examples/inout/inout.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/naval/naval.py` & `click-8.1.4/examples/naval/naval.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/repo/repo.py` & `click-8.1.4/examples/repo/repo.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/termui/termui.py` & `click-8.1.4/examples/termui/termui.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/examples/validation/validation.py` & `click-8.1.4/examples/validation/validation.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/requirements/dev.txt` & `click-8.1.4/requirements/dev.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,57 +4,61 @@
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r docs.txt
 -r tests.txt
 -r typing.txt
+build==0.10.0
+    # via pip-tools
+cachetools==5.3.1
+    # via tox
 cfgv==3.3.1
     # via pre-commit
-click==8.1.2
+chardet==5.1.0
+    # via tox
+click==8.1.3
     # via
     #   pip-compile-multi
     #   pip-tools
-distlib==0.3.4
+colorama==0.4.6
+    # via tox
+distlib==0.3.6
     # via virtualenv
-filelock==3.6.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
-identify==2.5.0
+identify==2.5.24
     # via pre-commit
-nodeenv==1.6.0
+nodeenv==1.8.0
     # via pre-commit
-pep517==0.12.0
-    # via pip-tools
-pip-compile-multi==2.4.5
+pip-compile-multi==2.6.3
     # via -r requirements/dev.in
-pip-tools==6.6.0
+pip-tools==6.13.0
     # via pip-compile-multi
-platformdirs==2.5.2
-    # via virtualenv
-pre-commit==2.18.1
-    # via -r requirements/dev.in
-pyyaml==6.0
-    # via pre-commit
-six==1.16.0
+platformdirs==3.8.0
     # via
     #   tox
     #   virtualenv
-toml==0.10.2
-    # via
-    #   pre-commit
-    #   tox
-toposort==1.7
+pre-commit==3.3.3
+    # via -r requirements/dev.in
+pyproject-api==1.5.2
+    # via tox
+pyproject-hooks==1.0.0
+    # via build
+pyyaml==6.0
+    # via pre-commit
+toposort==1.10
     # via pip-compile-multi
-tox==3.25.0
+tox==4.6.3
     # via -r requirements/dev.in
-virtualenv==20.14.1
+virtualenv==20.23.1
     # via
     #   pre-commit
     #   tox
-wheel==0.37.1
+wheel==0.40.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `click-8.1.3/requirements/docs.txt` & `click-8.1.4/requirements/docs.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,68 @@
 # SHA1:34fd4ca6516e97c7348e6facdd9c4ebb68209d1c
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-alabaster==0.7.12
+alabaster==0.7.13
     # via sphinx
-babel==2.10.1
+babel==2.12.1
     # via sphinx
-certifi==2021.10.8
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.0.12
+charset-normalizer==3.1.0
     # via requests
-docutils==0.17.1
+docutils==0.18.1
     # via
     #   sphinx
     #   sphinx-tabs
-idna==3.3
+idna==3.4
     # via requests
-imagesize==1.3.0
+imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via sphinx
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via jinja2
-packaging==21.3
+packaging==23.1
     # via
     #   pallets-sphinx-themes
     #   sphinx
-pallets-sphinx-themes==2.0.2
+pallets-sphinx-themes==2.1.1
     # via -r requirements/docs.in
-pygments==2.12.0
+pygments==2.15.1
     # via
     #   sphinx
     #   sphinx-tabs
-pyparsing==3.0.8
-    # via packaging
-pytz==2022.1
-    # via babel
-requests==2.27.1
+requests==2.31.0
     # via sphinx
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==4.5.0
+sphinx==7.0.1
     # via
     #   -r requirements/docs.in
     #   pallets-sphinx-themes
     #   sphinx-issues
     #   sphinx-tabs
     #   sphinxcontrib-log-cabinet
 sphinx-issues==3.0.1
     # via -r requirements/docs.in
-sphinx-tabs==3.3.1
+sphinx-tabs==3.4.1
     # via -r requirements/docs.in
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-log-cabinet==1.0.1
     # via -r requirements/docs.in
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-urllib3==1.26.9
+urllib3==2.0.3
     # via requests
```

### Comparing `click-8.1.3/setup.cfg` & `click-8.1.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,17 @@
 url = https://palletsprojects.com/p/click/
 project_urls = 
 	Donate = https://palletsprojects.com/donate
 	Documentation = https://click.palletsprojects.com/
 	Changes = https://click.palletsprojects.com/changes/
 	Source Code = https://github.com/pallets/click/
 	Issue Tracker = https://github.com/pallets/click/issues/
-	Twitter = https://twitter.com/PalletsTeam
 	Chat = https://discord.gg/pallets
 license = BSD-3-Clause
 license_files = LICENSE.rst
-author = Armin Ronacher
-author_email = armin.ronacher@active-4.com
 maintainer = Pallets
 maintainer_email = contact@palletsprojects.com
 description = Composable command line interface toolkit
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -54,26 +51,30 @@
 [flake8]
 select = B, E, F, W, B9, ISC
 ignore = 
 	E203
 	E501
 	E722
 	W503
+	B905
+	B028
+	B907
 max-line-length = 80
 per-file-ignores = 
 	src/click/__init__.py: F401
 
 [mypy]
 files = src/click
 python_version = 3.7
 show_error_codes = True
 disallow_subclassing_any = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 disallow_incomplete_defs = True
+disallow_any_generics = True
 check_untyped_defs = True
 no_implicit_optional = True
 local_partial_types = True
 no_implicit_reexport = True
 strict_equality = True
 warn_redundant_casts = True
 warn_unused_configs = True
```

### Comparing `click-8.1.3/src/click/__init__.py` & `click-8.1.4/src/click/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,8 @@
 from .utils import echo as echo
 from .utils import format_filename as format_filename
 from .utils import get_app_dir as get_app_dir
 from .utils import get_binary_stream as get_binary_stream
 from .utils import get_text_stream as get_text_stream
 from .utils import open_file as open_file
 
-__version__ = "8.1.3"
+__version__ = "8.1.4"
```

### Comparing `click-8.1.3/src/click/_compat.py` & `click-8.1.4/src/click/_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,19 @@
 import os
 import re
 import sys
 import typing as t
 from weakref import WeakKeyDictionary
 
 CYGWIN = sys.platform.startswith("cygwin")
-MSYS2 = sys.platform.startswith("win") and ("GCC" in sys.version)
-# Determine local App Engine environment, per Google's own suggestion
-APP_ENGINE = "APPENGINE_RUNTIME" in os.environ and "Development/" in os.environ.get(
-    "SERVER_SOFTWARE", ""
-)
-WIN = sys.platform.startswith("win") and not APP_ENGINE and not MSYS2
+WIN = sys.platform.startswith("win")
 auto_wrap_for_ansi: t.Optional[t.Callable[[t.TextIO], t.TextIO]] = None
 _ansi_re = re.compile(r"\033\[[;?0-9]*[a-zA-Z]")
 
 
-def get_filesystem_encoding() -> str:
-    return sys.getfilesystemencoding() or sys.getdefaultencoding()
-
-
 def _make_text_stream(
     stream: t.BinaryIO,
     encoding: t.Optional[str],
     errors: t.Optional[str],
     force_readable: bool = False,
     force_writable: bool = False,
 ) -> t.TextIO:
@@ -46,15 +37,15 @@
     """Checks if a given encoding is ascii."""
     try:
         return codecs.lookup(encoding).name == "ascii"
     except LookupError:
         return False
 
 
-def get_best_encoding(stream: t.IO) -> str:
+def get_best_encoding(stream: t.IO[t.Any]) -> str:
     """Returns the default stream encoding if not found."""
     rv = getattr(stream, "encoding", None) or sys.getdefaultencoding()
     if is_ascii_encoding(rv):
         return "utf-8"
     return rv
 
 
@@ -149,37 +140,37 @@
         try:
             self._stream.seek(self._stream.tell())
         except Exception:
             return False
         return True
 
 
-def _is_binary_reader(stream: t.IO, default: bool = False) -> bool:
+def _is_binary_reader(stream: t.IO[t.Any], default: bool = False) -> bool:
     try:
         return isinstance(stream.read(0), bytes)
     except Exception:
         return default
         # This happens in some cases where the stream was already
         # closed.  In this case, we assume the default.
 
 
-def _is_binary_writer(stream: t.IO, default: bool = False) -> bool:
+def _is_binary_writer(stream: t.IO[t.Any], default: bool = False) -> bool:
     try:
         stream.write(b"")
     except Exception:
         try:
             stream.write("")
             return False
         except Exception:
             pass
         return default
     return True
 
 
-def _find_binary_reader(stream: t.IO) -> t.Optional[t.BinaryIO]:
+def _find_binary_reader(stream: t.IO[t.Any]) -> t.Optional[t.BinaryIO]:
     # We need to figure out if the given stream is already binary.
     # This can happen because the official docs recommend detaching
     # the streams to get binary streams.  Some code might do this, so
     # we need to deal with this case explicitly.
     if _is_binary_reader(stream, False):
         return t.cast(t.BinaryIO, stream)
 
@@ -189,15 +180,15 @@
     # actually binary in case it's closed.
     if buf is not None and _is_binary_reader(buf, True):
         return t.cast(t.BinaryIO, buf)
 
     return None
 
 
-def _find_binary_writer(stream: t.IO) -> t.Optional[t.BinaryIO]:
+def _find_binary_writer(stream: t.IO[t.Any]) -> t.Optional[t.BinaryIO]:
     # We need to figure out if the given stream is already binary.
     # This can happen because the official docs recommend detaching
     # the streams to get binary streams.  Some code might do this, so
     # we need to deal with this case explicitly.
     if _is_binary_writer(stream, False):
         return t.cast(t.BinaryIO, stream)
 
@@ -237,19 +228,19 @@
     """
     return _is_compat_stream_attr(
         stream, "encoding", encoding
     ) and _is_compat_stream_attr(stream, "errors", errors)
 
 
 def _force_correct_text_stream(
-    text_stream: t.IO,
+    text_stream: t.IO[t.Any],
     encoding: t.Optional[str],
     errors: t.Optional[str],
-    is_binary: t.Callable[[t.IO, bool], bool],
-    find_binary: t.Callable[[t.IO], t.Optional[t.BinaryIO]],
+    is_binary: t.Callable[[t.IO[t.Any], bool], bool],
+    find_binary: t.Callable[[t.IO[t.Any]], t.Optional[t.BinaryIO]],
     force_readable: bool = False,
     force_writable: bool = False,
 ) -> t.TextIO:
     if is_binary(text_stream, False):
         binary_reader = t.cast(t.BinaryIO, text_stream)
     else:
         text_stream = t.cast(t.TextIO, text_stream)
@@ -283,15 +274,15 @@
         errors,
         force_readable=force_readable,
         force_writable=force_writable,
     )
 
 
 def _force_correct_text_reader(
-    text_reader: t.IO,
+    text_reader: t.IO[t.Any],
     encoding: t.Optional[str],
     errors: t.Optional[str],
     force_readable: bool = False,
 ) -> t.TextIO:
     return _force_correct_text_stream(
         text_reader,
         encoding,
@@ -299,15 +290,15 @@
         _is_binary_reader,
         _find_binary_reader,
         force_readable=force_readable,
     )
 
 
 def _force_correct_text_writer(
-    text_writer: t.IO,
+    text_writer: t.IO[t.Any],
     encoding: t.Optional[str],
     errors: t.Optional[str],
     force_writable: bool = False,
 ) -> t.TextIO:
     return _force_correct_text_stream(
         text_writer,
         encoding,
@@ -363,34 +354,35 @@
     rv = _get_windows_console_stream(sys.stderr, encoding, errors)
     if rv is not None:
         return rv
     return _force_correct_text_writer(sys.stderr, encoding, errors, force_writable=True)
 
 
 def _wrap_io_open(
-    file: t.Union[str, os.PathLike, int],
+    file: t.Union[str, "os.PathLike[str]", int],
     mode: str,
     encoding: t.Optional[str],
     errors: t.Optional[str],
-) -> t.IO:
+) -> t.IO[t.Any]:
     """Handles not passing ``encoding`` and ``errors`` in binary mode."""
     if "b" in mode:
         return open(file, mode)
 
     return open(file, mode, encoding=encoding, errors=errors)
 
 
 def open_stream(
-    filename: str,
+    filename: "t.Union[str, os.PathLike[str]]",
     mode: str = "r",
     encoding: t.Optional[str] = None,
     errors: t.Optional[str] = "strict",
     atomic: bool = False,
-) -> t.Tuple[t.IO, bool]:
+) -> t.Tuple[t.IO[t.Any], bool]:
     binary = "b" in mode
+    filename = os.fspath(filename)
 
     # Standard streams first. These are simple because they ignore the
     # atomic flag. Use fsdecode to handle Path("-").
     if os.fsdecode(filename) == "-":
         if any(m in mode for m in ["w", "a", "x"]):
             if binary:
                 return get_binary_stdout(), False
@@ -452,19 +444,19 @@
             raise
 
     if perm is not None:
         os.chmod(tmp_filename, perm)  # in case perm includes bits in umask
 
     f = _wrap_io_open(fd, mode, encoding, errors)
     af = _AtomicFile(f, tmp_filename, os.path.realpath(filename))
-    return t.cast(t.IO, af), True
+    return t.cast(t.IO[t.Any], af), True
 
 
 class _AtomicFile:
-    def __init__(self, f: t.IO, tmp_filename: str, real_filename: str) -> None:
+    def __init__(self, f: t.IO[t.Any], tmp_filename: str, real_filename: str) -> None:
         self._f = f
         self._tmp_filename = tmp_filename
         self._real_filename = real_filename
         self.closed = False
 
     @property
     def name(self) -> str:
@@ -479,34 +471,34 @@
 
     def __getattr__(self, name: str) -> t.Any:
         return getattr(self._f, name)
 
     def __enter__(self) -> "_AtomicFile":
         return self
 
-    def __exit__(self, exc_type, exc_value, tb):  # type: ignore
+    def __exit__(self, exc_type: t.Optional[t.Type[BaseException]], *_: t.Any) -> None:
         self.close(delete=exc_type is not None)
 
     def __repr__(self) -> str:
         return repr(self._f)
 
 
 def strip_ansi(value: str) -> str:
     return _ansi_re.sub("", value)
 
 
-def _is_jupyter_kernel_output(stream: t.IO) -> bool:
+def _is_jupyter_kernel_output(stream: t.IO[t.Any]) -> bool:
     while isinstance(stream, (_FixupStream, _NonClosingTextIOWrapper)):
         stream = stream._stream
 
     return stream.__class__.__module__.startswith("ipykernel.")
 
 
 def should_strip_ansi(
-    stream: t.Optional[t.IO] = None, color: t.Optional[bool] = None
+    stream: t.Optional[t.IO[t.Any]] = None, color: t.Optional[bool] = None
 ) -> bool:
     if color is None:
         if stream is None:
             stream = sys.stdin
         return not isatty(stream) and not _is_jupyter_kernel_output(stream)
     return not color
 
@@ -560,40 +552,45 @@
             pass
 
         return rv
 
 else:
 
     def _get_argv_encoding() -> str:
-        return getattr(sys.stdin, "encoding", None) or get_filesystem_encoding()
+        return getattr(sys.stdin, "encoding", None) or sys.getfilesystemencoding()
 
     def _get_windows_console_stream(
         f: t.TextIO, encoding: t.Optional[str], errors: t.Optional[str]
     ) -> t.Optional[t.TextIO]:
         return None
 
 
 def term_len(x: str) -> int:
     return len(strip_ansi(x))
 
 
-def isatty(stream: t.IO) -> bool:
+def isatty(stream: t.IO[t.Any]) -> bool:
     try:
         return stream.isatty()
     except Exception:
         return False
 
 
 def _make_cached_stream_func(
-    src_func: t.Callable[[], t.TextIO], wrapper_func: t.Callable[[], t.TextIO]
-) -> t.Callable[[], t.TextIO]:
+    src_func: t.Callable[[], t.Optional[t.TextIO]],
+    wrapper_func: t.Callable[[], t.TextIO],
+) -> t.Callable[[], t.Optional[t.TextIO]]:
     cache: t.MutableMapping[t.TextIO, t.TextIO] = WeakKeyDictionary()
 
-    def func() -> t.TextIO:
+    def func() -> t.Optional[t.TextIO]:
         stream = src_func()
+
+        if stream is None:
+            return None
+
         try:
             rv = cache.get(stream)
         except Exception:
             rv = None
         if rv is not None:
             return rv
         rv = wrapper_func()
```

### Comparing `click-8.1.3/src/click/_termui_impl.py` & `click-8.1.4/src/click/_termui_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import contextlib
 import math
 import os
 import sys
 import time
 import typing as t
 from gettext import gettext as _
+from io import StringIO
+from types import TracebackType
 
 from ._compat import _default_text_stdout
 from ._compat import CYGWIN
 from ._compat import get_best_encoding
 from ._compat import isatty
 from ._compat import open_stream
 from ._compat import strip_ansi
@@ -55,54 +57,68 @@
         self.empty_char = empty_char
         self.bar_template = bar_template
         self.info_sep = info_sep
         self.show_eta = show_eta
         self.show_percent = show_percent
         self.show_pos = show_pos
         self.item_show_func = item_show_func
-        self.label = label or ""
+        self.label: str = label or ""
+
         if file is None:
             file = _default_text_stdout()
+
+            # There are no standard streams attached to write to. For example,
+            # pythonw on Windows.
+            if file is None:
+                file = StringIO()
+
         self.file = file
         self.color = color
         self.update_min_steps = update_min_steps
         self._completed_intervals = 0
-        self.width = width
-        self.autowidth = width == 0
+        self.width: int = width
+        self.autowidth: bool = width == 0
 
         if length is None:
             from operator import length_hint
 
             length = length_hint(iterable, -1)
 
             if length == -1:
                 length = None
         if iterable is None:
             if length is None:
                 raise TypeError("iterable or length is required")
             iterable = t.cast(t.Iterable[V], range(length))
-        self.iter = iter(iterable)
+        self.iter: t.Iterable[V] = iter(iterable)
         self.length = length
         self.pos = 0
         self.avg: t.List[float] = []
+        self.last_eta: float
+        self.start: float
         self.start = self.last_eta = time.time()
-        self.eta_known = False
-        self.finished = False
+        self.eta_known: bool = False
+        self.finished: bool = False
         self.max_width: t.Optional[int] = None
-        self.entered = False
+        self.entered: bool = False
         self.current_item: t.Optional[V] = None
-        self.is_hidden = not isatty(self.file)
+        self.is_hidden: bool = not isatty(self.file)
         self._last_line: t.Optional[str] = None
 
-    def __enter__(self) -> "ProgressBar":
+    def __enter__(self) -> "ProgressBar[V]":
         self.entered = True
         self.render_progress()
         return self
 
-    def __exit__(self, exc_type, exc_value, tb):  # type: ignore
+    def __exit__(
+        self,
+        exc_type: t.Optional[t.Type[BaseException]],
+        exc_value: t.Optional[BaseException],
+        tb: t.Optional[TracebackType],
+    ) -> None:
         self.render_finish()
 
     def __iter__(self) -> t.Iterator[V]:
         if not self.entered:
             raise RuntimeError("You need to use progress bars in a with block.")
         self.render_progress()
         return self.generator()
@@ -340,14 +356,20 @@
             self.finish()
             self.render_progress()
 
 
 def pager(generator: t.Iterable[str], color: t.Optional[bool] = None) -> None:
     """Decide what method to use for paging through text."""
     stdout = _default_text_stdout()
+
+    # There are no standard streams attached to write to. For example,
+    # pythonw on Windows.
+    if stdout is None:
+        stdout = StringIO()
+
     if not isatty(sys.stdin) or not isatty(stdout):
         return _nullpager(stdout, generator, color)
     pager_cmd = (os.environ.get("PAGER", None) or "").strip()
     if pager_cmd:
         if WIN:
             return _tempfilepager(generator, pager_cmd, color)
         return _pipepager(generator, pager_cmd, color)
```

### Comparing `click-8.1.3/src/click/_textwrap.py` & `click-8.1.4/src/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/src/click/_winconsole.py` & `click-8.1.4/src/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/src/click/core.py` & `click-8.1.4/src/click/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import inspect
 import os
 import sys
 import typing as t
 from collections import abc
 from contextlib import contextmanager
 from contextlib import ExitStack
-from functools import partial
 from functools import update_wrapper
 from gettext import gettext as _
 from gettext import ngettext
 from itertools import repeat
+from types import TracebackType
 
 from . import types
 from .exceptions import Abort
 from .exceptions import BadParameter
 from .exceptions import ClickException
 from .exceptions import Exit
 from .exceptions import MissingParameter
@@ -260,15 +260,15 @@
     def __init__(
         self,
         command: "Command",
         parent: t.Optional["Context"] = None,
         info_name: t.Optional[str] = None,
         obj: t.Optional[t.Any] = None,
         auto_envvar_prefix: t.Optional[str] = None,
-        default_map: t.Optional[t.Dict[str, t.Any]] = None,
+        default_map: t.Optional[t.MutableMapping[str, t.Any]] = None,
         terminal_width: t.Optional[int] = None,
         max_content_width: t.Optional[int] = None,
         resilient_parsing: bool = False,
         allow_extra_args: t.Optional[bool] = None,
         allow_interspersed_args: t.Optional[bool] = None,
         ignore_unknown_options: t.Optional[bool] = None,
         help_option_names: t.Optional[t.List[str]] = None,
@@ -307,15 +307,15 @@
             default_map is None
             and info_name is not None
             and parent is not None
             and parent.default_map is not None
         ):
             default_map = parent.default_map.get(info_name)
 
-        self.default_map: t.Optional[t.Dict[str, t.Any]] = default_map
+        self.default_map: t.Optional[t.MutableMapping[str, t.Any]] = default_map
 
         #: This flag indicates if a subcommand is going to be executed. A
         #: group callback can use this information to figure out if it's
         #: being executed directly or because the execution flow passes
         #: onwards to a subcommand. By default it's None, but it can be
         #: the name of the subcommand to execute.
         #:
@@ -451,15 +451,20 @@
         }
 
     def __enter__(self) -> "Context":
         self._depth += 1
         push_context(self)
         return self
 
-    def __exit__(self, exc_type, exc_value, tb):  # type: ignore
+    def __exit__(
+        self,
+        exc_type: t.Optional[t.Type[BaseException]],
+        exc_value: t.Optional[BaseException],
+        tb: t.Optional[TracebackType],
+    ) -> None:
         self._depth -= 1
         if self._depth == 0:
             self.close()
         pop_context()
 
     @contextmanager
     def scope(self, cleanup: bool = True) -> t.Iterator["Context"]:
@@ -702,20 +707,38 @@
         """Create a new context of the same type as this context, but
         for a new command.
 
         :meta private:
         """
         return type(self)(command, info_name=command.name, parent=self)
 
+    @t.overload
     def invoke(
         __self,  # noqa: B902
-        __callback: t.Union["Command", t.Callable[..., t.Any]],
+        __callback: "t.Callable[..., V]",
+        *args: t.Any,
+        **kwargs: t.Any,
+    ) -> V:
+        ...
+
+    @t.overload
+    def invoke(
+        __self,  # noqa: B902
+        __callback: "Command",
         *args: t.Any,
         **kwargs: t.Any,
     ) -> t.Any:
+        ...
+
+    def invoke(
+        __self,  # noqa: B902
+        __callback: t.Union["Command", "t.Callable[..., V]"],
+        *args: t.Any,
+        **kwargs: t.Any,
+    ) -> t.Union[t.Any, V]:
         """Invokes a command callback in exactly the way it expects.  There
         are two ways to invoke this method:
 
         1.  the first argument can be a callback and all other arguments and
             keyword arguments are forwarded directly to the function.
         2.  the first argument is a click command object.  In that case all
             arguments are forwarded as well but proper click parameters
@@ -735,15 +758,15 @@
             other_cmd = __callback
 
             if other_cmd.callback is None:
                 raise TypeError(
                     "The given command does not have a callback that can be invoked."
                 )
             else:
-                __callback = other_cmd.callback
+                __callback = t.cast("t.Callable[..., V]", other_cmd.callback)
 
             ctx = __self._make_sub_context(other_cmd)
 
             for param in other_cmd.params:
                 if param.name not in kwargs and param.expose_value:
                     kwargs[param.name] = param.type_cast_value(  # type: ignore
                         ctx, param.get_default(ctx)
@@ -840,27 +863,27 @@
     allow_interspersed_args = True
     #: the default for the :attr:`Context.ignore_unknown_options` flag.
     ignore_unknown_options = False
 
     def __init__(
         self,
         name: t.Optional[str],
-        context_settings: t.Optional[t.Dict[str, t.Any]] = None,
+        context_settings: t.Optional[t.MutableMapping[str, t.Any]] = None,
     ) -> None:
         #: the name the command thinks it has.  Upon registering a command
         #: on a :class:`Group` the group will default the command name
         #: with this information.  You should instead use the
         #: :class:`Context`\'s :attr:`~Context.info_name` attribute.
         self.name = name
 
         if context_settings is None:
             context_settings = {}
 
         #: an optional dictionary with defaults passed to the context.
-        self.context_settings: t.Dict[str, t.Any] = context_settings
+        self.context_settings: t.MutableMapping[str, t.Any] = context_settings
 
     def to_info_dict(self, ctx: Context) -> t.Dict[str, t.Any]:
         """Gather information that could be useful for a tool generating
         user-facing documentation. This traverses the entire structure
         below this command.
 
         Use :meth:`click.Context.to_info_dict` to traverse the entire
@@ -894,15 +917,15 @@
 
         To quickly customize the context class used without overriding
         this method, set the :attr:`context_class` attribute.
 
         :param info_name: the info name for this invocation.  Generally this
                           is the most descriptive name for the script or
                           command.  For the toplevel script it's usually
-                          the name of the script, for commands below it it's
+                          the name of the script, for commands below it's
                           the name of the command.
         :param args: the arguments to parse as list of strings.
         :param parent: the parent context if available.
         :param extra: extra keyword arguments forwarded to the context
                       constructor.
 
         .. versionchanged:: 8.0
@@ -927,15 +950,15 @@
         """
         raise NotImplementedError("Base commands do not know how to parse arguments.")
 
     def invoke(self, ctx: Context) -> t.Any:
         """Given a context, this invokes the command.  The default
         implementation is raising a not implemented error.
         """
-        raise NotImplementedError("Base commands are not invokable by default")
+        raise NotImplementedError("Base commands are not invocable by default")
 
     def shell_complete(self, ctx: Context, incomplete: str) -> t.List["CompletionItem"]:
         """Return a list of completions for the incomplete value. Looks
         at the names of chained multi-commands.
 
         Any command could be part of a chained multi-command, so sibling
         commands are valid at any point during command completion. Other
@@ -1059,17 +1082,17 @@
                     # note that `rv` may actually contain data like "1" which
                     # has obvious effects
                     # more subtle case: `rv=[None, None]` can come out of
                     # chained commands which all returned `None` -- so it's not
                     # even always obvious that `rv` indicates success/failure
                     # by its truthiness/falsiness
                     ctx.exit()
-            except (EOFError, KeyboardInterrupt):
+            except (EOFError, KeyboardInterrupt) as e:
                 echo(file=sys.stderr)
-                raise Abort() from None
+                raise Abort() from e
             except ClickException as e:
                 if not standalone_mode:
                     raise
                 e.show()
                 sys.exit(e.exit_code)
             except OSError as e:
                 if e.errno == errno.EPIPE:
@@ -1095,29 +1118,33 @@
             if not standalone_mode:
                 raise
             echo(_("Aborted!"), file=sys.stderr)
             sys.exit(1)
 
     def _main_shell_completion(
         self,
-        ctx_args: t.Dict[str, t.Any],
+        ctx_args: t.MutableMapping[str, t.Any],
         prog_name: str,
         complete_var: t.Optional[str] = None,
     ) -> None:
         """Check if the shell is asking for tab completion, process
         that, then exit early. Called from :meth:`main` before the
         program is invoked.
 
         :param prog_name: Name of the executable in the shell.
         :param complete_var: Name of the environment variable that holds
             the completion instruction. Defaults to
             ``_{PROG_NAME}_COMPLETE``.
+
+        .. versionchanged:: 8.2.0
+            Dots (``.``) in ``prog_name`` are replaced with underscores (``_``).
         """
         if complete_var is None:
-            complete_var = f"_{prog_name}_COMPLETE".replace("-", "_").upper()
+            complete_name = prog_name.replace("-", "_").replace(".", "_")
+            complete_var = f"_{complete_name}_COMPLETE".upper()
 
         instruction = os.environ.get(complete_var)
 
         if not instruction:
             return
 
         from .shell_completion import shell_complete
@@ -1171,15 +1198,15 @@
     .. versionchanged:: 2.0
         Added the ``context_settings`` parameter.
     """
 
     def __init__(
         self,
         name: t.Optional[str],
-        context_settings: t.Optional[t.Dict[str, t.Any]] = None,
+        context_settings: t.Optional[t.MutableMapping[str, t.Any]] = None,
         callback: t.Optional[t.Callable[..., t.Any]] = None,
         params: t.Optional[t.List["Parameter"]] = None,
         help: t.Optional[str] = None,
         epilog: t.Optional[str] = None,
         short_help: t.Optional[str] = None,
         options_metavar: t.Optional[str] = "[OPTIONS]",
         add_help_option: bool = True,
@@ -1329,21 +1356,24 @@
         self.format_usage(ctx, formatter)
         self.format_help_text(ctx, formatter)
         self.format_options(ctx, formatter)
         self.format_epilog(ctx, formatter)
 
     def format_help_text(self, ctx: Context, formatter: HelpFormatter) -> None:
         """Writes the help text to the formatter if it exists."""
-        text = self.help if self.help is not None else ""
+        if self.help is not None:
+            # truncate the help text to the first form feed
+            text = inspect.cleandoc(self.help).partition("\f")[0]
+        else:
+            text = ""
 
         if self.deprecated:
             text = _("(Deprecated) {text}").format(text=text)
 
         if text:
-            text = inspect.cleandoc(text).partition("\f")[0]
             formatter.write_paragraph()
 
             with formatter.indentation():
                 formatter.write_text(text)
 
     def format_options(self, ctx: Context, formatter: HelpFormatter) -> None:
         """Writes all the options into the formatter if they exist."""
@@ -1458,14 +1488,15 @@
     :param chain: if this is set to `True` chaining of multiple subcommands
                   is enabled.  This restricts the form of commands in that
                   they cannot have optional arguments but it allows
                   multiple commands to be chained together.
     :param result_callback: The result callback to attach to this multi
         command. This can be set or changed later with the
         :meth:`result_callback` decorator.
+    :param attrs: Other command arguments described in :class:`Command`.
     """
 
     allow_extra_args = True
     allow_interspersed_args = False
 
     def __init__(
         self,
@@ -1565,15 +1596,15 @@
             old_callback = self._result_callback
 
             if old_callback is None or replace:
                 self._result_callback = f
                 return f
 
             def function(__value, *args, **kwargs):  # type: ignore
-                inner = old_callback(__value, *args, **kwargs)  # type: ignore
+                inner = old_callback(__value, *args, **kwargs)
                 return f(inner, *args, **kwargs)
 
             self._result_callback = rv = update_wrapper(t.cast(F, function), f)
             return rv
 
         return decorator
 
@@ -1756,15 +1787,15 @@
         Can also be a list of :class:`Command`, which will use
         :attr:`Command.name` to create the dict.
     :param attrs: Other command arguments described in
         :class:`MultiCommand`, :class:`Command`, and
         :class:`BaseCommand`.
 
     .. versionchanged:: 8.0
-        The ``commmands`` argument can be a list of command objects.
+        The ``commands`` argument can be a list of command objects.
     """
 
     #: If set, this is used by the group's :meth:`command` decorator
     #: as the default :class:`Command` class. This is useful to make all
     #: subcommands use a custom command class.
     #:
     #: .. versionadded:: 8.0
@@ -1782,26 +1813,28 @@
     #: .. versionadded:: 8.0
     group_class: t.Optional[t.Union[t.Type["Group"], t.Type[type]]] = None
     # Literal[type] isn't valid, so use Type[type]
 
     def __init__(
         self,
         name: t.Optional[str] = None,
-        commands: t.Optional[t.Union[t.Dict[str, Command], t.Sequence[Command]]] = None,
+        commands: t.Optional[
+            t.Union[t.MutableMapping[str, Command], t.Sequence[Command]]
+        ] = None,
         **attrs: t.Any,
     ) -> None:
         super().__init__(name, **attrs)
 
         if commands is None:
             commands = {}
         elif isinstance(commands, abc.Sequence):
             commands = {c.name: c for c in commands if c.name is not None}
 
         #: The registered subcommands by their exported names.
-        self.commands: t.Dict[str, Command] = commands
+        self.commands: t.MutableMapping[str, Command] = commands
 
     def add_command(self, cmd: Command, name: t.Optional[str] = None) -> None:
         """Registers another :class:`Command` with this group.  If the name
         is not provided, the name of the command is used.
         """
         name = name or cmd.name
         if name is None:
@@ -1834,26 +1867,26 @@
             This decorator can be applied without parentheses.
 
         .. versionchanged:: 8.0
             Added the :attr:`command_class` attribute.
         """
         from .decorators import command
 
-        if self.command_class and kwargs.get("cls") is None:
-            kwargs["cls"] = self.command_class
-
-        func: t.Optional[t.Callable] = None
+        func: t.Optional[t.Callable[..., t.Any]] = None
 
         if args and callable(args[0]):
             assert (
                 len(args) == 1 and not kwargs
             ), "Use 'command(**kwargs)(callable)' to provide arguments."
             (func,) = args
             args = ()
 
+        if self.command_class and kwargs.get("cls") is None:
+            kwargs["cls"] = self.command_class
+
         def decorator(f: t.Callable[..., t.Any]) -> Command:
             cmd: Command = command(*args, **kwargs)(f)
             self.add_command(cmd)
             return cmd
 
         if func is not None:
             return decorator(func)
@@ -1885,15 +1918,15 @@
             This decorator can be applied without parentheses.
 
         .. versionchanged:: 8.0
             Added the :attr:`group_class` attribute.
         """
         from .decorators import group
 
-        func: t.Optional[t.Callable] = None
+        func: t.Optional[t.Callable[..., t.Any]] = None
 
         if args and callable(args[0]):
             assert (
                 len(args) == 1 and not kwargs
             ), "Use 'group(**kwargs)(callable)' to provide arguments."
             (func,) = args
             args = ()
@@ -1922,14 +1955,17 @@
 
 
 class CommandCollection(MultiCommand):
     """A command collection is a multi command that merges multiple multi
     commands together into one.  This is a straightforward implementation
     that accepts a list of different multi commands as sources and
     provides all the commands for each of them.
+
+    See :class:`MultiCommand` and :class:`Command` for the description of
+    ``name`` and ``attrs``.
     """
 
     def __init__(
         self,
         name: t.Optional[str] = None,
         sources: t.Optional[t.List[MultiCommand]] = None,
         **attrs: t.Any,
@@ -1981,15 +2017,15 @@
 
     Some settings are supported by both options and arguments.
 
     :param param_decls: the parameter declarations for this option or
                         argument.  This is a list of flags or argument
                         names.
     :param type: the type that should be used.  Either a :class:`ParamType`
-                 or a Python type.  The later is converted into the former
+                 or a Python type.  The latter is converted into the former
                  automatically if supported.
     :param required: controls if this is optional or not.
     :param default: the default value if omitted.  This can also be a callable,
                     in which case it's invoked when the default is needed
                     without any arguments.
     :param callback: A function to further process or validate the value
         after type conversion. It is called as ``f(ctx, param, value)``
@@ -2065,18 +2101,21 @@
         shell_complete: t.Optional[
             t.Callable[
                 [Context, "Parameter", str],
                 t.Union[t.List["CompletionItem"], t.List[str]],
             ]
         ] = None,
     ) -> None:
+        self.name: t.Optional[str]
+        self.opts: t.List[str]
+        self.secondary_opts: t.List[str]
         self.name, self.opts, self.secondary_opts = self._parse_decls(
             param_decls or (), expose_value
         )
-        self.type = types.convert_type(type, default)
+        self.type: types.ParamType = types.convert_type(type, default)
 
         # Default nargs to what the type tells us if we have that
         # information available.
         if nargs is None:
             if self.type.is_composite:
                 nargs = self.type.arity
             else:
@@ -2256,37 +2295,38 @@
     def type_cast_value(self, ctx: Context, value: t.Any) -> t.Any:
         """Convert and validate a value against the option's
         :attr:`type`, :attr:`multiple`, and :attr:`nargs`.
         """
         if value is None:
             return () if self.multiple or self.nargs == -1 else None
 
-        def check_iter(value: t.Any) -> t.Iterator:
+        def check_iter(value: t.Any) -> t.Iterator[t.Any]:
             try:
                 return _check_iter(value)
             except TypeError:
                 # This should only happen when passing in args manually,
                 # the parser should construct an iterable when parsing
                 # the command line.
                 raise BadParameter(
                     _("Value must be an iterable."), ctx=ctx, param=self
                 ) from None
 
         if self.nargs == 1 or self.type.is_composite:
-            convert: t.Callable[[t.Any], t.Any] = partial(
-                self.type, param=self, ctx=ctx
-            )
+
+            def convert(value: t.Any) -> t.Any:
+                return self.type(value, param=self, ctx=ctx)
+
         elif self.nargs == -1:
 
-            def convert(value: t.Any) -> t.Tuple:
+            def convert(value: t.Any) -> t.Any:  # t.Tuple[t.Any, ...]
                 return tuple(self.type(x, self, ctx) for x in check_iter(value))
 
         else:  # nargs > 1
 
-            def convert(value: t.Any) -> t.Tuple:
+            def convert(value: t.Any) -> t.Any:  # t.Tuple[t.Any, ...]
                 value = tuple(check_iter(value))
 
                 if len(value) != self.nargs:
                     raise BadParameter(
                         ngettext(
                             "Takes {nargs} values but 1 was given.",
                             "Takes {nargs} values but {len} were given.",
@@ -2445,14 +2485,15 @@
     :param count: this flag makes an option increment an integer.
     :param allow_from_autoenv: if this is enabled then the value of this
                                parameter will be pulled from an environment
                                variable in case a prefix is defined on the
                                context.
     :param help: the help string.
     :param hidden: hide this option from help outputs.
+    :param attrs: Other command arguments described in :class:`Parameter`.
 
     .. versionchanged:: 8.1.0
         Help text indentation is cleaned here instead of only in the
         ``@option`` decorator.
 
     .. versionchanged:: 8.1.0
         The ``show_default`` parameter overrides
@@ -2525,27 +2566,33 @@
                 # Implicitly a flag because flag options were given.
                 is_flag = bool(self.secondary_opts)
         elif is_flag is False and not self._flag_needs_value:
             # Not a flag, and prompt is not enabled, can be used as a
             # flag if flag_value is set.
             self._flag_needs_value = flag_value is not None
 
+        self.default: t.Union[t.Any, t.Callable[[], t.Any]]
+
         if is_flag and default_is_missing and not self.required:
-            self.default: t.Union[t.Any, t.Callable[[], t.Any]] = False
+            if multiple:
+                self.default = ()
+            else:
+                self.default = False
 
         if flag_value is None:
             flag_value = not self.default
 
+        self.type: types.ParamType
         if is_flag and type is None:
             # Re-guess the type from the flag value instead of the
             # default.
             self.type = types.convert_type(None, flag_value)
 
         self.is_flag: bool = is_flag
-        self.is_bool_flag = is_flag and isinstance(self.type, types.BoolParamType)
+        self.is_bool_flag: bool = is_flag and isinstance(self.type, types.BoolParamType)
         self.flag_value: t.Any = flag_value
 
         # Counting
         self.count = count
         if count:
             if type is None:
                 self.type = types.IntRange(min=0)
@@ -2576,17 +2623,14 @@
             if self.count:
                 if self.multiple:
                     raise TypeError("'count' is not valid with 'multiple'.")
 
                 if self.is_flag:
                     raise TypeError("'count' is not valid with 'is_flag'.")
 
-            if self.multiple and self.is_flag:
-                raise TypeError("'multiple' is not valid with 'is_flag', use 'count'.")
-
     def to_info_dict(self) -> t.Dict[str, t.Any]:
         info_dict = super().to_info_dict()
         info_dict.update(
             help=self.help,
             prompt=self.prompt,
             is_flag=self.is_flag,
             flag_value=self.flag_value,
@@ -2813,15 +2857,15 @@
         # If we're a non boolean flag our default is more complex because
         # we need to look at all flags in the same group to figure out
         # if we're the default one in which case we return the flag
         # value as default.
         if self.is_flag and not self.is_bool_flag:
             for param in ctx.command.params:
                 if param.name == self.name and param.default:
-                    return param.flag_value  # type: ignore
+                    return t.cast(Option, param).flag_value
 
             return None
 
         return super().get_default(ctx, call=call)
 
     def prompt_for_value(self, ctx: Context) -> t.Any:
         """This is an alternative flow that can be activated in the full
@@ -2923,15 +2967,15 @@
 
 
 class Argument(Parameter):
     """Arguments are positional parameters to a command.  They generally
     provide fewer features than options but can have infinite ``nargs``
     and are required by default.
 
-    All parameters are passed onwards to the parameter constructor.
+    All parameters are passed onwards to the constructor of :class:`Parameter`.
     """
 
     param_type_name = "argument"
 
     def __init__(
         self,
         param_decls: t.Sequence[str],
```

### Comparing `click-8.1.3/src/click/decorators.py` & `click-8.1.4/src/click/decorators.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,44 +9,52 @@
 from .core import Context
 from .core import Group
 from .core import Option
 from .core import Parameter
 from .globals import get_current_context
 from .utils import echo
 
-F = t.TypeVar("F", bound=t.Callable[..., t.Any])
-FC = t.TypeVar("FC", bound=t.Union[t.Callable[..., t.Any], Command])
+if t.TYPE_CHECKING:
+    import typing_extensions as te
 
+    P = te.ParamSpec("P")
 
-def pass_context(f: F) -> F:
+R = t.TypeVar("R")
+T = t.TypeVar("T")
+_AnyCallable = t.Callable[..., t.Any]
+_Decorator: "te.TypeAlias" = t.Callable[[T], T]
+FC = t.TypeVar("FC", bound=t.Union[_AnyCallable, Command])
+
+
+def pass_context(f: "t.Callable[te.Concatenate[Context, P], R]") -> "t.Callable[P, R]":
     """Marks a callback as wanting to receive the current context
     object as first argument.
     """
 
-    def new_func(*args, **kwargs):  # type: ignore
+    def new_func(*args: "P.args", **kwargs: "P.kwargs") -> "R":
         return f(get_current_context(), *args, **kwargs)
 
-    return update_wrapper(t.cast(F, new_func), f)
+    return update_wrapper(new_func, f)
 
 
-def pass_obj(f: F) -> F:
+def pass_obj(f: "t.Callable[te.Concatenate[t.Any, P], R]") -> "t.Callable[P, R]":
     """Similar to :func:`pass_context`, but only pass the object on the
     context onwards (:attr:`Context.obj`).  This is useful if that object
     represents the state of a nested system.
     """
 
-    def new_func(*args, **kwargs):  # type: ignore
+    def new_func(*args: "P.args", **kwargs: "P.kwargs") -> "R":
         return f(get_current_context().obj, *args, **kwargs)
 
-    return update_wrapper(t.cast(F, new_func), f)
+    return update_wrapper(new_func, f)
 
 
 def make_pass_decorator(
-    object_type: t.Type, ensure: bool = False
-) -> "t.Callable[[F], F]":
+    object_type: t.Type[T], ensure: bool = False
+) -> t.Callable[["t.Callable[te.Concatenate[T, P], R]"], "t.Callable[P, R]"]:
     """Given an object type this creates a decorator that will work
     similar to :func:`pass_obj` but instead of passing the object of the
     current context, it will find the innermost context of type
     :func:`object_type`.
 
     This generates a decorator that works roughly like this::
 
@@ -61,102 +69,119 @@
         return decorator
 
     :param object_type: the type of the object to pass.
     :param ensure: if set to `True`, a new object will be created and
                    remembered on the context if it's not there yet.
     """
 
-    def decorator(f: F) -> F:
-        def new_func(*args, **kwargs):  # type: ignore
+    def decorator(f: "t.Callable[te.Concatenate[T, P], R]") -> "t.Callable[P, R]":
+        def new_func(*args: "P.args", **kwargs: "P.kwargs") -> "R":
             ctx = get_current_context()
 
+            obj: t.Optional[T]
             if ensure:
                 obj = ctx.ensure_object(object_type)
             else:
                 obj = ctx.find_object(object_type)
 
             if obj is None:
                 raise RuntimeError(
                     "Managed to invoke callback without a context"
                     f" object of type {object_type.__name__!r}"
                     " existing."
                 )
 
             return ctx.invoke(f, obj, *args, **kwargs)
 
-        return update_wrapper(t.cast(F, new_func), f)
+        return update_wrapper(new_func, f)
 
-    return decorator
+    return decorator  # type: ignore[return-value]
 
 
 def pass_meta_key(
     key: str, *, doc_description: t.Optional[str] = None
-) -> "t.Callable[[F], F]":
+) -> "t.Callable[[t.Callable[te.Concatenate[t.Any, P], R]], t.Callable[P, R]]":
     """Create a decorator that passes a key from
     :attr:`click.Context.meta` as the first argument to the decorated
     function.
 
     :param key: Key in ``Context.meta`` to pass.
     :param doc_description: Description of the object being passed,
         inserted into the decorator's docstring. Defaults to "the 'key'
         key from Context.meta".
 
     .. versionadded:: 8.0
     """
 
-    def decorator(f: F) -> F:
-        def new_func(*args, **kwargs):  # type: ignore
+    def decorator(f: "t.Callable[te.Concatenate[t.Any, P], R]") -> "t.Callable[P, R]":
+        def new_func(*args: "P.args", **kwargs: "P.kwargs") -> R:
             ctx = get_current_context()
             obj = ctx.meta[key]
             return ctx.invoke(f, obj, *args, **kwargs)
 
-        return update_wrapper(t.cast(F, new_func), f)
+        return update_wrapper(new_func, f)
 
     if doc_description is None:
         doc_description = f"the {key!r} key from :attr:`click.Context.meta`"
 
     decorator.__doc__ = (
         f"Decorator that passes {doc_description} as the first argument"
         " to the decorated function."
     )
-    return decorator
+    return decorator  # type: ignore[return-value]
 
 
 CmdType = t.TypeVar("CmdType", bound=Command)
 
 
+# variant: no call, directly as decorator for a function.
 @t.overload
-def command(
-    __func: t.Callable[..., t.Any],
-) -> Command:
+def command(name: _AnyCallable) -> Command:
     ...
 
 
+# variant: with positional name and with positional or keyword cls argument:
+# @command(namearg, CommandCls, ...) or @command(namearg, cls=CommandCls, ...)
 @t.overload
 def command(
-    name: t.Optional[str] = None,
+    name: t.Optional[str],
+    cls: t.Type[CmdType],
     **attrs: t.Any,
-) -> t.Callable[..., Command]:
+) -> t.Callable[[_AnyCallable], CmdType]:
     ...
 
 
+# variant: name omitted, cls _must_ be a keyword argument, @command(cmd=CommandCls, ...)
+# The correct way to spell this overload is to use keyword-only argument syntax:
+# def command(*, cls: t.Type[CmdType], **attrs: t.Any) -> ...
+# However, mypy thinks this doesn't fit the overloaded function. Pyright does
+# accept that spelling, and the following work-around makes pyright issue a
+# warning that CmdType could be left unsolved, but mypy sees it as fine. *shrug*
 @t.overload
 def command(
-    name: t.Optional[str] = None,
+    name: None = None,
     cls: t.Type[CmdType] = ...,
     **attrs: t.Any,
-) -> t.Callable[..., CmdType]:
+) -> t.Callable[[_AnyCallable], CmdType]:
     ...
 
 
+# variant: with optional string name, no cls argument provided.
+@t.overload
 def command(
-    name: t.Union[str, t.Callable[..., t.Any], None] = None,
-    cls: t.Optional[t.Type[Command]] = None,
+    name: t.Optional[str] = ..., cls: None = None, **attrs: t.Any
+) -> t.Callable[[_AnyCallable], Command]:
+    ...
+
+
+def command(
+    name: t.Union[t.Optional[str], _AnyCallable] = None,
+    cls: t.Optional[t.Type[CmdType]] = None,
     **attrs: t.Any,
-) -> t.Union[Command, t.Callable[..., Command]]:
+) -> t.Union[Command, t.Callable[[_AnyCallable], t.Union[Command, CmdType]]]:
     r"""Creates a new :class:`Command` and uses the decorated function as
     callback.  This will also automatically attach all decorated
     :func:`option`\s and :func:`argument`\s as parameters to the command.
 
     The name of the command defaults to the name of the function with
     underscores replaced by dashes.  If you want to change that, you can
     pass the intended name as the first argument.
@@ -178,26 +203,26 @@
         This decorator can be applied without parentheses.
 
     .. versionchanged:: 8.1
         The ``params`` argument can be used. Decorated params are
         appended to the end of the list.
     """
 
-    func: t.Optional[t.Callable[..., t.Any]] = None
+    func: t.Optional[t.Callable[[_AnyCallable], t.Any]] = None
 
     if callable(name):
         func = name
         name = None
         assert cls is None, "Use 'command(cls=cls)(callable)' to specify a class."
         assert not attrs, "Use 'command(**kwargs)(callable)' to provide arguments."
 
     if cls is None:
-        cls = Command
+        cls = t.cast(t.Type[CmdType], Command)
 
-    def decorator(f: t.Callable[..., t.Any]) -> Command:
+    def decorator(f: _AnyCallable) -> CmdType:
         if isinstance(f, Command):
             raise TypeError("Attempted to convert a callback into a command twice.")
 
         attr_params = attrs.pop("params", None)
         params = attr_params if attr_params is not None else []
 
         try:
@@ -207,115 +232,164 @@
         else:
             del f.__click_params__  # type: ignore
             params.extend(reversed(decorator_params))
 
         if attrs.get("help") is None:
             attrs["help"] = f.__doc__
 
-        cmd = cls(  # type: ignore[misc]
-            name=name or f.__name__.lower().replace("_", "-"),  # type: ignore[arg-type]
+        if t.TYPE_CHECKING:
+            assert cls is not None
+            assert not callable(name)
+
+        cmd = cls(
+            name=name or f.__name__.lower().replace("_", "-"),
             callback=f,
             params=params,
             **attrs,
         )
         cmd.__doc__ = f.__doc__
         return cmd
 
     if func is not None:
         return decorator(func)
 
     return decorator
 
 
+GrpType = t.TypeVar("GrpType", bound=Group)
+
+
+# variant: no call, directly as decorator for a function.
+@t.overload
+def group(name: _AnyCallable) -> Group:
+    ...
+
+
+# variant: with positional name and with positional or keyword cls argument:
+# @group(namearg, GroupCls, ...) or @group(namearg, cls=GroupCls, ...)
 @t.overload
 def group(
-    __func: t.Callable[..., t.Any],
-) -> Group:
+    name: t.Optional[str],
+    cls: t.Type[GrpType],
+    **attrs: t.Any,
+) -> t.Callable[[_AnyCallable], GrpType]:
     ...
 
 
+# variant: name omitted, cls _must_ be a keyword argument, @group(cmd=GroupCls, ...)
+# The _correct_ way to spell this overload is to use keyword-only argument syntax:
+# def group(*, cls: t.Type[GrpType], **attrs: t.Any) -> ...
+# However, mypy thinks this doesn't fit the overloaded function. Pyright does
+# accept that spelling, and the following work-around makes pyright issue a
+# warning that GrpType could be left unsolved, but mypy sees it as fine. *shrug*
 @t.overload
 def group(
-    name: t.Optional[str] = None,
+    name: None = None,
+    cls: t.Type[GrpType] = ...,
     **attrs: t.Any,
-) -> t.Callable[[F], Group]:
+) -> t.Callable[[_AnyCallable], GrpType]:
+    ...
+
+
+# variant: with optional string name, no cls argument provided.
+@t.overload
+def group(
+    name: t.Optional[str] = ..., cls: None = None, **attrs: t.Any
+) -> t.Callable[[_AnyCallable], Group]:
     ...
 
 
 def group(
-    name: t.Union[str, t.Callable[..., t.Any], None] = None, **attrs: t.Any
-) -> t.Union[Group, t.Callable[[F], Group]]:
+    name: t.Union[str, _AnyCallable, None] = None,
+    cls: t.Optional[t.Type[GrpType]] = None,
+    **attrs: t.Any,
+) -> t.Union[Group, t.Callable[[_AnyCallable], t.Union[Group, GrpType]]]:
     """Creates a new :class:`Group` with a function as callback.  This
     works otherwise the same as :func:`command` just that the `cls`
     parameter is set to :class:`Group`.
 
     .. versionchanged:: 8.1
         This decorator can be applied without parentheses.
     """
-    if attrs.get("cls") is None:
-        attrs["cls"] = Group
+    if cls is None:
+        cls = t.cast(t.Type[GrpType], Group)
 
     if callable(name):
-        grp: t.Callable[[F], Group] = t.cast(Group, command(**attrs))
-        return grp(name)
+        return command(cls=cls, **attrs)(name)
 
-    return t.cast(Group, command(name, **attrs))
+    return command(name, cls, **attrs)
 
 
-def _param_memo(f: FC, param: Parameter) -> None:
+def _param_memo(f: t.Callable[..., t.Any], param: Parameter) -> None:
     if isinstance(f, Command):
         f.params.append(param)
     else:
         if not hasattr(f, "__click_params__"):
             f.__click_params__ = []  # type: ignore
 
         f.__click_params__.append(param)  # type: ignore
 
 
-def argument(*param_decls: str, **attrs: t.Any) -> t.Callable[[FC], FC]:
+def argument(
+    *param_decls: str, cls: t.Optional[t.Type[Argument]] = None, **attrs: t.Any
+) -> _Decorator[FC]:
     """Attaches an argument to the command.  All positional arguments are
     passed as parameter declarations to :class:`Argument`; all keyword
     arguments are forwarded unchanged (except ``cls``).
     This is equivalent to creating an :class:`Argument` instance manually
     and attaching it to the :attr:`Command.params` list.
 
+    For the default argument class, refer to :class:`Argument` and
+    :class:`Parameter` for descriptions of parameters.
+
     :param cls: the argument class to instantiate.  This defaults to
                 :class:`Argument`.
+    :param param_decls: Passed as positional arguments to the constructor of
+        ``cls``.
+    :param attrs: Passed as keyword arguments to the constructor of ``cls``.
     """
+    if cls is None:
+        cls = Argument
 
     def decorator(f: FC) -> FC:
-        ArgumentClass = attrs.pop("cls", None) or Argument
-        _param_memo(f, ArgumentClass(param_decls, **attrs))
+        _param_memo(f, cls(param_decls, **attrs))
         return f
 
     return decorator
 
 
-def option(*param_decls: str, **attrs: t.Any) -> t.Callable[[FC], FC]:
+def option(
+    *param_decls: str, cls: t.Optional[t.Type[Option]] = None, **attrs: t.Any
+) -> _Decorator[FC]:
     """Attaches an option to the command.  All positional arguments are
     passed as parameter declarations to :class:`Option`; all keyword
     arguments are forwarded unchanged (except ``cls``).
     This is equivalent to creating an :class:`Option` instance manually
     and attaching it to the :attr:`Command.params` list.
 
+    For the default option class, refer to :class:`Option` and
+    :class:`Parameter` for descriptions of parameters.
+
     :param cls: the option class to instantiate.  This defaults to
                 :class:`Option`.
+    :param param_decls: Passed as positional arguments to the constructor of
+        ``cls``.
+    :param attrs: Passed as keyword arguments to the constructor of ``cls``.
     """
+    if cls is None:
+        cls = Option
 
     def decorator(f: FC) -> FC:
-        # Issue 926, copy attrs, so pre-defined options can re-use the same cls=
-        option_attrs = attrs.copy()
-        OptionClass = option_attrs.pop("cls", None) or Option
-        _param_memo(f, OptionClass(param_decls, **option_attrs))
+        _param_memo(f, cls(param_decls, **attrs))
         return f
 
     return decorator
 
 
-def confirmation_option(*param_decls: str, **kwargs: t.Any) -> t.Callable[[FC], FC]:
+def confirmation_option(*param_decls: str, **kwargs: t.Any) -> _Decorator[FC]:
     """Add a ``--yes`` option which shows a prompt before continuing if
     not passed. If the prompt is declined, the program will exit.
 
     :param param_decls: One or more option names. Defaults to the single
         value ``"--yes"``.
     :param kwargs: Extra arguments are passed to :func:`option`.
     """
@@ -331,15 +405,15 @@
     kwargs.setdefault("callback", callback)
     kwargs.setdefault("expose_value", False)
     kwargs.setdefault("prompt", "Do you want to continue?")
     kwargs.setdefault("help", "Confirm the action without prompting.")
     return option(*param_decls, **kwargs)
 
 
-def password_option(*param_decls: str, **kwargs: t.Any) -> t.Callable[[FC], FC]:
+def password_option(*param_decls: str, **kwargs: t.Any) -> _Decorator[FC]:
     """Add a ``--password`` option which prompts for a password, hiding
     input and asking to enter the value again for confirmation.
 
     :param param_decls: One or more option names. Defaults to the single
         value ``"--password"``.
     :param kwargs: Extra arguments are passed to :func:`option`.
     """
@@ -355,15 +429,15 @@
 def version_option(
     version: t.Optional[str] = None,
     *param_decls: str,
     package_name: t.Optional[str] = None,
     prog_name: t.Optional[str] = None,
     message: t.Optional[str] = None,
     **kwargs: t.Any,
-) -> t.Callable[[FC], FC]:
+) -> _Decorator[FC]:
     """Add a ``--version`` option which immediately prints the version
     number and exits the program.
 
     If ``version`` is not provided, Click will try to detect it using
     :func:`importlib.metadata.version` to get the version for the
     ``package_name``. On Python < 3.8, the ``importlib_metadata``
     backport must be installed.
@@ -445,16 +519,15 @@
 
         if version is None:
             raise RuntimeError(
                 f"Could not determine the version for {package_name!r} automatically."
             )
 
         echo(
-            t.cast(str, message)
-            % {"prog": prog_name, "package": package_name, "version": version},
+            message % {"prog": prog_name, "package": package_name, "version": version},
             color=ctx.color,
         )
         ctx.exit()
 
     if not param_decls:
         param_decls = ("--version",)
 
@@ -462,15 +535,15 @@
     kwargs.setdefault("expose_value", False)
     kwargs.setdefault("is_eager", True)
     kwargs.setdefault("help", _("Show the version and exit."))
     kwargs["callback"] = callback
     return option(*param_decls, **kwargs)
 
 
-def help_option(*param_decls: str, **kwargs: t.Any) -> t.Callable[[FC], FC]:
+def help_option(*param_decls: str, **kwargs: t.Any) -> _Decorator[FC]:
     """Add a ``--help`` option which immediately prints the help page
     and exits the program.
 
     This is usually unnecessary, as the ``--help`` option is added to
     each command automatically unless ``add_help_option=False`` is
     passed.
```

### Comparing `click-8.1.3/src/click/exceptions.py` & `click-8.1.4/src/click/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import os
 import typing as t
 from gettext import gettext as _
 from gettext import ngettext
 
 from ._compat import get_text_stderr
 from .utils import echo
+from .utils import format_filename
 
 if t.TYPE_CHECKING:
+    from .core import Command
     from .core import Context
     from .core import Parameter
 
 
 def _join_param_hints(
     param_hint: t.Optional[t.Union[t.Sequence[str], str]]
 ) -> t.Optional[str]:
@@ -32,15 +33,15 @@
 
     def format_message(self) -> str:
         return self.message
 
     def __str__(self) -> str:
         return self.message
 
-    def show(self, file: t.Optional[t.IO] = None) -> None:
+    def show(self, file: t.Optional[t.IO[t.Any]] = None) -> None:
         if file is None:
             file = get_text_stderr()
 
         echo(_("Error: {message}").format(message=self.format_message()), file=file)
 
 
 class UsageError(ClickException):
@@ -53,17 +54,17 @@
     """
 
     exit_code = 2
 
     def __init__(self, message: str, ctx: t.Optional["Context"] = None) -> None:
         super().__init__(message)
         self.ctx = ctx
-        self.cmd = self.ctx.command if self.ctx else None
+        self.cmd: t.Optional["Command"] = self.ctx.command if self.ctx else None
 
-    def show(self, file: t.Optional[t.IO] = None) -> None:
+    def show(self, file: t.Optional[t.IO[t.Any]] = None) -> None:
         if file is None:
             file = get_text_stderr()
         color = None
         hint = ""
         if (
             self.ctx is not None
             and self.ctx.command.get_help_option(self.ctx) is not None
@@ -257,15 +258,15 @@
     """Raised if a file cannot be opened."""
 
     def __init__(self, filename: str, hint: t.Optional[str] = None) -> None:
         if hint is None:
             hint = _("unknown error")
 
         super().__init__(hint)
-        self.ui_filename = os.fsdecode(filename)
+        self.ui_filename: str = format_filename(filename)
         self.filename = filename
 
     def format_message(self) -> str:
         return _("Could not open file {filename!r}: {message}").format(
             filename=self.ui_filename, message=self.message
         )
 
@@ -280,8 +281,8 @@
 
     :param code: the status code to exit with.
     """
 
     __slots__ = ("exit_code",)
 
     def __init__(self, code: int = 0) -> None:
-        self.exit_code = code
+        self.exit_code: int = code
```

### Comparing `click-8.1.3/src/click/formatting.py` & `click-8.1.4/src/click/formatting.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/src/click/globals.py` & `click-8.1.4/src/click/globals.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/src/click/parser.py` & `click-8.1.4/src/click/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         dest: t.Optional[str],
         action: t.Optional[str] = None,
         nargs: int = 1,
         const: t.Optional[t.Any] = None,
     ):
         self._short_opts = []
         self._long_opts = []
-        self.prefixes = set()
+        self.prefixes: t.Set[str] = set()
 
         for opt in opts:
             prefix, value = split_opt(opt)
             if not prefix:
                 raise ValueError(f"Invalid start character for option ({opt})")
             self.prefixes.add(prefix[0])
             if len(prefix) == 1 and len(value) == 1:
@@ -190,15 +190,15 @@
         self.const = const
         self.obj = obj
 
     @property
     def takes_value(self) -> bool:
         return self.action in ("store", "append")
 
-    def process(self, value: str, state: "ParsingState") -> None:
+    def process(self, value: t.Any, state: "ParsingState") -> None:
         if self.action == "store":
             state.opts[self.dest] = value  # type: ignore
         elif self.action == "store_const":
             state.opts[self.dest] = self.const  # type: ignore
         elif self.action == "append":
             state.opts.setdefault(self.dest, []).append(value)  # type: ignore
         elif self.action == "append_const":
@@ -268,20 +268,20 @@
         #: The :class:`~click.Context` for this parser.  This might be
         #: `None` for some advanced use cases.
         self.ctx = ctx
         #: This controls how the parser deals with interspersed arguments.
         #: If this is set to `False`, the parser will stop on the first
         #: non-option.  Click uses this to implement nested subcommands
         #: safely.
-        self.allow_interspersed_args = True
+        self.allow_interspersed_args: bool = True
         #: This tells the parser how to deal with unknown options.  By
         #: default it will error out (which is sensible), but there is a
         #: second mode where it will ignore it and continue processing
         #: after shifting all the unknown options into the resulting args.
-        self.ignore_unknown_options = False
+        self.ignore_unknown_options: bool = False
 
         if ctx is not None:
             self.allow_interspersed_args = ctx.allow_interspersed_args
             self.ignore_unknown_options = ctx.ignore_unknown_options
 
         self._short_opt: t.Dict[str, Option] = {}
         self._long_opt: t.Dict[str, Option] = {}
@@ -447,15 +447,15 @@
                 value = None
 
             option.process(value, state)
 
             if stop:
                 break
 
-        # If we got any unknown options we re-combinate the string of the
+        # If we got any unknown options we recombine the string of the
         # remaining options and re-attach the prefix, then report that
         # to the state as new larg.  This way there is basic combinatorics
         # that can be achieved while still ignoring unknown arguments.
         if self.ignore_unknown_options and unknown_options:
             state.largs.append(f"{prefix}{''.join(unknown_options)}")
 
     def _get_value_from_state(
```

### Comparing `click-8.1.3/src/click/shell_completion.py` & `click-8.1.4/src/click/shell_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .core import ParameterSource
 from .parser import split_arg_string
 from .utils import echo
 
 
 def shell_complete(
     cli: BaseCommand,
-    ctx_args: t.Dict[str, t.Any],
+    ctx_args: t.MutableMapping[str, t.Any],
     prog_name: str,
     complete_var: str,
     instruction: str,
 ) -> int:
     """Perform shell completion for the given CLI program.
 
     :param cli: Command being called.
@@ -76,17 +76,17 @@
     def __init__(
         self,
         value: t.Any,
         type: str = "plain",
         help: t.Optional[str] = None,
         **kwargs: t.Any,
     ) -> None:
-        self.value = value
-        self.type = type
-        self.help = help
+        self.value: t.Any = value
+        self.type: str = type
+        self.help: t.Optional[str] = help
         self._info = kwargs
 
     def __getattr__(self, name: str) -> t.Any:
         return self._info.get(name)
 
 
 # Only Bash >= 4.4 has the nosort option.
@@ -153,41 +153,43 @@
     fi
 
     if [ -n "$completions" ]; then
         compadd -U -V unsorted -a completions
     fi
 }
 
-compdef %(complete_func)s %(prog_name)s;
+if [[ $zsh_eval_context[-1] == loadautofunc ]]; then
+    # autoload from fpath, call function directly
+    %(complete_func)s "$@"
+else
+    # eval/source/. command, register function for later
+    compdef %(complete_func)s %(prog_name)s
+fi
 """
 
 _SOURCE_FISH = """\
-function %(complete_func)s;
-    set -l response;
-
-    for value in (env %(complete_var)s=fish_complete COMP_WORDS=(commandline -cp) \
-COMP_CWORD=(commandline -t) %(prog_name)s);
-        set response $response $value;
-    end;
-
-    for completion in $response;
-        set -l metadata (string split "," $completion);
-
-        if test $metadata[1] = "dir";
-            __fish_complete_directories $metadata[2];
-        else if test $metadata[1] = "file";
-            __fish_complete_path $metadata[2];
-        else if test $metadata[1] = "plain";
-            echo $metadata[2];
-        end;
-    end;
-end;
+function %(complete_func)s
+    set -l response (env %(complete_var)s=fish_complete COMP_WORDS=(commandline -cp) \
+COMP_CWORD=(commandline -t) %(prog_name)s)
+
+    for completion in $response
+        set -l metadata (string split "," $completion)
+
+        if test $metadata[1] = "dir"
+            __fish_complete_directories $metadata[2]
+        else if test $metadata[1] = "file"
+            __fish_complete_path $metadata[2]
+        else if test $metadata[1] = "plain"
+            echo $metadata[2]
+        end
+    end
+end
 
 complete --no-files --command %(prog_name)s --arguments \
-"(%(complete_func)s)";
+"(%(complete_func)s)"
 """
 
 
 class ShellComplete:
     """Base class for providing shell completion support. A subclass for
     a given shell will override attributes and methods to implement the
     completion instructions (``source`` and ``complete``).
@@ -210,15 +212,15 @@
     """Completion script template formatted by :meth:`source`. This must
     be provided by subclasses.
     """
 
     def __init__(
         self,
         cli: BaseCommand,
-        ctx_args: t.Dict[str, t.Any],
+        ctx_args: t.MutableMapping[str, t.Any],
         prog_name: str,
         complete_var: str,
     ) -> None:
         self.cli = cli
         self.ctx_args = ctx_args
         self.prog_name = prog_name
         self.complete_var = complete_var
@@ -299,15 +301,15 @@
     name = "bash"
     source_template = _SOURCE_BASH
 
     def _check_version(self) -> None:
         import subprocess
 
         output = subprocess.run(
-            ["bash", "-c", "echo ${BASH_VERSION}"], stdout=subprocess.PIPE
+            ["bash", "-c", 'echo "${BASH_VERSION}"'], stdout=subprocess.PIPE
         )
         match = re.search(r"^(\d+)\.(\d+)\.\d+", output.stdout.decode())
 
         if match is not None:
             major, minor = match.groups()
 
             if major < "4" or major == "4" and minor < "4":
@@ -385,38 +387,43 @@
     def format_completion(self, item: CompletionItem) -> str:
         if item.help:
             return f"{item.type},{item.value}\t{item.help}"
 
         return f"{item.type},{item.value}"
 
 
+ShellCompleteType = t.TypeVar("ShellCompleteType", bound=t.Type[ShellComplete])
+
+
 _available_shells: t.Dict[str, t.Type[ShellComplete]] = {
     "bash": BashComplete,
     "fish": FishComplete,
     "zsh": ZshComplete,
 }
 
 
 def add_completion_class(
-    cls: t.Type[ShellComplete], name: t.Optional[str] = None
-) -> None:
+    cls: ShellCompleteType, name: t.Optional[str] = None
+) -> ShellCompleteType:
     """Register a :class:`ShellComplete` subclass under the given name.
     The name will be provided by the completion instruction environment
     variable during completion.
 
     :param cls: The completion class that will handle completion for the
         shell.
     :param name: Name to register the class under. Defaults to the
         class's ``name`` attribute.
     """
     if name is None:
         name = cls.name
 
     _available_shells[name] = cls
 
+    return cls
+
 
 def get_completion_class(shell: str) -> t.Optional[t.Type[ShellComplete]]:
     """Look up a registered :class:`ShellComplete` subclass by the name
     provided by the completion instruction environment variable. If the
     name isn't registered, returns ``None``.
 
     :param shell: Name the class is registered under.
@@ -432,15 +439,16 @@
         parsed complete args.
     :param param: Argument object being checked.
     """
     if not isinstance(param, Argument):
         return False
 
     assert param.name is not None
-    value = ctx.params[param.name]
+    # Will be None if expose_value is False.
+    value = ctx.params.get(param.name)
     return (
         param.nargs == -1
         or ctx.get_parameter_source(param.name) is not ParameterSource.COMMANDLINE
         or (
             param.nargs > 1
             and isinstance(value, (tuple, list))
             and len(value) < param.nargs
@@ -478,15 +486,18 @@
         if _start_of_option(ctx, arg):
             last_option = arg
 
     return last_option is not None and last_option in param.opts
 
 
 def _resolve_context(
-    cli: BaseCommand, ctx_args: t.Dict[str, t.Any], prog_name: str, args: t.List[str]
+    cli: BaseCommand,
+    ctx_args: t.MutableMapping[str, t.Any],
+    prog_name: str,
+    args: t.List[str],
 ) -> Context:
     """Produce the context hierarchy starting with the command and
     traversing the complete arguments. This only follows the commands,
     it doesn't trigger input prompts or callbacks.
 
     :param cli: Command being called.
     :param prog_name: Name of the executable in the shell.
@@ -505,14 +516,16 @@
 
                 if cmd is None:
                     return ctx
 
                 ctx = cmd.make_context(name, args, parent=ctx, resilient_parsing=True)
                 args = ctx.protected_args + ctx.args
             else:
+                sub_ctx = ctx
+
                 while args:
                     name, cmd, args = command.resolve_command(ctx, args)
 
                     if cmd is None:
                         return ctx
 
                     sub_ctx = cmd.make_context(
```

### Comparing `click-8.1.3/src/click/termui.py` & `click-8.1.4/src/click/termui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import inspect
 import io
 import itertools
-import os
 import sys
 import typing as t
 from gettext import gettext as _
 
 from ._compat import isatty
 from ._compat import strip_ansi
-from ._compat import WIN
 from .exceptions import Abort
 from .exceptions import UsageError
 from .globals import resolve_color_default
 from .types import Choice
 from .types import convert_type
 from .types import ParamType
 from .utils import echo
@@ -69,15 +67,15 @@
     if default is not None and show_default:
         prompt = f"{prompt} [{_format_default(default)}]"
     return f"{prompt}{suffix}"
 
 
 def _format_default(default: t.Any) -> t.Any:
     if isinstance(default, (io.IOBase, LazyFile)) and hasattr(default, "name"):
-        return default.name  # type: ignore
+        return default.name
 
     return default
 
 
 def prompt(
     text: str,
     default: t.Optional[t.Any] = None,
@@ -439,18 +437,17 @@
     the whole visible space of the terminal and moving the cursor to the
     top left.  This does not do anything if not connected to a terminal.
 
     .. versionadded:: 2.0
     """
     if not isatty(sys.stdout):
         return
-    if WIN:
-        os.system("cls")
-    else:
-        sys.stdout.write("\033[2J\033[1;1H")
+
+    # ANSI escape \033[2J clears the screen, \033[1;1H moves the cursor
+    echo("\033[2J\033[1;1H", nl=False)
 
 
 def _interpret_color(
     color: t.Union[int, t.Tuple[int, int, int], str], offset: int = 0
 ) -> str:
     if isinstance(color, int):
         return f"{38 + offset};5;{color:d}"
```

### Comparing `click-8.1.3/src/click/testing.py` & `click-8.1.4/src/click/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,31 +75,31 @@
 
     @property
     def mode(self) -> str:
         return self._mode
 
 
 def make_input_stream(
-    input: t.Optional[t.Union[str, bytes, t.IO]], charset: str
+    input: t.Optional[t.Union[str, bytes, t.IO[t.Any]]], charset: str
 ) -> t.BinaryIO:
     # Is already an input stream.
     if hasattr(input, "read"):
-        rv = _find_binary_reader(t.cast(t.IO, input))
+        rv = _find_binary_reader(t.cast(t.IO[t.Any], input))
 
         if rv is not None:
             return rv
 
         raise TypeError("Could not find binary reader for input stream.")
 
     if input is None:
         input = b""
     elif isinstance(input, str):
         input = input.encode(charset)
 
-    return io.BytesIO(t.cast(bytes, input))
+    return io.BytesIO(input)
 
 
 class Result:
     """Holds the captured result of an invoked CLI script."""
 
     def __init__(
         self,
@@ -179,15 +179,15 @@
         self,
         charset: str = "utf-8",
         env: t.Optional[t.Mapping[str, t.Optional[str]]] = None,
         echo_stdin: bool = False,
         mix_stderr: bool = True,
     ) -> None:
         self.charset = charset
-        self.env = env or {}
+        self.env: t.Mapping[str, t.Optional[str]] = env or {}
         self.echo_stdin = echo_stdin
         self.mix_stderr = mix_stderr
 
     def get_default_prog_name(self, cli: "BaseCommand") -> str:
         """Given a command object it will return the default program name
         for it.  The default is the `name` attribute or ``"root"`` if not
         set.
@@ -202,15 +202,15 @@
         if overrides:
             rv.update(overrides)
         return rv
 
     @contextlib.contextmanager
     def isolation(
         self,
-        input: t.Optional[t.Union[str, bytes, t.IO]] = None,
+        input: t.Optional[t.Union[str, bytes, t.IO[t.Any]]] = None,
         env: t.Optional[t.Mapping[str, t.Optional[str]]] = None,
         color: bool = False,
     ) -> t.Iterator[t.Tuple[io.BytesIO, t.Optional[io.BytesIO]]]:
         """A context manager that sets up the isolation for invoking of a
         command line tool.  This sets up stdin with the given input data
         and `os.environ` with the overrides from the given dictionary.
         This also rebinds some internals in Click to be mocked (like the
@@ -297,15 +297,15 @@
 
             sys.stdout.flush()
             return char
 
         default_color = color
 
         def should_strip_ansi(
-            stream: t.Optional[t.IO] = None, color: t.Optional[bool] = None
+            stream: t.Optional[t.IO[t.Any]] = None, color: t.Optional[bool] = None
         ) -> bool:
             if color is None:
                 return not default_color
             return not color
 
         old_visible_prompt_func = termui.visible_prompt_func
         old_hidden_prompt_func = termui.hidden_prompt_func
@@ -346,15 +346,15 @@
             utils.should_strip_ansi = old_should_strip_ansi  # type: ignore
             formatting.FORCED_WIDTH = old_forced_width
 
     def invoke(
         self,
         cli: "BaseCommand",
         args: t.Optional[t.Union[str, t.Sequence[str]]] = None,
-        input: t.Optional[t.Union[str, bytes, t.IO]] = None,
+        input: t.Optional[t.Union[str, bytes, t.IO[t.Any]]] = None,
         env: t.Optional[t.Mapping[str, t.Optional[str]]] = None,
         catch_exceptions: bool = True,
         color: bool = False,
         **extra: t.Any,
     ) -> Result:
         """Invokes a command in an isolated environment.  The arguments are
         forwarded directly to the command line script, the `extra` keyword
@@ -445,34 +445,34 @@
             exit_code=exit_code,
             exception=exception,
             exc_info=exc_info,  # type: ignore
         )
 
     @contextlib.contextmanager
     def isolated_filesystem(
-        self, temp_dir: t.Optional[t.Union[str, os.PathLike]] = None
+        self, temp_dir: t.Optional[t.Union[str, "os.PathLike[str]"]] = None
     ) -> t.Iterator[str]:
         """A context manager that creates a temporary directory and
         changes the current working directory to it. This isolates tests
         that affect the contents of the CWD to prevent them from
         interfering with each other.
 
         :param temp_dir: Create the temporary directory under this
             directory. If given, the created directory is not removed
             when exiting.
 
         .. versionchanged:: 8.0
             Added the ``temp_dir`` parameter.
         """
         cwd = os.getcwd()
-        dt = tempfile.mkdtemp(dir=temp_dir)  # type: ignore[type-var]
+        dt = tempfile.mkdtemp(dir=temp_dir)
         os.chdir(dt)
 
         try:
-            yield t.cast(str, dt)
+            yield dt
         finally:
             os.chdir(cwd)
 
             if temp_dir is None:
                 try:
                     shutil.rmtree(dt)
                 except OSError:  # noqa: B014
```

### Comparing `click-8.1.3/src/click/types.py` & `click-8.1.4/src/click/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import stat
+import sys
 import typing as t
 from datetime import datetime
 from gettext import gettext as _
 from gettext import ngettext
 
 from ._compat import _get_argv_encoding
-from ._compat import get_filesystem_encoding
 from ._compat import open_stream
 from .exceptions import BadParameter
+from .utils import format_filename
 from .utils import LazyFile
 from .utils import safecall
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
     from .core import Context
     from .core import Parameter
@@ -158,15 +159,15 @@
     @property
     def arity(self) -> int:  # type: ignore
         raise NotImplementedError()
 
 
 class FuncParamType(ParamType):
     def __init__(self, func: t.Callable[[t.Any], t.Any]) -> None:
-        self.name = func.__name__
+        self.name: str = func.__name__
         self.func = func
 
     def to_info_dict(self) -> t.Dict[str, t.Any]:
         info_dict = super().to_info_dict()
         info_dict["func"] = self.func
         return info_dict
 
@@ -203,15 +204,15 @@
         self, value: t.Any, param: t.Optional["Parameter"], ctx: t.Optional["Context"]
     ) -> t.Any:
         if isinstance(value, bytes):
             enc = _get_argv_encoding()
             try:
                 value = value.decode(enc)
             except UnicodeError:
-                fs_enc = get_filesystem_encoding()
+                fs_enc = sys.getfilesystemencoding()
                 if fs_enc != enc:
                     try:
                         value = value.decode(fs_enc)
                     except UnicodeError:
                         value = value.decode("utf-8", "replace")
                 else:
                     value = value.decode("utf-8", "replace")
@@ -349,15 +350,19 @@
                     ``'%Y-%m-%d'``, ``'%Y-%m-%dT%H:%M:%S'``,
                     ``'%Y-%m-%d %H:%M:%S'``.
     """
 
     name = "datetime"
 
     def __init__(self, formats: t.Optional[t.Sequence[str]] = None):
-        self.formats = formats or ["%Y-%m-%d", "%Y-%m-%dT%H:%M:%S", "%Y-%m-%d %H:%M:%S"]
+        self.formats: t.Sequence[str] = formats or [
+            "%Y-%m-%d",
+            "%Y-%m-%dT%H:%M:%S",
+            "%Y-%m-%d %H:%M:%S",
+        ]
 
     def to_info_dict(self) -> t.Dict[str, t.Any]:
         info_dict = super().to_info_dict()
         info_dict["formats"] = self.formats
         return info_dict
 
     def get_metavar(self, param: "Parameter") -> str:
@@ -393,15 +398,15 @@
         )
 
     def __repr__(self) -> str:
         return "DateTime"
 
 
 class _NumberParamTypeBase(ParamType):
-    _number_class: t.ClassVar[t.Type]
+    _number_class: t.ClassVar[t.Type[t.Any]]
 
     def convert(
         self, value: t.Any, param: t.Optional["Parameter"], ctx: t.Optional["Context"]
     ) -> t.Any:
         try:
             return self._number_class(value)
         except ValueError:
@@ -658,15 +663,15 @@
     completion the file will be moved over to the original location.  This
     is useful if a file regularly read by other users is modified.
 
     See :ref:`file-args` for more information.
     """
 
     name = "filename"
-    envvar_list_splitter = os.path.pathsep
+    envvar_list_splitter: t.ClassVar[str] = os.path.pathsep
 
     def __init__(
         self,
         mode: str = "r",
         encoding: t.Optional[str] = None,
         errors: t.Optional[str] = "strict",
         lazy: t.Optional[bool] = None,
@@ -679,44 +684,46 @@
         self.atomic = atomic
 
     def to_info_dict(self) -> t.Dict[str, t.Any]:
         info_dict = super().to_info_dict()
         info_dict.update(mode=self.mode, encoding=self.encoding)
         return info_dict
 
-    def resolve_lazy_flag(self, value: t.Any) -> bool:
+    def resolve_lazy_flag(self, value: "t.Union[str, os.PathLike[str]]") -> bool:
         if self.lazy is not None:
             return self.lazy
-        if value == "-":
+        if os.fspath(value) == "-":
             return False
         elif "w" in self.mode:
             return True
         return False
 
     def convert(
-        self, value: t.Any, param: t.Optional["Parameter"], ctx: t.Optional["Context"]
-    ) -> t.Any:
-        try:
-            if hasattr(value, "read") or hasattr(value, "write"):
-                return value
+        self,
+        value: t.Union[str, "os.PathLike[str]", t.IO[t.Any]],
+        param: t.Optional["Parameter"],
+        ctx: t.Optional["Context"],
+    ) -> t.IO[t.Any]:
+        if _is_file_like(value):
+            return value
+
+        value = t.cast("t.Union[str, os.PathLike[str]]", value)
 
+        try:
             lazy = self.resolve_lazy_flag(value)
 
             if lazy:
-                f: t.IO = t.cast(
-                    t.IO,
-                    LazyFile(
-                        value, self.mode, self.encoding, self.errors, atomic=self.atomic
-                    ),
+                lf = LazyFile(
+                    value, self.mode, self.encoding, self.errors, atomic=self.atomic
                 )
 
                 if ctx is not None:
-                    ctx.call_on_close(f.close_intelligently)  # type: ignore
+                    ctx.call_on_close(lf.close_intelligently)
 
-                return f
+                return t.cast(t.IO[t.Any], lf)
 
             f, should_close = open_stream(
                 value, self.mode, self.encoding, self.errors, atomic=self.atomic
             )
 
             # If a context is provided, we automatically close the file
             # at the end of the context execution (or flush out).  If a
@@ -727,15 +734,15 @@
                 if should_close:
                     ctx.call_on_close(safecall(f.close))
                 else:
                     ctx.call_on_close(safecall(f.flush))
 
             return f
         except OSError as e:  # noqa: B014
-            self.fail(f"'{os.fsdecode(value)}': {e.strerror}", param, ctx)
+            self.fail(f"'{format_filename(value)}': {e.strerror}", param, ctx)
 
     def shell_complete(
         self, ctx: "Context", param: "Parameter", incomplete: str
     ) -> t.List["CompletionItem"]:
         """Return a special completion marker that tells the completion
         system to use the shell to provide file path completions.
 
@@ -746,14 +753,18 @@
         .. versionadded:: 8.0
         """
         from click.shell_completion import CompletionItem
 
         return [CompletionItem(incomplete, type="file")]
 
 
+def _is_file_like(value: t.Any) -> "te.TypeGuard[t.IO[t.Any]]":
+    return hasattr(value, "read") or hasattr(value, "write")
+
+
 class Path(ParamType):
     """The ``Path`` type is similar to the :class:`File` type, but
     returns the filename instead of an open file. Various checks can be
     enabled to validate the type of file and permissions.
 
     :param exists: The file or directory needs to exist for the value to
         be valid. If this is not set to ``True``, and the file does not
@@ -773,46 +784,46 @@
         ``None``, keep Python's default, which is ``str``. Useful to
         convert to :class:`pathlib.Path`.
 
     .. versionchanged:: 8.1
         Added the ``executable`` parameter.
 
     .. versionchanged:: 8.0
-        Allow passing ``type=pathlib.Path``.
+        Allow passing ``path_type=pathlib.Path``.
 
     .. versionchanged:: 6.0
         Added the ``allow_dash`` parameter.
     """
 
-    envvar_list_splitter = os.path.pathsep
+    envvar_list_splitter: t.ClassVar[str] = os.path.pathsep
 
     def __init__(
         self,
         exists: bool = False,
         file_okay: bool = True,
         dir_okay: bool = True,
         writable: bool = False,
         readable: bool = True,
         resolve_path: bool = False,
         allow_dash: bool = False,
-        path_type: t.Optional[t.Type] = None,
+        path_type: t.Optional[t.Type[t.Any]] = None,
         executable: bool = False,
     ):
         self.exists = exists
         self.file_okay = file_okay
         self.dir_okay = dir_okay
         self.readable = readable
         self.writable = writable
         self.executable = executable
         self.resolve_path = resolve_path
         self.allow_dash = allow_dash
         self.type = path_type
 
         if self.file_okay and not self.dir_okay:
-            self.name = _("file")
+            self.name: str = _("file")
         elif self.dir_okay and not self.file_okay:
             self.name = _("directory")
         else:
             self.name = _("path")
 
     def to_info_dict(self) -> t.Dict[str, t.Any]:
         info_dict = super().to_info_dict()
@@ -822,28 +833,33 @@
             dir_okay=self.dir_okay,
             writable=self.writable,
             readable=self.readable,
             allow_dash=self.allow_dash,
         )
         return info_dict
 
-    def coerce_path_result(self, rv: t.Any) -> t.Any:
-        if self.type is not None and not isinstance(rv, self.type):
+    def coerce_path_result(
+        self, value: "t.Union[str, os.PathLike[str]]"
+    ) -> "t.Union[str, bytes, os.PathLike[str]]":
+        if self.type is not None and not isinstance(value, self.type):
             if self.type is str:
-                rv = os.fsdecode(rv)
+                return os.fsdecode(value)
             elif self.type is bytes:
-                rv = os.fsencode(rv)
+                return os.fsencode(value)
             else:
-                rv = self.type(rv)
+                return t.cast("os.PathLike[str]", self.type(value))
 
-        return rv
+        return value
 
     def convert(
-        self, value: t.Any, param: t.Optional["Parameter"], ctx: t.Optional["Context"]
-    ) -> t.Any:
+        self,
+        value: "t.Union[str, os.PathLike[str]]",
+        param: t.Optional["Parameter"],
+        ctx: t.Optional["Context"],
+    ) -> "t.Union[str, bytes, os.PathLike[str]]":
         rv = value
 
         is_dash = self.file_okay and self.allow_dash and rv in (b"-", "-")
 
         if not is_dash:
             if self.resolve_path:
                 # os.path.realpath doesn't resolve symlinks on Windows
@@ -855,59 +871,59 @@
             try:
                 st = os.stat(rv)
             except OSError:
                 if not self.exists:
                     return self.coerce_path_result(rv)
                 self.fail(
                     _("{name} {filename!r} does not exist.").format(
-                        name=self.name.title(), filename=os.fsdecode(value)
+                        name=self.name.title(), filename=format_filename(value)
                     ),
                     param,
                     ctx,
                 )
 
             if not self.file_okay and stat.S_ISREG(st.st_mode):
                 self.fail(
                     _("{name} {filename!r} is a file.").format(
-                        name=self.name.title(), filename=os.fsdecode(value)
+                        name=self.name.title(), filename=format_filename(value)
                     ),
                     param,
                     ctx,
                 )
             if not self.dir_okay and stat.S_ISDIR(st.st_mode):
                 self.fail(
                     _("{name} '{filename}' is a directory.").format(
-                        name=self.name.title(), filename=os.fsdecode(value)
+                        name=self.name.title(), filename=format_filename(value)
                     ),
                     param,
                     ctx,
                 )
 
             if self.readable and not os.access(rv, os.R_OK):
                 self.fail(
                     _("{name} {filename!r} is not readable.").format(
-                        name=self.name.title(), filename=os.fsdecode(value)
+                        name=self.name.title(), filename=format_filename(value)
                     ),
                     param,
                     ctx,
                 )
 
             if self.writable and not os.access(rv, os.W_OK):
                 self.fail(
                     _("{name} {filename!r} is not writable.").format(
-                        name=self.name.title(), filename=os.fsdecode(value)
+                        name=self.name.title(), filename=format_filename(value)
                     ),
                     param,
                     ctx,
                 )
 
             if self.executable and not os.access(value, os.X_OK):
                 self.fail(
                     _("{name} {filename!r} is not executable.").format(
-                        name=self.name.title(), filename=os.fsdecode(value)
+                        name=self.name.title(), filename=format_filename(value)
                     ),
                     param,
                     ctx,
                 )
 
         return self.coerce_path_result(rv)
 
@@ -940,16 +956,16 @@
     For more information see :ref:`tuple-type`.
 
     This can be selected by using a Python tuple literal as a type.
 
     :param types: a list of types that should be used for the tuple items.
     """
 
-    def __init__(self, types: t.Sequence[t.Union[t.Type, ParamType]]) -> None:
-        self.types = [convert_type(ty) for ty in types]
+    def __init__(self, types: t.Sequence[t.Union[t.Type[t.Any], ParamType]]) -> None:
+        self.types: t.Sequence[ParamType] = [convert_type(ty) for ty in types]
 
     def to_info_dict(self) -> t.Dict[str, t.Any]:
         info_dict = super().to_info_dict()
         info_dict["types"] = [t.to_info_dict() for t in self.types]
         return info_dict
 
     @property
```

### Comparing `click-8.1.3/src/click/utils.py` & `click-8.1.4/src/click/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 import os
 import re
 import sys
 import typing as t
 from functools import update_wrapper
 from types import ModuleType
+from types import TracebackType
 
 from ._compat import _default_text_stderr
 from ._compat import _default_text_stdout
 from ._compat import _find_binary_writer
 from ._compat import auto_wrap_for_ansi
 from ._compat import binary_streams
-from ._compat import get_filesystem_encoding
 from ._compat import open_stream
 from ._compat import should_strip_ansi
 from ._compat import strip_ansi
 from ._compat import text_streams
 from ._compat import WIN
 from .globals import resolve_color_default
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
-F = t.TypeVar("F", bound=t.Callable[..., t.Any])
+    P = te.ParamSpec("P")
+
+R = t.TypeVar("R")
 
 
 def _posixify(name: str) -> str:
     return "-".join(name.split()).lower()
 
 
-def safecall(func: F) -> F:
+def safecall(func: "t.Callable[P, R]") -> "t.Callable[P, t.Optional[R]]":
     """Wraps a function so that it swallows exceptions."""
 
-    def wrapper(*args, **kwargs):  # type: ignore
+    def wrapper(*args: "P.args", **kwargs: "P.kwargs") -> t.Optional[R]:
         try:
             return func(*args, **kwargs)
         except Exception:
             pass
+        return None
 
-    return update_wrapper(t.cast(F, wrapper), func)
+    return update_wrapper(wrapper, func)
 
 
 def make_str(value: t.Any) -> str:
     """Converts a value into a valid string."""
     if isinstance(value, bytes):
         try:
-            return value.decode(get_filesystem_encoding())
+            return value.decode(sys.getfilesystemencoding())
         except UnicodeError:
             return value.decode("utf-8", "replace")
     return str(value)
 
 
 def make_default_short_help(help: str, max_length: int = 45) -> str:
     """Returns a condensed version of help string."""
@@ -105,28 +108,29 @@
     the file but it does perform some basic checks early to see if the
     filename parameter does make sense.  This is useful for safely opening
     files for writing.
     """
 
     def __init__(
         self,
-        filename: str,
+        filename: t.Union[str, "os.PathLike[str]"],
         mode: str = "r",
         encoding: t.Optional[str] = None,
         errors: t.Optional[str] = "strict",
         atomic: bool = False,
     ):
-        self.name = filename
+        self.name: str = os.fspath(filename)
         self.mode = mode
         self.encoding = encoding
         self.errors = errors
         self.atomic = atomic
-        self._f: t.Optional[t.IO]
+        self._f: t.Optional[t.IO[t.Any]]
+        self.should_close: bool
 
-        if filename == "-":
+        if self.name == "-":
             self._f, self.should_close = open_stream(filename, mode, encoding, errors)
         else:
             if "r" in mode:
                 # Open and close the file in case we're opening it for
                 # reading so that we can catch at least some errors in
                 # some cases early.
                 open(filename, mode).close()
@@ -135,17 +139,17 @@
 
     def __getattr__(self, name: str) -> t.Any:
         return getattr(self.open(), name)
 
     def __repr__(self) -> str:
         if self._f is not None:
             return repr(self._f)
-        return f"<unopened file '{self.name}' {self.mode}>"
+        return f"<unopened file '{format_filename(self.name)}' {self.mode}>"
 
-    def open(self) -> t.IO:
+    def open(self) -> t.IO[t.Any]:
         """Opens the file if it's not yet open.  This call might fail with
         a :exc:`FileError`.  Not handling this error will produce an error
         that Click shows.
         """
         if self._f is not None:
             return self._f
         try:
@@ -170,33 +174,43 @@
         """
         if self.should_close:
             self.close()
 
     def __enter__(self) -> "LazyFile":
         return self
 
-    def __exit__(self, exc_type, exc_value, tb):  # type: ignore
+    def __exit__(
+        self,
+        exc_type: t.Optional[t.Type[BaseException]],
+        exc_value: t.Optional[BaseException],
+        tb: t.Optional[TracebackType],
+    ) -> None:
         self.close_intelligently()
 
     def __iter__(self) -> t.Iterator[t.AnyStr]:
         self.open()
         return iter(self._f)  # type: ignore
 
 
 class KeepOpenFile:
-    def __init__(self, file: t.IO) -> None:
-        self._file = file
+    def __init__(self, file: t.IO[t.Any]) -> None:
+        self._file: t.IO[t.Any] = file
 
     def __getattr__(self, name: str) -> t.Any:
         return getattr(self._file, name)
 
     def __enter__(self) -> "KeepOpenFile":
         return self
 
-    def __exit__(self, exc_type, exc_value, tb):  # type: ignore
+    def __exit__(
+        self,
+        exc_type: t.Optional[t.Type[BaseException]],
+        exc_value: t.Optional[BaseException],
+        tb: t.Optional[TracebackType],
+    ) -> None:
         pass
 
     def __repr__(self) -> str:
         return repr(self._file)
 
     def __iter__(self) -> t.Iterator[t.AnyStr]:
         return iter(self._file)
@@ -249,14 +263,19 @@
     """
     if file is None:
         if err:
             file = _default_text_stderr()
         else:
             file = _default_text_stdout()
 
+        # There are no standard streams attached to write to. For example,
+        # pythonw on Windows.
+        if file is None:
+            return
+
     # Convert non bytes/text into the native string type.
     if message is not None and not isinstance(message, (str, bytes, bytearray)):
         out: t.Optional[t.Union[str, bytes]] = str(message)
     else:
         out = message
 
     if nl:
@@ -336,15 +355,15 @@
 def open_file(
     filename: str,
     mode: str = "r",
     encoding: t.Optional[str] = None,
     errors: t.Optional[str] = "strict",
     lazy: bool = False,
     atomic: bool = False,
-) -> t.IO:
+) -> t.IO[t.Any]:
     """Open a file, with extra behavior to handle ``'-'`` to indicate
     a standard stream, lazy open on write, and atomic write. Similar to
     the behavior of the :class:`~click.File` param type.
 
     If ``'-'`` is given to open ``stdout`` or ``stdin``, the stream is
     wrapped so that using it in a context manager will not close it.
     This makes it possible to use the function without accidentally
@@ -366,42 +385,66 @@
         early, then closed until it is read again.
     :param atomic: Write to a temporary file and replace the given file
         on close.
 
     .. versionadded:: 3.0
     """
     if lazy:
-        return t.cast(t.IO, LazyFile(filename, mode, encoding, errors, atomic=atomic))
+        return t.cast(
+            t.IO[t.Any], LazyFile(filename, mode, encoding, errors, atomic=atomic)
+        )
 
     f, should_close = open_stream(filename, mode, encoding, errors, atomic=atomic)
 
     if not should_close:
-        f = t.cast(t.IO, KeepOpenFile(f))
+        f = t.cast(t.IO[t.Any], KeepOpenFile(f))
 
     return f
 
 
 def format_filename(
-    filename: t.Union[str, bytes, os.PathLike], shorten: bool = False
+    filename: "t.Union[str, bytes, os.PathLike[str], os.PathLike[bytes]]",
+    shorten: bool = False,
 ) -> str:
-    """Formats a filename for user display.  The main purpose of this
-    function is to ensure that the filename can be displayed at all.  This
-    will decode the filename to unicode if necessary in a way that it will
-    not fail.  Optionally, it can shorten the filename to not include the
-    full path to the filename.
+    """Format a filename as a string for display. Ensures the filename can be
+    displayed by replacing any invalid bytes or surrogate escapes in the name
+    with the replacement character ``�``.
+
+    Invalid bytes or surrogate escapes will raise an error when written to a
+    stream with ``errors="strict". This will typically happen with ``stdout``
+    when the locale is something like ``en_GB.UTF-8``.
+
+    Many scenarios *are* safe to write surrogates though, due to PEP 538 and
+    PEP 540, including:
+
+    -   Writing to ``stderr``, which uses ``errors="backslashreplace"``.
+    -   The system has ``LANG=C.UTF-8``, ``C``, or ``POSIX``. Python opens
+        stdout and stderr with ``errors="surrogateescape"``.
+    -   None of ``LANG/LC_*`` are set. Python assumes ``LANG=C.UTF-8``.
+    -   Python is started in UTF-8 mode  with  ``PYTHONUTF8=1`` or ``-X utf8``.
+        Python opens stdout and stderr with ``errors="surrogateescape"``.
 
     :param filename: formats a filename for UI display.  This will also convert
                      the filename into unicode without failing.
     :param shorten: this optionally shortens the filename to strip of the
                     path that leads up to it.
     """
     if shorten:
         filename = os.path.basename(filename)
+    else:
+        filename = os.fspath(filename)
+
+    if isinstance(filename, bytes):
+        filename = filename.decode(sys.getfilesystemencoding(), "replace")
+    else:
+        filename = filename.encode("utf-8", "surrogateescape").decode(
+            "utf-8", "replace"
+        )
 
-    return os.fsdecode(filename)
+    return filename
 
 
 def get_app_dir(app_name: str, roaming: bool = True, force_posix: bool = False) -> str:
     r"""Returns the config folder for the application.  The default behavior
     is to return whatever is most appropriate for the operating system.
 
     To give you an idea, for an app called ``"Foo Bar"``, something like
@@ -421,15 +464,15 @@
       ``C:\Users\<user>\AppData\Local\Foo Bar``
 
     .. versionadded:: 2.0
 
     :param app_name: the application name.  This should be properly capitalized
                      and can contain whitespace.
     :param roaming: controls if the folder should be roaming or not on Windows.
-                    Has no affect otherwise.
+                    Has no effect otherwise.
     :param force_posix: if this is set to `True` then on any POSIX system the
                         folder will be stored in the home folder with a leading
                         dot instead of the XDG config home or darwin's
                         application support folder.
     """
     if WIN:
         key = "APPDATA" if roaming else "LOCALAPPDATA"
@@ -454,15 +497,15 @@
     from ``.flush()`` being called on broken pipe during the shutdown/final-GC
     of the Python interpreter. Notably ``.flush()`` is always called on
     ``sys.stdout`` and ``sys.stderr``. So as to have minimal impact on any
     other cleanup code, and the case where the underlying file is not a broken
     pipe, all calls and attributes are proxied.
     """
 
-    def __init__(self, wrapped: t.IO) -> None:
+    def __init__(self, wrapped: t.IO[t.Any]) -> None:
         self.wrapped = wrapped
 
     def flush(self) -> None:
         try:
             self.wrapped.flush()
         except OSError as e:
             import errno
@@ -502,15 +545,16 @@
 
     if not path:
         path = sys.argv[0]
 
     # The value of __package__ indicates how Python was called. It may
     # not exist if a setuptools script is installed as an egg. It may be
     # set incorrectly for entry points created with pip on Windows.
-    if getattr(_main, "__package__", None) is None or (
+    # It is set to "" inside a Shiv or PEX zipapp.
+    if getattr(_main, "__package__", None) in {None, ""} or (
         os.name == "nt"
         and _main.__package__ == ""
         and not os.path.exists(path)
         and os.path.exists(f"{path}.exe")
     ):
         # Executed a file, like "python app.py".
         return os.path.basename(path)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `click-8.1.3/src/click.egg-info/PKG-INFO` & `click-8.1.4/src/click.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: click
-Version: 8.1.3
+Version: 8.1.4
 Summary: Composable command line interface toolkit
 Home-page: https://palletsprojects.com/p/click/
-Author: Armin Ronacher
-Author-email: armin.ronacher@active-4.com
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://click.palletsprojects.com/
 Project-URL: Changes, https://click.palletsprojects.com/changes/
 Project-URL: Source Code, https://github.com/pallets/click/
 Project-URL: Issue Tracker, https://github.com/pallets/click/issues/
-Project-URL: Twitter, https://twitter.com/PalletsTeam
 Project-URL: Chat, https://discord.gg/pallets
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -98,12 +94,8 @@
 -----
 
 -   Documentation: https://click.palletsprojects.com/
 -   Changes: https://click.palletsprojects.com/changes/
 -   PyPI Releases: https://pypi.org/project/click/
 -   Source Code: https://github.com/pallets/click
 -   Issue Tracker: https://github.com/pallets/click/issues
--   Website: https://palletsprojects.com/p/click
--   Twitter: https://twitter.com/PalletsTeam
 -   Chat: https://discord.gg/pallets
-
-
```

### Comparing `click-8.1.3/src/click.egg-info/SOURCES.txt` & `click-8.1.4/src/click.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 examples/repo/setup.py
 examples/termui/README
 examples/termui/setup.py
 examples/termui/termui.py
 examples/validation/README
 examples/validation/setup.py
 examples/validation/validation.py
+requirements/build.txt
 requirements/dev.txt
 requirements/docs.txt
 requirements/tests.txt
 requirements/typing.txt
 src/click/__init__.py
 src/click/_compat.py
 src/click/_termui_impl.py
```

### Comparing `click-8.1.3/tests/test_arguments.py` & `click-8.1.4/tests/test_arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from unittest import mock
 
 import pytest
 
 import click
 
 
 def test_nargs_star(runner):
@@ -82,17 +83,20 @@
     @click.argument("arg")
     def from_bytes(arg):
         assert isinstance(
             arg, str
         ), "UTF-8 encoded argument should be implicitly converted to Unicode"
 
     # Simulate empty locale environment variables
-    monkeypatch.setattr(sys.stdin, "encoding", "utf-8")
     monkeypatch.setattr(sys, "getfilesystemencoding", lambda: "utf-8")
     monkeypatch.setattr(sys, "getdefaultencoding", lambda: "utf-8")
+    # sys.stdin.encoding is readonly, needs some extra effort to patch.
+    stdin = mock.Mock(wraps=sys.stdin)
+    stdin.encoding = "utf-8"
+    monkeypatch.setattr(sys, "stdin", stdin)
 
     runner.invoke(
         from_bytes,
         ["Something outside of ASCII range: 林".encode()],
         catch_exceptions=False,
     )
 
@@ -373,7 +377,27 @@
     @cmd.command()
     def subcmd():
         click.echo("subcommand")
 
     result = runner.invoke(cli, ["arg1", "cmd", "arg2", "subcmd", "--help"])
     assert not result.exception
     assert "Usage: cli ARG1 cmd ARG2 subcmd [OPTIONS]" in result.output
+
+
+def test_when_argument_decorator_is_used_multiple_times_cls_is_preserved():
+    class CustomArgument(click.Argument):
+        pass
+
+    reusable_argument = click.argument("art", cls=CustomArgument)
+
+    @click.command()
+    @reusable_argument
+    def foo(arg):
+        pass
+
+    @click.command()
+    @reusable_argument
+    def bar(arg):
+        pass
+
+    assert isinstance(foo.params[0], CustomArgument)
+    assert isinstance(bar.params[0], CustomArgument)
```

### Comparing `click-8.1.3/tests/test_basic.py` & `click-8.1.4/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/tests/test_chain.py` & `click-8.1.4/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/tests/test_command_decorators.py` & `click-8.1.4/tests/test_command_decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,34 @@
         click.echo("hello")
 
     result = runner.invoke(cli)
     assert result.exception is None
     assert result.output == "hello\n"
 
 
+def test_custom_command_no_parens(runner):
+    class CustomCommand(click.Command):
+        pass
+
+    class CustomGroup(click.Group):
+        command_class = CustomCommand
+
+    @click.group(cls=CustomGroup)
+    def grp():
+        pass
+
+    @grp.command
+    def cli():
+        click.echo("hello custom command class")
+
+    result = runner.invoke(cli)
+    assert result.exception is None
+    assert result.output == "hello custom command class\n"
+
+
 def test_group_no_parens(runner):
     @click.group
     def grp():
         click.echo("grp1")
 
     @grp.command
     def cmd1():
```

### Comparing `click-8.1.3/tests/test_commands.py` & `click-8.1.4/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,28 +91,14 @@
             r"special-chars\s+Login and store the token in ~/.netrc\.\s*",
             result.output,
         )
         is not None
     )
 
 
-def test_help_truncation(runner):
-    @click.command()
-    def cli():
-        """This is a command with truncated help.
-        \f
-
-        This text should be truncated.
-        """
-
-    result = runner.invoke(cli, ["--help"])
-    assert result.exit_code == 0
-    assert "This is a command with truncated help." in result.output
-
-
 def test_no_args_is_help(runner):
     @click.command(no_args_is_help=True)
     def cli():
         pass
 
     result = runner.invoke(cli, [])
     assert result.exit_code == 0
@@ -407,7 +393,19 @@
     @group.command()
     @click.option("!e", is_flag=True)
     def command2(e):
         pass
 
     runner.invoke(group, ["command1"])
     assert opt_prefixes == {"-", "--", "~", "+"}
+
+
+@pytest.mark.parametrize("exc", (EOFError, KeyboardInterrupt))
+def test_abort_exceptions_with_disabled_standalone_mode(runner, exc):
+    @click.command()
+    def cli():
+        raise exc("catch me!")
+
+    rv = runner.invoke(cli, standalone_mode=False)
+    assert rv.exit_code == 1
+    assert isinstance(rv.exception.__cause__, exc)
+    assert rv.exception.__cause__.args == ("catch me!",)
```

### Comparing `click-8.1.3/tests/test_context.py` & `click-8.1.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/tests/test_custom_classes.py` & `click-8.1.4/tests/test_custom_classes.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/tests/test_formatting.py` & `click-8.1.4/tests/test_formatting.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,14 +292,34 @@
         "  wrapped but it will be rewrapped.",
         "",
         "Options:",
         "  --help  Show this message and exit.",
     ]
 
 
+def test_truncating_docstring_no_help(runner):
+    @click.command()
+    @click.pass_context
+    def cli(ctx):
+        """
+        \f
+
+        This text should be truncated.
+        """
+
+    result = runner.invoke(cli, ["--help"], terminal_width=60)
+    assert not result.exception
+    assert result.output.splitlines() == [
+        "Usage: cli [OPTIONS]",
+        "",
+        "Options:",
+        "  --help  Show this message and exit.",
+    ]
+
+
 def test_removing_multiline_marker(runner):
     @click.group()
     def cli():
         pass
 
     @cli.command()
     def cmd1():
```

### Comparing `click-8.1.3/tests/test_imports.py` & `click-8.1.4/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/tests/test_info_dict.py` & `click-8.1.4/tests/test_info_dict.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/tests/test_normalization.py` & `click-8.1.4/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/tests/test_options.py` & `click-8.1.4/tests/test_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -907,18 +907,14 @@
 
 
 @pytest.mark.parametrize(
     ("kwargs", "message"),
     [
         ({"count": True, "multiple": True}, "'count' is not valid with 'multiple'."),
         ({"count": True, "is_flag": True}, "'count' is not valid with 'is_flag'."),
-        (
-            {"multiple": True, "is_flag": True},
-            "'multiple' is not valid with 'is_flag', use 'count'.",
-        ),
     ],
 )
 def test_invalid_flag_combinations(runner, kwargs, message):
     with pytest.raises(TypeError) as e:
         click.Option(["-a"], **kwargs)
 
     assert message in str(e.value)
```

### Comparing `click-8.1.3/tests/test_parser.py` & `click-8.1.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/tests/test_shell_completion.py` & `click-8.1.4/tests/test_shell_completion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pytest
 
+import click.shell_completion
 from click.core import Argument
 from click.core import Command
 from click.core import Group
 from click.core import Option
+from click.shell_completion import add_completion_class
 from click.shell_completion import CompletionItem
 from click.shell_completion import ShellComplete
 from click.types import Choice
 from click.types import File
 from click.types import Path
 
 
@@ -338,7 +340,77 @@
 def test_choice_case_sensitive(value, expect):
     cli = Command(
         "cli",
         params=[Option(["-a"], type=Choice(["Au", "al", "Bc"], case_sensitive=value))],
     )
     completions = _get_words(cli, ["-a"], "a")
     assert completions == expect
+
+
+@pytest.fixture()
+def _restore_available_shells(tmpdir):
+    prev_available_shells = click.shell_completion._available_shells.copy()
+    click.shell_completion._available_shells.clear()
+    yield
+    click.shell_completion._available_shells.clear()
+    click.shell_completion._available_shells.update(prev_available_shells)
+
+
+@pytest.mark.usefixtures("_restore_available_shells")
+def test_add_completion_class():
+    # At first, "mysh" is not in available shells
+    assert "mysh" not in click.shell_completion._available_shells
+
+    class MyshComplete(ShellComplete):
+        name = "mysh"
+        source_template = "dummy source"
+
+    # "mysh" still not in available shells because it is not registered
+    assert "mysh" not in click.shell_completion._available_shells
+
+    # Adding a completion class should return that class
+    assert add_completion_class(MyshComplete) is MyshComplete
+
+    # Now, "mysh" is finally in available shells
+    assert "mysh" in click.shell_completion._available_shells
+    assert click.shell_completion._available_shells["mysh"] is MyshComplete
+
+
+@pytest.mark.usefixtures("_restore_available_shells")
+def test_add_completion_class_with_name():
+    # At first, "mysh" is not in available shells
+    assert "mysh" not in click.shell_completion._available_shells
+    assert "not_mysh" not in click.shell_completion._available_shells
+
+    class MyshComplete(ShellComplete):
+        name = "not_mysh"
+        source_template = "dummy source"
+
+    # "mysh" and "not_mysh" are still not in available shells because
+    # it is not registered yet
+    assert "mysh" not in click.shell_completion._available_shells
+    assert "not_mysh" not in click.shell_completion._available_shells
+
+    # Adding a completion class should return that class.
+    # Because we are using the "name" parameter, the name isn't taken
+    # from the class.
+    assert add_completion_class(MyshComplete, name="mysh") is MyshComplete
+
+    # Now, "mysh" is finally in available shells
+    assert "mysh" in click.shell_completion._available_shells
+    assert "not_mysh" not in click.shell_completion._available_shells
+    assert click.shell_completion._available_shells["mysh"] is MyshComplete
+
+
+@pytest.mark.usefixtures("_restore_available_shells")
+def test_add_completion_class_decorator():
+    # At first, "mysh" is not in available shells
+    assert "mysh" not in click.shell_completion._available_shells
+
+    @add_completion_class
+    class MyshComplete(ShellComplete):
+        name = "mysh"
+        source_template = "dummy source"
+
+    # Using `add_completion_class` as a decorator adds the new shell immediately
+    assert "mysh" in click.shell_completion._available_shells
+    assert click.shell_completion._available_shells["mysh"] is MyshComplete
```

### Comparing `click-8.1.3/tests/test_termui.py` & `click-8.1.4/tests/test_termui.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,16 +171,17 @@
 
 def test_progressbar_init_exceptions(runner):
     with pytest.raises(TypeError, match="iterable or length is required"):
         click.progressbar()
 
 
 def test_progressbar_iter_outside_with_exceptions(runner):
+    progress = click.progressbar(length=2)
+
     with pytest.raises(RuntimeError, match="with block"):
-        progress = click.progressbar(length=2)
         iter(progress)
 
 
 def test_progressbar_is_iterator(runner, monkeypatch):
     @click.command()
     def cli():
         with click.progressbar(range(10), label="test") as progress:
```

### Comparing `click-8.1.3/tests/test_testing.py` & `click-8.1.4/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `click-8.1.3/tests/test_utils.py` & `click-8.1.4/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,23 @@
     import io
 
     f = io.StringIO()
     click.echo("hello", file=f)
     assert f.getvalue() == "hello\n"
 
 
+def test_echo_no_streams(monkeypatch, runner):
+    """echo should not fail when stdout and stderr are None with pythonw on Windows."""
+    with runner.isolation():
+        sys.stdout = None
+        sys.stderr = None
+        click.echo("test")
+        click.echo("test", err=True)
+
+
 @pytest.mark.parametrize(
     ("styles", "ref"),
     [
         ({"fg": "black"}, "\x1b[30mx y\x1b[0m"),
         ({"fg": "red"}, "\x1b[31mx y\x1b[0m"),
         ({"fg": "green"}, "\x1b[32mx y\x1b[0m"),
         ({"fg": "yellow"}, "\x1b[33mx y\x1b[0m"),
@@ -94,18 +103,15 @@
 
 
 def test_filename_formatting():
     assert click.format_filename(b"foo.txt") == "foo.txt"
     assert click.format_filename(b"/x/foo.txt") == "/x/foo.txt"
     assert click.format_filename("/x/foo.txt") == "/x/foo.txt"
     assert click.format_filename("/x/foo.txt", shorten=True) == "foo.txt"
-
-    # filesystem encoding on windows permits this.
-    if not WIN:
-        assert click.format_filename(b"/x/foo\xff.txt", shorten=True) == "foo\udcff.txt"
+    assert click.format_filename(b"/x/\xff.txt", shorten=True) == "�.txt"
 
 
 def test_prompts(runner):
     @click.command()
     def test():
         if click.confirm("Foo"):
             click.echo("yes!")
@@ -442,14 +448,15 @@
     ("path", "main", "expected"),
     [
         ("example.py", None, "example.py"),
         (str(pathlib.Path("/foo/bar/example.py")), None, "example.py"),
         ("example", None, "example"),
         (str(pathlib.Path("example/__main__.py")), "example", "python -m example"),
         (str(pathlib.Path("example/cli.py")), "example", "python -m example.cli"),
+        (str(pathlib.Path("./example")), "", "example"),
     ],
 )
 def test_detect_program_name(path, main, expected):
     assert click.utils._detect_program_name(path, _main=MockMain(main)) == expected
 
 
 def test_expand_args(monkeypatch):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

