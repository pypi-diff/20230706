# Comparing `tmp/sealights-python-agent-1.1.3.tar.gz` & `tmp/sealights-python-agent-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sealights-python-agent-1.1.3.tar", last modified: Tue Jun  6 12:12:13 2023, max compression
+gzip compressed data, was "dist/sealights-python-agent-1.1.4.tar", last modified: Thu Jul  6 07:54:41 2023, max compression
```

## Comparing `sealights-python-agent-1.1.3.tar` & `sealights-python-agent-1.1.4.tar`

### file list

```diff
@@ -1,321 +1,321 @@
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    17323 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/admin.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/bootstrap/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1171 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/bootstrap/sitecustomize.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/bootstrap/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/common/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8418 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/configuration_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1795 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/environment_variables_resolver.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2866 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/config_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2973 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/constants.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/common/autoupgrade/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3132 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/autoupgrade/autoupgrade_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/autoupgrade/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/common/token/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      353 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/token/token_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1328 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/token/token_parser.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/token/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/common/http/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8527 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/http/backend_proxy.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3041 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/http/sl_routes.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1838 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/http/requests_wrapper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/http/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/common/build_session/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      343 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/build_session/build_session_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/build_session/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4935 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/agent_events_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5448 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/env_vars.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      644 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_heartbeat_event.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      643 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_footprints_submission_error_event.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      467 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_stop_event.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1761 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_start_event.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      618 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_build_scan_error_event.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      626 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_tests_submission_error_event.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      120 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/agent_events/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/common/log/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2923 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/log/sealights_logging.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/common/log/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5356 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/utils.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/test_listener/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/test_listener/queues/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      821 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/queues/events_queue.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/queues/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      940 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/queues/footprints_queue.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/test_listener/web_frameworks/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1280 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/web_frameworks/bottle_framework.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1260 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/web_frameworks/flask_framework.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       51 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/web_frameworks/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/test_listener/coloring/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1396 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/coloring/requests_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2218 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/coloring/selenium_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      682 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/coloring/urllib2_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       68 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/coloring/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/test_listener/managers/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4000 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/managers/tia_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4883 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/managers/code_coverage_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3556 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/managers/agent_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7679 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/managers/footprints_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2986 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/managers/events_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/managers/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      453 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/footprints_collector.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2551 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/sealights_api.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/test_listener/services/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6000 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/services/footprints_service.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1200 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/services/events_service.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/services/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1026 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/line_footprints_collector.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      744 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3654 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/method_footprints_collector.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/test_listener/integrations/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      560 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/integrations/freezegun_patcher.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2806 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/integrations/multiprocessing_patcher.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      779 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/integrations/pytest_xdist_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5391 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/integrations/unittest_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4996 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/integrations/nose_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6774 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/integrations/pytest_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/integrations/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      239 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/upload_reports_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      130 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/footprint_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      308 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/footprints_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      417 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/events_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      461 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/start_execution_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      388 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/logs_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      608 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/upload_reports_metadata.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/test_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      197 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/file_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/entities/app_data.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/test_frameworks/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1539 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/test_frameworks/agent_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2002 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/test_frameworks/pytest_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1179 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/test_frameworks/unittest_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/test_frameworks/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1244 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/test_frameworks/nose_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2175 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/upload_reports.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      466 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/end_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      918 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/start_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2155 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/run.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/send_footprints.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      523 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/executors/anonymous_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1604 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/test_listener/state_tracker.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3113 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/scm/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7711 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/scm/git_integration.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2517 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/scm/scm_info.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/scm/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1537 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/file_scanner.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2419 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/visitors.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5735 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/app.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1363 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/ast_utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3782 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/method_hasher.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/entities/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2327 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/entities/environment_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/entities/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/entities/v3/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      263 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/entities/v3/build_mapping_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      620 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/entities/v3/method_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       91 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/entities/v3/code_element_with_hash.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/entities/v3/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      680 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/entities/v3/file_data.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/executors/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1404 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/executors/build.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1835 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/executors/config.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/build_scanner/executors/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      632 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/init.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/blinker/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4479 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/blinker/_utilities.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    16341 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/blinker/base.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9223 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/blinker/_saferef.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      322 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/blinker/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    22041 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/adapters.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3456 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1003 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/packages.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    35166 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/models.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      441 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/__version__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      475 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/certs.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6402 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/api.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      757 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/hooks.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18430 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/cookies.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    10207 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/auth.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    33321 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4071 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/help.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1096 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/_internal_utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5039 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4188 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/status_codes.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3005 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/structures.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2081 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/compat.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    29835 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/requests/sessions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    32452 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/six.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/certifi/
--rw-r--r--   0 jenkins    (498) jenkins    (497)   276001 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/certifi/cacert.pem
--rw-r--r--   0 jenkins    (498) jenkins    (497)      243 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/certifi/__main__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       96 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/certifi/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2537 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/certifi/core.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/jwt/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9186 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/jwt/api_jws.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      963 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/jwt/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1914 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/jwt/jwks_client.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8025 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/jwt/api_jwt.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    22392 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/jwt/algorithms.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3114 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/jwt/api_jwk.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3993 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/jwt/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/jwt/help.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1548 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/jwt/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/astunparse/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1222 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astunparse/__main__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20121 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astunparse/unparser36.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20690 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astunparse/unparser38.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1435 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astunparse/printer.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    26742 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astunparse/unparser.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3197 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astunparse/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20676 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astunparse/unparser37.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2917 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/string_repr.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    32032 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/code_gen.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        6 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/VERSION
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3268 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/file_util.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7373 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/source_repr.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6542 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/node_util.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2291 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6741 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/rtrip.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6020 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/tree_walk.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3191 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/op_util.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      204 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/astor/codegen.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)   107685 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/typing_extensions.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1862 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_adapters.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2166 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_text.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      743 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_collections.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1826 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_compat.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2895 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_functools.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1154 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_meta.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/py.typed
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2068 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_itertools.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    30533 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8425 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/zipp.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/click/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1353 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/_textwrap.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9167 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    16063 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/testing.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    35805 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/types.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    23451 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/_termui_impl.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18810 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/_compat.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3201 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/_unicodefun.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/py.typed
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7860 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/_winconsole.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1961 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/globals.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18682 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    19044 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/parser.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3138 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)   112782 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/core.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    16350 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/decorators.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9706 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/formatting.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18018 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/shell_completion.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    28355 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/click/termui.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    11076 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/cd.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3384 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/legacy.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    13303 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/models.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/assets/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    25485 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/assets/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/cli/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9364 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/cli/normalizer.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/cli/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20303 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/api.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/py.typed
--rw-r--r--   0 jenkins    (498) jenkins    (497)       80 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/version.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18191 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/md.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9308 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1790 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    19449 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/constant.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/semantic_version/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    48115 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/semantic_version/base.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      546 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/semantic_version/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/semantic_version/django_fields.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/idna/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3374 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/idna/codec.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1881 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/idna/intranges.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)   204400 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/idna/uts46data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       21 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/idna/package_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    44025 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/idna/idnadata.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/idna/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    12795 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/idna/core.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      321 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/idna/compat.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8217 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    28276 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/response.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8579 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/fields.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    39013 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/connectionpool.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       63 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/_version.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    19786 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/poolmanager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    10811 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/_collections.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2440 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/filepost.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20070 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/connection.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5758 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6895 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/ssltransport.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/response.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/proxy.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    17165 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/ssl_.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5404 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/wait.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    10003 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/timeout.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4901 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/connection.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      498 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/queue.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4225 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    22001 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/retry.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1155 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    14057 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/url.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5985 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/request.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4538 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/ntlmpool.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/_securetransport/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    13922 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    17632 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    34433 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/securetransport.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    16901 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      957 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    11010 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/appengine.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7097 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/socks.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2763 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/packages/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    34666 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/packages/six.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/packages/backports/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1417 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/packages/backports/makefile.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/packages/backports/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/urllib3/packages/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/python_agent/packages/freezegun/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    25911 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/freezegun/api.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      421 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/freezegun/_async.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      302 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/python_agent/packages/freezegun/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2305 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/LICENSE.txt
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/sealights_python_agent.egg-info/
--rw-r--r--   0 jenkins    (498) jenkins    (497)        1 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/sealights_python_agent.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)       95 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/sealights_python_agent.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)    12620 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/sealights_python_agent.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)      722 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/sealights_python_agent.egg-info/requires.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)       13 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/sealights_python_agent.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4043 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/sealights_python_agent.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (498) jenkins    (497)      873 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/requirements.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2076 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/CHANGES.rst
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1044 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/README.rst
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4043 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/PKG-INFO
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3846 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/setup.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       67 2023-06-06 12:12:13.000000 sealights-python-agent-1.1.3/setup.cfg
--rw-r--r--   0 jenkins    (498) jenkins    (497)      138 2023-06-06 12:12:12.000000 sealights-python-agent-1.1.3/MANIFEST.in
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    17323 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/admin.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/bootstrap/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1171 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/bootstrap/sitecustomize.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/bootstrap/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/common/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8418 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/configuration_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1795 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/environment_variables_resolver.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2866 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/config_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2973 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/constants.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/common/autoupgrade/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3132 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/autoupgrade/autoupgrade_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/autoupgrade/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/common/token/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      353 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/token/token_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1328 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/token/token_parser.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/token/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/common/http/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8527 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/http/backend_proxy.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3041 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/http/sl_routes.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1838 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/http/requests_wrapper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/http/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/common/build_session/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      343 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/build_session/build_session_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/build_session/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4935 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/agent_events_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5448 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/env_vars.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      644 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_heartbeat_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      643 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_footprints_submission_error_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      467 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_stop_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1820 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_start_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      618 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_build_scan_error_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      626 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_tests_submission_error_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      120 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/agent_events/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/common/log/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2948 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/log/sealights_logging.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/common/log/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5356 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/utils.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/test_listener/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/test_listener/queues/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      821 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/queues/events_queue.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/queues/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      940 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/queues/footprints_queue.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/test_listener/web_frameworks/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1280 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/web_frameworks/bottle_framework.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1260 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/web_frameworks/flask_framework.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       51 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/web_frameworks/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/test_listener/coloring/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1396 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/coloring/requests_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2218 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/coloring/selenium_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      682 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/coloring/urllib2_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       68 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/coloring/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/test_listener/managers/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4000 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/managers/tia_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4883 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/managers/code_coverage_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3556 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/managers/agent_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7679 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/managers/footprints_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2986 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/managers/events_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/managers/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      453 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/footprints_collector.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2551 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/sealights_api.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/test_listener/services/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6030 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/services/footprints_service.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1230 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/services/events_service.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/services/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1026 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/line_footprints_collector.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      744 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3654 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/method_footprints_collector.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/test_listener/integrations/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      560 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/integrations/freezegun_patcher.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2806 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/integrations/multiprocessing_patcher.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      779 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/integrations/pytest_xdist_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5391 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/integrations/unittest_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4996 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/integrations/nose_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6774 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/integrations/pytest_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/integrations/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      239 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/upload_reports_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      130 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/footprint_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      308 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/footprints_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      417 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/events_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      461 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/start_execution_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      388 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/logs_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      612 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/upload_reports_metadata.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/test_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      197 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/file_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/entities/app_data.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/test_frameworks/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1539 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/test_frameworks/agent_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2002 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/test_frameworks/pytest_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1179 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/test_frameworks/unittest_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/test_frameworks/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1244 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/test_frameworks/nose_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2175 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/upload_reports.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      466 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/end_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      918 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/start_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2155 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/run.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/send_footprints.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      523 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/executors/anonymous_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1604 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/test_listener/state_tracker.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3113 2023-07-06 07:54:39.000000 sealights-python-agent-1.1.4/python_agent/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/scm/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7711 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/scm/git_integration.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2517 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/scm/scm_info.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/scm/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1537 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/file_scanner.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2419 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/visitors.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5735 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/app.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1363 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/ast_utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3782 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/method_hasher.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/entities/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2383 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/entities/environment_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/entities/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/entities/v3/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      263 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/entities/v3/build_mapping_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      620 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/entities/v3/method_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       91 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/entities/v3/code_element_with_hash.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/entities/v3/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      680 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/entities/v3/file_data.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/executors/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1404 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/executors/build.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1835 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/executors/config.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/build_scanner/executors/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      632 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/init.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/blinker/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4479 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/blinker/_utilities.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16341 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/blinker/base.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9223 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/blinker/_saferef.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      322 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/blinker/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    22041 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/adapters.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3456 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1003 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/packages.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    35166 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/models.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      441 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/__version__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      475 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/certs.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6402 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/api.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      757 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/hooks.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18430 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/cookies.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    10207 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/auth.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    33321 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4071 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/help.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1096 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/_internal_utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5039 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4188 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/status_codes.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3005 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/structures.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2081 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/compat.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    29835 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/requests/sessions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    32452 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/six.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/certifi/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   276001 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/certifi/cacert.pem
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      243 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/certifi/__main__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       96 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/certifi/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2537 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/certifi/core.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/jwt/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9186 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/jwt/api_jws.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      963 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/jwt/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1914 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/jwt/jwks_client.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8025 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/jwt/api_jwt.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    22392 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/jwt/algorithms.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3114 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/jwt/api_jwk.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3993 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/jwt/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/jwt/help.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1548 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/jwt/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/astunparse/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1222 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astunparse/__main__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20121 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astunparse/unparser36.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20690 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astunparse/unparser38.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1435 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astunparse/printer.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    26742 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astunparse/unparser.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3197 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astunparse/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20676 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astunparse/unparser37.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2917 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/string_repr.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    32032 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/code_gen.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        6 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/VERSION
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3268 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/file_util.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7373 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/source_repr.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6542 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/node_util.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2291 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6741 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/rtrip.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6020 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/tree_walk.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3191 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/op_util.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      204 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/astor/codegen.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   107685 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/typing_extensions.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1862 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_adapters.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2166 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_text.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      743 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_collections.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1826 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_compat.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2895 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_functools.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1154 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_meta.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/py.typed
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2068 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_itertools.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    30533 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8425 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/zipp.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/click/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1353 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/_textwrap.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9167 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16063 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/testing.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    35805 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/types.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    23451 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/_termui_impl.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18810 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/_compat.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3201 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/_unicodefun.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/py.typed
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7860 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/_winconsole.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1961 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/globals.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18682 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    19044 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/parser.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3138 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   112782 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/core.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16350 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/decorators.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9706 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/formatting.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18018 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/shell_completion.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    28355 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/click/termui.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    11076 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/cd.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3384 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/legacy.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    13303 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/models.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/assets/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    25485 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/assets/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/cli/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9364 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/cli/normalizer.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/cli/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20303 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/api.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/py.typed
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       80 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/version.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18191 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/md.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9308 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1790 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    19449 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/constant.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/semantic_version/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    48115 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/semantic_version/base.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      546 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/semantic_version/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/semantic_version/django_fields.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/idna/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3374 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/idna/codec.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1881 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/idna/intranges.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   204400 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/idna/uts46data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       21 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/idna/package_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    44025 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/idna/idnadata.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/idna/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    12795 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/idna/core.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      321 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/idna/compat.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8217 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    28276 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/response.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8579 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/fields.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    39013 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/connectionpool.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       63 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/_version.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    19786 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/poolmanager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    10811 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/_collections.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2440 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/filepost.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20070 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/connection.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5758 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6895 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/ssltransport.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/response.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/proxy.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    17165 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5404 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/wait.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    10003 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/timeout.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4901 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/connection.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      498 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/queue.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4225 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    22001 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/retry.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1155 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    14057 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/url.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5985 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/request.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4538 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/ntlmpool.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/_securetransport/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    13922 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    17632 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    34433 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16901 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      957 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    11010 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/appengine.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7097 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/socks.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2763 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/packages/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    34666 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/packages/six.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/packages/backports/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1417 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/urllib3/packages/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/python_agent/packages/freezegun/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    25911 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/freezegun/api.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      421 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/freezegun/_async.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      302 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/python_agent/packages/freezegun/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2305 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/LICENSE.txt
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/sealights_python_agent.egg-info/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        1 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/sealights_python_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       95 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/sealights_python_agent.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    12620 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/sealights_python_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      722 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/sealights_python_agent.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       13 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/sealights_python_agent.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4043 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/sealights_python_agent.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      874 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/requirements.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2076 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/CHANGES.rst
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1044 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/README.rst
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4043 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/PKG-INFO
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3846 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/setup.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       67 2023-07-06 07:54:41.000000 sealights-python-agent-1.1.4/setup.cfg
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      138 2023-07-06 07:54:38.000000 sealights-python-agent-1.1.4/MANIFEST.in
```

### Comparing `sealights-python-agent-1.1.3/python_agent/admin.py` & `sealights-python-agent-1.1.4/python_agent/admin.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/bootstrap/sitecustomize.py` & `sealights-python-agent-1.1.4/python_agent/bootstrap/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/configuration_manager.py` & `sealights-python-agent-1.1.4/python_agent/common/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/environment_variables_resolver.py` & `sealights-python-agent-1.1.4/python_agent/common/environment_variables_resolver.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/config_data.py` & `sealights-python-agent-1.1.4/python_agent/common/config_data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/constants.py` & `sealights-python-agent-1.1.4/python_agent/common/constants.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/autoupgrade/autoupgrade_manager.py` & `sealights-python-agent-1.1.4/python_agent/common/autoupgrade/autoupgrade_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/token/token_parser.py` & `sealights-python-agent-1.1.4/python_agent/common/token/token_parser.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/http/backend_proxy.py` & `sealights-python-agent-1.1.4/python_agent/common/http/backend_proxy.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/http/sl_routes.py` & `sealights-python-agent-1.1.4/python_agent/common/http/sl_routes.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/http/requests_wrapper.py` & `sealights-python-agent-1.1.4/python_agent/common/http/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/agent_events/agent_events_manager.py` & `sealights-python-agent-1.1.4/python_agent/common/agent_events/agent_events_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/agent_events/env_vars.py` & `sealights-python-agent-1.1.4/python_agent/common/agent_events/env_vars.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_heartbeat_event.py` & `sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_heartbeat_event.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_footprints_submission_error_event.py` & `sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_footprints_submission_error_event.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_start_event.py` & `sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_start_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
                     "testStage": test_stage,
                     "labId": lab_id,
                     "sendsPing": True,
                     "argv": sys.argv[1:],
                     "envVars": get_ci_env_vars(),
                     "tags": [python_version()],
                     "agentConfig": {},
+                    "buildSessionId": self.buildSessionId,
                 },
                 "machineInfo": {
                     "machineName": socket.gethostname(),
                     "arch": platform.machine(),
                     "os": platform.system(),
                     "localDateTime": datetime.datetime.now().isoformat(),
                     "localDateTimeUnix_s": int(datetime.datetime.now().timestamp()),
```

### Comparing `sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_build_scan_error_event.py` & `sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_build_scan_error_event.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/agent_events/entites/agent_tests_submission_error_event.py` & `sealights-python-agent-1.1.4/python_agent/common/agent_events/entites/agent_tests_submission_error_event.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/common/log/sealights_logging.py` & `sealights-python-agent-1.1.4/python_agent/common/log/sealights_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class SealightsHTTPHandler(logging.Handler):
     def __init__(self, config_data, capacity=50):
         logging.Handler.__init__(self)
         self.capacity = capacity
         self.buffer = []
         self.backend_proxy = BackendProxy(config_data)
         self.config_data = config_data
-        self.environment = EnvironmentData(config_data.labId, config_data.testStage)
+        self.environment = EnvironmentData(config_data.labId, config_data.testStage, config_data.testGroupId)
         self.environment.environmentName = config_data.labId
         self.watchdog = BackgroundScheduler(**kwargs)
         self.watchdog.add_job(self.flush, interval.IntervalTrigger(seconds=constants.INTERVAL_IN_SECONDS))
         self.watchdog.start()
 
     def build_request(self, records):
         log = "\n".join(map(lambda record: self.format(record), records))
```

### Comparing `sealights-python-agent-1.1.3/python_agent/utils.py` & `sealights-python-agent-1.1.4/python_agent/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/queues/events_queue.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/queues/events_queue.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/queues/footprints_queue.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/queues/footprints_queue.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/web_frameworks/bottle_framework.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/web_frameworks/bottle_framework.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/web_frameworks/flask_framework.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/web_frameworks/flask_framework.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/coloring/requests_helper.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/coloring/requests_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/coloring/selenium_helper.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/coloring/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/coloring/urllib2_helper.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/coloring/urllib2_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/managers/tia_manager.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/managers/tia_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/managers/code_coverage_manager.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/managers/code_coverage_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/managers/agent_manager.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/managers/agent_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/managers/footprints_manager.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/managers/footprints_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/managers/events_manager.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/managers/events_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/sealights_api.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/sealights_api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/services/footprints_service.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/services/footprints_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             log.info("Sent Footprints to Server")
         except Exception as e:
             log.exception("Failed Sending Footprints. Error: %s" % str(e))
             raise
 
     def create_footprints_request(self, footprint_items):
         app_data = AppData(self.config_data.appName, self.config_data.branchName, self.config_data.buildName, [])
-        environment_data = EnvironmentData(self.config_data.labId, self.config_data.testStage)
+        environment_data = EnvironmentData(self.config_data.labId, self.config_data.testStage, self.config_data.testGroupId)
         footprints_request = FootprintsRequest(self.config_data.customerId, environment_data, self.config_data, [], [app_data])
         test_name_to_index = {}
         filename_to_file = {}
         unique_id_to_element = {}
         unique_id_to_hits_index = {}
         try:
             for footprint_item in footprint_items:
```

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/services/events_service.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/services/events_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self, config_data, backend_proxy):
         self.config_data = config_data
         self.backend_proxy = backend_proxy
 
     def send_events(self, events):
         try:
             log.info("Sending Events. Number Of Events: %s" % len(events))
-            environment_data = EnvironmentData(self.config_data.labId, self.config_data.testStage)
+            environment_data = EnvironmentData(self.config_data.labId, self.config_data.testStage, self.config_data.testGroupId)
             events_request = EventsRequest(self.config_data.customerId, self.config_data.appName,
                                            self.config_data.branchName, self.config_data.buildName, environment_data,
                                            events, self.config_data.testSelectionStatus)
             self.backend_proxy.send_events(events_request)
             log.info("Sent Events to Server. Number Of Events: %s" % len(events))
         except Exception as e:
             log.exception("Failed Sending Events. Number Of Events: %s. error: %s" % (len(events), str(e)))
```

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/line_footprints_collector.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/line_footprints_collector.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/utils.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/method_footprints_collector.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/method_footprints_collector.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/integrations/freezegun_patcher.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/integrations/freezegun_patcher.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/integrations/multiprocessing_patcher.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/integrations/multiprocessing_patcher.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/integrations/pytest_xdist_helper.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/integrations/pytest_xdist_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/integrations/unittest_helper.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/integrations/unittest_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/integrations/nose_helper.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/integrations/nose_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/integrations/pytest_helper.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/integrations/pytest_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/entities/upload_reports_metadata.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/entities/upload_reports_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,9 +6,9 @@
         self.source = source
         self.type = report_type
         self.customerId = config_data.customerId
         self.appName = config_data.appName
         self.branchName = config_data.branchName
         self.buildName = config_data.buildName
         self.hasMoreRequests = has_more_requests
-        self.environment = EnvironmentData(labid, None)
+        self.environment = EnvironmentData(labid, None, "")
         self.environment.environmentName = labid
```

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/executors/test_frameworks/agent_execution.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/executors/test_frameworks/agent_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/executors/test_frameworks/pytest_execution.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/executors/test_frameworks/pytest_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/executors/test_frameworks/unittest_execution.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/executors/test_frameworks/unittest_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/executors/test_frameworks/nose_execution.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/executors/test_frameworks/nose_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/executors/upload_reports.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/executors/upload_reports.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/executors/start_execution.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/executors/start_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/executors/run.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/executors/run.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/executors/send_footprints.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/executors/send_footprints.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/executors/anonymous_execution.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/executors/anonymous_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/test_listener/state_tracker.py` & `sealights-python-agent-1.1.4/python_agent/test_listener/state_tracker.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/__init__.py` & `sealights-python-agent-1.1.4/python_agent/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from python_agent.packages import urllib3
 from python_agent.packages.urllib3.exceptions import InsecureRequestWarning
 from logging.config import dictConfig
 
 urllib3.disable_warnings(InsecureRequestWarning)
 
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 __package_name__ = "sealights-python-agent"
 
 
 LOG_CONF = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
```

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/scm/git_integration.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/scm/git_integration.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/scm/scm_info.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/scm/scm_info.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/file_scanner.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/file_scanner.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/visitors.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/visitors.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/app.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/app.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/ast_utils.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/ast_utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/method_hasher.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/method_hasher.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/entities/environment_data.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/entities/environment_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 from python_agent import __version__ as VERSION
 
 
 class EnvironmentData(object):
     agentId = None
 
-    def __init__(self, lab_id, test_stage):
+    def __init__(self, lab_id, test_stage, test_group_id):
         self.labId = lab_id
         self.testStage = test_stage
+        self.testGroupId = test_group_id
         if not EnvironmentData.agentId:
             EnvironmentData.agentId = str(uuid.uuid4())
         self.agentId = EnvironmentData.agentId
         self.agentType = "python"
         self.agentVersion = VERSION
         self.machineName = socket.gethostname()
         self.platform = platform.platform()
```

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/entities/v3/method_data.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/entities/v3/method_data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/entities/v3/file_data.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/entities/v3/file_data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/executors/build.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/executors/build.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/build_scanner/executors/config.py` & `sealights-python-agent-1.1.4/python_agent/build_scanner/executors/config.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/init.py` & `sealights-python-agent-1.1.4/python_agent/init.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/blinker/_utilities.py` & `sealights-python-agent-1.1.4/python_agent/packages/blinker/_utilities.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/blinker/base.py` & `sealights-python-agent-1.1.4/python_agent/packages/blinker/base.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/blinker/_saferef.py` & `sealights-python-agent-1.1.4/python_agent/packages/blinker/_saferef.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/adapters.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/exceptions.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/packages.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/models.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/api.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/hooks.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/cookies.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/auth.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/utils.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/help.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/_internal_utils.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/status_codes.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/structures.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/compat.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/requests/sessions.py` & `sealights-python-agent-1.1.4/python_agent/packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/six.py` & `sealights-python-agent-1.1.4/python_agent/packages/six.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/certifi/cacert.pem` & `sealights-python-agent-1.1.4/python_agent/packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/certifi/core.py` & `sealights-python-agent-1.1.4/python_agent/packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/jwt/api_jws.py` & `sealights-python-agent-1.1.4/python_agent/packages/jwt/api_jws.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/jwt/exceptions.py` & `sealights-python-agent-1.1.4/python_agent/packages/jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/jwt/jwks_client.py` & `sealights-python-agent-1.1.4/python_agent/packages/jwt/jwks_client.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/jwt/api_jwt.py` & `sealights-python-agent-1.1.4/python_agent/packages/jwt/api_jwt.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/jwt/algorithms.py` & `sealights-python-agent-1.1.4/python_agent/packages/jwt/algorithms.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/jwt/api_jwk.py` & `sealights-python-agent-1.1.4/python_agent/packages/jwt/api_jwk.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/jwt/utils.py` & `sealights-python-agent-1.1.4/python_agent/packages/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/jwt/help.py` & `sealights-python-agent-1.1.4/python_agent/packages/jwt/help.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/jwt/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astunparse/__main__.py` & `sealights-python-agent-1.1.4/python_agent/packages/astunparse/__main__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astunparse/unparser36.py` & `sealights-python-agent-1.1.4/python_agent/packages/astunparse/unparser36.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astunparse/unparser38.py` & `sealights-python-agent-1.1.4/python_agent/packages/astunparse/unparser38.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astunparse/printer.py` & `sealights-python-agent-1.1.4/python_agent/packages/astunparse/printer.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astunparse/unparser.py` & `sealights-python-agent-1.1.4/python_agent/packages/astunparse/unparser.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astunparse/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/astunparse/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astunparse/unparser37.py` & `sealights-python-agent-1.1.4/python_agent/packages/astunparse/unparser37.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astor/string_repr.py` & `sealights-python-agent-1.1.4/python_agent/packages/astor/string_repr.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astor/code_gen.py` & `sealights-python-agent-1.1.4/python_agent/packages/astor/code_gen.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astor/file_util.py` & `sealights-python-agent-1.1.4/python_agent/packages/astor/file_util.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astor/source_repr.py` & `sealights-python-agent-1.1.4/python_agent/packages/astor/source_repr.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astor/node_util.py` & `sealights-python-agent-1.1.4/python_agent/packages/astor/node_util.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astor/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/astor/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astor/rtrip.py` & `sealights-python-agent-1.1.4/python_agent/packages/astor/rtrip.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astor/tree_walk.py` & `sealights-python-agent-1.1.4/python_agent/packages/astor/tree_walk.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/astor/op_util.py` & `sealights-python-agent-1.1.4/python_agent/packages/astor/op_util.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/typing_extensions.py` & `sealights-python-agent-1.1.4/python_agent/packages/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_adapters.py` & `sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_text.py` & `sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_collections.py` & `sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_compat.py` & `sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_functools.py` & `sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_meta.py` & `sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/_itertools.py` & `sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/importlib_metadata/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/zipp.py` & `sealights-python-agent-1.1.4/python_agent/packages/zipp.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/_textwrap.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/exceptions.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/testing.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/testing.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/types.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/types.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/_termui_impl.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/_compat.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/_compat.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/_unicodefun.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/_winconsole.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/globals.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/globals.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/utils.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/parser.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/parser.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/core.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/core.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/decorators.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/decorators.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/formatting.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/formatting.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/shell_completion.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/shell_completion.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/click/termui.py` & `sealights-python-agent-1.1.4/python_agent/packages/click/termui.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/cd.py` & `sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/legacy.py` & `sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/models.py` & `sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/assets/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/cli/normalizer.py` & `sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/cli/normalizer.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/api.py` & `sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/md.py` & `sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/utils.py` & `sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/charset_normalizer/constant.py` & `sealights-python-agent-1.1.4/python_agent/packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/semantic_version/base.py` & `sealights-python-agent-1.1.4/python_agent/packages/semantic_version/base.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/semantic_version/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/semantic_version/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/semantic_version/django_fields.py` & `sealights-python-agent-1.1.4/python_agent/packages/semantic_version/django_fields.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/idna/codec.py` & `sealights-python-agent-1.1.4/python_agent/packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/idna/intranges.py` & `sealights-python-agent-1.1.4/python_agent/packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/idna/uts46data.py` & `sealights-python-agent-1.1.4/python_agent/packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/idna/idnadata.py` & `sealights-python-agent-1.1.4/python_agent/packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/idna/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/idna/core.py` & `sealights-python-agent-1.1.4/python_agent/packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/exceptions.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/response.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/fields.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/connectionpool.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/poolmanager.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/_collections.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/filepost.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/connection.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/ssl_match_hostname.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/ssltransport.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/response.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/proxy.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/ssl_.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/wait.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/timeout.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/connection.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/request.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/retry.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/util/url.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/request.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/ntlmpool.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/_securetransport/low_level.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/_securetransport/bindings.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/securetransport.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/pyopenssl.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/_appengine_environ.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/appengine.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/contrib/socks.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/__init__.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/packages/six.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/urllib3/packages/backports/makefile.py` & `sealights-python-agent-1.1.4/python_agent/packages/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/python_agent/packages/freezegun/api.py` & `sealights-python-agent-1.1.4/python_agent/packages/freezegun/api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/LICENSE.txt` & `sealights-python-agent-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/sealights_python_agent.egg-info/SOURCES.txt` & `sealights-python-agent-1.1.4/sealights_python_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/sealights_python_agent.egg-info/requires.txt` & `sealights-python-agent-1.1.4/sealights_python_agent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/sealights_python_agent.egg-info/PKG-INFO` & `sealights-python-agent-1.1.4/sealights_python_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sealights-python-agent
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python Agent
 Home-page: https://github.com/Sealights/SL.OnPremise.Agents.Python
 Author: Shai Cantor
 Author-email: shai@sealights.io
 License: Other/Proprietary License
 Keywords: sealights python agent setuptools development
 Platform: UNKNOWN
```

### Comparing `sealights-python-agent-1.1.3/requirements.txt` & `sealights-python-agent-1.1.4/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 GitPython==3.1.18;python_version<"3.6.8"
 ####################
 gitdb==4.0.9
 smmap==5.0.0
 typing-extensions==4.1.1;python_version<"3.8"
 
 unittest_xml_reporting==3.1.0
+
 lxml==4.9.1;python_version<"3.6.8"
```

### Comparing `sealights-python-agent-1.1.3/CHANGES.rst` & `sealights-python-agent-1.1.4/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/README.rst` & `sealights-python-agent-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.1.3/PKG-INFO` & `sealights-python-agent-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sealights-python-agent
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python Agent
 Home-page: https://github.com/Sealights/SL.OnPremise.Agents.Python
 Author: Shai Cantor
 Author-email: shai@sealights.io
 License: Other/Proprietary License
 Keywords: sealights python agent setuptools development
 Platform: UNKNOWN
```

### Comparing `sealights-python-agent-1.1.3/setup.py` & `sealights-python-agent-1.1.4/setup.py`

 * *Files identical despite different names*

