# Comparing `tmp/adaux-2.5.0.tar.gz` & `tmp/adaux-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaux-2.5.0.tar", last modified: Sun Jun 25 23:31:03 2023, max compression
+gzip compressed data, was "adaux-2.6.0.tar", last modified: Thu Jul  6 21:06:29 2023, max compression
```

## Comparing `adaux-2.5.0.tar` & `adaux-2.6.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.471931 adaux-2.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-06-09 07:59:40.000000 adaux-2.5.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-25 23:31:03.471931 adaux-2.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-06-25 23:31:03.475932 adaux-2.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.127919 adaux-2.5.0/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.239923 adaux-2.5.0/source/adaux/
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-25 21:24:58.000000 adaux-2.5.0/source/adaux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_base_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    14267 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14719 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_cli_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.319926 adaux-2.5.0/source/adaux/_components/
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_00_extra_level.py
--rw-rw-rw-   0 root         (0) root         (0)     4879 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_01_file_io_support.py
--rw-rw-rw-   0 root         (0) root         (0)     5076 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_02_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_03_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_04_monotonic_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6664 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_05_project.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_06_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_07_package.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_08_pip.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_09_gitignore.py
--rw-rw-rw-   0 root         (0) root         (0)     4211 2023-06-25 21:32:20.000000 adaux-2.5.0/source/adaux/_components/_10_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     5813 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_11_precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     6494 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_12_pylint.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_13_executable.py
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_14_mypy.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_15_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_16_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     2801 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_17_docs.py
--rw-rw-rw-   0 root         (0) root         (0)    20260 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_18_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    17195 2023-06-25 23:21:24.000000 adaux-2.5.0/source/adaux/_components/_19_docker.py
--rw-rw-rw-   0 root         (0) root         (0)    11985 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_20_ci.py
--rw-rw-rw-   0 root         (0) root         (0)     3637 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_98_sentinel.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_99_all.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12673 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_aux_ci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.339927 adaux-2.5.0/source/adaux/_components/_payload/
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_docker_build.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)    15864 2023-06-25 22:36:13.000000 adaux-2.5.0/source/adaux/_components/_payload/_docker_executors.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-06-25 22:36:13.000000 adaux-2.5.0/source/adaux/_components/_payload/_docker_run.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_python.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_with_dependency.py
--rwxrwxrwx   0 root         (0) root         (0)     1629 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_create_badge.py
--rw-rw-rw-   0 root         (0) root         (0)    14742 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7090 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_proto_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_tick.py
--rw-rw-rw-   0 root         (0) root         (0)     3414 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_todo.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_util.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.343927 adaux-2.5.0/source/adaux/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.351927 adaux-2.5.0/source/adaux/src/CI/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/CI/00-main.yml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/CI/01-rules.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.355927 adaux-2.5.0/source/adaux/src/CI/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/CI/jinja-snippets/coverage.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/CI/jinja-snippets/tags.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.359927 adaux-2.5.0/source/adaux/src/docker/
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/comp-helper.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.171920 adaux-2.5.0/source/adaux/src/docker/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.371928 adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy/
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-06-25 21:24:58.000000 adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-06-25 23:21:24.000000 adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.371928 adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy-ext/
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-25 23:21:24.000000 adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy-ext/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.379928 adaux-2.5.0/source/adaux/src/docker/services/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.379928 adaux-2.5.0/source/adaux/src/docker/services/gitlab-release-run/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.383928 adaux-2.5.0/source/adaux/src/docker/services/image/
--rw-rw-rw-   0 root         (0) root         (0)     1760 2023-06-25 21:24:58.000000 adaux-2.5.0/source/adaux/src/docker/services/image/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-06-25 21:24:58.000000 adaux-2.5.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.383928 adaux-2.5.0/source/adaux/src/docker/services/image-pytest/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.407929 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-25 21:24:58.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/ansible_deploy.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-25 23:21:24.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/ansible_env.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-25 23:21:24.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.411929 adaux-2.5.0/source/adaux/src/docker/services/pkg-gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.415929 adaux-2.5.0/source/adaux/src/docker/services/pkg-pypi/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.419929 adaux-2.5.0/source/adaux/src/docker/services/pre-commit/
--rw-rw-rw-   0 root         (0) root         (0)     1176 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.419929 adaux-2.5.0/source/adaux/src/docker/services/pycov/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.427930 adaux-2.5.0/source/adaux/src/docker/services/pytest/
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.431930 adaux-2.5.0/source/adaux/src/docker/services/pytest-standalone/
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.435930 adaux-2.5.0/source/adaux/src/docker/services/python-deps/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.439930 adaux-2.5.0/source/adaux/src/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/default_conf.py.jinja2
--rwxrwxrwx   0 root         (0) root         (0)     1873 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/postprocess_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.439930 adaux-2.5.0/source/adaux/src/docs/static/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/static/git-link-color.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.443930 adaux-2.5.0/source/adaux/src/docs/user/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/user/conf.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/user/gitignore
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/user/index.rst.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/gitignore
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/install-dev.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.447930 adaux-2.5.0/source/adaux/src/license/
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/license/Apache-2.0.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/license/BSD-3_clause.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/license/MIT.txt.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.187921 adaux-2.5.0/source/adaux/src/payload/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.447930 adaux-2.5.0/source/adaux/src/payload/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.447930 adaux-2.5.0/source/adaux/src/payload/python/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2530 2023-06-25 23:29:48.000000 adaux-2.5.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/payload/python/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.447930 adaux-2.5.0/source/adaux/src/pip/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/pip/pip.conf.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.459931 adaux-2.5.0/source/adaux/src/pre-commit/
--rwxrwxrwx   0 root         (0) root         (0)     1680 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     5098 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/pre-commit/config.yaml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/pre-commit/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.467931 adaux-2.5.0/source/adaux/src/root/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/root/_setup.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/root/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/root/setup.cfg.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.471931 adaux-2.5.0/source/adaux/src/root/source/
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/root/source/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/temp-combination
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.263924 adaux-2.5.0/source/adaux.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-25 23:31:02.000000 adaux-2.5.0/source/adaux.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5451 2023-06-25 23:31:03.000000 adaux-2.5.0/source/adaux.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 23:31:02.000000 adaux-2.5.0/source/adaux.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-25 23:31:02.000000 adaux-2.5.0/source/adaux.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 23:29:46.000000 adaux-2.5.0/source/adaux.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-25 23:31:02.000000 adaux-2.5.0/source/adaux.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-25 23:31:02.000000 adaux-2.5.0/source/adaux.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.208302 adaux-2.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-06-09 07:59:40.000000 adaux-2.6.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-06 21:06:29.208302 adaux-2.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-07-06 21:06:29.208302 adaux-2.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.092298 adaux-2.6.0/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.124299 adaux-2.6.0/source/adaux/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-06 20:29:15.000000 adaux-2.6.0/source/adaux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_base_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14267 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14719 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_cli_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.148300 adaux-2.6.0/source/adaux/_components/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_00_extra_level.py
+-rw-rw-rw-   0 root         (0) root         (0)     4879 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_01_file_io_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5109 2023-07-06 20:46:38.000000 adaux-2.6.0/source/adaux/_components/_02_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_03_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_04_monotonic_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6664 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_05_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_06_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_07_package.py
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_08_pip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_09_gitignore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4211 2023-06-25 21:32:20.000000 adaux-2.6.0/source/adaux/_components/_10_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5813 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_11_precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6494 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_12_pylint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_13_executable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_14_mypy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_15_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_16_coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2801 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_17_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)    20260 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_18_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    17195 2023-06-25 23:21:24.000000 adaux-2.6.0/source/adaux/_components/_19_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11985 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_20_ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_98_sentinel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_99_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12678 2023-07-06 20:30:38.000000 adaux-2.6.0/source/adaux/_components/_aux_ci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.156300 adaux-2.6.0/source/adaux/_components/_payload/
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_payload/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_payload/_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_payload/_docker_build.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_payload/_docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)    15864 2023-06-25 22:36:13.000000 adaux-2.6.0/source/adaux/_components/_payload/_docker_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-06-25 22:36:13.000000 adaux-2.6.0/source/adaux/_components/_payload/_docker_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_payload/_python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_components/_payload/_with_dependency.py
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_create_badge.py
+-rw-rw-rw-   0 root         (0) root         (0)    14742 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     7090 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_proto_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_tick.py
+-rw-rw-rw-   0 root         (0) root         (0)     3414 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_todo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.160300 adaux-2.6.0/source/adaux/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.160300 adaux-2.6.0/source/adaux/src/CI/
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/CI/00-main.yml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/CI/01-rules.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.160300 adaux-2.6.0/source/adaux/src/CI/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/CI/jinja-snippets/coverage.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/CI/jinja-snippets/tags.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.164301 adaux-2.6.0/source/adaux/src/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/comp-helper.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.104298 adaux-2.6.0/source/adaux/src/docker/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.164301 adaux-2.6.0/source/adaux/src/docker/services/ansible-deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-06-25 21:24:58.000000 adaux-2.6.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-06-25 23:21:24.000000 adaux-2.6.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.164301 adaux-2.6.0/source/adaux/src/docker/services/ansible-deploy-ext/
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-25 23:21:24.000000 adaux-2.6.0/source/adaux/src/docker/services/ansible-deploy-ext/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.168301 adaux-2.6.0/source/adaux/src/docker/services/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.168301 adaux-2.6.0/source/adaux/src/docker/services/gitlab-release-run/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.168301 adaux-2.6.0/source/adaux/src/docker/services/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-06-25 21:24:58.000000 adaux-2.6.0/source/adaux/src/docker/services/image/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-06-25 21:24:58.000000 adaux-2.6.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.172301 adaux-2.6.0/source/adaux/src/docker/services/image-pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.180301 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-25 21:24:58.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/ansible_deploy.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-25 23:21:24.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/ansible_env.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-25 23:21:24.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.180301 adaux-2.6.0/source/adaux/src/docker/services/pkg-gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.184301 adaux-2.6.0/source/adaux/src/docker/services/pkg-pypi/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.184301 adaux-2.6.0/source/adaux/src/docker/services/pre-commit/
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.184301 adaux-2.6.0/source/adaux/src/docker/services/pycov/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.188301 adaux-2.6.0/source/adaux/src/docker/services/pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.188301 adaux-2.6.0/source/adaux/src/docker/services/pytest-standalone/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.192302 adaux-2.6.0/source/adaux/src/docker/services/python-deps/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.192302 adaux-2.6.0/source/adaux/src/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docs/default_conf.py.jinja2
+-rwxrwxrwx   0 root         (0) root         (0)     1873 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docs/postprocess_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.192302 adaux-2.6.0/source/adaux/src/docs/static/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docs/static/git-link-color.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.196302 adaux-2.6.0/source/adaux/src/docs/user/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docs/user/conf.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docs/user/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/docs/user/index.rst.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/gitignore
+-rwxrwxrwx   0 root         (0) root         (0)      410 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/install-dev.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.196302 adaux-2.6.0/source/adaux/src/license/
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/license/Apache-2.0.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/license/BSD-3_clause.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/license/MIT.txt.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.108298 adaux-2.6.0/source/adaux/src/payload/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.200302 adaux-2.6.0/source/adaux/src/payload/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.200302 adaux-2.6.0/source/adaux/src/payload/python/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-07-06 21:05:33.000000 adaux-2.6.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/payload/python/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.200302 adaux-2.6.0/source/adaux/src/pip/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/pip/pip.conf.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.204302 adaux-2.6.0/source/adaux/src/pre-commit/
+-rwxrwxrwx   0 root         (0) root         (0)     1680 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     5098 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/pre-commit/config.yaml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/pre-commit/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.204302 adaux-2.6.0/source/adaux/src/root/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/root/_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/root/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/root/setup.cfg.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.208302 adaux-2.6.0/source/adaux/src/root/source/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/root/source/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-09 07:59:41.000000 adaux-2.6.0/source/adaux/src/temp-combination
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:06:29.128299 adaux-2.6.0/source/adaux.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-06 21:06:28.000000 adaux-2.6.0/source/adaux.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5451 2023-07-06 21:06:29.000000 adaux-2.6.0/source/adaux.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 21:06:28.000000 adaux-2.6.0/source/adaux.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-06 21:06:28.000000 adaux-2.6.0/source/adaux.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 21:05:32.000000 adaux-2.6.0/source/adaux.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-06 21:06:28.000000 adaux-2.6.0/source/adaux.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-06 21:06:28.000000 adaux-2.6.0/source/adaux.egg-info/top_level.txt
```

### Comparing `adaux-2.5.0/LICENSE.txt` & `adaux-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/setup.cfg` & `adaux-2.6.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 	src/*
 	src/*/*
 	src/*/*/*
 	src/*/*/*/*
 
 [options.extras_require]
 dev = 
-	pre-commit>=2.20
-	mypy>=1.1.1
+	pre-commit>=3.3.3
+	mypy>=1.4.1
 	types-requests
 test = 
-	pytest>=7.2
+	pytest>=7.4
 	pytest-cov~=4.0
 
 [tool:pytest]
 markers = 
 	merge_only: run test only on merge request
 	local: run local tests that need docker
 addopts = --strict-markers -m "not merge_only and not local"
```

### Comparing `adaux-2.5.0/source/adaux/_base_parser.py` & `adaux-2.6.0/source/adaux/_base_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_cli.py` & `adaux-2.6.0/source/adaux/_cli.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_cli_mixin.py` & `adaux-2.6.0/source/adaux/_cli_mixin.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_01_file_io_support.py` & `adaux-2.6.0/source/adaux/_components/_01_file_io_support.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_02_base.py` & `adaux-2.6.0/source/adaux/_components/_02_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 from ._01_file_io_support import FileIOSupport
 
 
 class BaseComponent(FileIOSupport):
     def __init__(self) -> None:
         super().__init__()
         self.versions = _ProtoNamespace(
-            pytest="pytest>=7.2",
+            pytest="pytest>=7.4",
             pytest_cov="pytest-cov~=4.0",
-            pre_commit="pre-commit>=2.20",
-            mypy="mypy==1.1.1",
-            pylint="pylint==2.17.1",
-            black="black==23.1.0",
-            sphinx="sphinx>=5.3.0",
-            sphinx_rtd_theme="sphinx-rtd-theme>=1.0.0",
-            sphinx_click="sphinx-click>=4.3",
+            pre_commit="pre-commit>=3.3.3",
+            mypy="mypy==1.4.1",
+            pylint="pylint==2.17.4",
+            black="black==23.3.0",
+            sphinx="sphinx==6.2.1",  # rtd-theme forces sphinx <7
+            sphinx_rtd_theme="sphinx-rtd-theme>=1.2.2",
+            sphinx_click="sphinx-click>=4.4.0",
             jupyter_sphinx="jupyter-sphinx>=0.4",
             bash_kernel="bash_kernel>=0.8",
-            blacken_docs="blacken-docs==v1.12.1",
+            blacken_docs="blacken-docs==1.14.0",
             pre_commit_hooks="pre-commit-hooks==v4.4.0",
-            pyupgrade="pyupgrade==v3.3.1",
-            pycln="pycln==v2.1.3",
-            reorder_python_imports="reorder_python_imports==v3.9.0",
+            pyupgrade="pyupgrade==v3.8.0",
+            pycln="pycln==v2.1.5",
+            reorder_python_imports="reorder_python_imports==v3.10.0",
             isort="isort==5.12.0",
             encryption_check="encryption_check==v1.0.0",
-            docstr_coverage="docstr-coverage==v2.2.0",
-            requests="requests==2.28.2",
+            docstr_coverage="docstr-coverage==v2.3.0",
+            requests="requests==2.31.0",
             types_requests="types-requests",
             adaux=f"adaux=={LazyVersionStr()}",
             docker_compose_file="3.8",
             ci_docker_image="docker:20.10.23",
             ci_adaux_image=f"prostructura/adaux:{LazyVersionStr()}",
         )
         self.auxcon = _ProtoNamespace()
```

### Comparing `adaux-2.5.0/source/adaux/_components/_03_meta.py` & `adaux-2.6.0/source/adaux/_components/_03_meta.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_04_monotonic_version.py` & `adaux-2.6.0/source/adaux/_components/_04_monotonic_version.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_05_project.py` & `adaux-2.6.0/source/adaux/_components/_05_project.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_06_dependency.py` & `adaux-2.6.0/source/adaux/_components/_06_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_07_package.py` & `adaux-2.6.0/source/adaux/_components/_07_package.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_08_pip.py` & `adaux-2.6.0/source/adaux/_components/_08_pip.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_09_gitignore.py` & `adaux-2.6.0/source/adaux/_components/_09_gitignore.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_10_gitlab.py` & `adaux-2.6.0/source/adaux/_components/_10_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_11_precommit.py` & `adaux-2.6.0/source/adaux/_components/_11_precommit.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_12_pylint.py` & `adaux-2.6.0/source/adaux/_components/_12_pylint.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_13_executable.py` & `adaux-2.6.0/source/adaux/_components/_13_executable.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_14_mypy.py` & `adaux-2.6.0/source/adaux/_components/_14_mypy.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_15_pytest.py` & `adaux-2.6.0/source/adaux/_components/_15_pytest.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_17_docs.py` & `adaux-2.6.0/source/adaux/_components/_17_docs.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_18_payload.py` & `adaux-2.6.0/source/adaux/_components/_18_payload.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_19_docker.py` & `adaux-2.6.0/source/adaux/_components/_19_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_20_ci.py` & `adaux-2.6.0/source/adaux/_components/_20_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_98_sentinel.py` & `adaux-2.6.0/source/adaux/_components/_98_sentinel.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_99_all.py` & `adaux-2.6.0/source/adaux/_components/_99_all.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_aux_ci.py` & `adaux-2.6.0/source/adaux/_components/_aux_ci.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         elif self.status == StateEnum.SUCCESS:
             col = 2
         elif self.status == StateEnum.SKIPPED:
             col = 3
         elif self.status == StateEnum.UP_TO_DATE:
             col = 6
         else:
-            return self.status.value
+            return str(self.status.value)
         return f"\033[1;3{col}m{self.status.value}\033[0m"
 
 
 @dc.dataclass(frozen=True)
 class DoubleLinkedListNode(Job):  # pylint: disable=abstract-method
     state: State = dc.field(default_factory=State)
     children: tp.List["DoubleLinkedListNode"] = dc.field(default_factory=list)
```

### Comparing `adaux-2.5.0/source/adaux/_components/_payload/__init__.py` & `adaux-2.6.0/source/adaux/_components/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_payload/_base.py` & `adaux-2.6.0/source/adaux/_components/_payload/_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_payload/_docker.py` & `adaux-2.6.0/source/adaux/_components/_payload/_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_payload/_docker_build.py` & `adaux-2.6.0/source/adaux/_components/_payload/_docker_build.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_payload/_docker_executors.py` & `adaux-2.6.0/source/adaux/_components/_payload/_docker_executors.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_payload/_docker_run.py` & `adaux-2.6.0/source/adaux/_components/_payload/_docker_run.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_payload/_python.py` & `adaux-2.6.0/source/adaux/_components/_payload/_python.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_components/_payload/_with_dependency.py` & `adaux-2.6.0/source/adaux/_components/_payload/_with_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_create_badge.py` & `adaux-2.6.0/source/adaux/_create_badge.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_gitlab.py` & `adaux-2.6.0/source/adaux/_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_parser.py` & `adaux-2.6.0/source/adaux/_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_proto_namespace.py` & `adaux-2.6.0/source/adaux/_proto_namespace.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_tick.py` & `adaux-2.6.0/source/adaux/_tick.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_todo.py` & `adaux-2.6.0/source/adaux/_todo.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/_util.py` & `adaux-2.6.0/source/adaux/_util.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/CI/00-main.yml.jinja2` & `adaux-2.6.0/source/adaux/src/CI/00-main.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/CI/01-rules.yml.jinja2` & `adaux-2.6.0/source/adaux/src/CI/01-rules.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/image/Dockerfile.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/image/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2` & `adaux-2.6.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docs/default_conf.py.jinja2` & `adaux-2.6.0/source/adaux/src/docs/default_conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/docs/postprocess_html.py` & `adaux-2.6.0/source/adaux/src/docs/postprocess_html.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/license/Apache-2.0.txt.jinja2` & `adaux-2.6.0/source/adaux/src/license/Apache-2.0.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/license/BSD-3_clause.txt.jinja2` & `adaux-2.6.0/source/adaux/src/license/BSD-3_clause.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/license/MIT.txt.jinja2` & `adaux-2.6.0/source/adaux/src/license/MIT.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc` & `adaux-2.6.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/payload/python/functions.py` & `adaux-2.6.0/source/adaux/src/payload/python/functions.py`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2` & `adaux-2.6.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux/src/pre-commit/config.yaml.jinja2` & `adaux-2.6.0/source/adaux/src/pre-commit/config.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.5.0/source/adaux.egg-info/SOURCES.txt` & `adaux-2.6.0/source/adaux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

