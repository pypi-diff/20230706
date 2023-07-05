# Comparing `tmp/documenteer-1.0.0a1.tar.gz` & `tmp/documenteer-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "documenteer-1.0.0a1.tar", last modified: Wed Jun  7 19:12:56 2023, max compression
+gzip compressed data, was "documenteer-1.0.0a2.tar", last modified: Wed Jul  5 22:30:50 2023, max compression
```

## Comparing `documenteer-1.0.0a1.tar` & `documenteer-1.0.0a2.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/workflows/ci-cron.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.npmrc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.nvmrc
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.prettierrc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    29338 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.718858 documenteer-1.0.0a1/demo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/demo/rst-technote/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29338 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/dev/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/dev/api/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.conf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.ext.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.requestsutils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxconfig.rst
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxext.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxrunner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.stackdocs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/html-templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/theme-assets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/theme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/documenteer.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/configuration-preset.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/diagrams.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/extend-conf-py.rst
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/openapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/organization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/pyproject-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/rst-epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/tabsets.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/toml-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/docs/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/build-overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/cpp-api-linking.rst
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/package-docs-cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/stack-docs-cli.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/docs/sphinx-extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/autocppapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/autodocreset.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/docushare-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/jira-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/lsst-pybtex-style.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/lssttasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/openapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/package-toctree.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/remote-code-block.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/docs/technotes/
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/technotes/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/technotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/technotes/refresh-lsst-bib.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/astropy-helpers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/sphinx-issue.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/sphinx.txt
--rw-r--r--   0 runner    (1001) docker     (123)   212497 2023-06-07 19:12:44.000000 documenteer-1.0.0a1/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/assets/rubin-technote/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/src/assets/rubin-technote/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/_hacks.scss
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/_properties.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/_index.scss
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/_version-info.scss
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/rubin-technote.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon-transparent-32px.png
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-pydata-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/scripts/rubin-technote.js
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/scripts/rubin-technote.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/styles/rubin-technote.css
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/styles/rubin-technote.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/bin/buildstackdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/bin/refreshlsstbib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/guide.py
--rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/pipelinespkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/technote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/technotebeta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/autodocreset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/requestsutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/sphinxconfig/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/stackconf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/technoteconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lsstdocushare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/configfieldlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/crossrefs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/pyapisummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/taskutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topiclists.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topics.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/remotecodeblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/stackdocs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/stackdocs/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1063166 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
--rw-r--r--   0 runner    (1001) docker     (123)   105749 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/data/doxygen.defaults.conf
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/data/mainpage.dox
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/doxygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/packagecli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/stackcli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/documenteer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/templates/pydata/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/pydata/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/templates/technote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/templates/technote/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/components/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.750858 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/header-article.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/sidebar-primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/afw.doxygen.conf
--rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/doxygen.tag.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/tests/data/package_alpha/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/data/package_alpha/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/tests/data/package_alpha/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/data/package_alpha/doc/_static/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/_static/package_alpha/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/doxygen.conf.in
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/manifest.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/doc/package.alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/package.alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/doc/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/package_alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/include/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/src/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/tests/data/package_beta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_beta/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_beta/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/roots/test-autocppapi/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/roots/test-autocppapi/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/roots/test-autocppapi/doxygen.tag.zip
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/roots/test-autocppapi/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_conf_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_conf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_ext_autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_refreshlsstbib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxconfig_stackconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_lsstdocushare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_lssttasks_taskutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_doxygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_technoteconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.973590 documenteer-1.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.945589 documenteer-1.0.0a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.github/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.945589 documenteer-1.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.github/workflows/ci-cron.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.nvmrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.prettierrc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.945589 documenteer-1.0.0a2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30895 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-05 22:30:50.973590 documenteer-1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.937589 documenteer-1.0.0a2/demo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.945589 documenteer-1.0.0a2/demo/rst-technote/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/demo/rst-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/demo/rst-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/demo/rst-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/demo/rst-technote/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/demo/rst-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.949589 documenteer-1.0.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30895 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.949589 documenteer-1.0.0a2/docs/dev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.949589 documenteer-1.0.0a2/docs/dev/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/api/documenteer.conf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/api/documenteer.ext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/api/documenteer.requestsutils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/api/documenteer.sphinxconfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/api/documenteer.sphinxext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/api/documenteer.sphinxrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/api/documenteer.stackdocs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/html-templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/theme-assets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/dev/theme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/documenteer.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.953590 documenteer-1.0.0a2/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/configuration-preset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/diagrams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/extend-conf-py.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/organization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/pyproject-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/rst-epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/tabsets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/guides/toml-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.953590 documenteer-1.0.0a2/docs/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/pipelines/build-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/pipelines/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/pipelines/cpp-api-linking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/pipelines/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/pipelines/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/pipelines/package-docs-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/pipelines/stack-docs-cli.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.953590 documenteer-1.0.0a2/docs/sphinx-extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/sphinx-extensions/autocppapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/sphinx-extensions/autodocreset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/sphinx-extensions/docushare-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/sphinx-extensions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/sphinx-extensions/jira-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/sphinx-extensions/lsst-pybtex-style.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/sphinx-extensions/lssttasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/sphinx-extensions/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/sphinx-extensions/package-toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/sphinx-extensions/remote-code-block.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.953590 documenteer-1.0.0a2/docs/technotes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/technotes/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/technotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/docs/technotes/refresh-lsst-bib.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.953590 documenteer-1.0.0a2/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/licenses/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/licenses/astropy-helpers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/licenses/sphinx-issue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/licenses/sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   212497 2023-07-05 22:30:38.000000 documenteer-1.0.0a2/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 22:30:50.973590 documenteer-1.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.941589 documenteer-1.0.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.941589 documenteer-1.0.0a2/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.941589 documenteer-1.0.0a2/src/assets/rubin-technote/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.953590 documenteer-1.0.0a2/src/assets/rubin-technote/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/assets/rubin-technote/styles/_hacks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/assets/rubin-technote/styles/_properties.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.957589 documenteer-1.0.0a2/src/assets/rubin-technote/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/assets/rubin-technote/styles/components/_index.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/assets/rubin-technote/styles/components/_version-info.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/assets/rubin-technote/styles/rubin-technote.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.957589 documenteer-1.0.0a2/src/documenteer/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.957589 documenteer-1.0.0a2/src/documenteer/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/assets/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.957589 documenteer-1.0.0a2/src/documenteer/assets/rsd-assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-05 22:30:40.000000 documenteer-1.0.0a2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-07-05 22:30:40.000000 documenteer-1.0.0a2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/assets/rubin-favicon-transparent-32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/assets/rubin-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/assets/rubin-pydata-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.957589 documenteer-1.0.0a2/src/documenteer/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-05 22:30:40.000000 documenteer-1.0.0a2/src/documenteer/assets/scripts/rubin-technote.js
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-05 22:30:40.000000 documenteer-1.0.0a2/src/documenteer/assets/scripts/rubin-technote.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.957589 documenteer-1.0.0a2/src/documenteer/assets/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-07-05 22:30:40.000000 documenteer-1.0.0a2/src/documenteer/assets/styles/rubin-technote.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-05 22:30:40.000000 documenteer-1.0.0a2/src/documenteer/assets/styles/rubin-technote.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.957589 documenteer-1.0.0a2/src/documenteer/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/bin/buildstackdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/bin/refreshlsstbib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.961590 documenteer-1.0.0a2/src/documenteer/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/conf/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/conf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/conf/guide.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/conf/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/conf/pipelinespkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/conf/technote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/conf/technotebeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.961590 documenteer-1.0.0a2/src/documenteer/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/ext/autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/ext/autodocreset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/ext/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/requestsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.961590 documenteer-1.0.0a2/src/documenteer/sphinxconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxconfig/stackconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxconfig/technoteconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxconfig/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.961590 documenteer-1.0.0a2/src/documenteer/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/lsstdocushare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.965590 documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/configfieldlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/crossrefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/pyapisummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/topiclists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/remotecodeblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/sphinxrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.965590 documenteer-1.0.0a2/src/documenteer/stackdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.965590 documenteer-1.0.0a2/src/documenteer/stackdocs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1063166 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   105749 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/data/doxygen.defaults.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/data/mainpage.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/packagecli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/stackdocs/stackcli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.941589 documenteer-1.0.0a2/src/documenteer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.965590 documenteer-1.0.0a2/src/documenteer/templates/pydata/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/templates/pydata/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.965590 documenteer-1.0.0a2/src/documenteer/templates/technote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/templates/technote/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.965590 documenteer-1.0.0a2/src/documenteer/templates/technote/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/templates/technote/components/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.965590 documenteer-1.0.0a2/src/documenteer/templates/technote/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/templates/technote/sections/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/templates/technote/sections/header-article.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/templates/technote/sections/sidebar-primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/src/documenteer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.957589 documenteer-1.0.0a2/src/documenteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-05 22:30:50.000000 documenteer-1.0.0a2/src/documenteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-05 22:30:50.000000 documenteer-1.0.0a2/src/documenteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:30:50.000000 documenteer-1.0.0a2/src/documenteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-05 22:30:50.000000 documenteer-1.0.0a2/src/documenteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-05 22:30:50.000000 documenteer-1.0.0a2/src/documenteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 22:30:50.000000 documenteer-1.0.0a2/src/documenteer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.969590 documenteer-1.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.969590 documenteer-1.0.0a2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/data/afw.doxygen.conf
+-rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/data/doxygen.tag.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.941589 documenteer-1.0.0a2/tests/data/package_alpha/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.969590 documenteer-1.0.0a2/tests/data/package_alpha/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.941589 documenteer-1.0.0a2/tests/data/package_alpha/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.969590 documenteer-1.0.0a2/tests/data/package_alpha/doc/_static/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/data/package_alpha/doc/_static/package_alpha/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/data/package_alpha/doc/doxygen.conf.in
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/data/package_alpha/doc/manifest.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.969590 documenteer-1.0.0a2/tests/data/package_alpha/doc/package.alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/data/package_alpha/doc/package.alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.969590 documenteer-1.0.0a2/tests/data/package_alpha/doc/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/data/package_alpha/doc/package_alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.969590 documenteer-1.0.0a2/tests/data/package_alpha/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/data/package_alpha/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.969590 documenteer-1.0.0a2/tests/data/package_alpha/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/data/package_alpha/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.941589 documenteer-1.0.0a2/tests/data/package_beta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.969590 documenteer-1.0.0a2/tests/data/package_beta/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/data/package_beta/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.941589 documenteer-1.0.0a2/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:30:50.973590 documenteer-1.0.0a2/tests/roots/test-autocppapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/roots/test-autocppapi/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/roots/test-autocppapi/doxygen.tag.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/roots/test-autocppapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_conf_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_conf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_ext_autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_refreshlsstbib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_sphinxconfig_stackconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_sphinxconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_sphinxext_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_sphinxext_lsstdocushare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_sphinxext_lssttasks_taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_sphinxext_mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_sphinxext_packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_sphinxext_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_stackdocs_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_stackdocs_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_stackdocs_doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_stackdocs_pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_stackdocs_rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tests/test_technoteconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-05 22:30:31.000000 documenteer-1.0.0a2/webpack.config.js
```

### Comparing `documenteer-1.0.0a1/.github/workflows/ci-cron.yaml` & `documenteer-1.0.0a2/.github/workflows/ci-cron.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/.github/workflows/ci.yaml` & `documenteer-1.0.0a2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/.gitignore` & `documenteer-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/.pre-commit-config.yaml` & `documenteer-1.0.0a2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.12.0]
         args: [-l, '79', -t, py38]
 
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
```

### Comparing `documenteer-1.0.0a1/.vscode/tasks.json` & `documenteer-1.0.0a2/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/CHANGELOG.md` & `documenteer-1.0.0a2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,62 @@
 - Drop support for Python 3.7.
 - Drop support for Sphinx versions earlier than 5.
 - Temporarily pin pydata-sphinx-theme < 0.13 on account of a change in logo path checking (affects user guide projects).
 - Use [sphinxcontrib-jquery](https://github.com/sphinx-contrib/jquery/) to ensure jQuery is available for user guide and Pipelines documentation builds.
 - Add a new `sphinx.exclude` field to `documenteer.toml` to list files for exclusion from a documentation project.
   More files and directories like `.venv` and `requirements.txt` are now excluded, as well.
 - New support for embedding OpenAPI documentation in a Redoc-generated subsite. The `documenteer.ext.openapi` extension can call a user-specified function to generate and install the OpenAPI specification the Sphinx source. For user guide projects, the `[project.openapi]` table in `documenteer.toml` can be used to configure both the `documenteer.ext.openapi` and `sphinxcontrib-redoc` extensions. [sphinxcontrib-redoc](https://sphinxcontrib-redoc.readthedocs.io/en/stable/) is installed and configured by default for all Rubin user guide projects (projects that use `documenteer.conf.guide`).
+- Pin pydantic < 2.0.
+
+## 0.8.1 (2023-06-27)
+
+Fixes:
+
+- Fixed a bug in the in the `help` subcommand for the `package-docs` and `stack-docs` commands.
+
+## 0.8.0 (2023-06-23)
+
+New features:
+
+- Added a `-W` / `--warning-is-error` flag to the `package-docs build` and `stack-docs build` commands for Science Pipelines documentation builds. This flag causes Sphinx to treat warnings as errors, which is useful for CI builds.
+- Also added a `-n` / `--nitpicky` flag that enables Sphinx's nitpicky mode to flag warnings when links cannot resolve.
+
+Fixes:
+
+- Pinned `sphinx-autodoc-typehints<1.23.0` to avoid a Sphinx version conflict with `sphinx-design`. The former required Sphinx >= 7.
+
+## 0.7.5 (2023-06-07)
+
+Fixes:
+
+- Use [sphinxcontrib-jquery](https://github.com/sphinx-contrib/jquery/) to ensure jQuery is available for user guide and Pipelines documentation builds. Sphinx 6 dropped jQuery from its default theme, and the new pydata-sphinx-theme v0.12 does not include it either.
+
+## 0.7.4 (2023-05-16)
+
+Fixes:
+
+- Pinned Sphinx < 7 for the `pipelines` and `technote` extras since their themes are not currently compatible with Sphinx 7 and later.
+
+## 0.7.3 (2023-03-20)
+
+Fixes:
+
+- Add `requirements.txt` and `.venv`/`venv` to the default `exclude_patterns` for User Guides.
+
+## 0.7.2 (2023-03-01)
+
+Fixes:
+
+- Temporarily pin pydata-sphinx-theme to <0.13. The new version changed how it treats light/dark logos.
+
+## 0.7.1 (2023-02-23)
+
+Fixes:
+
+- Temporarily pinning Mermaid to 9.4.0 in the User Guide configuration to workaround a change in the Mermaid CDN.
 
 ## 0.7.0 (2022-10-20)
 
 - Documenteer provides a new Sphinx configuration profile for general Rubin user guide projects, `documenteer.conf.guide`.
   This configuration profile features the new [pydata-sphinx-theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/), with customizations based on design tokens from the [Rubin Style Dictionary](https://style-dictionary.lsst.io).
   Most metadata and Sphinx configurations can also be set through a `documenteer.toml` file, located alongside the standard Sphinx `conf.py` file.
   Install `documenteer[guide]` with `pip` to get the dependencies needed for this Sphinx configuration.
```

### Comparing `documenteer-1.0.0a1/LICENSE` & `documenteer-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/PKG-INFO` & `documenteer-1.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,15 +46,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: guide
 Provides-Extra: technote
 Provides-Extra: pipelines
 License-File: LICENSE
 
-[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documentation.lsst.io)
+[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documenteer.lsst.io)
 [![PyPI](https://img.shields.io/pypi/v/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![For Python 3.7+](https://img.shields.io/pypi/pyversions/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![MIT license](https://img.shields.io/pypi/l/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml)
 [![Weekly CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml)
 
 # Documenteer
@@ -66,15 +66,15 @@
 Browse the [lsst-doc-engineering](https://github.com/topics/lsst-doc-engineering) GitHub topic for more Rubin Observatory documentation engineering projects.
 
 ## Quick installation:
 
 For [user guides](https://documenteer.lsst.io/guides/index.html):
 
 ```sh
-pip install "documenteer[technote]"
+pip install "documenteer[guide]"
 ```
 
 For [technical note projects](https://documenteer.lsst.io/technotes/index.html):
 
 ```sh
 pip install "documenteer[technote]"
 ```
```

### Comparing `documenteer-1.0.0a1/README.md` & `documenteer-1.0.0a2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documentation.lsst.io)
+[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documenteer.lsst.io)
 [![PyPI](https://img.shields.io/pypi/v/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![For Python 3.7+](https://img.shields.io/pypi/pyversions/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![MIT license](https://img.shields.io/pypi/l/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml)
 [![Weekly CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml)
 
 # Documenteer
@@ -14,15 +14,15 @@
 Browse the [lsst-doc-engineering](https://github.com/topics/lsst-doc-engineering) GitHub topic for more Rubin Observatory documentation engineering projects.
 
 ## Quick installation:
 
 For [user guides](https://documenteer.lsst.io/guides/index.html):
 
 ```sh
-pip install "documenteer[technote]"
+pip install "documenteer[guide]"
 ```
 
 For [technical note projects](https://documenteer.lsst.io/technotes/index.html):
 
 ```sh
 pip install "documenteer[technote]"
 ```
```

### Comparing `documenteer-1.0.0a1/demo/rst-technote/index.rst` & `documenteer-1.0.0a2/demo/rst-technote/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/Makefile` & `documenteer-1.0.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/_rst_epilog.rst` & `documenteer-1.0.0a2/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/changelog.md` & `documenteer-1.0.0a2/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,62 @@
 - Drop support for Python 3.7.
 - Drop support for Sphinx versions earlier than 5.
 - Temporarily pin pydata-sphinx-theme < 0.13 on account of a change in logo path checking (affects user guide projects).
 - Use [sphinxcontrib-jquery](https://github.com/sphinx-contrib/jquery/) to ensure jQuery is available for user guide and Pipelines documentation builds.
 - Add a new `sphinx.exclude` field to `documenteer.toml` to list files for exclusion from a documentation project.
   More files and directories like `.venv` and `requirements.txt` are now excluded, as well.
 - New support for embedding OpenAPI documentation in a Redoc-generated subsite. The `documenteer.ext.openapi` extension can call a user-specified function to generate and install the OpenAPI specification the Sphinx source. For user guide projects, the `[project.openapi]` table in `documenteer.toml` can be used to configure both the `documenteer.ext.openapi` and `sphinxcontrib-redoc` extensions. [sphinxcontrib-redoc](https://sphinxcontrib-redoc.readthedocs.io/en/stable/) is installed and configured by default for all Rubin user guide projects (projects that use `documenteer.conf.guide`).
+- Pin pydantic < 2.0.
+
+## 0.8.1 (2023-06-27)
+
+Fixes:
+
+- Fixed a bug in the in the `help` subcommand for the `package-docs` and `stack-docs` commands.
+
+## 0.8.0 (2023-06-23)
+
+New features:
+
+- Added a `-W` / `--warning-is-error` flag to the `package-docs build` and `stack-docs build` commands for Science Pipelines documentation builds. This flag causes Sphinx to treat warnings as errors, which is useful for CI builds.
+- Also added a `-n` / `--nitpicky` flag that enables Sphinx's nitpicky mode to flag warnings when links cannot resolve.
+
+Fixes:
+
+- Pinned `sphinx-autodoc-typehints<1.23.0` to avoid a Sphinx version conflict with `sphinx-design`. The former required Sphinx >= 7.
+
+## 0.7.5 (2023-06-07)
+
+Fixes:
+
+- Use [sphinxcontrib-jquery](https://github.com/sphinx-contrib/jquery/) to ensure jQuery is available for user guide and Pipelines documentation builds. Sphinx 6 dropped jQuery from its default theme, and the new pydata-sphinx-theme v0.12 does not include it either.
+
+## 0.7.4 (2023-05-16)
+
+Fixes:
+
+- Pinned Sphinx < 7 for the `pipelines` and `technote` extras since their themes are not currently compatible with Sphinx 7 and later.
+
+## 0.7.3 (2023-03-20)
+
+Fixes:
+
+- Add `requirements.txt` and `.venv`/`venv` to the default `exclude_patterns` for User Guides.
+
+## 0.7.2 (2023-03-01)
+
+Fixes:
+
+- Temporarily pin pydata-sphinx-theme to <0.13. The new version changed how it treats light/dark logos.
+
+## 0.7.1 (2023-02-23)
+
+Fixes:
+
+- Temporarily pinning Mermaid to 9.4.0 in the User Guide configuration to workaround a change in the Mermaid CDN.
 
 ## 0.7.0 (2022-10-20)
 
 - Documenteer provides a new Sphinx configuration profile for general Rubin user guide projects, `documenteer.conf.guide`.
   This configuration profile features the new [pydata-sphinx-theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/), with customizations based on design tokens from the [Rubin Style Dictionary](https://style-dictionary.lsst.io).
   Most metadata and Sphinx configurations can also be set through a `documenteer.toml` file, located alongside the standard Sphinx `conf.py` file.
   Install `documenteer[guide]` with `pip` to get the dependencies needed for this Sphinx configuration.
```

### Comparing `documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxext.rst` & `documenteer-1.0.0a2/docs/dev/api/documenteer.sphinxext.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/dev/api/documenteer.stackdocs.rst` & `documenteer-1.0.0a2/docs/dev/api/documenteer.stackdocs.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/dev/development.rst` & `documenteer-1.0.0a2/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/dev/html-templates.rst` & `documenteer-1.0.0a2/docs/dev/html-templates.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/dev/release.rst` & `documenteer-1.0.0a2/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/dev/theme-assets.rst` & `documenteer-1.0.0a2/docs/dev/theme-assets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/documenteer.toml` & `documenteer-1.0.0a2/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/badges.rst` & `documenteer-1.0.0a2/docs/guides/badges.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/configuration.rst` & `documenteer-1.0.0a2/docs/guides/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/diagrams.rst` & `documenteer-1.0.0a2/docs/guides/diagrams.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/extend-conf-py.rst` & `documenteer-1.0.0a2/docs/guides/extend-conf-py.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/index.rst` & `documenteer-1.0.0a2/docs/guides/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/openapi.rst` & `documenteer-1.0.0a2/docs/guides/openapi.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 .. code-block:: python
    :caption: src/main.py
 
    import json
 
    from fastapi import FastAPI
+   from fastapi.openapi.utils import get_openapi
 
 
    app = FastAPI()
 
 
    def create_openapi() -> str:
        """Create the OpenAPI spec for static documentation."""
```

### Comparing `documenteer-1.0.0a1/docs/guides/organization.rst` & `documenteer-1.0.0a2/docs/guides/organization.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/overview.rst` & `documenteer-1.0.0a2/docs/guides/overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/pyproject-configuration.rst` & `documenteer-1.0.0a2/docs/guides/pyproject-configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/rst-epilog.rst` & `documenteer-1.0.0a2/docs/guides/rst-epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/tabsets.rst` & `documenteer-1.0.0a2/docs/guides/tabsets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/guides/toml-reference.rst` & `documenteer-1.0.0a2/docs/guides/toml-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/index.rst` & `documenteer-1.0.0a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/pipelines/build-overview.rst` & `documenteer-1.0.0a2/docs/pipelines/build-overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/pipelines/configuration.rst` & `documenteer-1.0.0a2/docs/pipelines/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/pipelines/cpp-api-linking.rst` & `documenteer-1.0.0a2/docs/pipelines/cpp-api-linking.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/pipelines/index.rst` & `documenteer-1.0.0a2/docs/pipelines/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/pipelines/install.rst` & `documenteer-1.0.0a2/docs/pipelines/install.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/pipelines/package-docs-cli.rst` & `documenteer-1.0.0a2/docs/pipelines/package-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/pipelines/stack-docs-cli.rst` & `documenteer-1.0.0a2/docs/pipelines/stack-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/sphinx-extensions/autocppapi.rst` & `documenteer-1.0.0a2/docs/sphinx-extensions/autocppapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/sphinx-extensions/autodocreset.rst` & `documenteer-1.0.0a2/docs/sphinx-extensions/autodocreset.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/sphinx-extensions/docushare-reference.rst` & `documenteer-1.0.0a2/docs/sphinx-extensions/docushare-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/sphinx-extensions/jira-reference.rst` & `documenteer-1.0.0a2/docs/sphinx-extensions/jira-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/sphinx-extensions/lsst-pybtex-style.rst` & `documenteer-1.0.0a2/docs/sphinx-extensions/lsst-pybtex-style.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/sphinx-extensions/lssttasks.rst` & `documenteer-1.0.0a2/docs/sphinx-extensions/lssttasks.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/sphinx-extensions/openapi.rst` & `documenteer-1.0.0a2/docs/sphinx-extensions/openapi.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 .. code-block:: python
    :caption: src/main.py
 
    import json
 
    from fastapi import FastAPI
+   from fastapi.openapi.utils import get_openapi
 
 
    app = FastAPI()
 
 
    def create_openapi() -> str:
        """Create the OpenAPI spec for static documentation."""
```

### Comparing `documenteer-1.0.0a1/docs/sphinx-extensions/package-toctree.rst` & `documenteer-1.0.0a2/docs/sphinx-extensions/package-toctree.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/sphinx-extensions/remote-code-block.rst` & `documenteer-1.0.0a2/docs/sphinx-extensions/remote-code-block.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/technotes/configuration.rst` & `documenteer-1.0.0a2/docs/technotes/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/technotes/index.rst` & `documenteer-1.0.0a2/docs/technotes/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/docs/technotes/refresh-lsst-bib.rst` & `documenteer-1.0.0a2/docs/technotes/refresh-lsst-bib.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/licenses/astropy-helpers.txt` & `documenteer-1.0.0a2/licenses/astropy-helpers.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/licenses/sphinx-issue.txt` & `documenteer-1.0.0a2/licenses/sphinx-issue.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/licenses/sphinx.txt` & `documenteer-1.0.0a2/licenses/sphinx.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/package-lock.json` & `documenteer-1.0.0a2/package-lock.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/package.json` & `documenteer-1.0.0a2/package.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/pyproject.toml` & `documenteer-1.0.0a2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "PyYAML",
     "GitPython",
     "requests",
     "click",
     "sphinxcontrib-bibtex>=2.0.0",                  # for pybtex plugin; bibtex_bibfiles config is required.
     "importlib_metadata; python_version < \"3.8\"",
     "tomli; python_version < \"3.11\"",
-    "pydantic",
+    "pydantic < 2.0.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "twine",
     # Documenteer's testing and deployment deps
     "coverage[toml]",
@@ -57,15 +57,15 @@
     "types-docutils",
     "types-mock",
 ]
 guide = [
     # Theme and extensions for Rubin user guide projects
     "sphinx_design",
     "pydata-sphinx-theme>=0.10.0,<0.13.0",
-    "sphinx-autodoc-typehints",
+    "sphinx-autodoc-typehints<1.23.0",  # avoid requiring Sphinx > 7 only
     "sphinx-automodapi",
     "sphinx-copybutton",
     "sphinx-prompt",
     "myst-parser",
     "markdown-it-py[linkify]",
     "sphinxcontrib-mermaid",
     "sphinxext-opengraph",
```

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/favicon.ico` & `documenteer-1.0.0a2/src/documenteer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg` & `documenteer-1.0.0a2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg` & `documenteer-1.0.0a2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon-transparent-32px.png` & `documenteer-1.0.0a2/src/documenteer/assets/rubin-favicon-transparent-32px.png`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon.svg` & `documenteer-1.0.0a2/src/documenteer/assets/rubin-favicon.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/rubin-pydata-theme.css` & `documenteer-1.0.0a2/src/documenteer/assets/rubin-pydata-theme.css`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg` & `documenteer-1.0.0a2/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg` & `documenteer-1.0.0a2/src/documenteer/assets/rubin-titlebar-imagotype-light.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/scripts/rubin-technote.js` & `documenteer-1.0.0a2/src/documenteer/assets/scripts/rubin-technote.js`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/scripts/rubin-technote.js.map` & `documenteer-1.0.0a2/src/documenteer/assets/scripts/rubin-technote.js.map`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/styles/rubin-technote.css` & `documenteer-1.0.0a2/src/documenteer/assets/styles/rubin-technote.css`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/assets/styles/rubin-technote.css.map` & `documenteer-1.0.0a2/src/documenteer/assets/styles/rubin-technote.css.map`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/bin/buildstackdocs.py` & `documenteer-1.0.0a2/src/documenteer/bin/buildstackdocs.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/bin/refreshlsstbib.py` & `documenteer-1.0.0a2/src/documenteer/bin/refreshlsstbib.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/conf/_toml.py` & `documenteer-1.0.0a2/src/documenteer/conf/_toml.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/conf/_utils.py` & `documenteer-1.0.0a2/src/documenteer/conf/_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/conf/guide.py` & `documenteer-1.0.0a2/src/documenteer/conf/guide.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/conf/pipelines.py` & `documenteer-1.0.0a2/src/documenteer/conf/pipelines.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/conf/pipelinespkg.py` & `documenteer-1.0.0a2/src/documenteer/conf/pipelinespkg.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/conf/technote.py` & `documenteer-1.0.0a2/src/documenteer/conf/technote.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/conf/technotebeta.py` & `documenteer-1.0.0a2/src/documenteer/conf/technotebeta.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/ext/autocppapi.py` & `documenteer-1.0.0a2/src/documenteer/ext/autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/ext/autodocreset.py` & `documenteer-1.0.0a2/src/documenteer/ext/autodocreset.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/ext/openapi.py` & `documenteer-1.0.0a2/src/documenteer/ext/openapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/packagemetadata.py` & `documenteer-1.0.0a2/src/documenteer/packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/requestsutils.py` & `documenteer-1.0.0a2/src/documenteer/requestsutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxconfig/stackconf.py` & `documenteer-1.0.0a2/src/documenteer/sphinxconfig/stackconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxconfig/technoteconf.py` & `documenteer-1.0.0a2/src/documenteer/sphinxconfig/technoteconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxconfig/utils.py` & `documenteer-1.0.0a2/src/documenteer/sphinxconfig/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/__init__.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/bibtex.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/bibtex.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/jira.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/jira.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/lsstdocushare.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/__init__.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/configfieldlists.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/configfieldlists.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/crossrefs.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/crossrefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/pyapisummary.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/pyapisummary.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/taskutils.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topiclists.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/topiclists.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topics.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/lssttasks/topics.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/mockcoderefs.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/packagetoctree.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/remotecodeblock.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/remotecodeblock.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxext/utils.py` & `documenteer-1.0.0a2/src/documenteer/sphinxext/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/sphinxrunner.py` & `documenteer-1.0.0a2/src/documenteer/sphinxrunner.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 __all__ = ["run_sphinx"]
 
 
 def run_sphinx(
     root_dir: Union[str, Path],
     job_count: int = 1,
     warnings_as_errors: bool = False,
+    nitpicky: bool = False,
 ) -> int:
     """Run the Sphinx build process.
 
     Parameters
     ----------
     root_dir : `str`
         Root directory of the Sphinx project and content source. This directory
         contains both the root ``index.rst`` file and the ``conf.py``
         configuration file.
     job_count : `int`
         Number of cores to run the Sphinx build with (``-j`` flag)
+    warnings_as_errors : `bool`
+        If ``True``, treat Sphinx warnings as errors (``-W`` flag).
+    nitpicky : `bool`
+        If ``True``, activate Sphinx's nitpicky mode (``-n`` flag).
 
     Returns
     -------
     status : `int`
         Sphinx status code. ``0`` is expected. Greater than ``0`` indicates
         an error.
 
@@ -47,14 +52,16 @@
         "-b",
         "html",
         "-d",
         os.path.join("_build", ".doctrees"),
     ]
     if warnings_as_errors:
         argv.append("-W")
+    if nitpicky:
+        argv.append("-n")
     argv.extend([src_dir, os.path.join("_build", "html")])
 
     start_dir = os.path.abspath(".")
     try:
         os.chdir(src_dir)
         status = build_main(argv=argv)
     finally:
```

### Comparing `documenteer-1.0.0a1/src/documenteer/stackdocs/build.py` & `documenteer-1.0.0a2/src/documenteer/stackdocs/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     prefer_doxygen_conf_in: bool = True,
     enable_doxygen_conf: bool = True,
     enable_doxygen: bool = True,
     enable_package_links: bool = True,
     enable_sphinx: bool = True,
     select_doxygen_packages: Optional[List[str]] = None,
     skip_doxygen_packages: Optional[List[str]] = None,
+    warning_is_error: bool = False,
+    nitpicky: bool = False,
 ) -> int:
     """Build stack Sphinx documentation (main entrypoint).
 
     Parameters
     ----------
     root_project_dir
         Path to the root directory of the main documentation project. This
@@ -73,14 +75,19 @@
     select_doxygen_packages
         If set, only EUPS packages named in this sequence will be processed by
         Doxygen. Packages still need to be set up and have ``doxygen.conf.in``
         files.
     skip_doxygen_packages
         If set, EUPS packages named in this sequence will be removed from the
         set of packages processed by Doxygen.
+    warning_is_error
+        If ``True``, warnings from Sphinx will be treated as errors.
+    nitpicky
+        If ``True``, run Sphinx in "nitpicky" mode that generates warnings
+        for more things like unresolved links.
 
     Returns
     -------
     sphinx_status : `int`
         The shell status code for the Sphinx build. If ``enable_sphinx`` is
         ``False``, the status defaults to ``0``.
     """
@@ -232,15 +239,19 @@
         else:
             # Write the doxygen configuration for debugging
             doxygen_conf_path = doxygen_build_dir / "doxygen.conf"
             doxygen_conf_path.write_text(doxygen_conf.render())
 
     # Trigger the Sphinx build
     if enable_sphinx:
-        return run_sphinx(root_project_dir)
+        return run_sphinx(
+            root_project_dir,
+            warnings_as_errors=warning_is_error,
+            nitpicky=nitpicky,
+        )
     else:
         return 0
 
 
 def link_directories(root_dir, package_doc_dirs):
     """Create symlinks to package/module documentation directories from the
     root documentation project.
```

### Comparing `documenteer-1.0.0a1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml` & `documenteer-1.0.0a2/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/stackdocs/data/doxygen.defaults.conf` & `documenteer-1.0.0a2/src/documenteer/stackdocs/data/doxygen.defaults.conf`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/stackdocs/doxygen.py` & `documenteer-1.0.0a2/src/documenteer/stackdocs/doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/stackdocs/doxygentag.py` & `documenteer-1.0.0a2/src/documenteer/stackdocs/doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/stackdocs/packagecli.py` & `documenteer-1.0.0a2/src/documenteer/stackdocs/packagecli.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 __all__ = ("main",)
 
 import logging
 import os
 import shutil
 import sys
+from typing import Any
 
 import click
 
 from ..sphinxrunner import run_sphinx
 from .rootdiscovery import discover_package_doc_dir
 
 # Add -h as a help shortcut option
@@ -59,17 +60,15 @@
 
     The key commands provided by package-docs are:
 
     - ``package-docs build``: compile the package's documentation.
     - ``package-docs clean``: removes documentation build products from a
       package.
     """
-    root_dir = discover_package_doc_dir(root_dir)
-
-    # Subcommands should use the click.pass_obj decorator to get this
+    # Subcommands should use the click.pass_context decorator to get this
     # ctx.obj object as the first argument.
     ctx.obj = {"root_dir": root_dir, "verbose": verbose}
 
     # Set up application logging. This ensures that only documenteer's
     # logger is activated. If necessary, we can add other app's loggers too.
     if verbose:
         log_level = logging.DEBUG
@@ -90,22 +89,31 @@
     if topic is None:
         click.echo(ctx.parent.get_help())
     else:
         click.echo(main.commands[topic].get_help(ctx))
 
 
 @main.command()
+@click.option(
+    "-W", "--warning-is-error", is_flag=True, help="Treat warnings as errors."
+)
+@click.option(
+    "-n", "--nitpicky", is_flag=True, help="Activate Sphinx's nitpicky mode."
+)
 @click.pass_context
-def build(ctx):
+def build(ctx: Any, warning_is_error: bool, nitpicky: bool) -> None:
     """Build documentation as HTML.
 
     The build HTML site is located in the ``doc/_build/html`` directory
     of the package.
     """
-    return_code = run_sphinx(ctx.obj["root_dir"])
+    root_dir = discover_package_doc_dir(ctx.obj["root_dir"])
+    return_code = run_sphinx(
+        root_dir, warnings_as_errors=warning_is_error, nitpicky=nitpicky
+    )
     if return_code > 0:
         sys.exit(return_code)
 
 
 @main.command()
 @click.pass_context
 def clean(ctx):
@@ -118,17 +126,17 @@
     directory:
 
     - ``_build`` (the Sphinx build itself)
     - ``py-api`` (pages created by automodapi for the Python API reference)
     """
     logger = logging.getLogger(__name__)
 
+    root_dir = discover_package_doc_dir(ctx.obj["root_dir"])
+
     dirnames = ["py-api", "_build"]
-    dirnames = [
-        os.path.join(ctx.obj["root_dir"], dirname) for dirname in dirnames
-    ]
+    dirnames = [os.path.join(root_dir, dirname) for dirname in dirnames]
     for dirname in dirnames:
         if os.path.isdir(dirname):
             shutil.rmtree(dirname)
             logger.debug("Cleaned up %r", dirname)
         else:
             logger.debug("Did not clean up %r (missing)", dirname)
```

### Comparing `documenteer-1.0.0a1/src/documenteer/stackdocs/pkgdiscovery.py` & `documenteer-1.0.0a2/src/documenteer/stackdocs/pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/stackdocs/rootdiscovery.py` & `documenteer-1.0.0a2/src/documenteer/stackdocs/rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/stackdocs/stackcli.py` & `documenteer-1.0.0a2/src/documenteer/stackdocs/stackcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,15 @@
       clear the build cache.
 
     See also: package-docs, a tool for building previews of package
     documentation.
 
     For more information about stack-docs, see https://documenteer.lsst.io.
     """
-    root_project_dir = discover_conf_py_directory(root_project_dir)
-
-    # Subcommands should use the click.pass_obj decorator to get this
+    # Subcommands should use the click.pass_context decorator to get this
     # ctx.obj object as the first argument.
     ctx.obj = {"root_project_dir": root_project_dir, "verbose": verbose}
 
     # Set up application logging. This ensures that only documenteer's
     # logger is activated. If necessary, we can add other app's loggers too.
     if verbose:
         log_level = logging.DEBUG
@@ -158,26 +156,34 @@
     ),
 )
 @click.option(
     "--skip-dox",
     multiple=True,
     help=("Skip running Doxygen on these packages."),
 )
+@click.option(
+    "-W", "--warning-is-error", is_flag=True, help="Treat warnings as errors."
+)
+@click.option(
+    "-n", "--nitpicky", is_flag=True, help="Activate Sphinx's nitpicky mode."
+)
 @click.pass_context
 def build(
     ctx,
     skip,
     enable_doxygen_conf,
     enable_doxygen,
     enable_symlinks,
     enable_sphinx,
     use_doxygen_conf_in,
     doxygen_conf_defaults_path,
     dox,
     skip_dox,
+    warning_is_error,
+    nitpicky,
 ):
     """Build documentation as HTML.
 
     This command performs these steps:
 
     1. Removes any existing symlinks in the ``modules``, ``packages``, and
        ``_static`` directories.
@@ -193,30 +199,34 @@
 
     By default, the build site is located in the ``_build/html`` directory
     of the ``pipelines_lsst_io`` repository.
 
     To peek inside the build process, see the ``documenteer.stackdocs.build``
     APIs.
     """
+    root_project_dir = discover_conf_py_directory(ctx.obj["root_project_dir"])
+
     if doxygen_conf_defaults_path is not None:
         _doxygen_conf_defaults_path = Path(doxygen_conf_defaults_path)
     else:
         _doxygen_conf_defaults_path = None
 
     return_code = build_stack_docs(
-        ctx.obj["root_project_dir"],
+        root_project_dir,
         skipped_names=skip,
         prefer_doxygen_conf_in=use_doxygen_conf_in,
         doxygen_conf_defaults_path=_doxygen_conf_defaults_path,
         enable_doxygen_conf=enable_doxygen_conf,
         enable_doxygen=enable_doxygen,
         enable_package_links=enable_symlinks,
         enable_sphinx=enable_sphinx,
         select_doxygen_packages=dox,
         skip_doxygen_packages=skip_dox,
+        warning_is_error=warning_is_error,
+        nitpicky=nitpicky,
     )
     if return_code > 0:
         sys.exit(return_code)
 
 
 @main.command()
 @click.pass_context
@@ -233,18 +243,18 @@
     - ``modules`` (symlinks to the module doc directories of Stack packages)
     - ``packages`` (symlinks to the package doc directories of Stack packages)
     - ``py-api`` (pages created by automodapi for the Python API reference)
     - ``_doxygen`` (the Doxygen build)
     """
     logger = logging.getLogger(__name__)
 
+    root_project_dir = discover_conf_py_directory(ctx.obj["root_project_dir"])
     dirnames = ["py-api", "_build", "modules", "packages", "_doxygen"]
     dirnames = [
-        os.path.join(ctx.obj["root_project_dir"], dirname)
-        for dirname in dirnames
+        os.path.join(root_project_dir, dirname) for dirname in dirnames
     ]
     for dirname in dirnames:
         if os.path.isdir(dirname):
             shutil.rmtree(dirname)
             logger.debug("Cleaned up %r", dirname)
         else:
             logger.debug("Did not clean up %r (missing)", dirname)
@@ -298,17 +308,16 @@
 
         :lsstcc:`{{name}}`
 
     Example usage::
 
         stack-docs listcc -t class -t function -p lsst::afw::table
     """
-    tag_path = os.path.join(
-        ctx.obj["root_project_dir"], "_doxygen", "doxygen.tag"
-    )
+    root_project_dir = discover_conf_py_directory(ctx.obj["root_project_dir"])
+    tag_path = os.path.join(root_project_dir, "_doxygen", "doxygen.tag")
 
     if pattern:
         p = re.compile(pattern)
 
     if not api_types:
         api_types = [
             "namespace",
```

### Comparing `documenteer-1.0.0a1/src/documenteer/templates/technote/sections/header-article.html` & `documenteer-1.0.0a2/src/documenteer/templates/technote/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/utils.py` & `documenteer-1.0.0a2/src/documenteer/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer/version.py` & `documenteer-1.0.0a2/src/documenteer/version.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer.egg-info/PKG-INFO` & `documenteer-1.0.0a2/src/documenteer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,15 +46,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: guide
 Provides-Extra: technote
 Provides-Extra: pipelines
 License-File: LICENSE
 
-[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documentation.lsst.io)
+[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documenteer.lsst.io)
 [![PyPI](https://img.shields.io/pypi/v/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![For Python 3.7+](https://img.shields.io/pypi/pyversions/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![MIT license](https://img.shields.io/pypi/l/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml)
 [![Weekly CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml)
 
 # Documenteer
@@ -66,15 +66,15 @@
 Browse the [lsst-doc-engineering](https://github.com/topics/lsst-doc-engineering) GitHub topic for more Rubin Observatory documentation engineering projects.
 
 ## Quick installation:
 
 For [user guides](https://documenteer.lsst.io/guides/index.html):
 
 ```sh
-pip install "documenteer[technote]"
+pip install "documenteer[guide]"
 ```
 
 For [technical note projects](https://documenteer.lsst.io/technotes/index.html):
 
 ```sh
 pip install "documenteer[technote]"
 ```
```

### Comparing `documenteer-1.0.0a1/src/documenteer.egg-info/SOURCES.txt` & `documenteer-1.0.0a2/src/documenteer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/src/documenteer.egg-info/requires.txt` & `documenteer-1.0.0a2/src/documenteer.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Sphinx
 PyYAML
 GitPython
 requests
 click
 sphinxcontrib-bibtex>=2.0.0
-pydantic
+pydantic<2.0.0
 
 [:python_version < "3.11"]
 tomli
 
 [:python_version < "3.8"]
 importlib_metadata
 
@@ -26,15 +26,15 @@
 types-PyYAML
 types-docutils
 types-mock
 
 [guide]
 sphinx_design
 pydata-sphinx-theme<0.13.0,>=0.10.0
-sphinx-autodoc-typehints
+sphinx-autodoc-typehints<1.23.0
 sphinx-automodapi
 sphinx-copybutton
 sphinx-prompt
 myst-parser
 markdown-it-py[linkify]
 sphinxcontrib-mermaid
 sphinxext-opengraph
```

### Comparing `documenteer-1.0.0a1/tests/conftest.py` & `documenteer-1.0.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/data/afw.doxygen.conf` & `documenteer-1.0.0a2/tests/data/afw.doxygen.conf`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/data/doxygen.tag.zip` & `documenteer-1.0.0a2/tests/data/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/roots/test-autocppapi/conf.py` & `documenteer-1.0.0a2/tests/roots/test-autocppapi/conf.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/roots/test-autocppapi/doxygen.tag.zip` & `documenteer-1.0.0a2/tests/roots/test-autocppapi/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_conf_toml.py` & `documenteer-1.0.0a2/tests/test_conf_toml.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_conf_utils.py` & `documenteer-1.0.0a2/tests/test_conf_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_ext_autocppapi.py` & `documenteer-1.0.0a2/tests/test_ext_autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_packagemetadata.py` & `documenteer-1.0.0a2/tests/test_packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_refreshlsstbib.py` & `documenteer-1.0.0a2/tests/test_refreshlsstbib.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_sphinxconfig_stackconf.py` & `documenteer-1.0.0a2/tests/test_sphinxconfig_stackconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_sphinxconfig_utils.py` & `documenteer-1.0.0a2/tests/test_sphinxconfig_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_sphinxext_jira.py` & `documenteer-1.0.0a2/tests/test_sphinxext_jira.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_sphinxext_lsstdocushare.py` & `documenteer-1.0.0a2/tests/test_sphinxext_lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_sphinxext_lssttasks_taskutils.py` & `documenteer-1.0.0a2/tests/test_sphinxext_lssttasks_taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_sphinxext_mockcoderefs.py` & `documenteer-1.0.0a2/tests/test_sphinxext_mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_sphinxext_packagetoctree.py` & `documenteer-1.0.0a2/tests/test_sphinxext_packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_sphinxext_utils.py` & `documenteer-1.0.0a2/tests/test_sphinxext_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_stackdocs_build.py` & `documenteer-1.0.0a2/tests/test_stackdocs_build.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_stackdocs_doxygen.py` & `documenteer-1.0.0a2/tests/test_stackdocs_doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_stackdocs_doxygentag.py` & `documenteer-1.0.0a2/tests/test_stackdocs_doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_stackdocs_pkgdiscovery.py` & `documenteer-1.0.0a2/tests/test_stackdocs_pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_stackdocs_rootdiscovery.py` & `documenteer-1.0.0a2/tests/test_stackdocs_rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tests/test_technoteconf.py` & `documenteer-1.0.0a2/tests/test_technoteconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/tox.ini` & `documenteer-1.0.0a2/tox.ini`

 * *Files identical despite different names*

### Comparing `documenteer-1.0.0a1/webpack.config.js` & `documenteer-1.0.0a2/webpack.config.js`

 * *Files identical despite different names*

