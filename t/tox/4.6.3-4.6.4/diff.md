# Comparing `tmp/tox-4.6.3.tar.gz` & `tmp/tox-4.6.4.tar.gz`

## Comparing `tox-4.6.3.tar` & `tox-4.6.4.tar`

### file list

```diff
@@ -1,221 +1,221 @@
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 tox-4.6.3/tox.ini
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/__main__.py
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/provision.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/py.typed
--rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/pytest.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/report.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/run.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/__init__.py
--rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/main.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/of_type.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/set_env.py
--rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/sets.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/cli/__init__.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/cli/env_var.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/cli/ini.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/cli/parse.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/cli/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/__init__.py
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/api.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/convert.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/memory.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/section.py
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/str_convert.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/stringify.py
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/ini/__init__.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/ini/factor.py
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/ini/replace.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/__init__.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/api.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/discover.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/ini.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/ini_section.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/legacy_toml.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/setup_cfg.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/tox_ini.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/__init__.py
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/api.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/pep517_backend.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/request.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/stream.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/util.py
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/local_sub_process/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread_unix.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread_windows.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/journal/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/journal/env.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/journal/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/plugin/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/plugin/inline.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/plugin/manager.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/plugin/spec.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/__init__.py
--rw-r--r--   0        0        0    18474 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/env_select.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/depends.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/devenv.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/exec_.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/legacy.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/list_env.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/quickstart.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/show_config.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/version_flag.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/run/__init__.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/run/common.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/run/parallel.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/run/sequential.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/run/single.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/__init__.py
--rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/api.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/errors.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/info.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/installer.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/package.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/register.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/runner.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/__init__.py
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/api.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/package.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/__init__.py
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/pip_install.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/req_file.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/req/__init__.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/req/args.py
--rw-r--r--   0        0        0    19762 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/req/file.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/req/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/api.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
--rw-r--r--   0        0        0    18379 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/package/pyproject.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/package/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/ci.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/cpu.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/file_view.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/graph.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/path.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/spinner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/__init__.py
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tox-4.6.3/tests/conftest.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.6.3/tests/test_call_modes.py
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 tox-4.6.3/tests/test_provision.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.6.3/tests/test_report.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.6.3/tests/test_run.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.3/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/__init__.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/conftest.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/test_main.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/test_of_types.py
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/test_set_env.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/test_sets.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/conftest.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/test_cli_env_var.py
--rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/test_cli_ini.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/test_parse.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/test_loader.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/test_memory_loader.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/test_section.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/test_str_convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/__init__.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/conftest.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/test_factor.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/test_ini_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/__init__.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/conftest.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_env_var.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_os_pathsep.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_os_sep.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_posargs.py
--rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_tox_env.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_tty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/source/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/source/test_discover.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/source/test_legacy_toml.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/source/test_setup_cfg.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/source/test_source_ini.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 tox-4.6.3/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.6.3/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.6.3/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.6.3/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.6.3/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/conftest.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/test_request.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/test_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/__init__.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/bad_process.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/local_subprocess_sigint.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/test_execute_util.py
--rw-r--r--   0        0        0    14176 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/test_local_subprocess.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/tty_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/journal/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.6.3/tests/journal/test_main_journal.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.6.3/tests/plugin/conftest.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.6.3/tests/plugin/test_inline.py
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 tox-4.6.3/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.6.3/tests/plugin/test_plugin_custom_config_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/pytest_/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.6.3/tests/pytest_/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/__init__.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/test_env_select.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/test_session_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/__init__.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_depends.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_devenv.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_exec_.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_legacy.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_list_envs.py
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_parallel.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_quickstart.py
--rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_sequential.py
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_show_config.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/run/__init__.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/run/test_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/test_api.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/test_info.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/test_register.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/test_tox_env_api.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/test_tox_env_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/__init__.py
--rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/test_python_api.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/test_python_runner.py
--rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/pip/test_pip_install.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/pip/test_req_file.py
--rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/pip/req/test_file.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/test-pkg/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/test_setuptools.py
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/test_virtualenv_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/package/conftest.py
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
--rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/package/test_python_package_util.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.6.3/tests/type_check/add_config_container_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/__init__.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/test_ci.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/test_cpu.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/test_graph.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/test_path.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/test_spinner.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.3/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.6.3/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.6.3/README.md
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 tox-4.6.3/pyproject.toml
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tox-4.6.3/PKG-INFO
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tox-4.6.4/tox.ini
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/__main__.py
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/provision.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/py.typed
+-rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/pytest.py
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/report.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/run.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/__init__.py
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/main.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/of_type.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/set_env.py
+-rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/sets.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/cli/__init__.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/cli/env_var.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/cli/ini.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/cli/parse.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/cli/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/__init__.py
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/api.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/convert.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/memory.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/section.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/str_convert.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/stringify.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/ini/factor.py
+-rw-r--r--   0        0        0    13368 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/ini/replace.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/__init__.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/api.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/discover.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/ini.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/ini_section.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/legacy_toml.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/setup_cfg.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/tox_ini.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/__init__.py
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/api.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/pep517_backend.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/request.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/stream.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/util.py
+-rw-r--r--   0        0        0    14203 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/local_sub_process/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread_unix.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread_windows.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/journal/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/journal/env.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/journal/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/plugin/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/plugin/inline.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/plugin/manager.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/plugin/spec.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/__init__.py
+-rw-r--r--   0        0        0    18458 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/env_select.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/depends.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/devenv.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/exec_.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/legacy.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/list_env.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/quickstart.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/show_config.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/version_flag.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/run/common.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/run/parallel.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/run/sequential.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/run/single.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/__init__.py
+-rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/api.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/errors.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/info.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/installer.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/package.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/register.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/runner.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/api.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/package.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/__init__.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/pip_install.py
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/req_file.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/req/__init__.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/req/args.py
+-rw-r--r--   0        0        0    19702 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/req/file.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/req/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/api.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
+-rw-r--r--   0        0        0    18379 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/package/pyproject.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/package/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/ci.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/cpu.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/file_view.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/graph.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/path.py
+-rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/spinner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/__init__.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tox-4.6.4/tests/conftest.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.6.4/tests/test_call_modes.py
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 tox-4.6.4/tests/test_provision.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.6.4/tests/test_report.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.6.4/tests/test_run.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.4/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/conftest.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/test_main.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/test_of_types.py
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/test_set_env.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/test_sets.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/conftest.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/test_cli_env_var.py
+-rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/test_cli_ini.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/test_parse.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/test_loader.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/test_memory_loader.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/test_section.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/test_str_convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/conftest.py
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/test_factor.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/test_ini_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/__init__.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/conftest.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace.py
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_env_var.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_os_pathsep.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_os_sep.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_posargs.py
+-rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_tox_env.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_tty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/source/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/source/test_discover.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/source/test_legacy_toml.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/source/test_setup_cfg.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/source/test_source_ini.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 tox-4.6.4/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.6.4/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.6.4/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.6.4/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.6.4/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/conftest.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/test_request.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/test_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/__init__.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/bad_process.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/local_subprocess_sigint.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/test_execute_util.py
+-rw-r--r--   0        0        0    14176 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/test_local_subprocess.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/tty_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/journal/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.6.4/tests/journal/test_main_journal.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.6.4/tests/plugin/conftest.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.6.4/tests/plugin/test_inline.py
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 tox-4.6.4/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.6.4/tests/plugin/test_plugin_custom_config_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/pytest_/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.6.4/tests/pytest_/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/__init__.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/test_env_select.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/test_session_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_depends.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_devenv.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_exec_.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_legacy.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_list_envs.py
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_parallel.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_quickstart.py
+-rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_sequential.py
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_show_config.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/run/test_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/test_api.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/test_info.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/test_register.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/test_tox_env_api.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/test_tox_env_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/__init__.py
+-rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/test_python_api.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/test_python_runner.py
+-rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/pip/test_pip_install.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/pip/test_req_file.py
+-rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/pip/req/test_file.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/test-pkg/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/test_setuptools.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/test_virtualenv_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/package/conftest.py
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
+-rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/package/test_python_package_util.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.6.4/tests/type_check/add_config_container_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/__init__.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/test_ci.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/test_cpu.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/test_graph.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/test_path.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/test_spinner.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.4/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.6.4/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.6.4/README.md
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 tox-4.6.4/pyproject.toml
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 tox-4.6.4/PKG-INFO
```

### Comparing `tox-4.6.3/tox.ini` & `tox-4.6.4/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -48,27 +48,28 @@
 commands =
     pre-commit run --all-files --show-diff-on-failure {posargs}
     python -c 'print(r"hint: run {envbindir}{/}pre-commit install to add checks as pre-commit hook")'
 
 [testenv:type]
 description = run type check on code base
 deps =
-    mypy==1.3
+    mypy==1.4.1
     types-cachetools>=5.3.0.5
     types-chardet>=5.0.4.6
 commands =
     mypy src/tox
     mypy tests
 
 [testenv:docs]
 description = build documentation
 extras =
     docs
 commands =
-    sphinx-build -d "{envtmpdir}{/}doctree" docs "{toxworkdir}{/}docs_out" --color -b html {posargs:-b linkcheck -W}
+    {posargs: sphinx-build -d "{envtmpdir}{/}doctree" docs "{toxworkdir}{/}docs_out" --color -b linkcheck}
+    sphinx-build -d "{envtmpdir}{/}doctree" docs "{toxworkdir}{/}docs_out" --color -b html -W
     python -c 'print(r"documentation available under file://{toxworkdir}{/}docs_out{/}index.html")'
 
 [testenv:pkg_meta]
 description = check that the long description is valid
 skip_install = true
 deps =
     build[virtualenv]>=0.10
```

### Comparing `tox-4.6.3/src/tox/provision.py` & `tox-4.6.4/src/tox/provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/pytest.py` & `tox-4.6.4/src/tox/pytest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/report.py` & `tox-4.6.4/src/tox/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import os
 import sys
 from contextlib import contextmanager
 from io import BytesIO, TextIOWrapper
 from pathlib import Path
 from threading import Thread, current_thread, enumerate, local
-from typing import IO, Iterator, Tuple
+from typing import IO, ClassVar, Iterator, Tuple
 
 from colorama import Fore, Style, init
 
 LEVELS = {
     0: logging.CRITICAL,
     1: logging.ERROR,
     2: logging.WARNING,
@@ -25,15 +25,15 @@
 LOGGER = logging.getLogger()
 OutErr = Tuple[TextIOWrapper, TextIOWrapper]
 
 
 class _LogThreadLocal(local):
     """A thread local variable that inherits values from its parent."""
 
-    _ident_to_data: dict[int | None, str] = {}
+    _ident_to_data: ClassVar[dict[int | None, str]] = {}
 
     def __init__(self, out_err: OutErr) -> None:
         self.name = self._ident_to_data.get(getattr(current_thread(), "parent_ident", None), "ROOT")
         self.out_err = out_err
 
     @staticmethod
     @contextmanager
```

### Comparing `tox-4.6.3/src/tox/run.py` & `tox-4.6.4/src/tox/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     state = setup_state(args)
     from tox.provision import provision
 
     result = provision(state)
     if result is not False:
         return result
     handler = state._options.cmd_handlers[state.conf.options.command]  # noqa: SLF001
-    result = handler(state)
-    return result
+    return handler(state)
 
 
 def setup_state(args: Sequence[str]) -> State:
     """Setup the state object of this run."""
     start = time.monotonic()
     # parse CLI arguments
     options = get_options(*args)
```

### Comparing `tox-4.6.3/src/tox/config/main.py` & `tox-4.6.4/src/tox/config/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/of_type.py` & `tox-4.6.4/src/tox/config/of_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     def __init__(  # noqa: PLR0913
         self,
         keys: Iterable[str],
         desc: str,
         of_type: type[T],
         default: Callable[[Config, str | None], T] | T,
         post_process: Callable[[T], T] | None = None,
-        factory: Factory[T] = None,
+        factory: Factory[T] | None = None,
     ) -> None:
         super().__init__(keys, desc)
         self.of_type = of_type
         self.default = default
         self.post_process = post_process
         self.factory = factory
         self._cache: object | T = _PLACE_HOLDER
```

### Comparing `tox-4.6.3/src/tox/config/set_env.py` & `tox-4.6.4/src/tox/config/set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/sets.py` & `tox-4.6.4/src/tox/config/sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def add_config(  # noqa: PLR0913
         self,
         keys: str | Sequence[str],
         of_type: type[V],
         default: Callable[[Config, str | None], V] | V,
         desc: str,
         post_process: Callable[[V], V] | None = None,
-        factory: Factory[Any] = None,
+        factory: Factory[Any] | None = None,
     ) -> ConfigDynamicDefinition[V]:
         """
         Add configuration value.
 
         :param keys: the keys under what to register the config (first is primary key)
         :param of_type: the type of the config value
         :param default: the default value of the config value
```

### Comparing `tox-4.6.3/src/tox/config/types.py` & `tox-4.6.4/src/tox/config/types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/cli/env_var.py` & `tox-4.6.4/src/tox/config/cli/env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/cli/ini.py` & `tox-4.6.4/src/tox/config/cli/ini.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Provides configuration values from tox.ini files."""
 from __future__ import annotations
 
 import logging
 import os
 from configparser import ConfigParser
 from pathlib import Path
-from typing import Any
+from typing import Any, ClassVar
 
 from platformdirs import user_config_dir
 
 from tox.config.loader.api import ConfigLoadArgs
 from tox.config.loader.ini import IniLoader
 from tox.config.source.ini_section import CORE
 
 DEFAULT_CONFIG_FILE = Path(user_config_dir("tox")) / "config.ini"
 
 
 class IniConfig:
     TOX_CONFIG_FILE_ENV_VAR = "TOX_USER_CONFIG_FILE"
-    STATE = {None: "failed to parse", True: "active", False: "missing"}
+    STATE: ClassVar[dict[bool | None, str]] = {None: "failed to parse", True: "active", False: "missing"}
 
     def __init__(self) -> None:
         config_file = os.environ.get(self.TOX_CONFIG_FILE_ENV_VAR, None)
         self.is_env_var = config_file is not None
         self.config_file = Path(config_file if config_file is not None else DEFAULT_CONFIG_FILE)
         self._cache: dict[tuple[str, type[Any]], Any] = {}
         self.has_config_file: bool | None = self.config_file.exists()
```

### Comparing `tox-4.6.3/src/tox/config/cli/parse.py` & `tox-4.6.4/src/tox/config/cli/parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/cli/parser.py` & `tox-4.6.4/src/tox/config/cli/parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/loader/api.py` & `tox-4.6.4/src/tox/config/loader/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/loader/convert.py` & `tox-4.6.4/src/tox/config/loader/convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/loader/memory.py` & `tox-4.6.4/src/tox/config/loader/memory.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/loader/section.py` & `tox-4.6.4/src/tox/config/loader/section.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         return self.key
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(prefix={self._prefix!r}, name={self._name!r})"
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, self.__class__) and (self._prefix, self._name) == (
-            other._prefix,  # noqa: SLF001
+            other._prefix,
             other.name,
         )
 
 
 __all__ = [
     "Section",
 ]
```

### Comparing `tox-4.6.3/src/tox/config/loader/str_convert.py` & `tox-4.6.4/src/tox/config/loader/str_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Convert string configuration values to tox python configuration objects."""
 from __future__ import annotations
 
 import shlex
 import sys
 from itertools import chain
 from pathlib import Path
-from typing import Any, Iterator
+from typing import TYPE_CHECKING, Any, Iterator
 
 from tox.config.loader.convert import Convert
 from tox.config.types import Command, EnvList
 
+if TYPE_CHECKING:
+    from typing import Final
+
 
 class StrConvert(Convert[str]):
     """A class converting string values to tox types."""
 
     @staticmethod
     def to_str(value: str) -> str:
         return str(value).strip()
@@ -107,16 +110,16 @@
     @staticmethod
     def to_env_list(value: str) -> EnvList:
         from tox.config.loader.ini.factor import extend_factors
 
         elements = list(chain.from_iterable(extend_factors(expr) for expr in value.split("\n")))
         return EnvList(elements)
 
-    TRUTHFUL_VALUES = {"true", "1", "yes", "on"}
-    FALSE_VALUES = {"false", "0", "no", "off", ""}
+    TRUTHFUL_VALUES: Final[set[str]] = {"true", "1", "yes", "on"}
+    FALSE_VALUES: Final[set[str]] = {"false", "0", "no", "off", ""}
     VALID_BOOL = sorted(TRUTHFUL_VALUES | FALSE_VALUES)
 
     @staticmethod
     def to_bool(value: str) -> bool:
         norm = str(value).strip().lower()
         if norm in StrConvert.TRUTHFUL_VALUES:
             return True
```

### Comparing `tox-4.6.3/src/tox/config/loader/stringify.py` & `tox-4.6.4/src/tox/config/loader/stringify.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/loader/ini/__init__.py` & `tox-4.6.4/src/tox/config/loader/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/loader/ini/factor.py` & `tox-4.6.4/src/tox/config/loader/ini/factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/loader/ini/replace.py` & `tox-4.6.4/src/tox/config/loader/ini/replace.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,16 +255,15 @@
                     if isinstance(src, SectionProxy):
                         return loader.process_raw(conf, conf_args.env_name, src[key])
                     value = src.load(key, conf_args.chain)
                 except KeyError as exc:  # if fails, keep trying maybe another source can satisfy
                     exception = exc
                 else:
                     as_str, _ = stringify(value)
-                    as_str = as_str.replace("#", r"\#")  # escape comment characters as these will be stripped
-                    return as_str
+                    return as_str.replace("#", r"\#")  # escape comment characters as these will be stripped
         except Exception as exc:  # noqa: BLE001
             exception = exc
         if exception is not None:
             if isinstance(exception, KeyError):  # if the lookup failed replace - else keep
                 default = settings["default"]
                 if default is not None:
                     return default
```

### Comparing `tox-4.6.3/src/tox/config/source/api.py` & `tox-4.6.4/src/tox/config/source/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/source/discover.py` & `tox-4.6.4/src/tox/config/source/discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/source/ini.py` & `tox-4.6.4/src/tox/config/source/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/source/ini_section.py` & `tox-4.6.4/src/tox/config/source/ini_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/source/legacy_toml.py` & `tox-4.6.4/src/tox/config/source/legacy_toml.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/config/source/setup_cfg.py` & `tox-4.6.4/src/tox/config/source/setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/execute/api.py` & `tox-4.6.4/src/tox/execute/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/execute/pep517_backend.py` & `tox-4.6.4/src/tox/execute/pep517_backend.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/execute/request.py` & `tox-4.6.4/src/tox/execute/request.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/execute/stream.py` & `tox-4.6.4/src/tox/execute/stream.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/execute/util.py` & `tox-4.6.4/src/tox/execute/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/execute/local_sub_process/__init__.py` & `tox-4.6.4/src/tox/execute/local_sub_process/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     def __init__(self, options: ExecuteOptions, out: SyncWrite, err: SyncWrite, process: Popen[bytes]) -> None:
         self._process: Popen[bytes] = process
         super().__init__(options, out, err)
         self._interrupted = False
 
     @property
     def exit_code(self) -> int | None:
+        # need to poll here, to make sure the returncode we get is current
+        self._process.poll()
         return self._process.returncode
 
     def interrupt(self) -> None:
         self._interrupted = True
         if self._process is not None:  # pragma: no branch
             # A three level stop mechanism for children - INT -> TERM -> KILL
             # communicate will wait for the app to stop, and then drain the standard streams and close them
```

### Comparing `tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread.py` & `tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread_unix.py` & `tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread_unix.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread_windows.py` & `tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread_windows.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/journal/env.py` & `tox-4.6.4/src/tox/journal/env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/journal/main.py` & `tox-4.6.4/src/tox/journal/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/plugin/__init__.py` & `tox-4.6.4/src/tox/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/plugin/inline.py` & `tox-4.6.4/src/tox/plugin/inline.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,11 +23,10 @@
     in_folder = path.parent
     module_name = path.stem
 
     sys.path.insert(0, str(in_folder))
     try:
         if module_name in sys.modules:
             del sys.modules[module_name]  # pragma: no cover
-        module = importlib.import_module(module_name)
-        return module
+        return importlib.import_module(module_name)
     finally:
         del sys.path[0]
```

### Comparing `tox-4.6.3/src/tox/plugin/manager.py` & `tox-4.6.4/src/tox/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/plugin/spec.py` & `tox-4.6.4/src/tox/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/env_select.py` & `tox-4.6.4/src/tox/session/env_select.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def __str__(self) -> str:
         return "ALL" if self.is_all else ("<env_list>" if self.is_default_list else ",".join(self))
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({'' if self.is_default_list else repr(str(self))})"
 
     def __eq__(self, other: Any) -> bool:
-        return type(self) == type(other) and self._names == other._names  # noqa: SLF001
+        return type(self) == type(other) and self._names == other._names
 
     def __ne__(self, other: Any) -> bool:
         return not (self == other)
 
     @property
     def is_all(self) -> bool:
         return self._names is not None and "ALL" in self._names
```

### Comparing `tox-4.6.3/src/tox/session/state.py` & `tox-4.6.4/src/tox/session/state.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/depends.py` & `tox-4.6.4/src/tox/session/cmd/depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/devenv.py` & `tox-4.6.4/src/tox/session/cmd/devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/exec_.py` & `tox-4.6.4/src/tox/session/cmd/exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/legacy.py` & `tox-4.6.4/src/tox/session/cmd/legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/list_env.py` & `tox-4.6.4/src/tox/session/cmd/list_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/quickstart.py` & `tox-4.6.4/src/tox/session/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/show_config.py` & `tox-4.6.4/src/tox/session/cmd/show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/version_flag.py` & `tox-4.6.4/src/tox/session/cmd/version_flag.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/run/common.py` & `tox-4.6.4/src/tox/session/cmd/run/common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/run/parallel.py` & `tox-4.6.4/src/tox/session/cmd/run/parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/run/sequential.py` & `tox-4.6.4/src/tox/session/cmd/run/sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/session/cmd/run/single.py` & `tox-4.6.4/src/tox/session/cmd/run/single.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/api.py` & `tox-4.6.4/src/tox/tox_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/info.py` & `tox-4.6.4/src/tox/tox_env/info.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/installer.py` & `tox-4.6.4/src/tox/tox_env/installer.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/package.py` & `tox-4.6.4/src/tox/tox_env/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/register.py` & `tox-4.6.4/src/tox/tox_env/register.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/runner.py` & `tox-4.6.4/src/tox/tox_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/util.py` & `tox-4.6.4/src/tox/tox_env/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/python/api.py` & `tox-4.6.4/src/tox/tox_env/python/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/python/package.py` & `tox-4.6.4/src/tox/tox_env/python/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/python/runner.py` & `tox-4.6.4/src/tox/tox_env/python/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/python/pip/pip_install.py` & `tox-4.6.4/src/tox/tox_env/python/pip/pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/python/pip/req_file.py` & `tox-4.6.4/src/tox/tox_env/python/pip/req_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from typing import TYPE_CHECKING
 
 from .req.file import ParsedRequirement, ReqFileLines, RequirementsFile
 
 if TYPE_CHECKING:
     from argparse import ArgumentParser, Namespace
     from pathlib import Path
+    from typing import Final
 
 
 class PythonDeps(RequirementsFile):
     # these options are valid in requirements.txt, but not via pip cli and
     # thus cannot be used in the testenv `deps` list
-    _illegal_options = ["hash"]
+    _illegal_options: Final[list[str]] = ["hash"]
 
     def __init__(self, raw: str, root: Path) -> None:
         super().__init__(root / "tox.ini", constraint=False)
         self._raw = self._normalize_raw(raw)
         self._unroll: tuple[list[str], list[str]] | None = None
         self._req_parser_: RequirementsFile | None = None
 
@@ -66,16 +67,15 @@
         # ignored
         raw = "".join(raw.replace("\r", "").split("\\\n"))
         lines: list[str] = []
         for line in raw.splitlines():
             # for tox<4 supporting requirement/constraint files via -rreq.txt/-creq.txt
             lines.append(PythonDeps._normalize_line(line))
         adjusted = "\n".join(lines)
-        raw = f"{adjusted}\n" if raw.endswith("\\\n") else adjusted  # preserve trailing newline if input has it
-        return raw
+        return f"{adjusted}\n" if raw.endswith("\\\n") else adjusted  # preserve trailing newline if input has it
 
     @staticmethod
     def _normalize_line(line: str) -> str:
         arg_match = next(
             (
                 arg
                 for arg in ONE_ARG
```

### Comparing `tox-4.6.3/src/tox/tox_env/python/pip/req/args.py` & `tox-4.6.4/src/tox/tox_env/python/pip/req/args.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/python/pip/req/file.py` & `tox-4.6.4/src/tox/tox_env/python/pip/req/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,16 +242,15 @@
         Content is unicode. Respects # -*- coding: declarations on the retrieved files.
 
         :param url:         File path or url.
         """
         scheme = get_url_scheme(url)
         if scheme in ["http", "https"]:
             with urlopen(url) as response:  # noqa: S310
-                text = self._read_decode(response)
-                return text
+                return self._read_decode(response)
         elif scheme == "file":
             url = url_to_path(url)
         try:
             with Path(url).open("rb") as file_handler:
                 text = self._read_decode(file_handler)
         except OSError as exc:
             msg = f"Could not open requirements file {url}: {exc}"
@@ -271,16 +270,15 @@
         Split, filter, and join lines, and return a line iterator.
 
         :param content: the content of the requirements file
         """
         lines_enum: ReqFileLines = enumerate(content.splitlines(), start=1)
         lines_enum = self._join_lines(lines_enum)
         lines_enum = self._ignore_comments(lines_enum)
-        lines_enum = self._expand_env_variables(lines_enum)
-        return lines_enum
+        return self._expand_env_variables(lines_enum)
 
     def _parse_line(self, line: str) -> tuple[str, Namespace]:
         args_str, options_str = self._break_args_options(line)
         args = shlex.split(options_str, posix=sys.platform != "win32")
         opts = self._parser.parse_args(args)
         return args_str, opts
```

### Comparing `tox-4.6.3/src/tox/tox_env/python/pip/req/util.py` & `tox-4.6.4/src/tox/tox_env/python/pip/req/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 def url_to_path(url: str) -> str:
     _, netloc, path, _, _ = urlsplit(url)
     if not netloc or netloc == "localhost":  # According to RFC 8089, same as empty authority.
         netloc = ""
     else:
         msg = f"non-local file URIs are not supported on this platform: {url!r}"
         raise ValueError(msg)
-    path = url2pathname(netloc + path)
-    return path
+    return url2pathname(netloc + path)
 
 
 def handle_binary_option(value: str, target: set[str], other: set[str]) -> None:
     new = value.split(",")
     while ":all:" in new:
         other.clear()
         target.clear()
```

### Comparing `tox-4.6.3/src/tox/tox_env/python/virtual_env/api.py` & `tox-4.6.4/src/tox/tox_env/python/virtual_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/python/virtual_env/runner.py` & `tox-4.6.4/src/tox/tox_env/python/virtual_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/python/virtual_env/package/cmd_builder.py` & `tox-4.6.4/src/tox/tox_env/python/virtual_env/package/cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/python/virtual_env/package/pyproject.py` & `tox-4.6.4/src/tox/tox_env/python/virtual_env/package/pyproject.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/tox_env/python/virtual_env/package/util.py` & `tox-4.6.4/src/tox/tox_env/python/virtual_env/package/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/util/ci.py` & `tox-4.6.4/src/tox/util/ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/util/file_view.py` & `tox-4.6.4/src/tox/util/file_view.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/util/graph.py` & `tox-4.6.4/src/tox/util/graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/util/path.py` & `tox-4.6.4/src/tox/util/path.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/src/tox/util/spinner.py` & `tox-4.6.4/src/tox/util/spinner.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from collections import OrderedDict
 from typing import IO, TYPE_CHECKING, NamedTuple, Sequence, TypeVar
 
 from colorama import Fore
 
 if TYPE_CHECKING:
     from types import TracebackType
+    from typing import Any, ClassVar
 
 if sys.platform == "win32":  # pragma: win32 cover
     import ctypes
 
     class _CursorInfo(ctypes.Structure):
-        _fields_ = [("size", ctypes.c_int), ("visible", ctypes.c_byte)]
+        _fields_: ClassVar[list[tuple[str, Any]]] = [("size", ctypes.c_int), ("visible", ctypes.c_byte)]
 
 
 def _file_support_encoding(chars: Sequence[str], file: IO[str]) -> bool:
     encoding = getattr(file, "encoding", None)
     if encoding is not None:  # pragma: no branch  # this should be always set, unless someone passes in something bad
         for char in chars:
             try:
@@ -43,16 +44,16 @@
     fail: str
     skip: str
 
 
 class Spinner:
     CLEAR_LINE = "\033[K"
     max_width = 120
-    UNICODE_FRAMES = ["⠋", "⠙", "⠹", "⠸", "⠼", "⠴", "⠦", "⠧", "⠇", "⠏"]
-    ASCII_FRAMES = ["|", "-", "+", "x", "*"]
+    UNICODE_FRAMES: ClassVar[list[str]] = ["⠋", "⠙", "⠹", "⠸", "⠼", "⠴", "⠦", "⠧", "⠇", "⠏"]
+    ASCII_FRAMES: ClassVar[list[str]] = ["|", "-", "+", "x", "*"]
     UNICODE_OUTCOME = Outcome(ok="✔", fail="✖", skip="⚠")
     ASCII_OUTCOME = Outcome(ok="+", fail="!", skip="?")
 
     def __init__(  # noqa: PLR0913
         self,
         enabled: bool = True,  # noqa: FBT001, FBT002
         refresh_rate: float = 0.1,
```

### Comparing `tox-4.6.3/tests/conftest.py` & `tox-4.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/test_provision.py` & `tox-4.6.4/tests/test_provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/test_report.py` & `tox-4.6.4/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/test_run.py` & `tox-4.6.4/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/test_version.py` & `tox-4.6.4/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/test_main.py` & `tox-4.6.4/tests/config/test_main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/test_of_types.py` & `tox-4.6.4/tests/config/test_of_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/test_set_env.py` & `tox-4.6.4/tests/config/test_set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/test_sets.py` & `tox-4.6.4/tests/config/test_sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/test_types.py` & `tox-4.6.4/tests/config/test_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/cli/conftest.py` & `tox-4.6.4/tests/config/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/cli/test_cli_env_var.py` & `tox-4.6.4/tests/config/cli/test_cli_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/cli/test_cli_ini.py` & `tox-4.6.4/tests/config/cli/test_cli_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/cli/test_parse.py` & `tox-4.6.4/tests/config/cli/test_parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/cli/test_parser.py` & `tox-4.6.4/tests/config/cli/test_parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/test_loader.py` & `tox-4.6.4/tests/config/loader/test_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/test_memory_loader.py` & `tox-4.6.4/tests/config/loader/test_memory_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/test_section.py` & `tox-4.6.4/tests/config/loader/test_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/test_str_convert.py` & `tox-4.6.4/tests/config/loader/test_str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/ini/conftest.py` & `tox-4.6.4/tests/config/loader/ini/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/ini/test_factor.py` & `tox-4.6.4/tests/config/loader/ini/test_factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/ini/test_ini_loader.py` & `tox-4.6.4/tests/config/loader/ini/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/ini/replace/conftest.py` & `tox-4.6.4/tests/config/loader/ini/replace/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/ini/replace/test_replace.py` & `tox-4.6.4/tests/config/loader/ini/replace/test_replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/ini/replace/test_replace_env_var.py` & `tox-4.6.4/tests/config/loader/ini/replace/test_replace_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/ini/replace/test_replace_os_sep.py` & `tox-4.6.4/tests/config/loader/ini/replace/test_replace_os_sep.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/ini/replace/test_replace_posargs.py` & `tox-4.6.4/tests/config/loader/ini/replace/test_replace_posargs.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/ini/replace/test_replace_tox_env.py` & `tox-4.6.4/tests/config/loader/ini/replace/test_replace_tox_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/loader/ini/replace/test_replace_tty.py` & `tox-4.6.4/tests/config/loader/ini/replace/test_replace_tty.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/source/test_discover.py` & `tox-4.6.4/tests/config/source/test_discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/source/test_setup_cfg.py` & `tox-4.6.4/tests/config/source/test_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/config/source/test_source_ini.py` & `tox-4.6.4/tests/config/source/test_source_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/demo_pkg_inline/build.py` & `tox-4.6.4/tests/demo_pkg_inline/build.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/execute/test_request.py` & `tox-4.6.4/tests/execute/test_request.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/execute/local_subprocess/bad_process.py` & `tox-4.6.4/tests/execute/local_subprocess/bad_process.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/execute/local_subprocess/local_subprocess_sigint.py` & `tox-4.6.4/tests/execute/local_subprocess/local_subprocess_sigint.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/execute/local_subprocess/test_execute_util.py` & `tox-4.6.4/tests/execute/local_subprocess/test_execute_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/execute/local_subprocess/test_local_subprocess.py` & `tox-4.6.4/tests/execute/local_subprocess/test_local_subprocess.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/journal/test_main_journal.py` & `tox-4.6.4/tests/journal/test_main_journal.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/plugin/test_inline.py` & `tox-4.6.4/tests/plugin/test_inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/plugin/test_plugin.py` & `tox-4.6.4/tests/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/plugin/test_plugin_custom_config_set.py` & `tox-4.6.4/tests/plugin/test_plugin_custom_config_set.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/pytest_/test_init.py` & `tox-4.6.4/tests/pytest_/test_init.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/test_env_select.py` & `tox-4.6.4/tests/session/test_env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/test_session_common.py` & `tox-4.6.4/tests/session/test_session_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/test_depends.py` & `tox-4.6.4/tests/session/cmd/test_depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/test_devenv.py` & `tox-4.6.4/tests/session/cmd/test_devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/test_exec_.py` & `tox-4.6.4/tests/session/cmd/test_exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/test_legacy.py` & `tox-4.6.4/tests/session/cmd/test_legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/test_list_envs.py` & `tox-4.6.4/tests/session/cmd/test_list_envs.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/test_parallel.py` & `tox-4.6.4/tests/session/cmd/test_parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/test_quickstart.py` & `tox-4.6.4/tests/session/cmd/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/test_sequential.py` & `tox-4.6.4/tests/session/cmd/test_sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/test_show_config.py` & `tox-4.6.4/tests/session/cmd/test_show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/test_state.py` & `tox-4.6.4/tests/session/cmd/test_state.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/session/cmd/run/test_common.py` & `tox-4.6.4/tests/session/cmd/run/test_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/test_api.py` & `tox-4.6.4/tests/tox_env/test_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/test_register.py` & `tox-4.6.4/tests/tox_env/test_register.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/test_tox_env_api.py` & `tox-4.6.4/tests/tox_env/test_tox_env_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/test_tox_env_runner.py` & `tox-4.6.4/tests/tox_env/test_tox_env_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/test_python_api.py` & `tox-4.6.4/tests/tox_env/python/test_python_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/test_python_runner.py` & `tox-4.6.4/tests/tox_env/python/test_python_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/pip/test_pip_install.py` & `tox-4.6.4/tests/tox_env/python/pip/test_pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/pip/test_req_file.py` & `tox-4.6.4/tests/tox_env/python/pip/test_req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/pip/req/test_file.py` & `tox-4.6.4/tests/tox_env/python/pip/req/test_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/virtual_env/test_setuptools.py` & `tox-4.6.4/tests/tox_env/python/virtual_env/test_setuptools.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/virtual_env/test_virtualenv_api.py` & `tox-4.6.4/tests/tox_env/python/virtual_env/test_virtualenv_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/virtual_env/package/conftest.py` & `tox-4.6.4/tests/tox_env/python/virtual_env/package/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py` & `tox-4.6.4/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/virtual_env/package/test_package_pyproject.py` & `tox-4.6.4/tests/tox_env/python/virtual_env/package/test_package_pyproject.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/tox_env/python/virtual_env/package/test_python_package_util.py` & `tox-4.6.4/tests/tox_env/python/virtual_env/package/test_python_package_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/util/test_ci.py` & `tox-4.6.4/tests/util/test_ci.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         "GITHUB_ACTIONS": "true",  # GitHub Actions
         "GITLAB_CI": None,  # GitLab CI
         "HEROKU_TEST_RUN_ID": None,  # Heroku CI
         "BUILD_ID": None,  # Hudson
         "TEAMCITY_VERSION": None,  # TeamCity
         "TRAVIS": "true",  # Travis CI
     }.items(),
-    ids=lambda v: v[0],  # type: ignore[no-any-return]
+    ids=lambda v: v[0],
 )
 def test_is_ci(env_var: tuple[str, str | None], monkeypatch: pytest.MonkeyPatch) -> None:
     for var in _ENV_VARS:
         monkeypatch.delenv(var, raising=False)
     monkeypatch.setenv(env_var[0], env_var[1] or "")
     assert is_ci()
 
@@ -37,15 +37,15 @@
         "TF_BUILD": "",  # Azure Pipelines
         "BUILDKITE": "",  # Buildkite
         "CIRCLECI": "",  # Circle CI
         "CIRRUS_CI": "",  # Cirrus CI
         "GITHUB_ACTIONS": "",  # GitHub Actions
         "TRAVIS": "",  # Travis CI
     }.items(),
-    ids=lambda v: v[0],  # type: ignore[no-any-return]
+    ids=lambda v: v[0],
 )
 def test_is_ci_bad_set(env_var: tuple[str, str], monkeypatch: pytest.MonkeyPatch) -> None:
     for var in _ENV_VARS:
         monkeypatch.delenv(var, raising=False)
     monkeypatch.setenv(env_var[0], env_var[1])
     assert not is_ci()
```

### Comparing `tox-4.6.3/tests/util/test_cpu.py` & `tox-4.6.4/tests/util/test_cpu.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/util/test_graph.py` & `tox-4.6.4/tests/util/test_graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/tests/util/test_spinner.py` & `tox-4.6.4/tests/util/test_spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/LICENSE` & `tox-4.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/README.md` & `tox-4.6.4/README.md`

 * *Files identical despite different names*

### Comparing `tox-4.6.3/pyproject.toml` & `tox-4.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -48,28 +48,28 @@
   "version",
 ]
 dependencies = [
   "cachetools>=5.3.1",
   "chardet>=5.1",
   "colorama>=0.4.6",
   "filelock>=3.12.2",
-  'importlib-metadata>=6.6; python_version < "3.8"',
+  'importlib-metadata>=6.7; python_version < "3.8"',
   "packaging>=23.1",
-  "platformdirs>=3.5.3",
-  "pluggy>=1",
+  "platformdirs>=3.8",
+  "pluggy>=1.2",
   "pyproject-api>=1.5.2",
   'tomli>=2.0.1; python_version < "3.11"',
   'typing-extensions>=4.6.3; python_version < "3.8"',
   "virtualenv>=20.23.1",
 ]
 optional-dependencies.docs = [
   "furo>=2023.5.20",
   "sphinx>=7.0.1",
   "sphinx-argparse-cli>=1.11.1",
-  "sphinx-autodoc-typehints!=1.23.4,>=1.23.2",
+  "sphinx-autodoc-typehints!=1.23.4,>=1.23.3",
   "sphinx-copybutton>=0.5.2",
   "sphinx-inline-tabs>=2023.4.21",
   "sphinxcontrib-towncrier>=0.2.1a0",
   "towncrier>=23.6",
 ]
 optional-dependencies.testing = [
   "build[virtualenv]>=0.10",
@@ -78,15 +78,15 @@
   "devpi-process>=0.3.1",
   "diff-cover>=7.6",
   "distlib>=0.3.6",
   "flaky>=3.7",
   "hatch-vcs>=0.3",
   "hatchling>=1.17.1",
   "psutil>=5.9.5",
-  "pytest>=7.3.2",
+  "pytest>=7.4",
   "pytest-cov>=4.1",
   "pytest-mock>=3.11.1",
   "pytest-xdist>=3.3.1",
   "re-assert>=1.1",
   'time-machine>=2.10; implementation_name != "pypy"',
   "wheel>=0.40",
 ]
```

### Comparing `tox-4.6.3/PKG-INFO` & `tox-4.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox
-Version: 4.6.3
+Version: 4.6.4
 Summary: tox is a generic virtualenv management and test command line tool
 Project-URL: Documentation, https://tox.wiki
 Project-URL: Homepage, http://tox.readthedocs.org
 Project-URL: Release Notes, https://tox.wiki/en/latest/changelog.html
 Project-URL: Source, https://github.com/tox-dev/tox
 Project-URL: Tracker, https://github.com/tox-dev/tox/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
@@ -30,26 +30,26 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Requires-Dist: cachetools>=5.3.1
 Requires-Dist: chardet>=5.1
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: filelock>=3.12.2
-Requires-Dist: importlib-metadata>=6.6; python_version < '3.8'
+Requires-Dist: importlib-metadata>=6.7; python_version < '3.8'
 Requires-Dist: packaging>=23.1
-Requires-Dist: platformdirs>=3.5.3
-Requires-Dist: pluggy>=1
+Requires-Dist: platformdirs>=3.8
+Requires-Dist: pluggy>=1.2
 Requires-Dist: pyproject-api>=1.5.2
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Requires-Dist: typing-extensions>=4.6.3; python_version < '3.8'
 Requires-Dist: virtualenv>=20.23.1
 Provides-Extra: docs
 Requires-Dist: furo>=2023.5.20; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.11.1; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23.2; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23.3; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs>=2023.4.21; extra == 'docs'
 Requires-Dist: sphinx>=7.0.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-towncrier>=0.2.1a0; extra == 'docs'
 Requires-Dist: towncrier>=23.6; extra == 'docs'
 Provides-Extra: testing
 Requires-Dist: build[virtualenv]>=0.10; extra == 'testing'
@@ -61,15 +61,15 @@
 Requires-Dist: flaky>=3.7; extra == 'testing'
 Requires-Dist: hatch-vcs>=0.3; extra == 'testing'
 Requires-Dist: hatchling>=1.17.1; extra == 'testing'
 Requires-Dist: psutil>=5.9.5; extra == 'testing'
 Requires-Dist: pytest-cov>=4.1; extra == 'testing'
 Requires-Dist: pytest-mock>=3.11.1; extra == 'testing'
 Requires-Dist: pytest-xdist>=3.3.1; extra == 'testing'
-Requires-Dist: pytest>=7.3.2; extra == 'testing'
+Requires-Dist: pytest>=7.4; extra == 'testing'
 Requires-Dist: re-assert>=1.1; extra == 'testing'
 Requires-Dist: time-machine>=2.10; implementation_name != 'pypy' and extra == 'testing'
 Requires-Dist: wheel>=0.40; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # tox
```

