# Comparing `tmp/sp_repo_review-2023.6.7.tar.gz` & `tmp/sp_repo_review-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jun  7 22:19:41 2023, max compression
+gzip compressed data, last modified: Thu Jul  6 19:13:47 2023, max compression
```

## Comparing `sp_repo_review-2023.6.7.tar` & `sp_repo_review-2023.7.6.tar`

### file list

```diff
@@ -1,116 +1,130 @@
--rw-r--r--   0        0        0      125 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.gitattributes
--rw-r--r--   0        0        0     2227 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      179 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      571 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.readthedocs.yml
--rw-r--r--   0        0        0        6 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.ruby-version
--rw-r--r--   0        0        0     1294 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/Gemfile
--rw-r--r--   0        0        0     2171 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/Gemfile.lock
--rw-r--r--   0        0        0     8658 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/README.md
--rw-r--r--   0        0        0     1160 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/_config.yml
--rw-r--r--   0        0        0      763 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/action.yml
--rw-r--r--   0        0        0      563 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/cookiecutter.json
--rw-r--r--   0        0        0     7033 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/noxfile.py
--rw-r--r--   0        0        0      640 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/dependabot.yml
--rw-r--r--   0        0        0      726 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1219 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2018 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-change-detection.yml
--rw-r--r--   0        0        0     5153 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-cookie.yml
--rw-r--r--   0        0        0      919 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-rr-tests.yml
--rw-r--r--   0        0        0      251 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/LICENSE
--rw-r--r--   0        0        0      730 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/README.md
--rw-r--r--   0        0        0     2180 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/head.html
--rw-r--r--   0        0        0     1019 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/head_custom.html
--rw-r--r--   0        0        0      547 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/interactive_repo_review.html
--rw-r--r--   0        0        0       92 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/rr.html
--rw-r--r--   0        0        0      150 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/toc.html
--rw-r--r--   0        0        0       22 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_sass/color_schemes/skhep.scss
--rw-r--r--   0        0        0     2611 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_sass/custom/custom.scss
--rw-r--r--   0        0        0    15086 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/favicon.ico
--rw-r--r--   0        0        0     8070 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      652 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/js/tabs.js
--rw-r--r--   0        0        0    10234 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/js/webapp.js
--rw-r--r--   0        0        0     2219 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/index.md
--rw-r--r--   0        0        0     4512 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/coverage.md
--rw-r--r--   0        0        0    11293 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_basic.md
--rw-r--r--   0        0        0     9205 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_pure.md
--rw-r--r--   0        0        0     8224 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_wheels.md
--rw-r--r--   0        0        0     2162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/index.md
--rw-r--r--   0        0        0     8606 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/mypy.md
--rw-r--r--   0        0        0    17927 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/packaging_classic.md
--rw-r--r--   0        0        0     9182 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/packaging_simple.md
--rw-r--r--   0        0        0    14552 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/pytest.md
--rw-r--r--   0        0        0      932 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/repo_review.md
--rw-r--r--   0        0        0    28595 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/style.md
--rw-r--r--   0        0        0     8853 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/tasks.md
--rw-r--r--   0        0        0     5310 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/writing-docs.md
--rw-r--r--   0        0        0     7027 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/patterns/data_files.md
--rw-r--r--   0        0        0      517 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/patterns/index.md
--rw-r--r--   0        0        0    11200 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/design.md
--rw-r--r--   0        0        0      561 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/index.md
--rw-r--r--   0        0        0     2209 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/process.md
--rw-r--r--   0        0        0     4816 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/dev-environment.md
--rw-r--r--   0        0        0      998 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/index.md
--rw-r--r--   0        0        0     2557 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/module.md
--rw-r--r--   0        0        0     3272 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/packaging.md
--rw-r--r--   0        0        0     4621 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/test.md
--rw-r--r--   0        0        0     1063 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/hooks/post_gen_project.py
--rw-r--r--   0        0        0      168 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      228 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/__init__.py
--rw-r--r--   0        0        0      166 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_version.pyi
--rw-r--r--   0        0        0      753 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/families.py
--rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0      290 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/__init__.py
--rw-r--r--   0        0        0     2849 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/general.py
--rw-r--r--   0        0        0     5018 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/github.py
--rw-r--r--   0        0        0     4133 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/mypy.py
--rw-r--r--   0        0        0     3162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/precommit.py
--rw-r--r--   0        0        0     5339 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/pyproject.py
--rw-r--r--   0        0        0     2868 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/ruff.py
--rw-r--r--   0        0        0      412 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/tests/test_cmd.py
--rw-r--r--   0        0        0      597 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/tests/test_package.py
--rw-r--r--   0        0        0      125 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitattributes
--rw-r--r--   0        0        0     2218 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2930 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      456 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.readthedocs.yml
--rw-r--r--   0        0        0      280 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/CMakeLists-skbuild.txt
--rw-r--r--   0        0        0      685 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/Cargo-maturin.toml
--rw-r--r--   0        0        0    14162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/LICENSE
--rw-r--r--   0        0        0      123 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/MANIFEST-setuptools,pybind11.in
--rw-r--r--   0        0        0     1910 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      909 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/meson-mesonpy.build
--rw-r--r--   0        0        0     2312 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/noxfile.py
--rw-r--r--   0        0        0     8580 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      723 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-pybind11.py
--rw-r--r--   0        0        0     1980 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools,pybind11.cfg
--rw-r--r--   0        0        0      374 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools.py
--rw-r--r--   0        0        0     2533 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/matchers/pylint.json
--rw-r--r--   0        0        0     3414 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1573 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/wheels-pybind11,skbuild,mesonpy,maturin.yml
--rw-r--r--   0        0        0     2031 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/docs/conf.py
--rw-r--r--   0        0        0      286 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/docs/index.rst
--rw-r--r--   0        0        0      562 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/lib-maturin.rs
--rw-r--r--   0        0        0      632 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/main-pybind11,skbuild,mesonpy.cpp
--rw-r--r--   0        0        0      430 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/__init__.py
--rw-r--r--   0        0        0      117 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_core-pybind11,skbuild,mesonpy,maturin.pyi
--rw-r--r--   0        0        0      118 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_version-setuptools,pybind11.pyi
--rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/py.typed
--rw-r--r--   0        0        0      213 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_compat/__init__.py
--rw-r--r--   0        0        0      498 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_compat/typing.py
--rw-r--r--   0        0        0      188 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/tests/test_compiled-pybind11,skbuild,mesonpy,maturin.py
--rw-r--r--   0        0        0      431 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/tests/test_package.py
--rw-r--r--   0        0        0     2248 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/LICENSE
--rw-r--r--   0        0        0     2375 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/README-rr.md
--rw-r--r--   0        0        0     5180 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/pyproject.toml
--rw-r--r--   0        0        0     3894 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.git_archival.txt
+-rw-r--r--   0        0        0       45 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.gitattributes
+-rw-r--r--   0        0        0     2547 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      179 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      702 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.readthedocs.yaml
+-rw-r--r--   0        0        0        6 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.ruby-version
+-rw-r--r--   0        0        0     1042 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/Gemfile
+-rw-r--r--   0        0        0     2737 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/Gemfile.lock
+-rw-r--r--   0        0        0    18677 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/README.md
+-rw-r--r--   0        0        0     1057 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/_config.yml
+-rw-r--r--   0        0        0      763 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/action.yml
+-rw-r--r--   0        0        0      877 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/cookiecutter.json
+-rw-r--r--   0        0        0     2120 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/copier.yml
+-rw-r--r--   0        0        0    11663 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/noxfile.py
+-rw-r--r--   0        0        0      640 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      162 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      825 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/bump.yml
+-rw-r--r--   0        0        0      726 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1219 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2109 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/reusable-change-detection.yml
+-rw-r--r--   0        0        0     5295 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/reusable-cookie.yml
+-rw-r--r--   0        0        0     1262 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/reusable-rr-tests.yml
+-rw-r--r--   0        0        0      251 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/LICENSE
+-rw-r--r--   0        0        0      829 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/README.md
+-rw-r--r--   0        0        0     2180 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/head.html
+-rw-r--r--   0        0        0     1019 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/head_custom.html
+-rw-r--r--   0        0        0      545 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/interactive_repo_review.html
+-rw-r--r--   0        0        0     2753 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/pyproject.md
+-rw-r--r--   0        0        0      145 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/toc.html
+-rw-r--r--   0        0        0      435 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_plugins/details.rb
+-rw-r--r--   0        0        0      512 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_plugins/repo_review.rb
+-rw-r--r--   0        0        0     1541 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_plugins/tabs.rb
+-rw-r--r--   0        0        0       22 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_sass/color_schemes/skhep.scss
+-rw-r--r--   0        0        0     2611 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_sass/custom/custom.scss
+-rw-r--r--   0        0        0    15086 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     8070 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      652 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/js/tabs.js
+-rw-r--r--   0        0        0    10211 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/js/webapp.js
+-rw-r--r--   0        0        0     3322 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/index.md
+-rw-r--r--   0        0        0     5085 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/coverage.md
+-rw-r--r--   0        0        0     9872 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/docs.md
+-rw-r--r--   0        0        0    22870 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/gha_basic.md
+-rw-r--r--   0        0        0     7836 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/gha_pure.md
+-rw-r--r--   0        0        0     8067 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/gha_wheels.md
+-rw-r--r--   0        0        0     2956 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/index.md
+-rw-r--r--   0        0        0    10386 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/mypy.md
+-rw-r--r--   0        0        0    18232 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/packaging_classic.md
+-rw-r--r--   0        0        0     9364 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/packaging_compiled.md
+-rw-r--r--   0        0        0     6194 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/packaging_simple.md
+-rw-r--r--   0        0        0    14312 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/pytest.md
+-rw-r--r--   0        0        0      947 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/repo_review.md
+-rw-r--r--   0        0        0    28349 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/style.md
+-rw-r--r--   0        0        0     9121 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/tasks.md
+-rw-r--r--   0        0        0     4260 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/backports.md
+-rw-r--r--   0        0        0     7171 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/data_files.md
+-rw-r--r--   0        0        0     3119 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/exports.md
+-rw-r--r--   0        0        0      738 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/index.md
+-rw-r--r--   0        0        0    11217 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/principles/design.md
+-rw-r--r--   0        0        0      561 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/principles/index.md
+-rw-r--r--   0        0        0     2209 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/principles/process.md
+-rw-r--r--   0        0        0     4526 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/dev-environment.md
+-rw-r--r--   0        0        0     4795 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/docs.md
+-rw-r--r--   0        0        0      998 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/index.md
+-rw-r--r--   0        0        0     2578 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/module.md
+-rw-r--r--   0        0        0     3300 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/packaging.md
+-rw-r--r--   0        0        0     4645 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/test.md
+-rw-r--r--   0        0        0      615 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/helpers/cog_helpers.py
+-rw-r--r--   0        0        0      699 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/helpers/extensions.py
+-rw-r--r--   0        0        0      246 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/__init__.py
+-rw-r--r--   0        0        0      166 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_version.pyi
+-rw-r--r--   0        0        0      822 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/families.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0      152 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/__init__.py
+-rw-r--r--   0        0        0     2849 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/general.py
+-rw-r--r--   0        0        0     5018 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/github.py
+-rw-r--r--   0        0        0     4133 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/mypy.py
+-rw-r--r--   0        0        0     3154 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/precommit.py
+-rw-r--r--   0        0        0     5339 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/pyproject.py
+-rw-r--r--   0        0        0     2565 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/readthedocs.py
+-rw-r--r--   0        0        0     3002 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/ruff.py
+-rw-r--r--   0        0        0      412 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/tests/test_cmd.py
+-rw-r--r--   0        0        0      597 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/tests/test_package.py
+-rw-r--r--   0        0        0      125 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.gitattributes
+-rw-r--r--   0        0        0     2218 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2901 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.readthedocs.yml
+-rw-r--r--   0        0        0     1689 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0     2928 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/noxfile.py
+-rw-r--r--   0        0        0     8661 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0     3987 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.__ci == 'gitlab' %}.gitlab-ci.yml{% endif %}
+-rw-r--r--   0        0        0      169 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}MANIFEST.in{% endif %}
+-rw-r--r--   0        0        0     2197 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}
+-rw-r--r--   0        0        0      691 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}
+-rw-r--r--   0        0        0      915 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}
+-rw-r--r--   0        0        0      727 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}
+-rw-r--r--   0        0        0      376 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='setuptools' %}setup.py{% endif %}
+-rw-r--r--   0        0        0      266 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='skbuild' %}CMakeLists.txt{% endif %}
+-rw-r--r--   0        0        0    11380 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'Apache' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0     1559 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'BSD' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0     1089 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'MIT' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0      102 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{{cookiecutter.__answers}}
+-rw-r--r--   0        0        0     2528 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/dependabot.yml
+-rwxr-xr-x   0        0        0      978 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}
+-rw-r--r--   0        0        0      668 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     3424 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1573 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type == 'compiled' %}wheels.yml{% endif %}
+-rw-r--r--   0        0        0      934 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/docs/conf.py
+-rw-r--r--   0        0        0      218 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0      632 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}
+-rw-r--r--   0        0        0      562 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}
+-rw-r--r--   0        0        0      422 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/py.typed
+-rw-r--r--   0        0        0      117 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.__type=='compiled' %}_core.pyi{% endif %}
+-rw-r--r--   0        0        0      118 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.backend in ['setuptools', 'pybind11'] %}_version.pyi{% endif %}
+-rw-r--r--   0        0        0      215 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/typing.py
+-rw-r--r--   0        0        0      378 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/tests/test_package.py
+-rw-r--r--   0        0        0      190 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/tests/{% if cookiecutter.__type=='compiled' %}test_compiled.py{% endif %}
+-rw-r--r--   0        0        0     2249 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.gitignore
+-rw-r--r--   0        0        0     1525 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/LICENSE
+-rw-r--r--   0        0        0     5530 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/pyproject.toml
+-rw-r--r--   0        0        0    10037 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/PKG-INFO
```

### Comparing `sp_repo_review-2023.6.7/.pre-commit-config.yaml` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,116 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
-exclude: "^({{cookiecutter\\.project_name}}|hooks/pre_gen_project.py$)"
-
 repos:
   - repo: https://github.com/psf/black
     rev: "23.3.0"
     hooks:
       - id: black-jupyter
 
-  - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
-    hooks:
-      - id: blacken-docs
-        additional_dependencies: [black==23.1.0]
-
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.270"
-    hooks:
-      - id: ruff
-        args: ["--fix", "--show-fixes"]
-
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: "v4.4.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
-        exclude: ^docs/_includes/rr.html$
       - id: mixed-line-ending
       - id: name-tests-test
         args: ["--pytest-test-first"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.10.0
+    rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
-    hooks:
-      - id: mypy
-        files: "(src|web|tests)"
-        args: []
-        additional_dependencies:
-          - click
-          - markdown-it-py
-          - pytest
-          - repo-review
-          - rich
-          - tomli
-          - types-PyYAML
-
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v2.7.1"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
+  - repo: https://github.com/asottile/blacken-docs
+    rev: "1.14.0"
+    hooks:
+      - id: blacken-docs
+        additional_dependencies: [black==23.3.0]
+
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.0.276"
+    hooks:
+      - id: ruff
+        args: ["--fix", "--show-fixes"]
+
+{%- if cookiecutter.backend == "setuptools" or cookiecutter.backend == "pybind11" %}
+
+  - repo: https://github.com/asottile/setup-cfg-fmt
+    rev: "v2.4.0"
+    hooks:
+      - id: setup-cfg-fmt
+        args: [--include-version-classifiers, --max-py-version=3.12]
+
+{%- endif %}
+
+{%- if cookiecutter.backend in ["pybind11", "skbuild", "mesonpy"] %}
+
+  - repo: https://github.com/pre-commit/mirrors-clang-format
+    rev: "v16.0.6"
+    hooks:
+      - id: clang-format
+        types_or: [c++, c, cuda]
+
+{%- endif %}
+
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: "v1.4.1"
+    hooks:
+      - id: mypy
+        files: src|tests
+        args: []
+        additional_dependencies:
+          - pytest
+
   - repo: https://github.com/codespell-project/codespell
-    rev: "v2.2.4"
+    rev: "v2.2.5"
     hooks:
       - id: codespell
-        exclude: ^Gemfile\.lock$
-        args: ["-Lnd"]
+
+  - repo: https://github.com/shellcheck-py/shellcheck-py
+    rev: "v0.9.0.5"
+    hooks:
+      - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
-        exclude: (.pre-commit-config.yaml|docs/pages/guides/style\.md)$
+        exclude: .pre-commit-config.yaml
+
+{%- if cookiecutter.backend in ["setuptools", "pybind11"] %}
+
+  - repo: https://github.com/mgedmin/check-manifest
+    rev: "0.49"
+    hooks:
+      - id: check-manifest
+        stages: [manual]
+{%- endif %}
+
+{%- if cookiecutter.backend == "skbuild" %}
+
+  - repo: https://github.com/cheshirekow/cmake-format-precommit
+    rev: "v0.6.13"
+    hooks:
+      - id: cmake-format
+
+{%- endif %}
```

### Comparing `sp_repo_review-2023.6.7/Gemfile.lock` & `sp_repo_review-2023.7.6/Gemfile.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,113 @@
 GEM
   remote: https://rubygems.org/
   specs:
-    addressable (2.8.1)
+    addressable (2.8.4)
       public_suffix (>= 2.0.2, < 6.0)
+    ast (2.4.2)
     colorator (1.1.0)
-    concurrent-ruby (1.1.10)
+    concurrent-ruby (1.2.2)
     em-websocket (0.5.3)
       eventmachine (>= 0.12.9)
       http_parser.rb (~> 0)
     eventmachine (1.2.7)
     ffi (1.15.5)
     forwardable-extended (2.6.0)
+    google-protobuf (3.23.3-x86_64-darwin)
+    google-protobuf (3.23.3-x86_64-linux)
     http_parser.rb (0.8.0)
-    i18n (1.12.0)
+    i18n (1.14.1)
       concurrent-ruby (~> 1.0)
-    jekyll (4.2.2)
+    jekyll (4.3.2)
       addressable (~> 2.4)
       colorator (~> 1.0)
       em-websocket (~> 0.5)
       i18n (~> 1.0)
-      jekyll-sass-converter (~> 2.0)
+      jekyll-sass-converter (>= 2.0, < 4.0)
       jekyll-watch (~> 2.0)
-      kramdown (~> 2.3)
+      kramdown (~> 2.3, >= 2.3.1)
       kramdown-parser-gfm (~> 1.0)
       liquid (~> 4.0)
-      mercenary (~> 0.4.0)
+      mercenary (>= 0.3.6, < 0.5)
       pathutil (~> 0.9)
-      rouge (~> 3.0)
+      rouge (>= 3.0, < 5.0)
       safe_yaml (~> 1.0)
-      terminal-table (~> 2.0)
-    jekyll-feed (0.16.0)
+      terminal-table (>= 1.8, < 4.0)
+      webrick (~> 1.7)
+    jekyll-feed (0.17.0)
       jekyll (>= 3.7, < 5.0)
-    jekyll-remote-theme (0.4.3)
-      addressable (~> 2.0)
-      jekyll (>= 3.5, < 5.0)
-      jekyll-sass-converter (>= 1.0, <= 3.0.0, != 2.0.0)
-      rubyzip (>= 1.3.0, < 3.0)
-    jekyll-sass-converter (2.2.0)
-      sassc (> 2.0.1, < 3.0)
+    jekyll-sass-converter (3.0.0)
+      sass-embedded (~> 1.54)
     jekyll-seo-tag (2.8.0)
       jekyll (>= 3.8, < 5.0)
     jekyll-watch (2.2.1)
       listen (~> 3.0)
-    just-the-docs (0.4.0.rc2)
+    json (2.6.3)
+    just-the-docs (0.5.3)
       jekyll (>= 3.8.5)
       jekyll-seo-tag (>= 2.0)
       rake (>= 12.3.1)
     kramdown (2.4.0)
       rexml
     kramdown-parser-gfm (1.1.0)
       kramdown (~> 2.0)
-    liquid (4.0.3)
-    listen (3.7.1)
+    liquid (4.0.4)
+    listen (3.8.0)
       rb-fsevent (~> 0.10, >= 0.10.3)
       rb-inotify (~> 0.9, >= 0.9.10)
     mercenary (0.4.0)
+    parallel (1.23.0)
+    parser (3.2.2.3)
+      ast (~> 2.4.1)
+      racc
     pathutil (0.16.2)
       forwardable-extended (~> 2.6)
-    public_suffix (5.0.0)
+    public_suffix (5.0.1)
+    racc (1.7.1)
+    rainbow (3.1.1)
     rake (13.0.6)
     rb-fsevent (0.11.2)
     rb-inotify (0.10.1)
       ffi (~> 1.0)
+    regexp_parser (2.8.1)
     rexml (3.2.5)
-    rouge (3.30.0)
-    rubyzip (2.3.2)
+    rouge (4.1.2)
+    rubocop (1.52.1)
+      json (~> 2.3)
+      parallel (~> 1.10)
+      parser (>= 3.2.2.3)
+      rainbow (>= 2.2.2, < 4.0)
+      regexp_parser (>= 1.8, < 3.0)
+      rexml (>= 3.2.5, < 4.0)
+      rubocop-ast (>= 1.28.0, < 2.0)
+      ruby-progressbar (~> 1.7)
+      unicode-display_width (>= 2.4.0, < 3.0)
+    rubocop-ast (1.29.0)
+      parser (>= 3.2.1.0)
+    ruby-progressbar (1.13.0)
     safe_yaml (1.0.5)
-    sassc (2.4.0)
-      ffi (~> 1.9)
-    terminal-table (2.0.0)
-      unicode-display_width (~> 1.1, >= 1.1.1)
-    unicode-display_width (1.8.0)
-    webrick (1.7.0)
+    sass-embedded (1.63.6)
+      google-protobuf (~> 3.23)
+      rake (>= 13.0.0)
+    terminal-table (3.0.2)
+      unicode-display_width (>= 1.1.1, < 3)
+    unicode-display_width (2.4.2)
+    wdm (0.1.1)
+    webrick (1.8.1)
 
 PLATFORMS
   x86_64-darwin-21
   x86_64-linux
 
 DEPENDENCIES
-  jekyll (~> 4.2)
+  jekyll (~> 4.3)
   jekyll-feed
-  jekyll-remote-theme
   jekyll-seo-tag
-  just-the-docs (= 0.4.0.rc2)
+  just-the-docs (~> 0.5.3)
   kramdown-parser-gfm
-  rake
+  rubocop (~> 1.52)
+  tzinfo (>= 1, < 3)
   tzinfo-data
-  webrick (~> 1.7)
+  wdm (~> 0.1.1)
 
 BUNDLED WITH
    2.3.7
```

### Comparing `sp_repo_review-2023.6.7/_config.yml` & `sp_repo_review-2023.7.6/_config.yml`

 * *Files 24% similar despite different names*

```diff
@@ -11,36 +11,36 @@
 markdown: kramdown
 theme: "just-the-docs"
 plugins:
   - jekyll-feed
 
 # Theme settings
 
-color_scheme: skhep
-
 logo: "/assets/images/logo.svg"
 
 # Enable or disable the site search
 search_enabled: true
 
 # Aux links for the upper right navigation
 aux_links:
   "Scientific Python Cookie":
     - "//github.com/scientific-python/cookie"
 
 gh_edit_link: true
 gh_edit_link_text: "View source for this page on GitHub."
 gh_edit_repository: "https://github.com/scientific-python/cookie"
 gh_edit_branch: "main"
+gh_edit_source: "docs"
 gh_edit_view_mode: "tree" # "tree" or "edit"
 
-# Exclude from processing.
-# The following items will not be processed, by default. Create a custom list
-# to override the default setting.
-# exclude:
-#   - Gemfile
-#   - Gemfile.lock
-#   - node_modules
-#   - vendor/bundle/
-#   - vendor/cache/
-#   - vendor/gems/
-#   - vendor/ruby/
+callouts:
+  warning:
+    color: red
+    title: Warning
+  note:
+    color: yellow
+    title: Note
+  important:
+    color: green
+    title: Important
+  highlight:
+    color: blue
```

### Comparing `sp_repo_review-2023.6.7/action.yml` & `sp_repo_review-2023.7.6/action.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/.devcontainer/devcontainer.json` & `sp_repo_review-2023.7.6/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/.github/workflows/cd.yml` & `sp_repo_review-2023.7.6/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/.github/workflows/ci.yml` & `sp_repo_review-2023.7.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/.github/workflows/reusable-change-detection.yml` & `sp_repo_review-2023.7.6/.github/workflows/reusable-change-detection.yml`

 * *Files 8% similar despite different names*

```diff
@@ -3,57 +3,62 @@
   workflow_call:
     outputs:
       run-cookie:
         description: Whether or not run the cookiecutter tests
         value: ${{ jobs.change-detection.outputs.run-cookie || false }}
       run-rr:
         description: Whether or not run the repo-review tests
-        value: ${{ jobs.change-detection.outputs.run-cookie || false }}
+        value: ${{ jobs.change-detection.outputs.run-rr || false }}
 
 jobs:
   change-detection:
     name: Identify source changes
     runs-on: ubuntu-latest
     timeout-minutes: 1
     outputs:
       run-cookie: ${{ steps.cookie-changes.outputs.run-cookie || false }}
       run-rr: ${{ steps.rr-changes.outputs.run-rr || false }}
     steps:
       - uses: actions/checkout@v3
 
-      - name: Get a list of the changed runtime-related files
+      - name: Changed cookie-related files
         if: github.event_name == 'pull_request'
         id: changed-cookie-files
         uses: Ana06/get-changed-files@v2.2.0
         with:
+          format: "json"
           filter: |
             {{cookiecutter.project_name}}/**
             .github/workflows/ci.yml
             .github/workflows/reusable-cookie.yml
             noxfile.py
             hooks/**
             cookiecutter.json
+            copier.yml
+            extensions.py
       - name: Set a flag for running the tests
         if: >-
           github.event_name != 'pull_request' ||
-          steps.changed-cookie-files.outputs.added_modified_renamed != ''
+          steps.changed-cookie-files.outputs.added_modified_renamed != '[]'
         id: cookie-changes
         run: echo "run-cookie=true" >> "${GITHUB_OUTPUT}"
 
-      - name: Get a list of the changed runtime-related files
+      - name: Changed sp-repo-review-related files
         if: github.event_name == 'pull_request'
         id: changed-rr-files
         uses: Ana06/get-changed-files@v2.2.0
         with:
+          format: "json"
           filter: |
-            tests/**
             .github/workflows/ci.yml
             .github/workflows/reusable-rr-tests.yml
+            README.md
             noxfile.py
-            src/**
             pyproject.toml
+            src/**
+            tests/**
       - name: Set a flag for running the tests
         if: >-
           github.event_name != 'pull_request' ||
-          steps.changed-rr-files.outputs.added_modified_renamed != ''
+          steps.changed-rr-files.outputs.added_modified_renamed != '[]'
         id: rr-changes
         run: echo "run-rr=true" >> "${GITHUB_OUTPUT}"
```

### Comparing `sp_repo_review-2023.6.7/.github/workflows/reusable-cookie.yml` & `sp_repo_review-2023.7.6/.github/workflows/reusable-cookie.yml`

 * *Files 5% similar despite different names*

```diff
@@ -51,27 +51,28 @@
 
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.11", "3.12-dev"]
+        python-version: ["3.8", "3.12"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
         include:
-          - python-version: pypy-3.8
+          - python-version: pypy-3.9
             runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
 
       - name: Install nox
         run: pip install nox
 
       - name: Test setuptools
         run: nox -s 'tests(setuptools)'
 
@@ -105,24 +106,29 @@
       - name: Test setuptools PEP 621
         run: nox -s 'tests(setuptools621)'
 
       - name: Native poetry tooling
         run: nox -s 'native(poetry)'
 
       - name: Native pdm tooling
-        if: matrix.python-version != 'pypy-3.7'
         run: nox -s 'native(pdm)'
 
       - name: Activate MSVC for Meson
         if: runner.os == 'Windows'
         uses: ilammy/msvc-dev-cmd@v1
 
       - name: Test meson-python
         run: nox -s 'tests(mesonpy)'
 
+      - name: Compare copier template generation
+        run: nox -s compare_copier
+
+      - name: Compare cruft template generation
+        run: nox -s compare_cruft
+
   nox:
     name: Check included Noxfile
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `sp_repo_review-2023.6.7/.github/workflows/reusable-rr-tests.yml` & `sp_repo_review-2023.7.6/.github/workflows/reusable-rr-tests.yml`

 * *Files 23% similar despite different names*

```diff
@@ -39,7 +39,24 @@
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Run sp-repo-review action
         uses: ./
+
+  cog:
+    name: Run cog on README
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+
+      - uses: actions/setup-python@v4
+        with:
+          python-version: "3.11"
+
+      - name: Rerender README
+        run: |
+          pipx run nox -s readme
+          git diff --exit-code
```

### Comparing `sp_repo_review-2023.6.7/docs/README.md` & `sp_repo_review-2023.7.6/docs/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Scientific Python Library Development Guide
 
 This is maintained by the scientific Python community for the benefit of fellow
 scientists and research software engineers. The repository contains:
 
 - A guide
-- A cookiecutter that generates a template for a scientific Python library
+- A copier/cookiecutter template that generates a template for a scientific
+  Python library
+- sp-repo-review, a plugin for [repo-review](https://repo-review.readthedocs.io)
 
 ## Contributing to the documentation
 
 To build locally, install rbenv (remember to run `rbenv init` after installing,
 and `rbenv install 3.1.2`). Then:
 
 ```bash
```

### Comparing `sp_repo_review-2023.6.7/docs/_includes/head.html` & `sp_repo_review-2023.7.6/docs/_includes/head.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/docs/_includes/head_custom.html` & `sp_repo_review-2023.7.6/docs/_includes/head_custom.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/docs/_sass/custom/custom.scss` & `sp_repo_review-2023.7.6/docs/_sass/custom/custom.scss`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/docs/assets/favicon.ico` & `sp_repo_review-2023.7.6/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/docs/assets/images/logo.svg` & `sp_repo_review-2023.7.6/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/docs/assets/js/tabs.js` & `sp_repo_review-2023.7.6/docs/assets/js/tabs.js`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/docs/assets/js/webapp.js` & `sp_repo_review-2023.7.6/docs/assets/js/webapp.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -272,15 +272,15 @@
         /MaterialUI.ThemeProvider>
     );
 }
 
 class App extends React.Component {
     constructor(props) {
         super(props);
-        const deps_str = props.deps.map((i) => `"${i}"`).join(", ");
+        const deps_str = props.deps.join(" ");
         this.state = {
             results: [],
             repo: urlParams.get("repo") || "",
             branch: urlParams.get("branch") || "",
             msg: `${DEFAULT_MSG} Packages: ${deps_str}`,
             progress: false,
             err_msg: "",
@@ -352,15 +352,15 @@
             }
             console.log(families);
             for (const val of results_list) {
                 results[val.family].push({
                     name: val.name.toString(),
                     description: val.description.toString(),
                     state: val.result,
-                    err_msg: val.err_markdown().toString(),
+                    err_msg: val.err_as_html().toString(),
                     url: val.url.toString(),
                 });
             }
 
             this.setState({
                 results: results,
                 families: families,
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/guides/coverage.md` & `sp_repo_review-2023.7.6/docs/pages/guides/coverage.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 permalink: /guides/coverage/
 nav_order: 3
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
+# Code Coverage
+
 The "Code coverage" value of a codebase indicates how much of the
 production/development code is covered by the running unit tests. Maintainers
 try their best to keep this percentage high, and this process is often automated
 using tools such as `GitHub Actions` and `Codecov`. Hence, code coverage becomes
 a good metric (not always) to check if a particular codebase is well tested and
 reliable.
 
@@ -19,38 +21,42 @@
 
 - `pytest-cov`: allows developers to calculate and visualize the coverage value
 - `Codecov`: integrates with remote repositories, allowing developers to see and
   compare coverage value with each CI run
 - `GitHub Actions`: allows users to automatically upload coverage reports to
   `Codecov`
 
-> ### Are there any alternatives?
+{: .note-title }
+
+> Are there any alternatives?
 >
 > `coverage.py` is a popular Python library used to calculate coverage values,
 > but it is usually paired with python's `unittest`. On the other hand,
 > `pytest-cov` is built to integrate with `pytest` with minimal extra
 > configurations. Further, Coveralls is an alternative coverage platform, but we
 > recommend using Codecov because of its ease of use and integration with GitHub
 > Actions.
 
-> ### Should increasing the coverage value be my top priority?
+{: .highlight-title }
+
+> Should increasing the coverage value be my top priority?
 >
 > A low coverage percentage will definitely motivate you to add more tests, but
 > adding weak tests just for coverage's sake is not a good idea. The tests
 > should test your codebase thoroughly and should not be unreliable.
 
 ### Calculating code coverage locally
 
 `pytest` allows users to pass the `--cov` option to automatically invoke
 `pytest-cov`, which then generates a `.coverage` file with the calculated
 coverage value. The value of `--cov` option should be set to the name of your
 package. For example, run the following command to run tests to generate a
 `.coverage` file for the vector package -
 
-```
+```bash
 python -m pytest -ra --cov=vector --cov-branch tests/
 ```
 
 `--cov` option will also print a minimal coverage report in the terminal itself!
 See the [docs](https://pytest-cov.readthedocs.io/en/latest/) for more options.
 The `--cov-branch` option will enable
 [branch coverage](https://linearb.io/blog/what-is-branch-coverage/).
@@ -58,15 +64,15 @@
 ### Calculating code coverage in your workflows
 
 Your workflows should also run tests with the `--cov` option, which must be set
 to your package name. For example -
 
 ```yaml
 - name: Test package
-  run: python -m pytest -ra --cov=vector tests/
+  run: python -m pytest --cov=vector tests/
 ```
 
 This will automatically invoke `pytest-cov`, and generate a `.coverage` file,
 which can then be uploaded to `Codecov` using the [codecov/codecov-action][]
 action.
 
 ### Configuring Codecov and uploading coverage reports
@@ -93,25 +99,39 @@
 ### Using codecov.yml
 
 One can also configure `Codecov` and coverage reports passed to `Codecov` using
 `codecov.yml`. `codecov.yml` should be placed inside the `.github` folder, along
 with your `workflows` folder. Additionally, `Codecov` allows you to create and
 edit this `YAML` file directly through your `Codecov` project's settings!
 
-A recommended configuration for `Codecov`:
+A recommended configuration for `.github/codecov.yml`:
 
 ```yaml
 codecov:
   notify:
     after_n_builds: x
+coverage:
+  status:
+    project:
+      default:
+        target: auto
+        threshold: 5%
+    patch:
+      default:
+        informational: true
 ```
 
 where `x` is the number of uploaded reports `Codecov` should wait to receive
 before sending statuses. This would ensure that the `Codecov` checks don't fail
-before all the coverage reports are uploaded. See the
+before all the coverage reports are uploaded. You can control the levels which
+are considered failing; the config above sets a loss of up to 5% as okay, and
+avoids patch coverage reporting a failure (otherwise, just changing a single
+uncovered line could cause a "failure" report on the PR). If you have 100%
+coverage, then you can remove the coverage failure settings, as you want any
+loss of coverage to fail. See the
 [docs](https://docs.codecov.com/docs/codecov-yaml) for all the options.
 
 <!-- ### Coverage for projects written in Python and C++
 
 TODO -->
 
 [codecov/codecov-action]: https://github.com/codecov/codecov-action
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/guides/gha_basic.md` & `sp_repo_review-2023.7.6/docs/pages/guides/mypy.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,348 +1,313 @@
 ---
 layout: page
-title: "GHA: GitHub Actions intro"
-permalink: /guides/gha-basic/
-nav_order: 11
+title: "Static type checking"
+permalink: /guides/mypy/
+nav_order: 9
 parent: Topical Guides
-custom_title: GitHub Actions introduction
 ---
 
 {% include toc.html %}
 
-{% include rr.html id="GH100" %} The recommended CI for scientific Python
-projects is GitHub Actions (GHA), although its predecessor Azure is also in
-heavy usage, and other popular services (Travis, Appveyor, and Circle CI) may be
-found in a few packages. GHA is preferred due to the flexible, extensible design
-and the tight integration with the GitHub permissions model (and UI). Here is a
-guide in setting up a new package with GHA.
+# Static type checking
 
-GHA is made up of workflows which consist of actions. Here are some of the
-workflows you will probably want in your package. These should be in a file
-named `.github/workflows/main.yml` or similar.
+## Basics
 
-## Header
+The most exciting thing happening right now in Python development is static
+typing. Since Python 3.0, we've had function annotations, and since 3.6,
+variable annotations. In 3.5, we got a "typing" library, which provides tools to
+describe types. This is what static type hints look like:
 
-Your main CI workflow file should begin something like this:
+```python
+def f(x: int) -> int:
+    return x * 5
+```
 
-```yaml
-name: CI
+This does nothing at runtime, except store the object. If you add
+`from __future__ import annotations`, it doesn't even store the actual object,
+just the string you type here, so then anything that can pass the Python parser
+is allowed here.
 
-on:
-  pull_request:
-  push:
-    branches:
-      - main
+It is not useless though! For one, it helps the reader. Knowing the types
+expected really gives you a much better idea of what is going on and what you
+can do and can't do.
 
-jobs:
-```
+But the key goal is: static type checking! There are a collection of static type
+checkers, the most "official" and famous of which is MyPy. You can think of this
+as the "compiler" for compiled languages like C++; it checks to make sure you
+are not lying about the types. For example, passing in anything that is not an
+int to `f` will fail a mypy check, _before you run or deploy any code_.
 
-This gives the workflow a nice name {% include rr.html id="GH101" %}, and
-defines the conditions under which it runs. This will run on all pull requests,
-or pushes to main. If you use a develop branch, you probably will want to
-include that. You can also specify specific branches for pull requests instead
-of running on all PRs (will run on PRs targeting those branches only).
+Your tests cannot test every possible branch, every line of code. MyPy can
+(though it doesn't by default, due to gradual typing). You may have code that
+runs rarely, that requires remote resources, that is slow, etc. All those can be
+checked by MyPy. It also keeps you (too?) truthful in your types.
 
-## Pre-commit
+### Adding types
 
-If you use [pre-commit](https://pre-commit.com) (and you should), and you don't
-want to / can't use [pre-commit.ci](https://pre-commit.ci) yet, then this is a
-job that will check pre-commit for you:
+There are three ways to add types.
 
-{% raw %}
+1. They can be inline as annotations. Best for Python 3 code, usually.
+2. They can be in special "type comments". Originally designed for Python 2
+   code, and still requires the proper imports.
+3. They can be in a separate file with the same name but with a `.pyi`
+   extension. This is important for type stubs or for cases where you don't want
+   to add imports or touch the original code. You can annotate compiled files or
+   libraries you don't control this way.
 
-```yaml
-lint:
-  name: Lint
-  runs-on: ubuntu-latest
-  steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: "3.x"
-    - uses: pre-commit/action@v3.0.0
-```
+If you have a library you don't control, you can add "type stubs" for it, then
+give MyPy your stubs directory. MyPy will pull the types from your stubs. If you
+are writing code for a Raspberry Pi, for example, you could add the stubs for
+the Pi libraries, and then validate your code, without ever even installing the
+Pi-only libraries!
 
-{% endraw %}
+You do not have to add types for every object - most of the time, you just need
+it for parameters and returns from functions. When running MyPy, you can use
+`reveal_type(...)` to show the inferred type of any object, which is like a
+print statement but at type-checking time, or `reveal_locals()` to see all local
+types.
 
-If you do use [pre-commit.ci](https://pre-commit.ci), but you need this job to
-run a manual check, like check-manifest, then you can keep it but just use
-`with: extra_args: --all-files --hook-stage manual check-manifest` to run just
-this one check. You can also use `needs: lint` in your other jobs to keep them
-from running if the lint check does not pass.
+### Configuration
 
-## Unit tests
+By default, MyPy does as little as possible, so that you can add it iteratively
+to a code base. By default:
 
-Implementing unit tests is also easy. Since you should be following best
-practices listed in the previous sections, this becomes an almost directly
-copy-and-paste formula, regardless of the package details. You might need to
-adjust the Python versions to suit your taste; you can also test on different
-OS's if you'd like by adding them to the matrix and inputting them into
-`runs-on`.
+- All untyped variables and return values will be `Any`.
+- Code inside untyped functions is not checked _at all_.
 
-{% raw %}
+You can add configuration to `pyproject.toml` (and a little bit to the files
+themselves), or you can go all the way and pass `--strict`, which will turn on
+everything. Try to turn on as much as possible, and increase it until you can
+run with full `strict` checking. See the [style page][] for configuration
+suggestions.
 
-```yaml
-tests:
-  runs-on: ubuntu-latest
-  strategy:
-    fail-fast: false
-    matrix:
-      python-version:
-        - "3.7"
-        - "3.11"
-        - "3.12-dev"
-  name: Check Python ${{ matrix.python-version }}
-  steps:
-    - uses: actions/checkout@v3
-      with:
-        fetch-depth: 0 # Only needed if using setuptools-scm
+[style page]: {% link pages/guides/style.md %}
 
-    - name: Setup Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.python-version }}
+For a library to support typing, it has to a) add types using any of the three
+methods, and b) add a `py.typed` empty file to indicate that it's okay to look
+for types inside it. MyPy also looks in `typeshed`, which is a library full of
+type hints for (mostly) the standard library.
 
-    - name: Install package
-      run: python -m pip install -e .[test]
-
-    - name: Test package
-      run: python -m pytest
-```
+Third party libraries that are typed sometimes forget this last step, by the
+way!
 
-{% endraw %}
+## Features
 
-A few things to note from above:
+### Type narrowing
 
-The matrix should contain the versions you are interested in. You can also test
-on other OS's if you are building any extensions or are worried about your
-package on macOS or Windows. Fail-fast is optional.
+One of the key features of type checking is type narrowing. The type checker
+monitors the types of a variable, and "narrows" it when something restricts it.
+For example:
 
-The formula here for installing should be identical for all users; and using
-[PEP 517](https://www.python.org/dev/peps/pep-0517/)/[518](https://www.python.org/dev/peps/pep-0518/)
-builds, you are even guaranteed a consistent wheel will be produced just as if
-you were building a final package.
+```python
+x: Union[A, B]
+if isinstance(x, A):
+    reveal_type(x)
+else:
+    reveal_type(x)
+```
 
-## Updating
+This will print `A`, then `B`. It prints `A` because that's the only thing that
+can exist in the first branch, and then the remaining types (`B`) must be the
+type in the second branch. And it prints both because it's not actually running
+the code, just type checking it, so both sides of the if are checked.
 
-{% include rr.html id="GH200" %} {% include rr.html id="GH210" %} If you use
-non-default actions in your repository (you will see some in the following
-pages), then it's a good idea to keep them up to date. GitHub provided a way to
-do this with dependabot. Just add the following file as
-`.github/dependabot.yml`:
+You can manually force type narrowing with assert:
 
-```yaml
-version: 2
-updates:
-  # Maintain dependencies for GitHub Actions
-  - package-ecosystem: "github-actions"
-    directory: "/"
-    schedule:
-      interval: "weekly"
+```python
+x: Union[A, B]
+assert isinstance(x, A)
+reveal_type(x)
 ```
 
-This will check to see if there are updates to the action weekly, and will make
-a PR if there are updates, including the changelog and commit summary in the PR.
-If you select a name like `v1`, this should only look for updates of the same
-form (since April 2022) - there is no need to restrict updates for "moving tag"
-updates anymore {% include rr.html id="PY006" %}. You can also use SHA's and
-dependabot will respect that too.
+This will print `A` because you removed B via the type narrowing using the
+`assert`.
 
-You can use this for other ecosystems too, including Python.
+### Protocols
 
-## Common needs
+One of the best features of MyPy is support for structural subtyping via
+Protocols - formalized duck-typing, basically. This allows cross library
+interoperability, unlike traditional inheritance. Here’s how it works:
 
-### Single OS steps
+```python
+from typing import Protocol
 
-If you need to have a step run only on a specific OS, use an if on that step
-with `runner.os`:
 
-```yaml
-if: runner.os != 'Windows' # also 'macOS' and 'Linux'
+class Duck(Protocol):
+    def quack() -> str:
+        ...
 ```
 
-Using `runner.os` is better than `matrix.<something>`. You also have an
-environment variable `$RUNNER_OS` as well. Single quotes are required here.
+Now any object that can "quack" (and return a string) is a Duck. We can even add
+`@runtime_checkable` which will allow us to check this (minus the types) at
+runtime in `isinstance`. So now we can design code like this:
 
-### Changing the environment in a step
+```python
+def pester_duck(a_duck: Duck) -> None:
+    print(a_duck.quack())
+    print(a_duck.quack())
+```
 
-If you need to change environment variables for later steps, such combining with
-an if condition for only for one OS, then you add it to a special file:
+And the type checker will ensure we only write code valid on all `Duck`s. And,
+we can write a duck implementation and test it like this:
 
-```yaml
-run: echo "MY_VAR=1" >> $GITHUB_ENV
+```python
+class MyDuck:
+    def quack() -> str:
+        return "quack"
 ```
 
-Later steps will see this environment variable.
+This will pass a check for being a `Duck`, for example something like this:
 
-### Common useful actions
+```python
+import typing
+
+if typing.TYPE_CHECKING:
+    _: Duck = typing.cast(MyDuck, None)
+```
 
-There are a variety of useful actions. There are GitHub supplied ones:
+Notice the complete lack of dependencies here. We don’t need `MyDuck` to write
+`pester_duck`, or vice-versa. And, we don't even need `Duck` to write either one
+at runtime! The dependence on `Duck` for `pester_duck` is entirely a
+type-check-time dependence (unless we want to use a `runtime_checkable` powered
+`isinstance`).
 
-- [actions/checkout](https://github.com/actions/checkout): Almost always the
-  first action. v2+ does not keep Git history unless `with: fetch-depth: 0` is
-  included (important for SCM versioning). v1 works on very old docker images.
-- [actions/setup-python](https://github.com/actions/setup-python): Do not use
-  v1; v2+ can setup any Python, including uninstalled ones and pre-releases. v4
-  requires a Python version to be selected.
-- [actions/cache](https://github.com/actions/cache): Can store files and restore
-  them on future runs, with a settable key.
-- [actions/upload-artifact](https://github.com/actions/upload-artifact): Upload
-  a file to be accessed from the UI or from a later job.
-- [actions/download-artifact](https://github.com/actions/download-artifact):
-  Download a file that was previously uploaded, often for releasing. Match
-  upload-artifact version.
+There are lots of built-in Protocols, most of which pre-date typing and are
+available in an Abstract Base Class form. Most of them check for one or more
+special methods, like `Iterable`, `Iterator`, etc.
 
-And many other useful ones:
+### Other features
 
-- [ilammy/msvc-dev-cmd](https://github.com/ilammy/msvc-dev-cmd): Setup MSVC
-  compilers.
-- [jwlawson/actions-setup-cmake](https://github.com/jwlawson/actions-setup-cmake):
-  Setup any version of CMake on almost any image.
-- [wntrblm/nox](https://github.com/wntrblm/nox): Setup all versions of Python
-  and provide nox.
-- [pypa/gh-action-pypi-publish](https://github.com/pypa/gh-action-pypi-publish):
-  Publish Python packages to PyPI.
-- [pre-commit/action](https://github.com/pre-commit/action): Run pre-commit with
-  built-in caching.
-- [conda-incubator/setup-miniconda](https://github.com/conda-incubator/setup-miniconda):
-  Setup conda or mamba on GitHub Actions.
-- [ruby/setup-ruby](https://github.com/ruby/setup-ruby) Setup Ruby if you need
-  it for something.
+Static typing has some great features worth checking out:
 
-There are also a few useful tools installed which can really simplify your
-workflow or adding custom actions. This includes system package managers (like
-brew, chocolaty, NuGet, Vcpkg, etc), as well as a fantastic cross platform one:
+- Unions (New syntax in Python 3.10)
+- Generic Types (New syntax in Python 3.9)
+- Literals
+- TypedDict
+- Nicer NamedTuple definition (very popular in Python 3 code)
+- MyPy validates with the Python version you ask for, regardless of what version
+  you are actually running.
 
-- [pipx](https://github.com/pypy/pipx): This is pre-installed on all runners
-  (GitHub uses to set up other things), and is kept up to date. It enables you
-  to use any PyPI application in a single line with `pipx run <app>`.
+## Complete example
 
-You can also run GitHub Actions locally:
+### Runtime compatible types
 
-- [act](https://github.com/nektos/act): Run GitHub Actions in a docker image
-  locally.
+Here's the classic syntax, which you need to use if you want to access the type
+annotations at runtime and you need to support Python < 3.10:
 
-### Custom actions
+```python
+from typing import Union, List
 
-You can
-[write your own actions](https://docs.github.com/en/actions/creating-actions)
-locally or in a shared GitHub repo in either GitHub actions syntax itself
-(called "composite"), JavaScript, or Docker. Combined with pipx, composite
-actions are very easy to write!
 
-You can also make reusable workflows.
+# Generic types take bracket arguments
+def f(x: int) -> List[int]:
+    return list(range(x))
 
-### GitHub pages
 
-GitHub has finished moving their pages build infrastructure to Actions, and they
-[now provide](https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/)
-the ability to directly push to Pages from Actions. This replaced the old
-workarounds of (force) pushing output to a branch or to separate repository.
+# Unions are a list of types that all could be allowed
+def g(x: Union[str, int]) -> None:
+    # Type narrowing - Unions get narrowed
+    if isinstance(x, str):
+        print("string", x.lower())
+    else:
+        print("int", x)
 
-<details markdown="1"><summary>Setting up GitHub Pages custom builds</summary>
+    # Calling x.lower() is invalid here!
+```
 
-Before starting, make sure in the Pages settings the source is set to "Actions".
+### Types as strings
 
-You'll probably want this job to run on both your main branch, as well as
-`workflow_dispatch`, just in case you want to manually trigger a rebuild. You
-should set the permission so that the built-in `GITHUB_TOKEN` can write to
-pages:
+If you don't access the types at runtime, or if you use Python 3.10+ only, then
+you can use a much nicer syntax. The `annotations` future feature causes the
+annotations to be stored as strings and not evaluated, which allows you to write
+things that are not yet valid, like `list[int]`!
 
-```yaml
-permissions:
-  contents: read
-  pages: write
-  id-token: write
-```
+```python
+from __future__ import annotations
 
-{% include rr.html id="GH103" %} You probably only want one deployment at a
-time, so you can use:
 
-```yaml
-concurrency:
-  group: "pages"
-  cancel-in-progress: true
-```
+def f(x: int) -> list[int]:
+    return list(range(x))
 
-Now you'll want three custom actions in your `steps:`. First, you need to
-configure Pages.
 
-```yaml
-- name: Setup Pages
-  id: pages
-  uses: actions/configure-pages@v3
+def g(x: str | int) -> None:
+    if isinstance(x, str):
+        print("string", x.lower())
+    else:
+        print("int", x)
 ```
 
-{% raw %}
+Notice that there are no imports from typing! Note that you cannot use the "new"
+syntax in non annotation locations (like unions in `isinstance`) unless Python
+supports it at runtime. And some libraries, like Typer and cattrs, use the
+annotations at runtime.
 
-Notice this action sets an `id:`; this will allow you to use the outputs from
-this action later; specifically, may want to use
-`${{ steps.pages.outputs.base_path }}` when building (you can also get `origin`,
-`base_url`, or `host` - see the action
-[config](https://github.com/actions/configure-pages/blob/main/action.yml)).
+You can use the above in earlier Python versions if you use strings manually,
+with the same caveats.
 
-{% endraw %}
+## Tips for good types
 
-```yaml
-- name: Upload artifact
-  uses: actions/upload-pages-artifact@v1
-```
+These are some guidelines to help you in writing good type hints.
 
-This actions defaults to uploading `_site`, but you can give any `with: path:`
-if you want, including `"."` which is the whole repository.
+### Loose vs. specific types
 
-Finally, you'll need to deploy the artifact (named `github-pages`) to Pages. You
-can make this a custom job with `needs:` pointing at your previous job (in this
-example, the previous job is called `build`):
+When you have a function, you should take as generic a type as possible, and
+return as specific a type as possible. For example:
 
-{% raw %}
+```python
+from __future__ import annotations
+from collections.abc import Iterable, Mapping
 
-```yaml
-deploy:
-  environment:
-    name: github-pages
-    url: ${{ steps.deployment.outputs.page_url }}
-  runs-on: ubuntu-latest
-  needs: [build]
-  steps:
-    - name: Deploy to GitHub Pages
-      id: deployment
-      uses: actions/deploy-pages@v2
-```
 
-{% endraw %}
-
-The deploy-pages job gives a `page_url`, which is the same as `base_url` on the
-configure step, and can be set in the `environment`. If you want to do
-everything in one job, you only need one of these.
+# Bad!!!
+def count(x: list[str]) -> Mapping[str, int]:
+    result = {}
+    for item in x:
+        result[x] = result.get(x, 0) + 1
+    return result
+```
 
-See the
-[official starter workflows](https://github.com/actions/starter-workflows/tree/main/pages)
-for examples.
+This will require the user pass a list to use this function, when in fact any
+iterable of strings would work just fine. Then, using valid dictionary
+operations on the return value, like mutating operations, will be marked as
+invalid, since your type checker don't know you have an actual dict. Compare
+with this:
 
-</details>
+```python
+# Good
+def count(x: Iterable[str]) -> dict[str, int]:
+    result = {}
+    for item in x:
+        result[x] = result.get(x, 0) + 1
+    return result
+```
 
-## Advanced usage
+Now all iterables are accepted, and the type checkers knows you have an actual
+dict in the return. Usually functions should take `Iterable` (if the argument is
+iterated once) or `Sequence` (if it is iterated multiple times or used with
+`in`), or `Mapping`, or `Set`. Very rarely you might need `MutableMapping` or
+`MutableSet`, and if you really do, having it in the type helps a reader know
+that it's going to be mutated.
 
-These are some things you might need.
+If you have an output type that depends on an input type, try to pass that
+through, usually using TypeVar (or the new generic syntax in Python 3.12, but
+that's not available for older Pythons via an import).
 
-### Cancel existing runs
+Also note that the best place to get these in modern Python is
+`collections.abc`, but if you need to subscript them at runtime, you'll need
+Python 3.9+ or the versions in `typing`.
 
-{% include rr.html id="GH102" %} If you add the following, you can ensure only
-one run per PR/branch happens at a time, cancelling the old run when a new one
-starts:
+## Final words
 
-{% raw %}
+When run alongside a good linter like flake8, this can catch a huge number of
+issues before tests or they are discovered in the wild! It also prompts _better
+design_, because you are thinking about how types work and interact. It's also
+more readable, since if I give you code like this:
 
-```yaml
-concurrency:
-  group: ${{ github.workflow }}-${{ github.ref }}
-  cancel-in-progress: true
+```python
+def compute(timestamp):
+    ...
 ```
 
-{% endraw %}
-
-Anything with a matching group name will count in the same group - the ref is
-the "from" name for the PR. If you want, you can replace `github.ref` with
-`github.event.pull_request.number || github.sha`; this will still cancel on PR
-pushes but will build each commit on `main`.
+You don't know "what" timestamp is. Is it an int? A float? An object? With
+types, you'll know what I was intending to give you. You can use type aliases to
+really give expressive names here!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/guides/gha_pure.md` & `sp_repo_review-2023.7.6/docs/pages/guides/gha_pure.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 ---
 layout: page
 title: "GHA: Pure Python wheels"
 permalink: /guides/gha-pure/
-nav_order: 12
+nav_order: 11
 parent: Topical Guides
 custom_title: GitHub Actions for pure Python wheels
 ---
 
 {% include toc.html %}
 
+# GitHub Actions: Pure Python wheels
+
 We will cover binary wheels [on the next page][], but if you do not have a
 compiled extension, this is called a universal (pure Python) package, and the
 procedure to make a "built" wheel is simple. At the end of this page, there is a
 recipe that can often be used exactly for pure Python wheels (if the previous
 recommendations were followed).
 
-> Note: Why make a wheel when there is nothing to compile? There are a multitude
-> of reasons that a wheel is better than only providing an sdist:
+{: .note }
+
+> Why make a wheel when there is nothing to compile? There are a multitude of
+> reasons that a wheel is better than only providing an sdist:
 >
-> - Wheels do not run setup.py, but simply install files into locations
+> - Wheels do not run `setup.py`, but simply install files into locations
 >   - Lower install requirements - users don't need your setup tools
 >   - Faster installs
 >   - Safer installs - no arbitrary code execution
 >   - Highly consistent installs
 > - Wheels pre-compile bytecode when they install
 >   - Initial import is not slower than subsequent import
 >   - Less chance of a permission issue
@@ -54,17 +58,14 @@
 instead of the releases - however, _please_ remember to make a GitHub release of
 your tag! It shows up in the GUI and it notifies anyone watching
 releases(-only). You will also need to change the event filter below.
 
 You can merge the CI job and the CD job if you want. To do that, preferably with
 the name "CI/CD", you can just combine the two `on` dicts.
 
-[`workflow_dispatch`]:
-  https://github.blog/changelog/2020-07-06-github-actions-manual-triggers-with-workflow_dispatch/
-
 ## Distribution: Pure Python wheels
 
 {% raw %}
 
 ```yaml
 dist:
   runs-on: ubuntu-latest
@@ -96,51 +97,41 @@
 different input folder if you want.
 
 You could use the setup-python action, install `build` and `twine` with `pip`,
 and then use `python -m build` or `pyproject-build`, but it's better to use
 `pipx` to install and run python applications. Pipx is provided by default by
 GitHub Actions (in fact, they use it to setup other applications).
 
-<details markdown="1"><summary>Classic SDist builds (click to expand)</summary>
-
-If you don't have a pyproject.toml, you might need to use the raw `setup.py`
-commands. This is the classic way to do things, though you should consider
-direct usage of setup.py to be an implementation detail, and setup.py is not
-even required in modern packages.
-
-You must install SDist requirements by hand since `python setup.py sdist` does
-not get the benefits of having pip install things. If you have any special
-requirements in your `pyproject.toml` (and still don't want to use `build`),
-you'll need to list them. This is special just for the SDist, not for making
-wheels (which should be done by the PEP 517/518 process for you because you will
-use `build` or `pip`).
-
-To build the wheel, you can use `python -m pip wheel . -w wheelhouse`. Unlike
-build, this is a wheelhouse, not the output wheel; any wheels it makes during
-the process will be put here, not just the one you wanted to upload. Be sure to
-use something like `wheelhouse/my_package*.whl` when you pick your items from
-this folder so as not to pick a random dependency that didn't have a binary
-wheel already. Or just use PyPA/build.
-
-</details>
-
 We upload the artifact just to make it available via the GitHub PR/Checks API.
 You can download a file to test locally if you want without making a release.
 
 We also add an optional check using twine for the metadata (it will be tested
 later in the upload action for the release job, as well).
 
-And then, you need a release job:
+{: .highlight-title }
+
+> All-in-one action
+>
+> There is an
+> [all-in-one action](https://github.com/hynek/build-and-inspect-python-package)
+> that does all the work for you for a pure Python package, including extra
+> pre-upload checks & nice GitHub summaries.
+>
+> ```yaml
+> steps:
+>   - uses: actions/checkout@v3
+>   - uses: hynek/build-and-inspect-python-package@v1
+> ```
+>
+> The artifact it produces is named `Packages`, so that's what you need to use
+> later to publish.
 
-<div class="skhep-bar d-flex m-2" style="justify-content:center;">
-  <button class="skhep-bar-item oidc-btn btn m-2 btn-purple" onclick="openTab('oidc')">Trusted Publishing</button>
-  <button class="skhep-bar-item token-btn btn m-2" onclick="openTab('token')" id='token-btn'>Token</button>
-</div>
+And then, you need a release job:
 
-<div class="skhep-tab oidc-tab" markdown="1">
+{% tabs %} {% tab oidc Trusted Publishing %}
 
 {% raw %}
 
 ```yaml
 publish:
   needs: [dist]
   environment: pypi
@@ -161,16 +152,15 @@
 
 When you make a GitHub release in the web UI, we publish to PyPI. You'll just
 need to tell PyPI which org, repo, workflow, and set the `pypi` environment to
 allow pushes from GitHub. If it's the first time you've published a package, go
 to the [PyPI trusted publisher docs] for instructions on preparing PyPI to
 accept your initial package publish.
 
-</div>
-<div class="skhep-tab token-tab" markdown="1" style="display:none;">
+{% endtab %} {% tab token Token %}
 
 {% raw %}
 
 ```yaml
 publish:
   needs: [dist]
   runs-on: ubuntu-latest
@@ -189,24 +179,24 @@
 {% endraw %}
 
 When you make a GitHub release in the web UI, we publish to PyPI. You'll need to
 go to PyPI, generate a token for your user, and put it into `pypi_password` on
 your repo's secrets page. Once you have a project, you should delete your
 user-scoped token and generate a new project-scoped token.
 
-</div>
+{% endtab %} {% endtabs %}
 
-<details markdown="1"><summary>Complete recipe (click to expand)</summary>
+{% details Complete recipe %}
 
 This can be used on almost any package with a standard
 `.github/workflows/cd.yml` recipe. This works because `pyproject.toml` describes
 exactly how to build your package, hence all packages build exactly via the same
 interface:
 
-<div class="skhep-tab oidc-tab" markdown="1">
+{% tabbodies %} {% tab oidc Trusted Publishing %}
 
 {% raw %}
 
 ```yaml
 name: CD
 
 on:
@@ -219,27 +209,18 @@
       - published
 
 jobs:
   dist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
-
         with:
           fetch-depth: 0
 
-      - name: Build SDist and wheel
-        run: pipx run build
-
-      - uses: actions/upload-artifact@v3
-        with:
-          path: dist/*
-
-      - name: Check metadata
-        run: pipx run twine check dist/*
+      - uses: hynek/build-and-inspect-python-package@v1
 
   publish:
     needs: [dist]
     environment: pypi
     permissions:
       id-token: write
     runs-on: ubuntu-latest
@@ -252,16 +233,15 @@
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@release/v1
 ```
 
 {% endraw %}
 
-</div>
-<div class="skhep-tab token-tab" markdown="1" style="display:none;">
+{% endtab %} {% tab token Token %}
 
 {% raw %}
 
 ```yaml
 name: CD
 
 on:
@@ -274,52 +254,45 @@
       - published
 
 jobs:
   dist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
-
         with:
           fetch-depth: 0
 
-      - name: Build SDist and wheel
-        run: pipx run build
-
-      - uses: actions/upload-artifact@v3
-        with:
-          path: dist/*
-
-      - name: Check metadata
-        run: pipx run twine check dist/*
+      - uses: hynek/build-and-inspect-python-package@v1
 
   publish:
     needs: [dist]
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
       - uses: actions/download-artifact@v3
         with:
-          name: artifact
+          name: Packages
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.pypi_password }}
 ```
 
 {% endraw %}
 
-</div>
+{% endtab %} {% endtabbodies %}
 
-</details>
+{% enddetails %}
 
 <!-- prettier-ignore-start -->
 
 [pep 517]: https://www.python.org/dev/peps/pep-0517/
 [pep 518]: https://www.python.org/dev/peps/pep-0518/
 [pypi trusted publisher docs]: https://docs.pypi.org/trusted-publishers/creating-a-project-through-oidc/
+[`workflow_dispatch`]: https://github.blog/changelog/2020-07-06-github-actions-manual-triggers-with-workflow_dispatch/
+
 
 <!-- prettier-ignore-end -->
 
 <script src="{% link assets/js/tabs.js %}"></script>
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/guides/gha_wheels.md` & `sp_repo_review-2023.7.6/docs/pages/guides/gha_wheels.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 ---
 layout: page
 title: "GHA: Binary wheels"
 permalink: /guides/gha-wheels/
-nav_order: 13
+nav_order: 12
 parent: Topical Guides
 custom_title: GitHub Actions for Binary Wheels
 ---
 
 {% include toc.html %}
 
+# GitHub Actions: Binary wheels
+
 Building binary wheels is a bit more involved, but can still be done effectively
 with GHA. This document will introduce [cibuildwheel][] for use in your project.
 The benefits of cibuildwheel are a larger user base, fast fixes from CI and pip,
 works on all major CI vendors (no lock-in), and covers cases we were not able to
 cover (like ARM). We will focus on GHA below.
 
 ## Header
@@ -115,15 +117,15 @@
 
   steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
         submodules: true
 
-    - uses: pypa/cibuildwheel@v2.13.0
+    - uses: pypa/cibuildwheel@v2.13.1
 
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         path: wheelhouse/*.whl
 ```
 
@@ -156,20 +158,15 @@
 You can even put any docker image here, as needed by the project. Note that
 manylinux1 was discontinued on Jan 1, 2022, and updates will cease whenever they
 break. If you always need a specific image, you can set that in the
 `pyproject.toml` file instead.
 
 ## Publishing
 
-<div class="skhep-bar d-flex m-2" style="justify-content:center;">
-  <button class="skhep-bar-item oidc-btn btn  m-2 btn-purple" onclick="openTab('oidc')">Trusted Publishing</button>
-  <button class="skhep-bar-item token-btn btn m-2" onclick="openTab('token')">Token</button>
-</div>
-
-<div class="skhep-tab oidc-tab" markdown="1">
+{% tabs %} {% tab oidc Trusted Publishing %}
 
 {% raw %}
 
 ```yaml
 upload_all:
   needs: [build_wheels, make_sdist]
   environment: pypi
@@ -190,16 +187,15 @@
 
 When you make a GitHub release in the web UI, we publish to PyPI. You'll just
 need to tell PyPI which org, repo, workflow, and set the `pypi` environment to
 allow pushes from GitHub. If it's the first time you've published a package, go
 to the [PyPI trusted publisher docs] for instructions on preparing PyPI to
 accept your initial package publish.
 
-</div>
-<div class="skhep-tab token-tab" markdown="1" style="display:none;">
+{% endtab %} {% tab token Token %}
 
 {% raw %}
 
 ```yaml
 upload_all:
   needs: [build_wheels, make_sdist]
   runs-on: ubuntu-latest
@@ -218,27 +214,32 @@
 {% endraw %}
 
 When you make a GitHub release in the web UI, we publish to PyPI. You'll need to
 go to PyPI, generate a token for your user, and put it into `pypi_password` on
 your repo's secrets page. Once you have a project, you should delete your
 user-scoped token and generate a new project-scoped token.
 
-</div>
+{% endtab %} {% endtabs %}
 
 If you have multiple jobs, you will want to collect your artifacts from above.
 If you only have one job, you can combine this into a single job like we did for
 pure Python wheels, using dist instead of wheelhouse. If you upload from
 multiple places, you can set `skip_existing` (but generally it's better to not
 try to upload the same file from two places - you can trick Travis into avoiding
 the sdist, for example).
 
+{: .note-title }
+
+> Other architectures
+>
 > On Travis, `cibuildwheel` even has the ability to create ARM and PowerPC
 > builds natively. IBM Z builds are also available but in beta. However, due to
 > Travis CI's recent dramatic reduction on open source support, emulating these
-> architectures on GHA or Azure is probably better.
+> architectures on GHA or Azure is probably better. Maybe look into Cirrus CI,
+> which has some harder-to-find architectures.
 
 <!-- prettier-ignore-start -->
 
 [`cibw_before_build`]: https://cibuildwheel.readthedocs.io/en/stable/options/#before-build
 [`cibw_environment`]: https://cibuildwheel.readthedocs.io/en/stable/options/#environment
 [cibw custom]: https://cibuildwheel.readthedocs.io/en/stable/options/#build-skip
 [cibuildwheel]: https://cibuildwheel.readthedocs.io/en/stable/
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/guides/mypy.md` & `sp_repo_review-2023.7.6/docs/pages/guides/tasks.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,259 +1,289 @@
 ---
 layout: page
-title: "Static type checking"
-permalink: /guides/mypy/
-nav_order: 8
+title: Task runners
+permalink: /guides/tasks/
+nav_order: 30
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
-## Basics
+# Task runners
 
-The most exciting thing happening right now in Python development is static
-typing. Since Python 3.0, we've had function annotations, and since 3.6,
-variable annotations. In 3.5, we got a "typing" library, which provides tools to
-describe types. This is what static type hints look like:
+A task runner, like [make][] (fully general), [rake][] (Ruby general),
+[invoke][] (Python general), [tox][] (Python packages), or [nox][] (Python
+simi-general), is a tool that lets you specify a set of tasks via a common
+interface. These have been discouraged by some community projects in the past,
+since they can be a crutch, allowing poor packaging practices to be employed
+behind a custom script, and they can hide what is actually happening.
+
+We are carefully allowing an exception: [nox][]. Nox has two strong points that
+help with the above concerns. First, it is very explicit, and even prints what
+it is doing as it operates. Unlike the older tox, it does not have any implicit
+assumptions built-in. Second, it has very elegant built-in support for both
+virtual and Conda environments. This can greatly reduce new contributor friction
+with your codebase.
+
+A daily developer is _not_ expected to use nox for simple tasks, like running
+tests or linting. You should _not_ rely on nox to make a task that should be
+made simple and standard (like building a package) complicated. You are not
+expected to use nox for linting on CI, or often even for testing on CI, even if
+those tasks are provided for users. Nox is a few seconds slower than running
+directly in a custom environment - but for new users, and rarely run tasks, it
+is _much_ faster than explaining how to get setup or manually messing with
+virtual environments. It is also highly reproducible, creating and destroying
+the temporary environment each time.
+
+{% rr PY007 %} You _should_ use nox to make it easy and simple for new
+contributors to run things. You _should_ use nox to make specialized developer
+tasks easy. You _should_ use nox to avoid making single-use virtual environments
+for docs and other rarely run tasks.
+
+Nox doesn't handle binary builds very well, so for compiled projects, it might
+be best left to just specialized tasks.
+
+[nox]: https://nox.thea.codes
+[tox]: https://tox.readthedocs.io
+[invoke]: https://www.pyinvoke.org
+[rake]: https://ruby.github.io/rake/
+[make]: https://www.gnu.org/software/make/
+
+## Nox
+
+### Installing
+
+Installing nox should be handled like any other Python _application_. You should
+either use a good package manager, like brew on macOS, or you should use pipx;
+either permanently (`pipx install nox`) or by running `pipx run nox` instead of
+`nox`.
+
+On GitHub Actions or Azure, pipx is available by default, so you should use
+`pipx run nox`. To give it access to all Python versions, you can use this
+action:
 
-```python
-def f(x: int) -> int:
-    return x * 5
+```yaml
+- uses: wntrblm/nox@2022.8.7
 ```
 
-This does nothing at runtime, except store the object. If you add
-`from __future__ import annotations`, it doesn't even store the actual object,
-just the string you type here, so then anything that can pass the Python parser
-is allowed here.
-
-It is not useless though! For one, it helps the reader. Knowing the types
-expected really gives you a much better idea of what is going on and what you
-can do and can't do.
-
-But the key goal is: static type checking! There are a collection of static type
-checkers, the most "official" and famous of which is MyPy. You can think of this
-as the "compiler" for compiled languages like C++; it checks to make sure you
-are not lying about the types. For example, passing in anything that is not an
-int to `f` will fail a mypy check, _before you run or deploy any code_.
-
-Your tests cannot test every possible branch, every line of code. MyPy can
-(though it doesn't by default, due to gradual typing). You may have code that
-runs rarely, that requires remote resources, that is slow, etc. All those can be
-checked by MyPy. It also keeps you (too?) truthful in your types.
-
-### Adding types
-
-There are three ways to add types.
-
-1. They can be inline as annotations. Best for Python 3 code, usually.
-2. They can be in special "type comments". Originally designed for Python 2
-   code, and still requires the proper imports.
-3. They can be in a separate file with the same name but with a `.pyi`
-   extension. This is important for type stubs or for cases where you don't want
-   to add imports or touch the original code. You can annotate compiled files or
-   libraries you don't control this way.
-
-If you have a library you don't control, you can add "type stubs" for it, then
-give MyPy your stubs directory. MyPy will pull the types from your stubs. If you
-are writing code for a Raspberry Pi, for example, you could add the stubs for
-the Pi libraries, and then validate your code, without ever even installing the
-Pi-only libraries!
-
-You do not have to add types for every object - most of the time, you just need
-it for parameters and returns from functions. When running MyPy, you can use
-`reveal_type(...)` to show the inferred type of any object, which is like a
-print statement but at type-checking time, or `reveal_locals()` to see all local
-types.
-
-### Configuration
+You can now access all current versions of Python from nox. At least in GitHub
+Actions, you should add `--forcecolor` to your nox runs to get color output in
+your logs, or set `env: FORCE_COLOR: 3`. If you'd like to customise the versions
+of Python prepared for you, then use this input:
+
+```yaml
+- uses: wntrblm/nox@2022.8.7
+  with:
+    python-versions: "3.8, 3.9, 3.10, 3.11, 3.12, pypy-3.9, pypy-3.10-nightly"
+```
 
-By default, MyPy does as little as possible, so that you can add it iteratively
-to a code base. By default:
+### Introduction
 
-- All untyped variables and return values will be `Any`.
-- Code inside untyped functions is not checked _at all_.
+Nox is a tool for running tasks, called "sessions", inside temporary virtual
+environments. It is configured through Python and is designed to resemble
+pytest. The file it looks for is called `noxfile.py` by default. This is an
+example of a simple nox file:
 
-You can add configuration to `pyproject.toml` (and a little bit to the files
-themselves), or you can go all the way and pass `--strict`, which will turn on
-everything. Try to turn on as much as possible, and increase it until you can
-run with full `strict` checking. See the [style page][] for configuration
-suggestions.
+```python
+import nox
 
-[style page]: {% link pages/guides/style.md %}
 
-For a library to support typing, it has to a) add types using any of the three
-methods, and b) add a `py.typed` empty file to indicate that it's okay to look
-for types inside it. MyPy also looks in `typeshed`, which is a library full of
-type hints for (mostly) the standard library.
+@nox.session
+def tests(session: nox.Session) -> None:
+    """
+    Run the unit and regular tests.
+    """
+    session.install(".[test]")
+    session.run("pytest", *session.posargs)
+```
 
-Third party libraries that are typed sometimes forget this last step, by the
-way!
+This will create a session called `tests`. The function receives the "session"
+argument, which gives you access to the virtual environment it creates. You can
+use `.install()` to install inside the environment, and `.run()` to run inside
+the environment. We are also using `session.posargs` to allow extra arguments to
+be passed through to pytest. There are
+[more useful methods](https://nox.thea.codes/en/stable/config.html#module-nox.sessions)
+as well.
 
-## Features
+You can run this using:
 
-### Type narrowing
+```console
+$ nox -s tests
+```
 
-One of the key features of type checking is type narrowing. The type checker
-monitors the types of a variable, and "narrows" it when something restricts it.
-For example:
+You can see all defined sessions (along with the docstrings) using:
 
-```python
-x: Union[A, B]
-if isinstance(x, A):
-    reveal_type(x)
-else:
-    reveal_type(x)
+```console
+$ nox -l
 ```
 
-This will print `A`, then `B`. It prints `A` because that's the only thing that
-can exist in the first branch, and then the remaining types (`B`) must be the
-type in the second branch. And it prints both because it's not actually running
-the code, just type checking it, so both sides of the if are checked.
-
-You can manually force type narrowing with assert:
+It is a good idea to list the sessions you want by default by setting
+`nox.options.sessions` near the top of your file:
 
 ```python
-x: Union[A, B]
-assert isinstance(x, A)
-reveal_type(x)
+nox.options.sessions = ["lint", "tests"]
 ```
 
-This will print `A` because you removed B via the type narrowing using the
-`assert`.
+This will keep you from running extra things like `docs` by default.
 
-### Protocols
+### Parametrizing
 
-One of the best features of MyPy is support for structural subtyping via
-Protocols - formalized duck-typing, basically. This allows cross library
-interoperability, unlike traditional inheritance. Here’s how it works:
+You can parametrize sessions. either on Python or on any other item.
 
 ```python
-from typing import Protocol  # or typing_extensions for < 3.8
+# Shortcut to parametrize Python
+@nox.session(python=["3.8", "3.9", "3.10", "3.11", "3.12"])
+def my_session(session: nox.Session) -> None:
+    ...
 
 
-class Duck(Protocol):
-    def quack() -> str:
-        ...
+# General parametrization
+@nox.session
+@nox.parametrize("letter", ["a", "b"], ids=["a", "b"])
+def my_session(session: nox.Session, letter: str) -> None:
+    ...
 ```
 
-Now any object that can "quack" (and return a string) is a Duck. We can even add
-`@runtime_checkable` which will allow us to check this (minus the types) at
-runtime in `isinstance`. So now we can design code like this:
-
-```python
-def pester_duck(a_duck: Duck) -> None:
-    print(a_duck.quack())
-    print(a_duck.quack())
-```
+The optional `ids=` parameter can give the parametrization nice names, like in
+pytest.
 
-And the type checker will ensure we only write code valid on all `Duck`s. And,
-we can write a duck implementation and test it like this:
+If a user does not have a particular version of Python installed, it will be
+skipped. You can use a Docker container to run in an environment where all
+Python's (3.6+) are available:
 
-```python
-class MyDuck:
-    def quack() -> str:
-        return "quack"
+```console
+$ docker run --rm -itv $PWD:/src -w /src quay.io/pypa/manylinux_2_28_x86_64:latest pipx run nox
 ```
 
-This will pass a check for being a `Duck`, for example something like this:
+Another container you can use is `thekevjames/nox:latest`; this has nox
+pre-installed (no pipx) and Python 2.7 and 3.5 as well.
 
-```python
-import typing
+### Useful sessions
 
-if typing.TYPE_CHECKING:
-    _: Duck = typing.cast(MyDuck, None)
-```
+Things like bumping the versions can be made sessions - since nox handles the
+environment for you, you can use any Python dependencies you like, and not have
+to worry about installing anything. Here are some commonly useful sessions that
+will likely look similar across different projects:
 
-Notice the complete lack of dependencies here. We don’t need `MyDuck` to write
-`pester_duck`, or vice-versa. And, we don't even need `Duck` to write either one
-at runtime! The dependence on `Duck` for `pester_duck` is entirely a
-type-check-time dependence (unless we want to use a `runtime_checkable` powered
-`isinstance`).
+#### Lint
 
-There are lots of built-in Protocols, most of which pre-date typing and are
-available in an Abstract Base Class form. Most of them check for one or more
-special methods, like `Iterable`, `Iterator`, etc.
+Ideally, all developers should be using pre-commit directly, but this helps new
+users.
 
-### Other features
+```python
+@nox.session
+def lint(session: nox.Session) -> None:
+    """
+    Run the linter.
+    """
+    session.install("pre-commit")
+    session.run(
+        "pre-commit", "run", "--show-diff-on-failure", "--all-files", *session.posargs
+    )
+```
 
-Static typing has some great features worth checking out:
+#### Tests
 
-- Unions (New syntax in Python 3.10)
-- Generic Types (New syntax in Python 3.9)
-- Literals
-- TypedDict
-- Nicer NamedTuple definition (very popular in Python 3 code)
-- MyPy validates with the Python version you ask for, regardless of what version
-  you are actually running.
+```python
+import nox
 
-## Complete example
 
-### Runtime compatible types
+@nox.session
+def tests(session: nox.Session) -> None:
+    """
+    Run the unit and regular tests.
+    """
+    session.install(".[test]")
+    session.run("pytest", *session.posargs)
+```
 
-Here's the classic syntax, which you need to use if you want to access the type
-annotations at runtime and you need to support Python < 3.10:
+#### Docs
 
 ```python
-from typing import Union, List
-
-
-# Generic types take bracket arguments
-def f(x: int) -> List[int]:
-    return list(range(x))
-
+@nox.session(reuse_venv=True)
+def docs(session: nox.Session) -> None:
+    """
+    Build the docs. Pass "--serve" to serve.
+    """
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--serve", action="store_true", help="Serve after building")
+    args, posargs = parser.parse_known_args(session.posargs)
+
+    session.install("-e.[docs]")
+    session.chdir("docs")
+
+    session.run(
+        "sphinx-build",
+        "-n",  # nitpicky mode
+        "--keep-going",  # show all errors
+        "-T",  # full tracebacks
+        "-b",
+        "html",
+        ".",
+        f"_build/html",
+        *posargs,
+    )
+
+    if args.serve:
+        session.log("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
+        session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
+```
 
-# Unions are a list of types that all could be allowed
-def g(x: Union[str, int]) -> None:
-    # Type narrowing - Unions get narrowed
-    if isinstance(x, str):
-        print("string", x.lower())
-    else:
-        print("int", x)
+This supports setting up a quick server as well, run like this:
 
-    # Calling x.lower() is invalid here!
+```console
+$ nox -s docs -- --serve
 ```
 
-### Types as strings
+#### Build (pure Python)
 
-If you don't access the types at runtime, or if you use Python 3.10+ only, then
-you can use a much nicer syntax. The `annotations` future feature causes the
-annotations to be stored as strings and not evaluated, which allows you to write
-things that are not yet valid, like `list[int]`!
+For pure Python packages, this could be useful:
 
 ```python
-from __future__ import annotations
-
-
-def f(x: int) -> list[int]:
-    return list(range(x))
-
+from pathlib import Path
+import shutil
 
-def g(x: str | int) -> None:
-    if isinstance(x, str):
-        print("string", x.lower())
-    else:
-        print("int", x)
-```
-
-Notice that there are no imports from typing! Note that you cannot use the "new"
-syntax in non annotation locations (like unions in `isinstance`) unless Python
-supports it at runtime. And some libraries, like Typer and cattrs, use the
-annotations at runtime.
+DIR = Path(__file__).parent.resolve()
 
-You can use the above in earlier Python versions if you use strings manually,
-with the same caveats.
 
-## Final words
+@nox.session
+def build(session: nox.Session) -> None:
+    """
+    Build an SDist and wheel.
+    """
 
-When run alongside a good linter like flake8, this can catch a huge number of
-issues before tests or they are discovered in the wild! It also prompts _better
-design_, because you are thinking about how types work and interact. It's also
-more readable, since if I give you code like this:
+    build_path = DIR.joinpath("build")
+    if build_path.exists():
+        shutil.rmtree(build_path)
 
-```python
-def compute(timestamp):
-    ...
+    session.install("build")
+    session.run("python", "-m", "build")
 ```
 
-You don't know "what" timestamp is. Is it an int? A float? An object? With
-types, you'll know what I was intending to give you. You can use type aliases to
-really give expressive names here!
+### Examples
+
+A standard
+[powered by nox](https://github.com/scikit-hep/hist/blob/main/noxfile.py)
+package in Pure Python can be found in the Hist project of Scikit-HEP.
+
+A package that happens to use PDM (like Poetry but better) is Scikit-HEP UHI,
+which is
+[powered by nox](https://github.com/scikit-hep/uhi/blob/main/noxfile.py). Nox
+can setup a conda environment with ROOT (slow, but only nox and conda are
+required). There also is a version bump session, and does some custom logic too.
+
+The complex testing procedure powering Scientific Python Cookie is
+[powered by nox](https://github.com/scientific-python/cookie/blob/main/noxfile.py).
+It allows the complex CI jobs that generate projects and lint/test/build them to
+be run locally with no other setup.
+
+PyPA's cibuildwheel also is
+[powered by nox](https://github.com/pypa/cibuildwheel/blob/main/noxfile.py),
+running pip-tools' compile on every Python version to pin dependencies, as well
+as providing a standard interface to update Python and project listing update
+scripts. The docs job there runs mkdocs instead of Sphinx. Other PyPA projects
+using nox include [pip](https://github.com/pypa/pip/blob/main/noxfile.py),
+[pipx](https://github.com/pypa/pipx/blob/main/noxfile.py),
+[manylinux](https://github.com/pypa/manylinux/blob/main/noxfile.py),
+[packaging](https://github.com/pypa/packaging/blob/main/noxfile.py), and
+[packaging.python.org](https://github.com/pypa/packaging.python.org/blob/main/noxfile.py).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/guides/packaging_classic.md` & `sp_repo_review-2023.7.6/docs/pages/guides/packaging_classic.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 ---
 layout: page
-title: Classic Packaging
-permalink: /guides/packaging_classic/
-nav_order: 6
+title: Classic packaging
+permalink: /guides/packaging-classic/
+nav_order: 7
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
+# Classic packaging
+
 The libraries in the scientific Python ecosytem have a variety of different
 packaging styles, but this document is intended to outline a recommended style
 that new packages should follow, and existing packages should slowly adopt. The
 reasoning for each decision is outlined as well.
 
 There are currently several popular packaging systems. This guide covers
 [Setuptools][], which is currently the only system that supports compiled
 extensions. If you are not planning on writing C/C++ code, other systems like
 [Hatch][] are drastically simpler - most of this page is unneeded for those
 systems.
 
 Also see the [Python packaging guide][], especially the [Python packaging
 tutorial][].
 
-> <h2 class="no_toc">Note:</h2>
->
+{: .note }
+
 > Raw source lives in git and has a `setup.py`. You _can_ install directly from
 > git via pip, but normally users install from distributions hosted on PyPI.
 > There are three options: **A)** A source package, called an SDist and has a
 > name that ends in `.tar.gz`. This is a copy of the GitHub repository, stripped
 > of a few specifics like CI files, and possibly with submodules included (if
 > there are any). **B)** A pure python wheel, which ends in `.whl`; this is only
 > possible if there are no compiled extensions in the library. This does _not_
 > contain a setup.py, but rather a `PKG_INFO` file that is rendered from
 > setup.py (or from another build system). **C)** If not pure Python, a
 > collection of wheels for every binary platform, generally one per supported
 > Python version and OS as well.
 >
 > Developer requirements (users of A or git) are generally higher than the
-> requirements to use B or C. Poetry creates SDists that include a setup.py, and
-> both alternate packing systems produce "normal" wheels.
+> requirements to use B or C. Poetry and optionally flit create SDists that
+> include a `setup.py`, and all alternate packing systems produce "normal"
+> wheels.
 
 ## Package structure (medium priority)
 
 All packages _should_ have a `src` folder, with the package code residing inside
 it, such as `src/<package>/`. This may seem like extra hassle; after all, you
 can type "`python`" in the main directory and avoid installing it if you don't
 have a `src` folder! However, this is a bad practice, and it causes several
@@ -83,16 +86,16 @@
 binary packages to be created and a few common developer needs, like editable
 installs, look slightly different (a way to include editable installs in PEP 517
 is being worked on). Usage of these "[hypermodern][]" packaging tools are
 generally not found in scientific Python packages, but not discouraged; all
 tools build the same wheels (and they often build setuptools compliant SDists,
 as well).
 
-{% include rr.html id="PP003" %} Note that `"wheel"` is never required; it is
-injected automatically by setuptools only when needed.
+{% rr PP003 %} Note that `"wheel"` is never required; it is injected
+automatically by setuptools only when needed.
 
 ### Special additions: NumPy
 
 You may want to build against NumPy (mostly for Cython packages, pybind11 does
 not need to access the NumPy headers). This is the recommendation for scientific
 Python packages:
 
@@ -191,15 +194,17 @@
 ```
 
 {% endraw %}
 
 If you fill in the override version setting when triggering a manual workflow
 run, that version will be forced, otherwise, it works as normal.
 
-> Note: Make sure you have a good gitignore, probably starting from
+{: .note }
+
+> Make sure you have a good gitignore, probably starting from
 > [GitHub's Python one](https://github.com/github/gitignore/blob/main/Python.gitignore)
 > or using a [generator site](https://www.toptal.com/developers/gitignore).
 
 You should also add these two files:
 
 `.git_archival.txt`:
 
@@ -213,16 +218,16 @@
 And `.gitattributes` (or add this line if you are already using this file):
 
 ```text
 .git_archival.txt  export-subst
 ```
 
 This will allow git archives (including the ones generated from GitHub) to also
-support versioning. This will only work with `setuptools_scm>=7`, which requires
-Python 3.7+ (though adding the files won't hurt older versions).
+support versioning. This will only work with `setuptools_scm>=7` (though adding
+the files won't hurt older versions).
 
 ### Classic in-source versioning
 
 Recent versions of `setuptools` have improved in-source versioning. If you have
 a simple file that includes a line with a simple PEP 440 style version, like
 `version = "2.3.4.beta1"`, then you can use a line like this in your
 `setup.cfg`:
@@ -258,29 +263,28 @@
 long_description_content_type = text/markdown
 url = https://github.com/organization/package
 author = My Name
 author_email = me@email.com
 maintainer = My Organization
 maintainer_email = organization@email.com
 license = BSD-3-Clause
-license_file = LICENSE
+license_files = LICENSE
 classifiers =
     Development Status :: 4 - Beta
     Intended Audience :: Developers
     Intended Audience :: Information Technology
     Intended Audience :: Science/Research
     License :: OSI Approved :: BSD License
     Operating System :: MacOS
     Operating System :: Microsoft :: Windows
     Operating System :: POSIX
     Operating System :: Unix
     Programming Language :: C++
     Programming Language :: Python
     Programming Language :: Python :: 3 :: Only
-    Programming Language :: Python :: 3.7
     Programming Language :: Python :: 3.8
     Programming Language :: Python :: 3.9
     Programming Language :: Python :: 3.10
     Programming Language :: Python :: 3.11
     Programming Language :: Python :: 3.12
     Topic :: Scientific/Engineering
     Topic :: Scientific/Engineering :: Information Analysis
@@ -295,15 +299,15 @@
     Changelog = https://package.readthedocs.io/en/latest/changelog.html
 
 
 [options]
 packages = find:
 install_requires =
     numpy>=1.13.3
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir =
     =src
 zip_safe = False
 
 [options.packages.find]
 where = src
@@ -414,28 +418,40 @@
 PyPI SDist could fail. Also, development mode (`-e`) is not covered by this
 procedure, so you should have at least one CI run that does not include the `-e`
 (pip 21.3+ required for non-setuptools editable installs).
 
 The files that go into the SDist are controlled by [MANIFEST.in][], which
 generally should be specified. If you use `setuptools_scm`, the [default should
 be all of git][setuptools_scm file]; if you do not, the default is a few common
-files, like any `.py` files and standard tooling. Here is a useful default for
-complete control over a src structure, though be sure to update it to include
-any files that need to be included:
+files, like any `.py` files and standard tooling. Here is a useful default,
+though be sure to update it to include any files that need to be included:
 
 ```
-prune **
 graft src
 graft tests
 
 include LICENSE README.md pyproject.toml setup.py setup.cfg
-global-exclude __pycache__ *.py[cod] .*
+global-exclude __pycache__ *.py[cod] .venv
+```
+
+## Command line
+
+If you want to ship an "app" that a user can run from the command line, you need
+to add a `console_scripts` entry point. The form is:
+
+```ini
+[options.entry_points]
+console_scripts =
+    cliapp = packakge.__main__:main
 ```
 
-Note that Scikit-build currently may have issues with MANIFEST.in.
+The format is command line app name as the key, and the value is the path to the
+function, followed by a colon, then the function to call. If you use
+`__main__.py` as the file, then `python -m` + the module will also work to call
+the app.
 
 [^1]:
     You shouldn't ever have to run commands like this, they are implementation
     details of setuptools. For this command, you should use `python -m build -s`
     instead (and `pip install build`).
 
 [^2]:
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/guides/pytest.md` & `sp_repo_review-2023.7.6/docs/pages/guides/pytest.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 permalink: /guides/pytest/
 nav_order: 2
 parent: Topical Guides
 ---
 
 {% include toc.html %}
 
+# Testing with pytest
+
 Tests are crucial to writing reliable software. A good test suite allows you to:
 
 - Immediately know if a new platform or software version works,
 - Refactor and cleanup your code with confidence,
 - Evaluate the effect of additions and changes.
 
 Python used to have three major choices for tests; but now [pytest][] is used
@@ -23,15 +25,17 @@
 - Coverage: using as many inputs as possible increases the chances of finding
   something that breaks.
 - Performance: the faster the tests, the more situations you can run your tests
   in CI.
 - Reporting: when things break, you should get good information about what
   broke.
 
-> ### What about other choices?
+{: .note-title }
+
+> What about other choices?
 >
 > The alternative library, `nose`, has been abandoned in favor of `pytest`,
 > which can run nose-style tests. The standard library has a test suite as well,
 > but it's extremely verbose and complex; and since "developers" run tests, your
 > test requirements don't affect users. And `pytest` can run stdlib style
 > testing too. So just use `pytest`. All major packages use it too, including
 > `NumPy`. Most other choices, like [Hypothesis][], are related to `pytest` and
@@ -58,50 +62,47 @@
 - The Python `assert` statement is rewritten by pytest to capture exactly what
   happens. If it fails, you will get a clear, detailed report on what each value
   was.
 
 ### Configuring pytest
 
 pytest supports configuration in `pytest.ini`, `setup.cfg`, or, since version 6,
-`pyproject.toml` {% include rr.html id="PP301" %}. Remember, pytest is a
-developer requirement, not a user one, so always require 6+ (or 7+) and use
-`pyproject.toml`. This is an example configuration:
+`pyproject.toml` {% rr PP301 %}. Remember, pytest is a developer requirement,
+not a user one, so always require 6+ (or 7+) and use `pyproject.toml`. This is
+an example configuration:
 
 ```toml
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = ["error"]
 log_cli_level = "info"
 testpaths = [
   "tests",
-  "ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest",
 ]
 ```
 
-{% include rr.html id="PP302" %} The `minversion` will print a nicer error if
-your `pytest` is too old (though, ironically, it won't read this is the version
-is too old, so setting "6" or less in `pyproject.toml` is rather pointless). The
-`addopts` setting will add whatever you put there to the command line when you
-run; {% include rr.html id="PP308" %} `-ra` will print a summary "r"eport of
-"a"ll results, which gives you a quick way to review what tests failed and were
-skipped, and why. `--showlocals` will print locals in tracebacks.
-{% include rr.html id="PP307" %} `--strict-markers` will make sure you don't try
-to use an unspecified fixture. {% include rr.html id="PP306" %} And
-`--strict-config` will error if you make a mistake in your config.
-{% include rr.html id="PP305" %} `xfail_strict` will change the default for
-`xfail` to fail the tests if it doesn't fail - you can still override locally in
-a specific xfail for a flaky failure. {% include rr.html id="PP309" %}
-`filter_warnings` will cause all warnings to be errors (you can add allowed
-warnings here too, see below). {% include rr.html id="PP304" %} `log_cli_level`
-will report `INFO` and above log messages on a failure.
-{% include rr.html id="PP303" %} Finally, `testpaths` will limit `pytest` to
-just looking in the folders given - useful if it tries to pick up things that
-are not tests from other directories.
+{% rr PP302 %} The `minversion` will print a nicer error if your `pytest` is too
+old (though, ironically, it won't read this is the version is too old, so
+setting "6" or less in `pyproject.toml` is rather pointless). The `addopts`
+setting will add whatever you put there to the command line when you run;
+{% rr PP308 %} `-ra` will print a summary "r"eport of "a"ll results, which gives
+you a quick way to review what tests failed and were skipped, and why.
+`--showlocals` will print locals in tracebacks. {% rr PP307 %}
+`--strict-markers` will make sure you don't try to use an unspecified fixture.
+{% rr PP306 %} And `--strict-config` will error if you make a mistake in your
+config. {% rr PP305 %} `xfail_strict` will change the default for `xfail` to
+fail the tests if it doesn't fail - you can still override locally in a specific
+xfail for a flaky failure. {% rr PP309 %} `filter_warnings` will cause all
+warnings to be errors (you can add allowed warnings here too, see below).
+{% rr PP304 %} `log_cli_level` will report `INFO` and above log messages on a
+failure. {% rr PP303 %} Finally, `testpaths` will limit `pytest` to just looking
+in the folders given - useful if it tries to pick up things that are not tests
+from other directories.
 [See the docs](https://docs.pytest.org/en/stable/customize.html) for more
 options.
 
 pytest also checks the current and parent directories for a `conftest.py` file.
 If it finds them, they will get run outer-most to inner-most. These files let
 you add fixtures and other pytest configurations (like hooks for test discovery,
 etc) for each directory. For example, you could have a "mock" folder, and in
@@ -131,19 +132,18 @@
 `filename.py::test_name`.
 
 If a test fails, you have lots of options to save time in debugging. Adding
 `-l`/`--showlocals` will print out the local values in the tracebacks (and can
 be added by default, see above). You can run `pytest` with `--pdb`, which will
 drop you into a debugger on each failure. Or you can use `--trace` which will
 drop you into a debugger at the start of each test selected (so probably use the
-selection methods above). `pytest` also supports `breakpoint()` in Python 3.7+.
-You can also start out in your debugger at the beginning of the last failed test
-with `--trace --lf`.
-[See the docs](https://docs.pytest.org/en/stable/usage.html) for more running
-tips.
+selection methods above). `pytest` also supports `breakpoint()`. You can also
+start out in your debugger at the beginning of the last failed test with
+`--trace --lf`. [See the docs](https://docs.pytest.org/en/stable/usage.html) for
+more running tips.
 
 ## Guidelines for writing good tests
 
 Time spent learning all the powerful tools pytest has to offer will be well
 spent! You can make your tests more granular, mock things that aren't available
 (or are slow to run), parametrize, and much more.
 
@@ -277,21 +277,21 @@
 like tests marked "slow", for example. Just add `-m <marker>` when running
 pytest to run a group of marked tests. This is an expression; you can use
 `not <marker>` as well.
 
 Probably the most useful built-in mark is `skipif`:
 
 ```python
-@pytest.mark.skipif("sys.version_info >= (3, 7)")
-def test_only_on_37plus():
+@pytest.mark.skipif("sys.version_info >= (3, 8)")
+def test_only_on_38plus():
     x = 3
     assert f"{x = }" == "x = 3"
 ```
 
-Now this test will only run on Python 3.7 or newer, and will be skipped on
+Now this test will only run on Python 3.8 or newer, and will be skipped on
 earlier versions. You don't have to use a string for the condition, but if you
 don't, add a `reason=` so there will still be a nice printout explaining why the
 test was skipped.
 
 You can also use `xfail` for tests that are expected to fail (you can even
 strictly test them as failing if you want). You can use `parametrize` to make a
 single parameterized test instead of sharing them (with fixtures). There's a
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/guides/repo_review.md` & `sp_repo_review-2023.7.6/docs/pages/guides/repo_review.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 ---
 layout: page
-title: Repo Review
+title: Repo-Review
 permalink: /guides/repo-review/
 nav_order: 110
 parent: Topical Guides
 interactive_repo_review: true
 ---
 
+# Repo-Review
+
 You can check the style of a GitHub repository below. Enter any repository, such
 as `scikit-hep/hist`, and the branch you want to check, such as `main` (it must
 exist). This will produce a list of results - green checkmarks mean this rule is
 followed, red errors mean the rule is not. A yellow warning sign means that the
 check was skipped because a previous required check failed. Some checks will
 fail, that's okay - the goal is bring all possible issues to your attention, not
 to force compliance with arbitrary checks.
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/guides/style.md` & `sp_repo_review-2023.7.6/docs/pages/guides/style.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 nav_order: 8
 parent: Topical Guides
 custom_title: Style guide
 ---
 
 {% include toc.html %}
 
+# Style (static checkers)
+
 ## Pre-commit
 
-{% include rr.html id="PY006" %} Scientific Python projects often use
-[pre-commit][] to check code style. It can be installed through `brew` (macOS)
-or `pip` (anywhere). There are two modes to use it locally; you can check
-manually with `pre-commit run` (changes only) or `pre-commit run --all-files`
-(all). You can also run `pre-commit install` to add checks as a git pre-commit
-hook (which is where it gets its name). It's worth trying, even if you've tried
-and failed to set up a custom pre-commit hook before; it's quite elegant and
-does not add or commit the changes, it just makes the changes and allows you to
-check and add them. You can always override the hook with `-n`.
+{% rr PY006 %} Scientific Python projects often use [pre-commit][] to check code
+style. It can be installed through `brew` (macOS) or `pip` (anywhere). There are
+two modes to use it locally; you can check manually with `pre-commit run`
+(changes only) or `pre-commit run --all-files` (all). You can also run
+`pre-commit install` to add checks as a git pre-commit hook (which is where it
+gets its name). It's worth trying, even if you've tried and failed to set up a
+custom pre-commit hook before; it's quite elegant and does not add or commit the
+changes, it just makes the changes and allows you to check and add them. You can
+always override the hook with `-n`.
 
 [pre-commit]: https://pre-commit.com
 
-{% include rr.html id="PC100" %} Here is a minimal `.pre-commit-config.yaml`
-file with some handy options:
+{% rr PC100 %} Here is a minimal `.pre-commit-config.yaml` file with some handy
+options:
 
 ```yaml
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.4.0"
     hooks:
       - id: check-added-large-files
@@ -66,35 +68,35 @@
 Now there will be a new check, and pre-commit.ci will commit changes if the
 pre-commit check made any changes. Note that there are a couple of missing
 features: Docker based checks will not work (pre-commit.ci already runs in
 docker), you cannot enable a `--manual` flag, so extra checks will not run, and
 jobs should not download packages (use `additional-dependencies:` to add what
 you need).
 
-{% include rr.html id="PC901" %} You can customize the pre-commit message with:
+{% rr PC901 %} You can customize the pre-commit message with:
 
 ```yaml
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
 ```
 
 ## Black
 
-{% include rr.html id="PC110" %}
-[Black](https://black.readthedocs.io/en/latest/) is a popular auto-formatter
-from the Python Software Foundation. One of the main features of Black is that
-it is "opinionated"; that is, it is almost completely unconfigurable. Instead of
-allowing you to come up with your own format, it enforces one on you. While I am
-quite sure you can come up with a better format, having a single standard makes
-it possible to learn to read code very fast - you can immediately see nested
-lists, matching brackets, etc. There also is a faction of developers that
-dislikes all auto-formatting tools, but inside a system like pre-commit,
-auto-formatters are ideal. They also speed up the writing of code because you
-can ignore formatting your code when you write it. By imposing a standard, all
-scientific Python developers can quickly read any package's code.
+{% rr PC110 %} [Black](https://black.readthedocs.io/en/latest/) is a popular
+auto-formatter from the Python Software Foundation. One of the main features of
+Black is that it is "opinionated"; that is, it is almost completely
+unconfigurable. Instead of allowing you to come up with your own format, it
+enforces one on you. While I am quite sure you can come up with a better format,
+having a single standard makes it possible to learn to read code very fast - you
+can immediately see nested lists, matching brackets, etc. There also is a
+faction of developers that dislikes all auto-formatting tools, but inside a
+system like pre-commit, auto-formatters are ideal. They also speed up the
+writing of code because you can ignore formatting your code when you write it.
+By imposing a standard, all scientific Python developers can quickly read any
+package's code.
 
 Also, properly formatted code has other benefits, such as if two developers make
 the same change, they get the same formatting, and merge requests are easier.
 The style choices in Black were explicitly made to optimize git diffs!
 
 There are a _few_ options, mostly to enable/disable certain files, remove string
 normalization, and to change the line length, and those go in your
@@ -105,76 +107,75 @@
 ```yaml
 - repo: https://github.com/psf/black
   rev: "23.3.0"
   hooks:
     - id: black
 ```
 
-<details markdown="1"><summary>You can add a Black badge to your repo as well</summary>
+{% details You can add a Black badge to your repo as well %}
 
 ```md
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ```
 
 ```rst
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 ```
 
-</details>
+{% enddetails %}
 
 In _very_ specific situations, you may want to retain special formatting. After
 carefully deciding that it is a special use case, you can use `# fmt: on` and
 `# fmt: off` around a code block to have it keep custom formatting. _Always_
 consider refactoring before you try this option! Most of the time, you can find
 a way to make the Blacked code look better by rewriting your code; factor out
 long unreadable portions into a variable, avoid writing matrices as 1D lists,
 etc.
 
-<details markdown="1"><summary>Documentation / README snippets support</summary>
+{% details Documentation / README snippets support %}
 
-{% include rr.html id="PC111" %} If you want Black used in your documentation,
-you can use blacken-docs. This can even catch syntax errors in code snippets! It
-supports markdown and restructured text. Note that because black is in
+{% rr PC111 %} If you want Black used in your documentation, you can use
+blacken-docs. This can even catch syntax errors in code snippets! It supports
+markdown and restructured text. Note that because black is in
 `additional_dependencies`, you'll have to keep it up to date manually.
 
 ```yaml
 - repo: https://github.com/asottile/blacken-docs
-  rev: "1.13.0"
+  rev: "1.14.0"
   hooks:
     - id: blacken-docs
-      additional_dependencies: [black==23.1.0]
+      additional_dependencies: [black==23.3.0]
 ```
 
-</details>
+{% enddetails %}
 
 ## Ruff
 
-{% include rr.html id="PC190" %} [Ruff][] [(docs)][ruff docs] is a Python code
-linter and autofixer that replaces many other tools in the ecosystem with a
-ultra-fast (written in Rust), single zero-dependency package. All plugins are
-compiled in, so you can't get new failures from plugins updating without
-updating your pre-commit hook.
+{% rr PC190 %} [Ruff][] [(docs)][ruff docs] is a Python code linter and
+autofixer that replaces many other tools in the ecosystem with a ultra-fast
+(written in Rust), single zero-dependency package. All plugins are compiled in,
+so you can't get new failures from plugins updating without updating your
+pre-commit hook.
 
 [ruff docs]: https://beta.ruff.rs
-[ruff]: https://github.com/charliermarsh/ruff
+[ruff]: https://github.com/astral-sh/ruff
 
 ```yaml
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: "v0.0.271"
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: "v0.0.276"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
 ```
 
-{% include rr.html id="PC191" %} The `--fix` argument is optional, but
-recommended, since you can inspect and undo changes in git.
+{% rr PC191 %} The `--fix` argument is optional, but recommended, since you can
+inspect and undo changes in git.
 
-{% include rr.html id="RF001" %} Ruff is configured in your `pyproject.toml`.
-Here's an example:
+{% rr RF001 %} Ruff is configured in your `pyproject.toml`. Here's an example:
 
 ```toml
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
   "B",           # flake8-bugbear
   "I",           # isort
@@ -200,15 +201,14 @@
   "PD",          # pandas-vet
 ]
 extend-ignore = [
   "PLR",    # Design related pylint codes
   "E501",   # Line too long
   "PT004",  # Use underscore for non-returning fixture (use usefixture instead)
 ]
-target-version = "py37"
 typing-modules = ["mypackage._compat.typing"]
 src = ["src"]
 unfixable = [
   "T20",  # Removes print statements
   "F841", # Removes unused variables
 ]
 exclude = []
@@ -224,37 +224,46 @@
 sequences (with the special exception of pylint's "PL" shortcut), then you can
 also include leading or whole error codes. Codes starting with 9 must be
 selected explicitly, with at least the letters followed by a 9. You can also
 ignore certain error codes via `extend-ignore`. You can also set codes per paths
 to ignore in `per-file-ignores`. If you don't like certain auto-fixes, you can
 disable auto-fixing for specific error codes via `unfixable`.
 
-There are other configuration options, such as `target-version`, which selects
-the minimum version you want to target (primarily for `"UP"` and `"I"`)
-{% include rr.html id="RF002" %}, the `src` list which tells it where to look
-for top level packages (mostly for "I" codes, which also have a lot of custom
-configuration options) {% include rr.html id="RF003" %}, `typing-modules`, which
+There are other configuration options, such as the `src` list which tells it
+where to look for top level packages (mostly for "I" codes, which also have a
+lot of custom configuration options) {% rr RF003 %}, `typing-modules`, which
 helps apply typing-specific rules to a re-exported typing module (a common
 practice for unifying typing and `typing_extensions` based on Python version).
 There's also a file `exclude` set, which you can override if you are running
 this entirely from pre-commit (default excludes include "build", so if you have
 a `build` module or file named `build.py`, it would get skipped by default
 without this).
 
+{: .warning }
+
+> If you don't use a `[project]` table (older setuptools or Poetry), then you
+> should also set:
+>
+> ```toml
+> target-version = "py38"
+> ```
+>
+> This selects the minimum version you want to target (primarily for `"UP"` and
+> `"I"`) {% rr RF002 %},
+
 Here are some good error codes to enable on most (but not all!) projects:
 
 - `E`, `F`, `W`: These are the standard flake8 checks, classic checks that have
   stood the test of time.
-- `B`: This finds patterns that are very bug-prone.
-  {% include rr.html id="RF101" %}
+- `B`: This finds patterns that are very bug-prone. {% rr RF101 %}
 - `I`: This sorts your includes. There are multiple benefits, such as smaller
   diffs, fewer conflicts, a way to auto-inject `__future__` imports, and easier
   for readers to tell what's built-in, third-party, and local. It has a lot of
   configuration options, but defaults to a Black-compatible style.
-  {% include rr.html id="RF102" %}
+  {% rr RF102 %}
 - `ARG`: This looks for unused arguments. You might need to `# noqa: ARG001`
   occasionally, but it's overall pretty useful.
 - `C4`: This looks for places that could use comprehensions, and can autofix
   them.
 - `EM`: Very opinionated trick for error messages: it stops you from putting the
   error string directly in the exception you are throwing, producing a cleaner
   traceback without duplicating the error string.
@@ -268,21 +277,20 @@
   many are helpful.
 - `PTH`: Want to move to using modern pathlib? This will help. There are some
   cases where performance matters, but otherwise, pathlib is easier to read and
   use.
 - `RUF`: Codes specific to Ruff, including removing noqa's that aren't used.
 - `T20`: Disallow `print` in your code (built on the assumption that it's a
   common debugging tool).
-- `UP`: Upgrade old Python syntax to your `target-version`.
-  {% include rr.html id="RF103" %}
+- `UP`: Upgrade old Python syntax to your `target-version`. {% rr RF103 %}
 
 A few others small ones are included above, and there are even more available in
 Ruff.
 
-<details markdown="1"><summary>Separate tools that Ruff replaces</summary>
+{% details Separate tools that Ruff replaces %}
 
 ### PyCln
 
 [PyCln][] will clean up your imports if you have any that are not needed. There
 is a Flake8 check for this, but it's usually nicer to automatically do the
 cleanup instead of forcing a user to manually delete unneeded imports. If you
 use the manual stage, it's opt-in instead of automatic.
@@ -351,40 +359,40 @@
 - [`flake8-import-order`](https://pypi.org/project/flake8-import-order/):
   Enforces PEP8 grouped imports (you may prefer isort). Code: `I`
 - [`pep8-naming`](https://pypi.org/project/pep8-naming/): Enforces PEP8 naming
   rules. Code: `N`
 - [`flake8-print`](https://pypi.org/project/pep8-naming/): Makes sure you don't
   have print statements that sneak in. Code: `T`
 
-<details markdown="1"><summary>Flake8-print details:</summary>
+{% details Flake8-print details %}
 
 Having something verify you don't add a print statement by mistake is _very_
 useful. A common need for the print checker would be to add it to a single
 directory (`src` if you are following the convention recommended). You can do
 the next best thing by removing directories and file just for this check (`T`)
 in your flake8 config:
 
 ```ini
 [flake8]
 per-file-ignores =
     tests/*: T
     examples/*: T
 ```
 
-</details>
+{% enddetails %}
 
 ### YesQA
 
 Over time, you can end up with extra "noqa" comments that are no longer needed.
 This is a flake8 helper that removes those comments when they are no longer
 required.
 
 ```yaml
 - repo: https://github.com/asottile/yesqa
-  rev: "v1.4.0"
+  rev: "v1.5.0"
   hooks:
     - id: yesqa
 ```
 
 You need to have the same extra dependencies as flake8. In YAML, you can save
 the list given to yesqa and repeat it in flake8 using `&flake8-dependencies` and
 `*flake8-dependencies` after the colon.
@@ -423,82 +431,81 @@
 style syntax. Most useful to keep Python 2 outdated constructs out, it can even
 do some code updates for different versions of Python 3, like adding f-strings
 when clearly better (please always use them, they are faster) if you set
 `--py36-plus` (for example). This is a recommended addition for any project.
 
 ```yaml
 - repo: https://github.com/asottile/pyupgrade
-  rev: "v3.4.0"
+  rev: "v3.8.0"
   hooks:
     - id: pyupgrade
-      args: ["--py37-plus"]
+      args: ["--py38-plus"]
 ```
 
 [pyupgrade]: https://github.com/asottile/pyupgrade:
 
-> <h4 class="no_toc">Note:</h4>
->
-> If you set this to `--py37-plus`, you can add the annotations import by adding
-> the following line to your isort pre-commit hook configuration:
+{: .note }
+
+> If you set this to at least `--py37-plus`, you can add the annotations import
+> by adding the following line to your isort pre-commit hook configuration:
 >
 > ```yaml
 > args: ["-a", "from __future__ import annotations"]
 > ```
 >
 > Also make sure isort comes before pyupgrade. Now when you run pre-commit, it
 > will clean up your annotations to 3.7+ style, too!
 
-</details>
+{% enddetails %}
 
 ## Type checking
 
-{% include rr.html id="PC140" %} One of the most exciting advancements in Python
-in the last 10 years has been static type hints. Scientific Python projects vary
-in the degree to which they are type-hint ready. One of the challenges for
-providing static type hints is that it was developed in the Python 3 era and it
-really shines in a Python 3.7+ codebase (due to
-`from __future__ import annotations`, which turns annotations into strings and
-allows you to use future Python features in Python 3.7+ annotations as long as
-your type checker supports them). For now, it is recommended that you make an
-attempt to support type checking through your public API in the best way that
-you can (based on your supported Python versions). Stub files can be used
-instead for out-of-line typing. [MyPy](https://mypy.readthedocs.io/en/stable/)
-is suggested for type checking, though there are several other good options to
-try, as well. If you have built-in support for type checking, you need to add
-empty `py.typed` files to all packages/subpackages to indicate that you support
-it.
+{% rr PC140 %} One of the most exciting advancements in Python in the last 10
+years has been static type hints. Scientific Python projects vary in the degree
+to which they are type-hint ready. One of the challenges for providing static
+type hints is that it was developed in the Python 3 era and it really shines in
+a Python 3.7+ codebase (due to `from __future__ import annotations`, which turns
+annotations into strings and allows you to use future Python features in Python
+3.7+ annotations as long as your type checker supports them). For now, it is
+recommended that you make an attempt to support type checking through your
+public API in the best way that you can (based on your supported Python
+versions). Stub files can be used instead for out-of-line typing.
+[MyPy](https://mypy.readthedocs.io/en/stable/) is suggested for type checking,
+though there are several other good options to try, as well. If you have
+built-in support for type checking, you need to add empty `py.typed` files to
+all packages/subpackages to indicate that you support it.
 
 Read more about type checking on the [dedicated page][mypy page].
 
 The MyPy addition for pre-commit:
 
 ```yaml
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: "v1.3.0"
+  rev: "v1.4.1"
   hooks:
     - id: mypy
       files: src
       args: []
 ```
 
 You should always specify args, as the hook's default hides issues - it's
 designed to avoid configuration, but you should add configuration. You can also
 add items to the virtual environment setup for MyPy by pre-commit, for example:
 
 ```yaml
-additional_dependencies: [attrs==21.2.0]
+additional_dependencies: [attrs==23.1.0]
 ```
 
-{% include rr.html id="MY100" %} MyPy has a config section in `pyproject.toml`
-that looks like this:
+{% rr MY100 %} MyPy has a config section in `pyproject.toml` that looks like
+this:
 
 ```ini
 [tool.mypy]
 files = "src"
-python_version = "3.7"
+python_version = "3.8"
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 
 
 # You can disable imports or control per-module/file settings here
@@ -512,33 +519,31 @@
 as you go (possibly by slowly uncommenting items in the list above). You can
 ignore missing imports on libraries as shown above, one section each. And you
 can disable MyPy on a line with `# type: ignore`. One strategy would be to
 enable `check_untyped_defs` first, followed by `disallow_untyped_defs` then
 `disallow_incomplete_defs`. You can add these _per file_ by adding a
 `# mypy: <option>` at the top of a file. You can also pass `--strict` on the
 command line. `strict = true` is now allowed in config files, too
-{% include rr.html id="MY101" %}.
+{% rr MY101 %}.
 
-The extra strict options shown above, like `warn_unreachable`
-{% include rr.html id="MY103" %}, and `ignore-without-code`
-{% include rr.html id="MY104" %}, `redundant-expr`
-{% include rr.html id="MY105" %}, and `truthy-bool`
-{% include rr.html id="MY106" %} can trigger too often (like on `sys.platform`
+The extra strict options shown above, like `warn_unreachable` {% rr MY103 %},
+and `ignore-without-code` {% rr MY104 %}, `redundant-expr` {% rr MY105 %}, and
+`truthy-bool` {% rr MY106 %} can trigger too often (like on `sys.platform`
 checks) and have to be ignored occasionally, but can find some signifiant logic
 errors in your typing.
 
-{% include rr.html id="MY102" %} You should enable `show_error_codes`.
+{% rr MY102 %} You should enable `show_error_codes`.
 
 [mypy page]: {% link pages/guides/mypy.md %}
 
 ## Setuptools specific checks
 
 If you use setuptools, these checks are useful:
 
-<details markdown="1"><summary>Setuptools-only checks</summary>
+{% details Setuptools-only checks %}
 
 ### Check-Manifest (setuptools only)
 
 [Check-manifest](https://pypi.org/project/check-manifest/) is a fantastic,
 highly recommended tool that verifies you have working SDists. You can install
 it from PyPI. Run it on your repository and see what it says. If you want to
 ignore files (like test folders, example folders, docs, etc) you can add these
@@ -562,57 +567,57 @@
 
 If you use `setuptools_scm`, you might want to add:
 
 ```yaml
 additional_dependencies: ["setuptools_scm[toml]"]
 ```
 
-<details markdown="1"><summary>If this is too slow:</summary>
+{% details If this is too slow: %}
 
 **Warning**: For a complex package, this may be slow. You can optionally set
 `stages: [manual]` just below the id, and then only run this explicitly
 (probably in CI only). In GHA, you should enable the manual stage, which will
 run all checks:
 
 ```yaml
 - uses: pre-commit/action@v3.0.0
   with:
     extra_args: --show-diff-on-failure --all-files --hook-stage manual
 ```
 
-</details>
+{% enddetails %}
 
 ### Setup.cfg format (setuptools only)
 
 There is a tool that keeps your `setup.cfg` organized, and makes sure that
 important parts (like Python classifiers) are in sync. This tool,
 `setup-cfg-fmt`, has native support for pre-commit:
 
 ```yaml
 - repo: https://github.com/asottile/setup-cfg-fmt
-  rev: "v2.3.0"
+  rev: "v2.4.0"
   hooks:
     - id: setup-cfg-fmt
       args: [--include-version-classifiers, --max-py-version=3.12]
 ```
 
 Make sure you list the highest version of Python you are testing with here.
 
-</details>
+{% enddetails %}
 
 ## Spelling
 
-{% include rr.html id="PC160" %} You can and should check for spelling errors in
-your code too. If you want to add this, you can use [codespell][] for common
-spelling mistakes. Unlike most spell checkers, this has a list of mistakes it
-looks for, rather than a list of "valid" words. To use:
+{% rr PC160 %} You can and should check for spelling errors in your code too. If
+you want to add this, you can use [codespell][] for common spelling mistakes.
+Unlike most spell checkers, this has a list of mistakes it looks for, rather
+than a list of "valid" words. To use:
 
 ```yaml
 - repo: https://github.com/codespell-project/codespell
-  rev: "v2.2.4"
+  rev: "v2.2.5"
   hooks:
     - id: codespell
       args: ["-L", "sur,nd"]
 ```
 
 You can list allowed spellings in a comma separated string passed to `-L` (or
 `--ignore-words-list` - usually it is better to use long options when you are
@@ -639,15 +644,15 @@
 
 You can also add the `-w` flag to have it automatically correct errors - this is
 probably not something you want regularly, but is very helpful to quickly make
 corrections if you have a lot of them when first adding the check.
 
 ## PyGrep hooks
 
-{% include rr.html id="PC170" %} This is a repository with a
+{% rr PC170 %} This is a repository with a
 [collection of pre-commit extra hooks](https://github.com/pre-commit/pygrep-hooks)
 that protect against some common, easy to detect, mistakes. You can pick and
 choose the hooks you want from the repo; here are some common ones:
 
 ```yaml
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: "v1.10.0"
@@ -676,15 +681,15 @@
 ## Clang-format (C++ only)
 
 If you have C++ code, you should have a `.clang-format` file and use the
 following pre-commit config:
 
 ```yaml
 - repo: https://github.com/pre-commit/mirrors-clang-format
-  rev: "v16.0.4"
+  rev: "v16.0.6"
   hooks:
     - id: clang-format
       types_or: [c++, c, cuda]
 ```
 
 This will use 1-2 MB binary wheels from PyPI on all common platforms. You can
 generated such a file using
@@ -700,16 +705,16 @@
   rev: "v0.9.0.5"
   hooks:
     - id: shellcheck
 ```
 
 ## Prettier
 
-{% include rr.html id="PC180" %} The [prettier](https://prettier.io) tool can
-format a large number of different file types. An example of usage:
+{% rr PC180 %} The [prettier](https://prettier.io) tool can format a large
+number of different file types. An example of usage:
 
 ```yaml
 - repo: https://github.com/pre-commit/mirrors-prettier
   rev: "v2.7.1"
   hooks:
     - id: prettier
       types_or: [yaml, markdown, html, css, scss, javascript, json]
@@ -738,15 +743,15 @@
 get some very nice linting, including catching some problematic code that
 otherwise is hard to catch. PyLint is generally not a good candidate for
 pre-commit, since it needs to have your package installed - it is less static of
 check than Flake8. Here is a suggested pyproject.toml entry to get you started:
 
 ```toml
 [tool.pylint]
-py-version = "3.7"
+py-version = "3.8"
 jobs = "0"
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.enable = ["useless-suppression"]
 messages_control.disable = [
   "design",
   "fixme",
@@ -776,20 +781,27 @@
 [nbQA](https://github.com/nbQA-dev/nbQA). The most useful one is probably Ruff:
 
 ```yaml
 - repo: https://github.com/nbQA-dev/nbQA
   rev: "1.7.0"
   hooks:
     - id: nbqa-ruff
-      additional_dependencies: [ruff==0.0.253]
+      additional_dependencies: [ruff==0.0.275]
 ```
 
 You can pass extra flags to Ruff via the hook, like
 `args: ["--extend-ignore=F821,F401"]`.
 
+{: .note-title }
+
+> Native notebook support
+>
+> Ruff 0.257 added experimental notebook support! You currently have to enable
+> checking `.ipynb` files both in Ruff and pre-commit to use it.
+
 ### Black
 
 For Black, just make sure you use the `id: black-jupyter` hook instead of
 `id: black`; that will also include notebooks.
 
 ### Stripping output
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/guides/writing-docs.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/docs.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,18 @@
 ---
 layout: page
 title: Writing documentation
-permalink: /guides/writing-docs/
-nav_order: 4
-parent: Topical Guides
+permalink: /tutorials/docs/
+nav_order: 5
+parent: Tutorials
 ---
 
 {% include toc.html %}
 
-# Writing Documentation
-
-## What to include
-
-Ideally, software documentation should include:
-
-- Introductory **tutorials**, to help new users (or potential users) understand
-  what the software can do and take their first steps
-- Task-oriented **guides**, examples that address specific uses
-- **Reference**, specifying the detailed inputs and outputs of every public
-  object in the codebase
-- **Explanations** to convey deeper understanding of why and how the software
-  operates the way it does
-
-This overall framework has a name, [Diátaxis][], and you can read more about it
-if you are interested.
+# Writing documentation
 
 ## Build the documentation
 
 Scientific Python software documentation can be written in the Markdown syntax,
 which looks like this:
 
 ````markdown
@@ -66,14 +51,15 @@
 `docs/conf.py`.
 
 ```py
 # content of docs/conf.py
 
 project = "example"
 extensions = ["myst_parser"]
+source_suffix = [".rst", ".md"]
 ```
 
 And, at `docs/index.md`, we will create a minimal front page for our
 documentation.
 
 ```markdown
 # Example documentation
@@ -164,37 +150,30 @@
 inputs and outputs of every public object in the codebase. This should not be
 written by hand; that would be tedious and have a high probably of human error
 or drifting out of sync over time.
 
 MyST recommends using [sphinx-autodoc2][]. However, we currently recommend using
 the built-in sphinx `autodoc` and `autosummary` extensions because they
 interoperates well with docstrings written to the numpydoc standard. To invoke
-them, we need to employ yet another syntax (reST). F:ortunately, you can simply
+them, we need to employ yet another syntax (reST). Fortunately, you can simply
 copy/paste these examples.
 
-Install `numpydoc`.
-
-```bash
-pip install numpydoc
-```
-
 In `docs/conf.py`, add to the list of extensions.
 
 ```py
 extensions = [
     # whatever you already have in here...
-
-    "numpydoc",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
+    "sphinx.ext.napoleon",
 ]
 ```
 
-(Note that `sphinx.ext.autodoc` and `sphinx.ext.autosummary` come installed with
-`sphinx`, so there is nothing more to install.)
+(Note that these extensions come with `sphinx`, so there is nothing more to
+install.)
 
 You can document a single object (e.g. function), shown inline on the page
 
 ````markdown
 ```{eval-rst}
 .. autofunction:: example.refraction.snell
     :noindex:
@@ -210,14 +189,17 @@
     :nosignatures:
     :toctree: generated
 
     example.refraction.snell
 ```
 ````
 
+See the [guide]({% link pages/guides/docs.md %}) for more information on how to
+integrate this into a package, and setup for nox.
+
 <!-- prettier-ignore-start -->
 [diátaxis]: https://diataxis.fr/
 [sphinx]: https://www.sphinx-doc.org/
 [myst]: https://myst-parser.readthedocs.io/
 [organizing content]: https://myst-parser.readthedocs.io/en/latest/syntax/organising_content.html
 [sphinx-autodoc2]: https://sphinx-autodoc2.readthedocs.io/
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/patterns/data_files.md` & `sp_repo_review-2023.7.6/docs/pages/patterns/data_files.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ---
 layout: page
 title: Including data files
-permalink: /patterns/data_files/
-nav_order: 30
+permalink: /patterns/data-files/
+nav_order: 3
 parent: Patterns
 ---
 
 {% include toc.html %}
 
-# Including Data Files
+# Including data files
 
 In this section you will:
 
 - Understand the importance of keeping large files out of your package.
 - Learn some alternative approaches.
 - Learn how to include small data files in your package.
 
@@ -36,17 +36,17 @@
   enough to simulate it accurately, you don't know enough to write useful tests
   against it.
 - Can you write a Python function that fetches the data on demand from some
   public URL? This is the approach used by projects such as scikit-learn that
   need to download large datasets for their examples and tests.
 
 If you use one these alternatives, add the names of the generated or downloaded
-files to the project's `.gitignore` file, which was provided by the cookiecutter
-template. This helps protect you against accidentally committing the file to
-git.
+files to the project's `.gitignore` file, which is provided by the
+[copier][]/[cookiecutter][] template. This helps protect you against
+accidentally committing the file to git.
 
 If the file in question is a text file and not very large (\< 100 kB) than it's
 reasonable to just bundle it with the package. If not, see the recommendation at
 the end.
 
 ## How to Package Data Files
 
@@ -94,15 +94,15 @@
 add an `__init__.py` in `src/package/peak_spacing`. This can be an empty file;
 it's purpose is to tell Python that this can be loaded.
 
 You'll want to make sure your Python building backend is placing these files in
 the SDist and wheel. If you are using anything other than setuptools, this
 should be automatic.
 
-<details markdown="1"><summary>Setuptools-specific instructions</summary>
+{% details Setuptools-specific instructions %}
 
 There are two ways to include data files in setuptools. You can either list the
 package data explicitly:
 
 ```ini
 # setup.cfg
 [options.package_data]
@@ -121,15 +121,15 @@
 But then you'll need to _also_ make sure the files are in the SDist, too:
 
 ```text
 # MANIFEST.in
 include src/package/peak_spacings/*.txt
 ```
 
-</details>
+{% enddetails %}
 
 Finally, wherever we actually use the files in our scientific code, we can
 access them using `importlib_resources`. For users with Python >= 3.9 the
 standard library `importlib.resources` module can be used directly instead of
 relying on `importlib_resources`.
 
 ```python
@@ -197,11 +197,15 @@
     known_hash="sha256:50ef9a52c621b7c0c506ad1fe1b8ee8a158a4d7c8e50ddfce1e273a422dca3f9",
 )
 ```
 
 On repeated runs of this command, the locally cached filename would be used
 instead of downloading the data again.
 
+<!-- prettier-ignore-start -->
 [importlib_resources]: https://importlib-resources.readthedocs.io/en/latest/
 [osf.io]: https://osf.io/
 [pooch]: https://www.fatiando.org/pooch/latest/
 [zenodo]: https://zenodo.org/
+[copier]: https://copier.readthedocs.io
+[cookiecutter]: https://cookiecutter.readthedocs.io
+<!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/principles/design.md` & `sp_repo_review-2023.7.6/docs/pages/principles/design.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,50 +4,52 @@
 permalink: /principles/design/
 nav_order: 2
 parent: Principles
 ---
 
 {% include toc.html %}
 
-# Design Recommendations
+# Design recommendations
 
-## Keep I/O Separate
+## Keep I/O separate
 
 One of the biggest impediments to reuse of scientific code is when I/O
 code---assuming certain file locations, names, formats, or layouts---is
 interspersed with scientific logic.
 
 I/O-related functions should _only_ perform I/O. For example, they should take
 in a filepath and return a numpy array, or a dictionary of arrays and metadata.
 The valuable scientific logic should be encoded in functions that take in
 standard data types and return standard data types. This makes them easier to
 test, maintain when data formats change, or reuse for unforeseen applications.
 
-## Duck Typing is a Good Idea
+## Duck typing is a good idea
 
 [Duck typing][] treats objects based on what they can _do_, not based on what
 type they _are_. "If it walks like a duck and it quacks like a duck, then it
 must be a duck."
 
 Python in general and scientific Python in particular leverage _interfaces_
 (also known as Protocols) to support interoperability and reuse. For example, it
 is possible to pass a pandas DataFrame to the `numpy.sum` function even though
 pandas was created long after `numpy.sum`. This is because `numpy.sum` avoids
 assuming it will be passed specific data types; it accepts any object that
 provides the right methods (interfaces). Where possible, avoid `isinstance`
 checks in your code, and try to make your functions work on the broadest
 possible range of input types.
 
-## Consider: Can this just be a function?
+## Consider: can this just be a function?
 
 Not everything needs to be object-oriented. Object-oriented design needs to
 follow the same principles as other code, like modularity, and be well tested.
 If you can get away with writing functions processing existing datatypes like a
 DataFrame, do so.
 
+{: .highlight }
+
 > It is better to have 100 functions operate on one data structure than 10
 > functions on 10 data structures.
 >
 > -- From ACM's SIGPLAN publication, (September, 1982), Article "Epigrams in
 > Programming", by Alan J. Perlis of Yale University.
 
 A popular talk, ["Stop Writing Classes"][], illustrates how some situations that
@@ -95,15 +97,15 @@
 
 These classes don’t have to be immutable. Maybe you can load more data to loaded
 data. But they are easier to use correctly when they at least avoid a mutating
 state that makes subsets of available operations (i.e. methods) invalid. Note
 that tab completion in this case would show exactly the allowed set of
 operations each time.
 
-## Consider: Do I really want a custom class?
+## Consider: do I really want a custom class?
 
 Using built-in Python types (`int`, `float`, `str`) and standard scientific
 Python types like NumPy array and Pandas DataFrame makes code interoperable. It
 enables data to flow between different libraries smoothly, and to be extended in
 unforeseen ways.
 
 As an example, the widely-used library scikit-image initially experimented with
@@ -141,15 +143,15 @@
 You'll remember (well, at least you are more likely to remember) to handle
 special cases like lists vs strings or values that could also be `None`.
 
 When using static typing, duck typing is expressed via Protocols. These should
 be strongly preferred over older solutions like inheritance or ABCs if possible,
 as they trade a little extra code to remove dependencies between objects.
 
-## Permissiveness Isn't Always Convenient
+## Permissiveness isn't always convenient
 
 Overly permissive code can lead to very confusing bugs. If you need a flexible
 user-facing interface that tries to "do the right thing" by guessing what the
 users wants, separate it into two layers: a thin "friendly" layer on top of a
 "cranky" layer that takes in only exactly what it needs and does the actual
 work. The cranky layer should be easy to test; it should be constrained about
 what it accepts and what it returns. This layered design makes it possible to
@@ -161,28 +163,28 @@
 
 Exceptions should just be raised: don't catch them and print. Exceptions are a
 tool for being clear about what the code needs and letting the caller decide
 what to do about it. _Application_ code (e.g. GUIs) should catch and handle
 errors to avoid crashing, but _library_ code should generally raise errors
 unless it is sure how the user or the caller wants to handle them.
 
-## Write Useful Error Messages
+## Write useful error messages
 
 Be specific. Include what the wrong value was, what was wrong with it, and
 perhaps how it might be fixed. For example, if the code fails to locate a file
 it needs, it should say what it was looking for and where it looked.
 
-## Write for Readability
+## Write for readability
 
 Unless you are writing a script that you plan to delete tomorrow or next week,
 your code will probably be read many more times than it is written. And today's
 "temporary solution" often becomes tomorrow's critical code. Therefore, optimize
 for clarity over brevity, using descriptive and consistent names.
 
-## Complexity is Always Conserved
+## Complexity is always conserved
 
 Complexity is always conserved and is strictly greater than the system the code
 is modeling. Attempts to hide complexity from the user frequently backfire.
 
 For example, it is often tempting to hide certain reused keywords in a function,
 shortening this:
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/principles/index.md` & `sp_repo_review-2023.7.6/docs/pages/principles/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/docs/pages/principles/process.md` & `sp_repo_review-2023.7.6/docs/pages/principles/process.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 permalink: /principles/process/
 nav_order: 1
 parent: Principles
 ---
 
 {% include toc.html %}
 
-# Process Recommendations
+# Process recommendations
 
 ## Collaborate
 
 Software developed by several people is preferable to software developed by one.
 By adopting the conventions and tooling used by many other scientific software
 projects, you are well on your way to making it easy for others to contribute.
 Familiarity works in both directions: it will be easier for others to understand
@@ -29,23 +29,23 @@
 Having more than one person understanding every part of the code prevents
 systematic risks for the project and keeps you from being tied to that code.
 
 If you can bring together contributors with diverse scientific backgrounds, it
 becomes easier to identify functionality that should be generalized for reuse by
 different fields.
 
-## Don't Be Afraid to Refactor
+## Don't be afraid to refactor
 
 No code is ever right the first (or second) time.
 
 Refactoring the code once you understand the problem and the design trade-offs
 more fully helps keep the code maintainable. Version control, tests, and linting
 are your safety net, empowering you to make changes with confidence.
 
-## Prefer "Wide" over "Deep"
+## Prefer "wide" over "deep"
 
 It should be possible to reuse pieces of software in a way not anticipated by
 the original author. That is, branching out from the initial use case should
 enable unplanned functionality without a massive increase in complexity.
 
 When building new things, work your way down to the lowest level, understand
 that level, and then build back up. Try to imagine what else you would want to
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/tutorials/dev-environment.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/dev-environment.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 permalink: /tutorials/dev-environment/
 nav_order: 1
 parent: Tutorials
 ---
 
 {% include toc.html %}
 
+# Intro to development
+
 In this section you will:
 
 - Create an isolated software area ("virtual environment") to work in.
 - Open a code editor.
 
-# Development environment
+## Development environment
 
 If you want to work on Python software, you should _always_ have a virtual
 environment, an area to install the software that is isolated from other
 programs running on your system. A user may not always have one, but a developer
 always should.
 
 Why? You do not want to risk interfering with your main system environment, you
@@ -27,15 +29,15 @@
 delete one and start over---while it is very hard to clean up or update a main
 system environment.
 
 There are many (arguably _too_ many) ways to do this in Python. Any modern tool
 should be fine, but here we recommend two options popular in the scientific
 Python community. If you already use a different way, that's fine, use that.
 
-## Option 1: Using pip
+### Option 1: Using pip
 
 The most basic option is to use `venv`, which comes by default with Python.
 
 ```bash
 python3 -m venv .venv
 ```
 
@@ -43,55 +45,53 @@
 only need to do this step once, per project, per machine you work on. Later, if
 something about your software installation breaks and you want to start fresh,
 you can simply delete this directory to remove all trace of the virtual
 environment.
 
 To activate the virtual environment, type:
 
-<div class="skhep-bar d-flex m-2" style="justify-content:center;">
-  <button class="skhep-bar-item munix-btn btn m-2 btn-purple" onclick="openTab('unix')">Linux/macOS</button>
-  <button class="skhep-bar-item windows-btn btn m-2" onclick="openTab('windows')">Windows</button>
-</div>
-
-<div class="skhep-tab unix-tab" markdown="1">
+{% tabs %} {% tab unix Linux/macOS %}
 
 ```bash
 . .venv/bin/activate
 ```
 
-</div>
-<div class="skhep-tab windows-tab" markdown="1" style="display:none;">
+{% endtab %} {% tab windows Windows %}
 
 ```bat
 .venv\bin\Activate.bat
 ```
 
-</div>
+{% endtab %} {% endtabs %}
 
 You need to do this step every time you open a new shell (i.e. Terminal, Command
 Prompt) to work on your project. The `.` is short for `source`, which runs the
 script `activate` in your current shell. This causes `pip` and `python` to work
 within this new environment, isolated from system-wide packages. It adds a bit
 of text to your prompt so you don't forget that you are in an environment.
 
 The activation script installs a function `deactivate`; type that at any time to
 leave the environment (or just close your shell).
 
-> <h4 class="no_toc">Optional Alternative</h4>
+{: .note-title }
+
+> Optional Alternative
 >
 > Alternatively, you can use the `virtualenv` package, which has the same syntax
 > as `venv` and is a little faster. Unlike `venv`, it is not built in to Python;
 > it has to be installed as `pip install virtualenv`.
 
-> <h4 class="no_toc">For Advanced Users Using Custom Shells</h4>
+{: .highlight-title }
+
+> For Advanced Users Using Custom Shells
 >
 > If you like a different shell, like fish, there are several `activate`
 > scripts; the default one expects a bash-like shell.
 
-## Option 2: Using conda
+### Option 2: Using conda
 
 You can also develop in conda. This is an especially good option if:
 
 - You want an easy way to choose a specific version of Python
 - Your project will depend on complex software libraries that are not readily
   pip-installable
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/tutorials/index.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/docs/pages/tutorials/module.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/module.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 permalink: /tutorials/module/
 nav_order: 2
 parent: Tutorials
 ---
 
 {% include toc.html %}
 
+# Inline documentation
+
 In this section you will:
 
 - Place some code in a module.
 - Provide inline documentation (a "docstring").
 
-# Module
+## Module
 
 As a concrete example, let's suppose we have a simple function that encodes
 [Snell's Law][]. Perhaps this function currently lives in a Jupyter notebook or
 a `.py` file in an email attachment. We want to put into some more lasting,
 maintainable, reusable, and/or shareable form.
 
 Here is the code:
@@ -68,15 +70,15 @@
 - At the top, there is a succinct, one-line summary of the function's purpose.
   It must one line.
 
 - (Optional) There is an paragraph elaborating on that summary.
 
 - There is a section listing input parameters, with the structure
 
-  ```none
+  ```
   parameter_name : parameter_type
       optional description
   ```
 
   Note that space before the `:`. That is part of the standard.
 
 - Similar parameters may be combined into one entry for brevity's sake, as we
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/tutorials/packaging.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/packaging.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 ---
 layout: page
-title: Package
+title: Packaging
 permalink: /tutorials/packaging/
 nav_order: 3
 parent: Tutorials
 ---
 
+{% include toc.html %}
+
+# Packaging
+
 In the section you will:
 
 - Place your module in an installable package.
 - Employ version control.
 - Install and use the package.
 
 For more about packaging, see our [packaging guide][].
 
-# Package
-
 ## Create a minimal installable Python package
 
 Let’s create a Python package that contains this function.
 
 First, create a new directory for your software package, called `example`, and
 move into that:
```

### Comparing `sp_repo_review-2023.6.7/docs/pages/tutorials/test.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/test.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 layout: page
 title: Test
 permalink: /tutorials/test/
 nav_order: 4
 parent: Tutorials
 ---
 
+{% include toc.html %}
+
+# Test
+
 In this section you will:
 
 - Write a test to verify the correctness of the code.
 
 If you already know pytest, check our advanced [pytest guide][].
 
-# Test
-
 You should add a test right away while the details are still fresh in mind.
 Writing tests lets you make future improvements with confidence that any
 unintended changes or breakage with not go unnoticed. Writing tests also tends
 to encouraging you to write modular, reusable code, because it is easier to
 test.
 
 ## Write some tests
```

### Comparing `sp_repo_review-2023.6.7/src/sp_repo_review/families.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/families.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,8 +32,11 @@
         ),
         "mypy": Family(
             name="MyPy",
         ),
         "ruff": Family(
             name="Ruff",
         ),
+        "docs": Family(
+            name="Documentation",
+        ),
     }
```

### Comparing `sp_repo_review-2023.6.7/src/sp_repo_review/checks/general.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/general.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/src/sp_repo_review/checks/github.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/github.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/src/sp_repo_review/checks/mypy.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/mypy.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/src/sp_repo_review/checks/precommit.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/precommit.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "Uses blacken-docs"
     requires = {"PY006", "PC110"}
     repo = "https://github.com/asottile/blacken-docs"
 
 
 class PC190(PreCommit):
     "Uses Ruff"
-    repo = "https://github.com/charliermarsh/ruff-pre-commit"
+    repo = "https://github.com/astral-sh/ruff-pre-commit"
 
 
 class PC140(PreCommit):
     "Uses mypy"
     repo = "https://github.com/pre-commit/mirrors-mypy"
 
 
@@ -78,15 +78,15 @@
     "Uses prettier"
     repo = "https://github.com/pre-commit/mirrors-prettier"
 
 
 class PC191(PreCommit):
     "Ruff show fixes if fixes enabled"
     requires = {"PC190"}
-    repo = "https://github.com/charliermarsh/ruff-pre-commit"
+    repo = "https://github.com/astral-sh/ruff-pre-commit"
 
     @classmethod
     def check(cls, precommit: dict[str, Any]) -> bool | None:
         """
         If `--fix` is present, `--show-fixes` must be too.
         """
         for repo in precommit.get("repos", {}):
```

### Comparing `sp_repo_review-2023.6.7/src/sp_repo_review/checks/pyproject.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/pyproject.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/src/sp_repo_review/checks/ruff.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/ruff.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,22 @@
     "Target version must be set"
     requires = {"RF001"}
 
     @staticmethod
     def check(pyproject: dict[str, Any]) -> bool:
         """
         Must select a minimum version to target. Affects pyupgrade,
-        isort, and others.
+        isort, and others. Can be inferred from `project.requires-python`.
         """
 
         match pyproject:
             case {"tool": {"ruff": {"target-version": str()}}}:
                 return True
+            case {"project": {"requires-python": str()}}:
+                return True
             case _:
                 return False
 
 
 class RF003(Ruff):
     "src directory specified if used"
```

### Comparing `sp_repo_review-2023.6.7/tests/test_package.py` & `sp_repo_review-2023.7.6/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitignore` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/Cargo-maturin.toml` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
-name = "{{ cookiecutter.project_slug }}"
+name = "{{ cookiecutter.__project_slug }}"
 version = "0.1.0"
 edition = "2018"
 
 [lib]
 name = "_core"
 # "cdylib" is necessary to produce a shared library for Python to import from.
 crate-type = ["cdylib"]
 
 [package.metadata.maturin]
-name = "{{ cookiecutter.project_slug }}._core"
-python-packages = ["{{ cookiecutter.project_slug }}"]
+name = "{{ cookiecutter.__project_slug }}._core"
+python-packages = ["{{ cookiecutter.__project_slug }}"]
 python-source = "src"
 
 [dependencies]
 rand = "0.8.3"
 
 [dependencies.pyo3]
 version = "0.18.1"
 # "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
-# "abi3-py37" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.7
-features = ["extension-module", "abi3-py37"]
+# "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
+features = ["extension-module", "abi3-py38"]
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/LICENSE` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'Apache' %}LICENSE{% endif %}`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-{%- if cookiecutter.license == "BSD" %}
-BSD 3-Clause License
-
-Copyright (c) {{ cookiecutter.year }}, {{ cookiecutter.full_name }}.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the vector package developers nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-{%- elif cookiecutter.license == "Apache" %}
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -214,41 +183,20 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright {{ cookiecutter.year }} {{ cookiecutter.full_name }}
+   Copyright {{ cookiecutter.__year }} {{ cookiecutter.full_name }}
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
-{%- elif cookiecutter.license == "MIT" %}
-Copyright {{ cookiecutter.year }} {{ cookiecutter.full_name }}
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-{%- endif %}
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/README.md` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,31 +4,30 @@
 [![Documentation Status][rtd-badge]][rtd-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![Conda-Forge][conda-badge]][conda-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
-[![Gitter][gitter-badge]][gitter-link]
-{%- if cookiecutter.org == "Scikit-HEP" %}
+{%- if cookiecutter.org | lower == "scikit-hep" %}
 [![Scikit-HEP][sk-badge]](https://scikit-hep.org/)
 {%- endif %}
 
+<!-- SPHINX-START -->
+
 <!-- prettier-ignore-start -->
 [actions-badge]:            {{cookiecutter.url}}/workflows/CI/badge.svg
 [actions-link]:             {{cookiecutter.url}}/actions
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/{{cookiecutter.project_name}}
 [conda-link]:               https://github.com/conda-forge/{{cookiecutter.project_name}}-feedstock
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
 [github-discussions-link]:  {{cookiecutter.url}}/discussions
-[gitter-badge]:             https://badges.gitter.im/{{cookiecutter.url}}/community.svg
-[gitter-link]:              https://gitter.im/{{cookiecutter.url}}/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
 [pypi-link]:                https://pypi.org/project/{{cookiecutter.project_name}}/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/{{cookiecutter.project_name}}
 [pypi-version]:             https://img.shields.io/pypi/v/{{cookiecutter.project_name}}
 [rtd-badge]:                https://readthedocs.org/projects/{{cookiecutter.project_name}}/badge/?version=latest
 [rtd-link]:                 https://{{cookiecutter.project_name}}.readthedocs.io/en/latest/?badge=latest
-{%- if cookiecutter.org == "Scikit-HEP" %}
+{%- if cookiecutter.org | lower == "scikit-hep" %}
 [sk-badge]:                 https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
 {%- endif %}
 
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/meson-mesonpy.build` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 project(
-  '{{ cookiecutter.project_slug }}',
+  '{{ cookiecutter.__project_slug }}',
   'cpp',
   version: '0.1.0',
   license: '{{ cookiecutter.license }}',
   meson_version: '>= 0.64.0',
   default_options: [
     'buildtype=debugoptimized',
     'cpp_std=c++11',
   ],
 )
-name = '{{ cookiecutter.project_slug }}'
+name = '{{ cookiecutter.__project_slug }}'
 
 py_mod = import('python')
 py = py_mod.find_installation(pure: false)
 
 pybind11_config = find_program('pybind11-config')
 pybind11_config_ret = run_command(pybind11_config, ['--includes'], check: true)
 pybind11 = declare_dependency(
     include_directories: [pybind11_config_ret.stdout().split('-I')[-1].strip()],
 )
 
 install_subdir('src' / name, install_dir: py.get_install_dir() / name, strip_directory: true)
 
 py.extension_module('_core',
     'src/main.cpp',
-    subdir: '{{ cookiecutter.project_slug }}',
+    subdir: '{{ cookiecutter.__project_slug }}',
     install: true,
     dependencies : [pybind11],
     link_language : 'cpp',
     override_options: [
         'cpp_rtti=true',
     ]
 )
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/noxfile.py` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/noxfile.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import argparse
-{%- if cookiecutter.project_type != "pybind11" %}
+{%- if cookiecutter.backend != "pybind11" %}
 import shutil
 from pathlib import Path
 {%- endif %}
 
 import nox
 
-{% if cookiecutter.project_type != "pybind11" -%}
+{% if cookiecutter.backend != "pybind11" -%}
 DIR = Path(__file__).parent.resolve()
 
 {% endif -%}
 
 nox.options.sessions = ["lint", "pylint", "tests"]
 
 
@@ -49,22 +49,46 @@
 def docs(session: nox.Session) -> None:
     """
     Build the docs. Pass "--serve" to serve.
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--serve", action="store_true", help="Serve after building")
-    args = parser.parse_args(session.posargs)
+    parser.add_argument(
+        "-b", dest="builder", default="html", help="Build target (default: html)"
+    )
+    args, posargs = parser.parse_known_args(session.posargs)
+
+    if args.builder != "html" and args.serve:
+        session.error("Must not specify non-HTML builder with --serve")
 
     session.install(".[docs]")
     session.chdir("docs")
-    session.run("sphinx-build", "-M", "html", ".", "_build")
+
+    if args.builder == "linkcheck":
+        session.run(
+            "sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs
+        )
+        return
+
+    session.run(
+        "sphinx-build",
+        "-n",  # nitpicky mode
+        "-T",  # full tracebacks
+        "-W",  # Warnings as errors
+        "--keep-going",  # See all errors
+        "-b",
+        args.builder,
+        ".",
+        f"_build/{args.builder}",
+        *posargs,
+    )
 
     if args.serve:
-        print("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
+        session.log("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
         session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
 
 
 @nox.session
 def build_api_docs(session: nox.Session) -> None:
     """
     Build (regenerate) API docs.
@@ -72,22 +96,22 @@
 
     session.install("sphinx")
     session.chdir("docs")
     session.run(
         "sphinx-apidoc",
         "-o",
         "api/",
+        "--module-first",
         "--no-toc",
         "--force",
-        "--module-first",
-        "../src/{{ cookiecutter.project_name.replace('-', '_') }}",
+        "../src/{{ cookiecutter.__project_slug }}",
     )
 
 
-{%- if cookiecutter.project_type != "pybind11" %}
+{%- if cookiecutter.backend != "pybind11" %}
 
 
 @nox.session
 def build(session: nox.Session) -> None:
     """
     Build an SDist and wheel.
     """
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/pyproject.toml` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 [build-system]
-{%- if cookiecutter.project_type == "trampolim" %}
+{%- if cookiecutter.backend == "trampolim" %}
 requires = ["trampolim>=0.1.0"]
 build-backend = "trampolim"
-{%- elif cookiecutter.project_type == "whey" %}
+{%- elif cookiecutter.backend == "whey" %}
 requires = ["whey>=0.0.17"]
 build-backend = "whey"
-{%- elif cookiecutter.project_type == "pdm" %}
+{%- elif cookiecutter.backend == "pdm" %}
 requires = ["pdm-backend"]
 build-backend = "pdm.backend"
-{%- elif cookiecutter.project_type == "maturin" %}
+{%- elif cookiecutter.backend == "maturin" %}
 requires = ["maturin>=0.12,<0.15"]
 build-backend = "maturin"
-{%- elif cookiecutter.project_type == "hatch" %}
+{%- elif cookiecutter.backend == "hatch" %}
 requires = ["hatchling"]
 build-backend = "hatchling.build"
-{%- elif cookiecutter.project_type == "setuptools621" %}
+{%- elif cookiecutter.backend == "setuptools621" %}
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
-{%- elif cookiecutter.project_type == "flit" %}
+{%- elif cookiecutter.backend == "flit" %}
 requires = ["flit_core >=3.4"]
 build-backend = "flit_core.buildapi"
-{%- elif cookiecutter.project_type == "setuptools" %}
+{%- elif cookiecutter.backend == "setuptools" %}
 requires = ["setuptools>=42", "setuptools_scm[toml]>=3.4"]
 build-backend = "setuptools.build_meta"
-{%- elif cookiecutter.project_type == "pybind11" %}
+{%- elif cookiecutter.backend == "pybind11" %}
 requires = ["setuptools>=42", "setuptools_scm[toml]>=3.4", "pybind11"]
 build-backend = "setuptools.build_meta"
-{%- elif cookiecutter.project_type == "skbuild"  %}
+{%- elif cookiecutter.backend == "skbuild"  %}
 requires = ["pybind11", "scikit-build-core"]
 build-backend = "scikit_build_core.build"
-{%- elif cookiecutter.project_type == "mesonpy"  %}
+{%- elif cookiecutter.backend == "mesonpy"  %}
 requires = ["pybind11", "meson-python"]
 build-backend = "mesonpy"
-{%- elif cookiecutter.project_type == "poetry" %}
+{%- elif cookiecutter.backend == "poetry" %}
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 {%- endif %}
 
-{%- if cookiecutter.project_type in ["setuptools", "pybind11"] %}
+{%- if cookiecutter.backend in ["setuptools", "pybind11"] %}
 
 
 [tool.setuptools_scm]
-write_to = "src/{{ cookiecutter.project_slug }}/_version.py"
+write_to = "src/{{ cookiecutter.__project_slug }}/_version.py"
 
 
 [tool.check-manifest]
 ignore = [
   ".github/**",
   "docs/**",
   ".pre-commit-config.yaml",
-  ".readthedocs.yml",
+  ".readthedocs.yaml",
   "src/*/_version.py",
   "noxfile.py",
 ]
 
-{%- elif cookiecutter.project_type == "poetry" %}
+{%- elif cookiecutter.backend == "poetry" %}
 
 
 [tool.poetry]
 name = "{{ cookiecutter.project_name }}"
 version = "0.1.0"
 authors = [
   "{{ cookiecutter.full_name }} <{{ cookiecutter.email }}>",
 ]
-{%- if cookiecutter.org == "Scikit-HEP" %}
+{%- if cookiecutter.org == "scikit-hep" %}
 maintainers = [
   "The Scikit-HEP admins <scikit-hep-admins@googlegroups.com>",
 ]
 {%- endif %}
 homepage = "{{ cookiecutter.url }}"
 repository = "{{ cookiecutter.url }}"
 {%- if cookiecutter.license == "BSD" %}
@@ -86,58 +86,60 @@
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7"
-typing_extensions = { version = ">=3.7", python = "<3.8" }
+python = ">=3.8"
+typing_extensions = { version = ">=4.6", python = "<3.11" }
 
 furo = { version = ">=22", optional = true }
 myst_parser = { version = ">=0.13", optional = true }
 pytest = { version = ">=6", optional = true }
 pytest-cov = { version = ">=3", optional = true }
 sphinx = { version = ">=4.0", optional = true }
 sphinx_copybutton = { version = ">=0.3.0", optional = true }
+sphinx-autodoc-typehints = { version = "*", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = ">= 6"
 pytest-cov = ">= 3"
 
 [tool.poetry.extras]
 test = ["pytest", "pytest-cov"]
 dev = ["pytest", "pytest-cov"]
 docs = [
   "furo",
   "myst_parser",
   "sphinx",
+  "sphinx_autodoc_typehints",
   "sphinx_copybutton",
 ]
 
 
 {%- else %}
 
 
 [project]
 name = "{{ cookiecutter.project_name }}"
-{%- if cookiecutter.project_type not in ["trampolim", "flit", "hatch"] %}
+{%- if cookiecutter.backend not in ["trampolim", "flit", "hatch"] %}
 version = "0.1.0"
 {%- endif %}
 authors = [
   { name = "{{ cookiecutter.full_name }}", email = "{{ cookiecutter.email }}" },
 ]
-{%- if cookiecutter.org == "Scikit-HEP" %}
+{%- if cookiecutter.org | lower == "scikit-hep" %}
 maintainers = [
   { name = "The Scikit-HEP admins", email = "scikit-hep-admins@googlegroups.com" },
 ]
 {%- endif %}
 description = "{{ cookiecutter.project_short_description }}"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
 {%- if cookiecutter.license == "BSD" %}
   "License :: OSI Approved :: BSD License",
 {%- elif cookiecutter.license == "Apache" %}
@@ -145,73 +147,73 @@
 {%- elif cookiecutter.license == "MIT" %}
   "License :: OSI Approved :: MIT License",
 {%- endif %}
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
-{%- if cookiecutter.project_type in ["trampolim", "flit", "hatch"] %}
+{%- if cookiecutter.backend in ["trampolim", "flit", "hatch"] %}
 dynamic = ["version"]
 {%- endif %}
 dependencies = [
-  "typing_extensions >=3.7; python_version<'3.8'",
+  "typing_extensions >=4.6; python_version<'3.11'",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
 dev = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
 docs = [
   "sphinx>=4.0",
   "myst_parser>=0.13",
-  "sphinx-book-theme>=0.1.0",
+  "sphinx_book_theme>=0.1.0",
   "sphinx_copybutton",
+  "sphinx_autodoc_typehints",
   "furo",
 ]
 
 [project.urls]
 Homepage = "{{ cookiecutter.url }}"
 "Bug Tracker" = "{{ cookiecutter.url }}/issues"
 Discussions = "{{ cookiecutter.url }}/discussions"
 Changelog = "{{ cookiecutter.url }}/releases"
 {%- endif %}
 
 
-{%- if cookiecutter.project_type == "skbuild" %}
+{%- if cookiecutter.backend == "skbuild" %}
 [tool.scikit-build]
 minimum-version = "0.2"
 build-dir = "build/{cache_tag}"
-{%- elif cookiecutter.project_type == "whey" %}
+{%- elif cookiecutter.backend == "whey" %}
 [tool.whey]
 source-dir = "src"
-{%- elif cookiecutter.project_type == "trampolim" %}
+{%- elif cookiecutter.backend == "trampolim" %}
 [tool.trampolim]
 module-location = "src"
-{%- elif cookiecutter.project_type == "hatch" %}
+{%- elif cookiecutter.backend == "hatch" %}
 [tool.hatch]
-version.path = "src/{{ cookiecutter.project_slug  }}/__init__.py"
+version.path = "src/{{ cookiecutter.__project_slug  }}/__init__.py"
 envs.default.dependencies = [
   "pytest",
   "pytest-cov",
 ]
-{%- elif cookiecutter.project_type == "pdm" %}
+{%- elif cookiecutter.backend == "pdm" %}
 [tool.pdm.dev-dependencies]
 devtest = ["pytest", "pytest-cov"]
 {%- endif %}
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
@@ -224,34 +226,34 @@
 log_cli_level = "INFO"
 testpaths = [
   "tests",
 ]
 
 
 [tool.coverage]
-run.source = ["{{ cookiecutter.project_slug }}"]
+run.source = ["{{ cookiecutter.__project_slug }}"]
 port.exclude_lines = [
   'pragma: no cover',
   '\.\.\.',
   'if typing.TYPE_CHECKING:',
 ]
 
 [tool.mypy]
 files = ["src", "tests"]
-python_version = "3.7"
+python_version = "3.8"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
 
 [[tool.mypy.overrides]]
-module = "{{ cookiecutter.project_slug  }}.*"
+module = "{{ cookiecutter.__project_slug  }}.*"
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
@@ -278,16 +280,18 @@
   "NPY",         # NumPy specific rules
   "PD",          # pandas-vet
 ]
 extend-ignore = [
   "PLR",    # Design related pylint codes
   "E501",   # Line too long
 ]
-target-version = "py37"
-typing-modules = ["{{ cookiecutter.project_slug }}._compat.typing"]
+{%- if cookiecutter.backend in ["setuptools", "pybind11", "poetry"] %}
+target-version = "py38"
+{%- endif %}
+typing-modules = ["{{ cookiecutter.__project_slug }}._compat.typing"]
 src = ["src"]
 unfixable = [
   "T20",  # Removes print statements
   "F841", # Removes unused variables
 ]
 exclude = []
 flake8-unused-arguments.ignore-variadic-names = true
@@ -295,16 +299,16 @@
 
 [tool.ruff.per-file-ignores]
 "tests/**" = ["T20"]
 "noxfile.py" = ["T20"]
 
 
 [tool.pylint]
-py-version = "3.7"
-ignore-paths= ["src/{{ cookiecutter.project_slug }}/_version.py"]
+py-version = "3.8"
+ignore-paths= ["src/{{ cookiecutter.__project_slug }}/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
   "design",
   "fixme",
   "line-too-long",
   "missing-module-docstring",
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-pybind11.py` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) {{ cookiecutter.year }}, {{ cookiecutter.full_name }}
+# Copyright (c) {{ cookiecutter.__year }}, {{ cookiecutter.full_name }}
 #
 # Distributed under the 3-clause BSD license, see accompanying file LICENSE
 # or {{ cookiecutter.url }} for details.
 
 from __future__ import annotations
 
 from setuptools import setup  # isort:skip
@@ -12,15 +12,15 @@
 
 # Note:
 #   Sort input source files if you glob sources to ensure bit-for-bit
 #   reproducible builds (https://github.com/pybind/python_example/pull/53)
 
 ext_modules = [
     Pybind11Extension(
-        "{{ cookiecutter.project_slug }}._core",
+        "{{ cookiecutter.__project_slug }}._core",
         ["src/main.cpp"],
         cxx_std=11,
     ),
 ]
 
 
 setup(
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools,pybind11.cfg` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 [metadata]
-name = {{ cookiecutter.project_slug }}
+name = {{ cookiecutter.__project_slug }}
 description = {{ cookiecutter.project_short_description }}
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = {{ cookiecutter.url }}
 author = {{ cookiecutter.full_name }}
 author_email = {{ cookiecutter.email }}
-{%- if cookiecutter.org == "Scikit-HEP" %}
+{%- if cookiecutter.org | lower == "scikit-hep" %}
 maintainer = The Scikit-HEP admins
 maintainer_email = scikit-hep-admins@googlegroups.com
 {%- endif %}
+{%- if cookiecutter.license == "BSD" %}
 license = BSD-3-Clause
-license_file = LICENSE
+{%- elif cookiecutter.license == "Apache" %}
+license = Apache-2.0
+{%- elif cookiecutter.license == "MIT" %}
+license = MIT
+{%- endif %}
+license_files = LICENSE
 platforms =
     Any
 classifiers =
     Development Status :: 1 - Planning
     Intended Audience :: Developers
     Intended Audience :: Science/Research
 {%- if cookiecutter.license == "BSD" %}
@@ -25,32 +31,32 @@
 {%- elif cookiecutter.license == "MIT" %}
     License :: OSI Approved :: MIT License
 {%- endif %}
     Operating System :: OS Independent
     Programming Language :: Python
     Programming Language :: Python :: 3
     Programming Language :: Python :: 3 :: Only
-    Programming Language :: Python :: 3.7
     Programming Language :: Python :: 3.8
     Programming Language :: Python :: 3.9
     Programming Language :: Python :: 3.10
     Programming Language :: Python :: 3.11
+    Programming Language :: Python :: 3.12
     Topic :: Scientific/Engineering
     Typing :: Typed
 project_urls =
     Documentation = https://{{ cookiecutter.project_name }}.readthedocs.io/
     Bug Tracker = {{ cookiecutter.url }}/issues
     Discussions = {{ cookiecutter.url }}/discussions
     Changelog = {{ cookiecutter.url }}/releases
 
 [options]
 packages = find:
 install_requires =
-    typing-extensions>=3.7;python_version<'3.8'
-python_requires = >=3.7
+    typing-extensions>=4.6;python_version<'3.11'
+python_requires = >=3.8
 include_package_data = True
 package_dir =
     =src
 
 [options.packages.find]
 where = src
 
@@ -58,11 +64,12 @@
 dev =
     pytest>=6
     pytest-cov>=3
 docs =
     furo>=22
     myst-parser>=0.13
     sphinx>=4.0
+    sphinx-autodoc-typehints
     sphinx-copybutton
 test =
     pytest>=6
     pytest-cov>=3
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Nox handles everything for you, including setting up an temporary virtual
 environment for each run.
 
 # Setting up a development environment manually
 
 You can set up a development environment by running:
 
-{% if cookiecutter.project_type == "poetry" -%}
+{% if cookiecutter.backend == "poetry" -%}
 
 ```bash
 poetry install
 ```
 
 {%- else -%}
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/matchers/pylint.json` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/ci.yml` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- set compiled = cookiecutter.project_type in ["pybind11", "maturin", "skbuild", "mesonpy"] -%}
+{%- set compiled = cookiecutter.backend in ["pybind11", "maturin", "skbuild", "mesonpy"] -%}
 name: CI
 
 on:
   workflow_dispatch:
   pull_request:
   push:
     branches:
@@ -44,46 +44,47 @@
   checks:
     name: {% raw %}Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}{% endraw %}
     runs-on: {% raw %}${{ matrix.runs-on }}{% endraw %}
     needs: [pre-commit]
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.11", "3.12-dev"]
+        python-version: ["3.8", "3.11", "3.12"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
         include:
-          - python-version: pypy-3.8
+          - python-version: pypy-3.9
             runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - uses: actions/setup-python@v4
         with:
           python-version: {% raw %}${{ matrix.python-version }}{% endraw %}
+          allow-prereleases: true
 
-      {%- if cookiecutter.project_type == "mesonpy" %}
+      {%- if cookiecutter.backend == "mesonpy" %}
       - name: Activate MSVC for Meson
         if: runner.os == 'Windows'
         uses: ilammy/msvc-dev-cmd@v1
       {%- endif %}
 
       - name: Install package
         run: python -m pip install .[test]
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.4
 
   {%- if not compiled %}
 
   dist:
     needs: [pre-commit]
     name: Distribution build
     runs-on: ubuntu-latest
@@ -96,15 +97,15 @@
       - name: Build sdist and wheel
         run: pipx run build
 
       - uses: actions/upload-artifact@v3
         with:
           path: dist
 
-      {%- if cookiecutter.project_type != "trampolim" %}
+      {%- if cookiecutter.backend != "trampolim" %}
 
       - name: Check products
         run: pipx run twine check dist/*
 
       {%- endif %}
 
   publish:
@@ -124,13 +125,13 @@
 
       - uses: pypa/gh-action-pypi-publish@release/v1
         if: github.event_name == 'release' && github.event.action == 'published'
         with:
           # Remember to tell (test-)pypi about this repo before publishing
           # Remove this line to publish to PyPI
           repository-url: https://test.pypi.org/legacy/
-          {%- if cookiecutter.project_type == "trampolim" %}
+          {%- if cookiecutter.backend == "trampolim" %}
           # Check not supported currently by twine + trampolim
           verify-metadata: false
           {%- endif %}
 
   {%- endif %}
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/wheels-pybind11,skbuild,mesonpy,maturin.yml` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type == 'compiled' %}wheels.yml{% endif %}`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         os: [ubuntu-latest, windows-latest, macos-latest]
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
-      - uses: pypa/cibuildwheel@v2.12.3
+      - uses: pypa/cibuildwheel@v2.13.1
 
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           path: wheelhouse/*.whl
 
   upload_all:
```

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/lib-maturin.rs` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/main-pybind11,skbuild,mesonpy.cpp` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/.gitignore` & `sp_repo_review-2023.7.6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
 # setuptools_scm
-src/*/version.py
+src/*/_version.py
 
 # Jeykll stuff
 .jekyll-cache/
 .jekyll-metadata
 _site/
 
 # NodeJS stuff, just in case (developer tooling)
```

### Comparing `sp_repo_review-2023.6.7/LICENSE` & `sp_repo_review-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.7/pyproject.toml` & `sp_repo_review-2023.7.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [build-system]
-requires = ["hatchling", "hatch-vcs"]
+requires = ["hatchling", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "sp_repo_review"
 authors = [
   { name = "Henry Schreiner", email = "henryfs@princeton.edu" },
 ]
 description = "Review repos for compliance to the Scientific-Python development guidelines"
-readme = "README-rr.md"
 requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Environment :: WebAssembly :: Emscripten",
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
@@ -25,88 +24,98 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python",
   "Topic :: Scientific/Engineering",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Software Development :: Quality Assurance",
   "Typing :: Typed",
 ]
-dynamic = ["version"]
+dynamic = ["version", "readme"]
 dependencies = [
   "pyyaml",
-  "repo-review>=0.7.0b4,<0.8",
+  "repo-review>=0.7,<0.9",
 ]
 
 [project.optional-dependencies]
 cli = [
   "repo-review[cli]",
 ]
 test = [
   "pytest >=7",
 ]
 dev = [
   "pytest >=7",
 ]
 
 [project.urls]
-Homepage = "https://github.com/scientific-python/cookie"
-Webpage = "https://scientific-python.github.io/cookie"
+Guide = "https://learn.scientific-python.org/development"
+Homepage = "https://scientific-python.github.io/cookie"
 Preview = "https://scientific-python-cookie.readthedocs.io"
+Source = "https://github.com/scientific-python/cookie"
 
 
 [project.entry-points."pipx.run"]
 sp-repo-review = "repo_review.__main__:main"
 
 [project.entry-points."repo_review.checks"]
 general = "sp_repo_review.checks.general:repo_review_checks"
 pyproject = "sp_repo_review.checks.pyproject:repo_review_checks"
 precommit = "sp_repo_review.checks.precommit:repo_review_checks"
 ruff = "sp_repo_review.checks.ruff:repo_review_checks"
 mypy = "sp_repo_review.checks.mypy:repo_review_checks"
 github = "sp_repo_review.checks.github:repo_review_checks"
+readthedocs = "sp_repo_review.checks.readthedocs:repo_review_checks"
 
 [project.entry-points."repo_review.fixtures"]
 workflows = "sp_repo_review.checks.github:workflows"
 dependabot = "sp_repo_review.checks.github:dependabot"
 precommit = "sp_repo_review.checks.precommit:precommit"
+readthedocs = "sp_repo_review.checks.readthedocs:readthedocs"
 
 [project.entry-points."repo_review.families"]
 scikit-hep = "sp_repo_review.families:get_familes"
 
+
 [tool.hatch]
 version.source = "vcs"
 build.hooks.vcs.version-file = "src/sp_repo_review/_version.py"
 
+[tool.hatch.metadata.hooks.fancy-pypi-readme]
+content-type = "text/markdown"
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
+path = "README.md"
+start-after = "<!-- sp-repo-review -->"
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = ["-ra", "--strict-markers", "--strict-config"]
 xfail_strict = true
 log_cli_level = "INFO"
 filterwarnings = [
   'error',
-  'ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest',
 ]
 norecursedirs = ['{{cookiecutter.project_name}}']
 testpaths = ["tests"]
 
 
 [tool.mypy]
-files = ["src", "web", "tests"]
+files = ["src", "tests"]
 python_version = "3.10"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 disallow_untyped_defs = false
 
 [[tool.mypy.overrides]]
 module = "sp_repo_review.*"
 disallow_untyped_defs = true
 
+
 [tool.pylint]
 master.py-version = "3.10"
 master.ignore-paths= ["src/sp_repo_review/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
   "design",
@@ -122,15 +131,15 @@
   "no-member",  # better handled by mypy, etc.
 ]
 
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
-  "B", "B904",   # flake8-bugbear
+  "B",           # flake8-bugbear
   "I",           # isort
   "ARG",         # flake8-unused-arguments
   "C4",          # flake8-comprehensions
   "EM",          # flake8-errmsg
   "ICN",         # flake8-import-conventions
   "ISC",         # flake8-implicit-str-concat
   "PGH",         # pygrep-hooks
@@ -146,16 +155,16 @@
   "UP",          # pyupgrade
   "YTT",         # flake8-2020
 ]
 extend-ignore = [
   "PLR",    # Design related pylint codes
   "E501",   # Line too long
   "PT004",  # Incorrect check, usefixtures is the correct way to do this
+  "RUF012", # Would require a lot of ClassVar's
 ]
-target-version = "py310"
 src = ["src"]
 unfixable = [
   "T20",  # Removes print statements
   "F841", # Removes unused variables
 ]
 exclude = []
 flake8-unused-arguments.ignore-variadic-names = true
@@ -167,7 +176,10 @@
 "typing.Sequence".msg = "Use collections.abc.Sequence instead."
 "typing.Set".msg = "Use collections.abc.Set instead."
 "importlib.abc".msg = "Use sp_repo_review._compat.importlib.resources.abc instead."
 "importlib.resources.abc".msg = "Use sp_repo_review._compat.importlib.resources.abc instead."
 
 [tool.ruff.per-file-ignores]
 "src/sp_repo_review/_compat/**.py" = ["TID251"]
+
+[tool.repo-review]
+ignore = ["RTD103"]
```

