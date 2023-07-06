# Comparing `tmp/overhave-4.0.4.tar.gz` & `tmp/overhave-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overhave-4.0.4.tar", max compression
+gzip compressed data, was "overhave-4.0.5.tar", max compression
```

## Comparing `overhave-4.0.4.tar` & `overhave-4.0.5.tar`

### file list

```diff
@@ -1,245 +1,245 @@
--rw-r--r--   0        0        0    23136 2023-07-05 12:19:16.107698 overhave-4.0.4/README.rst
--rw-r--r--   0        0        0     3193 2023-07-05 12:19:16.119699 overhave-4.0.4/overhave/__init__.py
--rw-r--r--   0        0        0       63 2023-07-05 12:19:16.119699 overhave-4.0.4/overhave/admin/__init__.py
--rw-r--r--   0        0        0     5172 2023-07-05 12:19:16.119699 overhave-4.0.4/overhave/admin/app.py
--rw-r--r--   0        0        0   735118 2023-07-05 12:19:16.123700 overhave-4.0.4/overhave/admin/files/ace-src/ace.js
--rw-r--r--   0        0        0     5426 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/files/ace-src/mode-gherkin.js
--rw-r--r--   0        0        0     1263 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/files/css/overhave.css
--rw-r--r--   0        0        0    38062 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/files/favicon.ico
--rw-r--r--   0        0        0      138 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/flask/__init__.py
--rw-r--r--   0        0        0     1819 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/flask/flask_admin.py
--rw-r--r--   0        0        0      287 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/flask/flask_app.py
--rw-r--r--   0        0        0     2134 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/flask/login_manager.py
--rw-r--r--   0        0        0      187 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/draft_detail.html
--rw-r--r--   0        0        0      405 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/emulation.html
--rw-r--r--   0        0        0      194 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/emulation_create.html
--rw-r--r--   0        0        0      190 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/emulation_edit.html
--rw-r--r--   0        0        0      860 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/emulation_run_detail.html
--rw-r--r--   0        0        0    10071 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/feature.html
--rw-r--r--   0        0        0      404 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/feature_create.html
--rw-r--r--   0        0        0      465 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/feature_edit.html
--rw-r--r--   0        0        0      177 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/index.html
--rw-r--r--   0        0        0     2414 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/login.html
--rw-r--r--   0        0        0      149 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/overhave_master.html
--rw-r--r--   0        0        0     1696 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/test_run.html
--rw-r--r--   0        0        0     1535 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/test_run_detail.html
--rw-r--r--   0        0        0      189 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/test_run_list.html
--rw-r--r--   0        0        0      606 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/test_user.html
--rw-r--r--   0        0        0      210 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/test_user_create.html
--rw-r--r--   0        0        0      208 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/templates/test_user_edit.html
--rw-r--r--   0        0        0      451 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/__init__.py
--rw-r--r--   0        0        0     1386 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/access.py
--rw-r--r--   0        0        0     2914 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/base.py
--rw-r--r--   0        0        0     1105 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/draft.py
--rw-r--r--   0        0        0     3407 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/emulation.py
--rw-r--r--   0        0        0     1620 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/emulation_run.py
--rw-r--r--   0        0        0    10257 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/feature.py
--rw-r--r--   0        0        0      306 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/formatters/__init__.py
--rw-r--r--   0        0        0     4997 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/formatters/formatters.py
--rw-r--r--   0        0        0      631 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/formatters/helpers.py
--rw-r--r--   0        0        0     1404 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/formatters/safe_formatter.py
--rw-r--r--   0        0        0       51 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/index/__init__.py
--rw-r--r--   0        0        0     1648 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/index/custom_page.py
--rw-r--r--   0        0        0     1578 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/index/login_form.py
--rw-r--r--   0        0        0     2645 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/index/view.py
--rw-r--r--   0        0        0     1794 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/scenario_test_run.py
--rw-r--r--   0        0        0     1329 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/tag.py
--rw-r--r--   0        0        0     3665 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/admin/views/testing_users.py
--rw-r--r--   0        0        0       52 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/__init__.py
--rw-r--r--   0        0        0     5970 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/app.py
--rw-r--r--   0        0        0      216 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/asgi.py
--rw-r--r--   0        0        0      143 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/auth/__init__.py
--rw-r--r--   0        0        0      348 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/auth/models.py
--rw-r--r--   0        0        0     1271 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/auth/regular.py
--rw-r--r--   0        0        0      867 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/auth/token.py
--rw-r--r--   0        0        0     2422 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/deps.py
--rw-r--r--   0        0        0      848 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/settings.py
--rw-r--r--   0        0        0      580 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/views/__init__.py
--rw-r--r--   0        0        0     1304 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/views/auth_views.py
--rw-r--r--   0        0        0      550 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/views/emulation_views.py
--rw-r--r--   0        0        0      586 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/views/extra_views.py
--rw-r--r--   0        0        0      461 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/views/feature_type_views.py
--rw-r--r--   0        0        0     1184 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/views/feature_views.py
--rw-r--r--   0        0        0      969 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/views/tags_views.py
--rw-r--r--   0        0        0     2041 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/views/testrun_views.py
--rw-r--r--   0        0        0     4486 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/api/views/testuser_views.py
--rw-r--r--   0        0        0     4047 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/base_settings.py
--rw-r--r--   0        0        0      164 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/cli/__init__.py
--rw-r--r--   0        0        0      557 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/cli/admin.py
--rw-r--r--   0        0        0      534 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/cli/api.py
--rw-r--r--   0        0        0      647 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/cli/consumers.py
--rw-r--r--   0        0        0       84 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/cli/db_cmds/__init__.py
--rw-r--r--   0        0        0      830 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/cli/db_cmds/group.py
--rw-r--r--   0        0        0     1755 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/cli/db_cmds/regular.py
--rw-r--r--   0        0        0      358 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/cli/group.py
--rw-r--r--   0        0        0     3048 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/cli/s3.py
--rw-r--r--   0        0        0     1573 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/cli/synchronizer.py
--rw-r--r--   0        0        0      455 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/db/__init__.py
--rw-r--r--   0        0        0     3283 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/db/base.py
--rw-r--r--   0        0        0     1349 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/db/statuses.py
--rw-r--r--   0        0        0     8141 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/db/tables.py
--rw-r--r--   0        0        0      795 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/db/users.py
--rw-r--r--   0        0        0     1249 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/db/utils.py
--rw-r--r--   0        0        0       46 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/emulation/__init__.py
--rw-r--r--   0        0        0     4103 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/emulation/emulator.py
--rw-r--r--   0        0        0      897 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/entities/__init__.py
--rw-r--r--   0        0        0     1231 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/entities/archiver.py
--rw-r--r--   0        0        0      247 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/entities/auth_managers/__init__.py
--rw-r--r--   0        0        0      316 2023-07-05 12:19:16.127700 overhave-4.0.4/overhave/entities/auth_managers/abstract.py
--rw-r--r--   0        0        0      497 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/auth_managers/base.py
--rw-r--r--   0        0        0      557 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/auth_managers/default.py
--rw-r--r--   0        0        0      116 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/auth_managers/ldap/__init__.py
--rw-r--r--   0        0        0     2891 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/auth_managers/ldap/manager.py
--rw-r--r--   0        0        0      198 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/auth_managers/ldap/settings.py
--rw-r--r--   0        0        0     1394 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/auth_managers/secret_mixin.py
--rw-r--r--   0        0        0     1258 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/auth_managers/simple.py
--rw-r--r--   0        0        0      169 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/feature/__init__.py
--rw-r--r--   0        0        0      425 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/feature/abstract.py
--rw-r--r--   0        0        0      221 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/feature/errors.py
--rw-r--r--   0        0        0     2748 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/feature/extractor.py
--rw-r--r--   0        0        0     1098 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/file_extractor.py
--rw-r--r--   0        0        0     1760 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/git_initializer.py
--rw-r--r--   0        0        0       55 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/language/__init__.py
--rw-r--r--   0        0        0     1198 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/language/prefixes.py
--rw-r--r--   0        0        0      102 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/report_manager/__init__.py
--rw-r--r--   0        0        0      415 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/report_manager/models.py
--rw-r--r--   0        0        0     5825 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/report_manager/report_manager.py
--rw-r--r--   0        0        0     6633 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/entities/settings.py
--rw-r--r--   0        0        0       54 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/extra/__init__.py
--rw-r--r--   0        0        0      386 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/extra/prefixes.py
--rw-r--r--   0        0        0      739 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/__init__.py
--rw-r--r--   0        0        0     7209 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/base_factory.py
--rw-r--r--   0        0        0      418 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/components/__init__.py
--rw-r--r--   0        0        0      306 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/components/abstract_consumer.py
--rw-r--r--   0        0        0     4555 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/components/admin_factory.py
--rw-r--r--   0        0        0     1312 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/components/emulation_factory.py
--rw-r--r--   0        0        0     3960 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/components/publication_factory.py
--rw-r--r--   0        0        0      486 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/components/s3_init_factory.py
--rw-r--r--   0        0        0     2184 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/components/synchronizer_factory.py
--rw-r--r--   0        0        0     1888 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/components/test_execution_factory.py
--rw-r--r--   0        0        0     2045 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/consumer_factory.py
--rw-r--r--   0        0        0      550 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/context/__init__.py
--rw-r--r--   0        0        0     2950 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/context/admin_context.py
--rw-r--r--   0        0        0     4028 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/context/base_context.py
--rw-r--r--   0        0        0      506 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/context/emulation_context.py
--rw-r--r--   0        0        0     2032 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/context/publication_context.py
--rw-r--r--   0        0        0     1288 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/context/synchronizer_context.py
--rw-r--r--   0        0        0     2519 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/context/test_execution_context.py
--rw-r--r--   0        0        0      769 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/factory/getters.py
--rw-r--r--   0        0        0      353 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/metrics/__init__.py
--rw-r--r--   0        0        0      193 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/metrics/client/__init__.py
--rw-r--r--   0        0        0     3140 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/metrics/client/container.py
--rw-r--r--   0        0        0      983 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/metrics/getters.py
--rw-r--r--   0        0        0      342 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/__init__.py
--rw-r--r--   0        0        0      399 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/abstract_publisher.py
--rw-r--r--   0        0        0     4126 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/base_publisher.py
--rw-r--r--   0        0        0      532 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/errors.py
--rw-r--r--   0        0        0     5036 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/git_publisher.py
--rw-r--r--   0        0        0      224 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/gitlab/__init__.py
--rw-r--r--   0        0        0     4316 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/gitlab/gitlab_publisher.py
--rw-r--r--   0        0        0     1408 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/gitlab/settings.py
--rw-r--r--   0        0        0      171 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/gitlab/tokenizer/__init__.py
--rw-r--r--   0        0        0     2157 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/gitlab/tokenizer/client.py
--rw-r--r--   0        0        0     1015 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/gitlab/tokenizer/settings.py
--rw-r--r--   0        0        0      178 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/objects.py
--rw-r--r--   0        0        0      877 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/settings.py
--rw-r--r--   0        0        0      119 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/stash/__init__.py
--rw-r--r--   0        0        0     1672 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/stash/settings.py
--rw-r--r--   0        0        0     4431 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/publication/stash/stash_publisher.py
--rw-r--r--   0        0        0      371 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/__init__.py
--rw-r--r--   0        0        0     3538 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/config_injector.py
--rw-r--r--   0        0        0      827 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/deps.py
--rw-r--r--   0        0        0      530 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/helpers/__init__.py
--rw-r--r--   0        0        0      305 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/helpers/allure_utils/__init__.py
--rw-r--r--   0        0        0      927 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
--rw-r--r--   0        0        0     1102 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/helpers/allure_utils/links.py
--rw-r--r--   0        0        0     1260 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/helpers/allure_utils/severity.py
--rw-r--r--   0        0        0     2452 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
--rw-r--r--   0        0        0     1638 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/helpers/bdd_item.py
--rw-r--r--   0        0        0      981 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/helpers/parsed_info.py
--rw-r--r--   0        0        0     2874 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/helpers/tag_controller.py
--rw-r--r--   0        0        0     6192 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/plugin.py
--rw-r--r--   0        0        0     2223 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/plugin_resolver.py
--rw-r--r--   0        0        0     3945 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/pytest_plugin/proxy_manager.py
--rw-r--r--   0        0        0      517 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/__init__.py
--rw-r--r--   0        0        0      157 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/compiler/__init__.py
--rw-r--r--   0        0        0     5173 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/compiler/compiler.py
--rw-r--r--   0        0        0      631 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/compiler/settings.py
--rw-r--r--   0        0        0      150 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/file_manager/__init__.py
--rw-r--r--   0        0        0     3495 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/file_manager/file_manager.py
--rw-r--r--   0        0        0     2820 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/file_manager/settings.py
--rw-r--r--   0        0        0      230 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/parser/__init__.py
--rw-r--r--   0        0        0      854 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/parser/models.py
--rw-r--r--   0        0        0     8442 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/parser/parser.py
--rw-r--r--   0        0        0      263 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/parser/settings.py
--rw-r--r--   0        0        0      235 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/prefix_mixin.py
--rw-r--r--   0        0        0       95 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/validator/__init__.py
--rw-r--r--   0        0        0      229 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/validator/abstract.py
--rw-r--r--   0        0        0     1441 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/validator/duplicate_id_mixin.py
--rw-r--r--   0        0        0      510 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/validator/errors.py
--rw-r--r--   0        0        0     2827 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/scenario/validator/validator.py
--rw-r--r--   0        0        0     1226 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/storage/__init__.py
--rw-r--r--   0        0        0     1180 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/storage/api_auth_storage.py
--rw-r--r--   0        0        0     3271 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/storage/converters.py
--rw-r--r--   0        0        0     6178 2023-07-05 12:19:16.131700 overhave-4.0.4/overhave/storage/draft_storage.py
--rw-r--r--   0        0        0     5323 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/storage/emulation_storage.py
--rw-r--r--   0        0        0     4947 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/storage/feature_storage.py
--rw-r--r--   0        0        0     1566 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/storage/feature_tag_storage.py
--rw-r--r--   0        0        0     2176 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/storage/feature_type_storage.py
--rw-r--r--   0        0        0     1902 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/storage/scenario_storage.py
--rw-r--r--   0        0        0      593 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/storage/system_user_group_storage.py
--rw-r--r--   0        0        0     2464 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/storage/system_user_storage.py
--rw-r--r--   0        0        0     3054 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/storage/test_run_storage.py
--rw-r--r--   0        0        0     4451 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/storage/test_user_storage.py
--rw-r--r--   0        0        0      192 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/synchronization/__init__.py
--rw-r--r--   0        0        0      260 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/synchronization/abstract.py
--rw-r--r--   0        0        0     3702 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/synchronization/storage_manager.py
--rw-r--r--   0        0        0     6973 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/synchronization/synchronizer.py
--rw-r--r--   0        0        0      307 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/test_execution/__init__.py
--rw-r--r--   0        0        0     4256 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/test_execution/executor.py
--rw-r--r--   0        0        0     1056 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/test_execution/objects.py
--rw-r--r--   0        0        0     1750 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/test_execution/settings.py
--rw-r--r--   0        0        0     4106 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/test_execution/step_collector.py
--rw-r--r--   0        0        0     1617 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/test_execution/test_runner.py
--rw-r--r--   0        0        0      983 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/__init__.py
--rw-r--r--   0        0        0      623 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/__init__.py
--rw-r--r--   0        0        0      122 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/api_client/__init__.py
--rw-r--r--   0        0        0     1810 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/api_client/authenticator.py
--rw-r--r--   0        0        0      237 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/api_client/models.py
--rw-r--r--   0        0        0      499 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/api_client/settings.py
--rw-r--r--   0        0        0      208 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/base_client/__init__.py
--rw-r--r--   0        0        0      590 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/base_client/auth.py
--rw-r--r--   0        0        0     2139 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/base_client/client.py
--rw-r--r--   0        0        0      110 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/base_client/objects.py
--rw-r--r--   0        0        0     1287 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/base_client/settings.py
--rw-r--r--   0        0        0      258 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/gitlab_client/__init__.py
--rw-r--r--   0        0        0     2003 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/gitlab_client/client.py
--rw-r--r--   0        0        0      609 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/gitlab_client/models.py
--rw-r--r--   0        0        0      144 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/gitlab_client/objects.py
--rw-r--r--   0        0        0      377 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/gitlab_client/settings.py
--rw-r--r--   0        0        0      741 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/gitlab_client/utils.py
--rw-r--r--   0        0        0      326 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/stash_client/__init__.py
--rw-r--r--   0        0        0     2115 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/stash_client/client.py
--rw-r--r--   0        0        0     2757 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/stash_client/models.py
--rw-r--r--   0        0        0      569 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/http/stash_client/settings.py
--rw-r--r--   0        0        0      109 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/ldap/__init__.py
--rw-r--r--   0        0        0     1896 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/ldap/authenticator.py
--rw-r--r--   0        0        0      420 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/ldap/settings.py
--rw-r--r--   0        0        0      430 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/redis/__init__.py
--rw-r--r--   0        0        0     2937 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/redis/consumer.py
--rw-r--r--   0        0        0     1661 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/redis/deps.py
--rw-r--r--   0        0        0     2439 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/redis/objects.py
--rw-r--r--   0        0        0     1319 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/redis/producer.py
--rw-r--r--   0        0        0     1384 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/redis/runner.py
--rw-r--r--   0        0        0     1674 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/redis/settings.py
--rw-r--r--   0        0        0      132 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/s3/__init__.py
--rw-r--r--   0        0        0     8494 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/s3/manager.py
--rw-r--r--   0        0        0     2082 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/s3/models.py
--rw-r--r--   0        0        0      181 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/s3/objects.py
--rw-r--r--   0        0        0      885 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/transport/s3/settings.py
--rw-r--r--   0        0        0      103 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/utils/__init__.py
--rw-r--r--   0        0        0       84 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/utils/mocks.py
--rw-r--r--   0        0        0      139 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/utils/time.py
--rw-r--r--   0        0        0      148 2023-07-05 12:19:16.135701 overhave-4.0.4/overhave/utils/url.py
--rw-r--r--   0        0        0     3522 2023-07-05 12:19:16.135701 overhave-4.0.4/pyproject.toml
--rw-r--r--   0        0        0    25392 1970-01-01 00:00:00.000000 overhave-4.0.4/PKG-INFO
+-rw-r--r--   0        0        0    23136 2023-07-06 06:26:56.936672 overhave-4.0.5/README.rst
+-rw-r--r--   0        0        0     3193 2023-07-06 06:26:56.948672 overhave-4.0.5/overhave/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-06 06:26:56.948672 overhave-4.0.5/overhave/admin/__init__.py
+-rw-r--r--   0        0        0     5172 2023-07-06 06:26:56.948672 overhave-4.0.5/overhave/admin/app.py
+-rw-r--r--   0        0        0   735118 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/files/ace-src/ace.js
+-rw-r--r--   0        0        0     5426 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/files/ace-src/mode-gherkin.js
+-rw-r--r--   0        0        0     1263 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/files/css/overhave.css
+-rw-r--r--   0        0        0    38062 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/files/favicon.ico
+-rw-r--r--   0        0        0      138 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/flask/__init__.py
+-rw-r--r--   0        0        0     1819 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/flask/flask_admin.py
+-rw-r--r--   0        0        0      287 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/flask/flask_app.py
+-rw-r--r--   0        0        0     2134 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/flask/login_manager.py
+-rw-r--r--   0        0        0      187 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/draft_detail.html
+-rw-r--r--   0        0        0      405 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/emulation.html
+-rw-r--r--   0        0        0      194 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/emulation_create.html
+-rw-r--r--   0        0        0      190 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/emulation_edit.html
+-rw-r--r--   0        0        0      860 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/emulation_run_detail.html
+-rw-r--r--   0        0        0    10071 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/feature.html
+-rw-r--r--   0        0        0      404 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/feature_create.html
+-rw-r--r--   0        0        0      465 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/feature_edit.html
+-rw-r--r--   0        0        0      177 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/index.html
+-rw-r--r--   0        0        0     2414 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/login.html
+-rw-r--r--   0        0        0      149 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/overhave_master.html
+-rw-r--r--   0        0        0     1696 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_run.html
+-rw-r--r--   0        0        0     1535 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_run_detail.html
+-rw-r--r--   0        0        0      189 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_run_list.html
+-rw-r--r--   0        0        0      606 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_user.html
+-rw-r--r--   0        0        0      210 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_user_create.html
+-rw-r--r--   0        0        0      208 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/templates/test_user_edit.html
+-rw-r--r--   0        0        0      451 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/__init__.py
+-rw-r--r--   0        0        0     1386 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/access.py
+-rw-r--r--   0        0        0     2914 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/base.py
+-rw-r--r--   0        0        0     1105 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/draft.py
+-rw-r--r--   0        0        0     3407 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/emulation.py
+-rw-r--r--   0        0        0     1620 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/emulation_run.py
+-rw-r--r--   0        0        0    10257 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/feature.py
+-rw-r--r--   0        0        0      306 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/formatters/__init__.py
+-rw-r--r--   0        0        0     4997 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/formatters/formatters.py
+-rw-r--r--   0        0        0      631 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/formatters/helpers.py
+-rw-r--r--   0        0        0     1404 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/formatters/safe_formatter.py
+-rw-r--r--   0        0        0       51 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/index/__init__.py
+-rw-r--r--   0        0        0     1648 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/index/custom_page.py
+-rw-r--r--   0        0        0     1578 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/index/login_form.py
+-rw-r--r--   0        0        0     2645 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/index/view.py
+-rw-r--r--   0        0        0     1794 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/scenario_test_run.py
+-rw-r--r--   0        0        0     1329 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/tag.py
+-rw-r--r--   0        0        0     3665 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/admin/views/testing_users.py
+-rw-r--r--   0        0        0       52 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/api/__init__.py
+-rw-r--r--   0        0        0     5970 2023-07-06 06:26:56.952672 overhave-4.0.5/overhave/api/app.py
+-rw-r--r--   0        0        0      216 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/asgi.py
+-rw-r--r--   0        0        0      143 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/auth/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/auth/models.py
+-rw-r--r--   0        0        0     1271 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/auth/regular.py
+-rw-r--r--   0        0        0      867 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/auth/token.py
+-rw-r--r--   0        0        0     2422 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/deps.py
+-rw-r--r--   0        0        0      848 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/settings.py
+-rw-r--r--   0        0        0      580 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/__init__.py
+-rw-r--r--   0        0        0     1304 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/auth_views.py
+-rw-r--r--   0        0        0      550 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/emulation_views.py
+-rw-r--r--   0        0        0      586 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/extra_views.py
+-rw-r--r--   0        0        0      461 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/feature_type_views.py
+-rw-r--r--   0        0        0     1184 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/feature_views.py
+-rw-r--r--   0        0        0      969 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/tags_views.py
+-rw-r--r--   0        0        0     2041 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/testrun_views.py
+-rw-r--r--   0        0        0     4486 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/api/views/testuser_views.py
+-rw-r--r--   0        0        0     4047 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/base_settings.py
+-rw-r--r--   0        0        0      164 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/__init__.py
+-rw-r--r--   0        0        0      557 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/admin.py
+-rw-r--r--   0        0        0      534 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/api.py
+-rw-r--r--   0        0        0      647 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/consumers.py
+-rw-r--r--   0        0        0       84 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/db_cmds/__init__.py
+-rw-r--r--   0        0        0      830 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/db_cmds/group.py
+-rw-r--r--   0        0        0     1755 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/db_cmds/regular.py
+-rw-r--r--   0        0        0      358 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/group.py
+-rw-r--r--   0        0        0     3048 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/s3.py
+-rw-r--r--   0        0        0     1573 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/cli/synchronizer.py
+-rw-r--r--   0        0        0      455 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/__init__.py
+-rw-r--r--   0        0        0     3283 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/base.py
+-rw-r--r--   0        0        0     1349 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/statuses.py
+-rw-r--r--   0        0        0     8141 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/tables.py
+-rw-r--r--   0        0        0      795 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/users.py
+-rw-r--r--   0        0        0     1249 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/db/utils.py
+-rw-r--r--   0        0        0       46 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/emulation/__init__.py
+-rw-r--r--   0        0        0     4103 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/emulation/emulator.py
+-rw-r--r--   0        0        0      897 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/__init__.py
+-rw-r--r--   0        0        0     1231 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/archiver.py
+-rw-r--r--   0        0        0      247 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/__init__.py
+-rw-r--r--   0        0        0      316 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/abstract.py
+-rw-r--r--   0        0        0      497 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/base.py
+-rw-r--r--   0        0        0      557 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/default.py
+-rw-r--r--   0        0        0      116 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/ldap/__init__.py
+-rw-r--r--   0        0        0     2891 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/ldap/manager.py
+-rw-r--r--   0        0        0      198 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/ldap/settings.py
+-rw-r--r--   0        0        0     1394 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/secret_mixin.py
+-rw-r--r--   0        0        0     1258 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/auth_managers/simple.py
+-rw-r--r--   0        0        0      169 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/feature/__init__.py
+-rw-r--r--   0        0        0      425 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/feature/abstract.py
+-rw-r--r--   0        0        0      221 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/feature/errors.py
+-rw-r--r--   0        0        0     2748 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/feature/extractor.py
+-rw-r--r--   0        0        0     1098 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/file_extractor.py
+-rw-r--r--   0        0        0     1760 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/git_initializer.py
+-rw-r--r--   0        0        0       55 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/language/__init__.py
+-rw-r--r--   0        0        0     1198 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/language/prefixes.py
+-rw-r--r--   0        0        0      102 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/report_manager/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/report_manager/models.py
+-rw-r--r--   0        0        0     5825 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/report_manager/report_manager.py
+-rw-r--r--   0        0        0     6633 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/entities/settings.py
+-rw-r--r--   0        0        0       54 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/extra/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/extra/prefixes.py
+-rw-r--r--   0        0        0      739 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/__init__.py
+-rw-r--r--   0        0        0     7209 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/base_factory.py
+-rw-r--r--   0        0        0      418 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/__init__.py
+-rw-r--r--   0        0        0      306 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/abstract_consumer.py
+-rw-r--r--   0        0        0     4555 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/admin_factory.py
+-rw-r--r--   0        0        0     1312 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/emulation_factory.py
+-rw-r--r--   0        0        0     3956 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/publication_factory.py
+-rw-r--r--   0        0        0      486 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/s3_init_factory.py
+-rw-r--r--   0        0        0     2184 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/synchronizer_factory.py
+-rw-r--r--   0        0        0     1888 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/components/test_execution_factory.py
+-rw-r--r--   0        0        0     2045 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/consumer_factory.py
+-rw-r--r--   0        0        0      550 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/__init__.py
+-rw-r--r--   0        0        0     2950 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/admin_context.py
+-rw-r--r--   0        0        0     4028 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/base_context.py
+-rw-r--r--   0        0        0      506 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/emulation_context.py
+-rw-r--r--   0        0        0     2032 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/publication_context.py
+-rw-r--r--   0        0        0     1288 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/synchronizer_context.py
+-rw-r--r--   0        0        0     2519 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/context/test_execution_context.py
+-rw-r--r--   0        0        0      769 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/factory/getters.py
+-rw-r--r--   0        0        0      353 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/metrics/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/metrics/client/__init__.py
+-rw-r--r--   0        0        0     3140 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/metrics/client/container.py
+-rw-r--r--   0        0        0      983 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/metrics/getters.py
+-rw-r--r--   0        0        0      342 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/__init__.py
+-rw-r--r--   0        0        0      399 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/abstract_publisher.py
+-rw-r--r--   0        0        0     4015 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/base_publisher.py
+-rw-r--r--   0        0        0      532 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/errors.py
+-rw-r--r--   0        0        0     4928 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/git_publisher.py
+-rw-r--r--   0        0        0      224 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/__init__.py
+-rw-r--r--   0        0        0     4208 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/gitlab_publisher.py
+-rw-r--r--   0        0        0     1408 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/settings.py
+-rw-r--r--   0        0        0      171 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/tokenizer/__init__.py
+-rw-r--r--   0        0        0     2157 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/tokenizer/client.py
+-rw-r--r--   0        0        0     1015 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/gitlab/tokenizer/settings.py
+-rw-r--r--   0        0        0      178 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/objects.py
+-rw-r--r--   0        0        0      877 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/settings.py
+-rw-r--r--   0        0        0      119 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/stash/__init__.py
+-rw-r--r--   0        0        0     1672 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/stash/settings.py
+-rw-r--r--   0        0        0     4323 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/publication/stash/stash_publisher.py
+-rw-r--r--   0        0        0      371 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0     3538 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/config_injector.py
+-rw-r--r--   0        0        0      827 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/deps.py
+-rw-r--r--   0        0        0      530 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/__init__.py
+-rw-r--r--   0        0        0      305 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/__init__.py
+-rw-r--r--   0        0        0      927 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
+-rw-r--r--   0        0        0     1102 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/links.py
+-rw-r--r--   0        0        0     1260 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/severity.py
+-rw-r--r--   0        0        0     2452 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
+-rw-r--r--   0        0        0     1638 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/bdd_item.py
+-rw-r--r--   0        0        0      981 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/parsed_info.py
+-rw-r--r--   0        0        0     2874 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/helpers/tag_controller.py
+-rw-r--r--   0        0        0     6192 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/plugin.py
+-rw-r--r--   0        0        0     2223 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/plugin_resolver.py
+-rw-r--r--   0        0        0     3945 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/pytest_plugin/proxy_manager.py
+-rw-r--r--   0        0        0      517 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/scenario/__init__.py
+-rw-r--r--   0        0        0      157 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/scenario/compiler/__init__.py
+-rw-r--r--   0        0        0     5173 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/scenario/compiler/compiler.py
+-rw-r--r--   0        0        0      631 2023-07-06 06:26:56.956672 overhave-4.0.5/overhave/scenario/compiler/settings.py
+-rw-r--r--   0        0        0      150 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/file_manager/__init__.py
+-rw-r--r--   0        0        0     3495 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/file_manager/file_manager.py
+-rw-r--r--   0        0        0     2820 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/file_manager/settings.py
+-rw-r--r--   0        0        0      230 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/parser/__init__.py
+-rw-r--r--   0        0        0      854 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/parser/models.py
+-rw-r--r--   0        0        0     8442 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/parser/parser.py
+-rw-r--r--   0        0        0      263 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/parser/settings.py
+-rw-r--r--   0        0        0      235 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/prefix_mixin.py
+-rw-r--r--   0        0        0       95 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/validator/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/validator/abstract.py
+-rw-r--r--   0        0        0     1441 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/validator/duplicate_id_mixin.py
+-rw-r--r--   0        0        0      510 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/validator/errors.py
+-rw-r--r--   0        0        0     2827 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/scenario/validator/validator.py
+-rw-r--r--   0        0        0     1226 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/__init__.py
+-rw-r--r--   0        0        0     1180 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/api_auth_storage.py
+-rw-r--r--   0        0        0     3271 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/converters.py
+-rw-r--r--   0        0        0     6178 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/draft_storage.py
+-rw-r--r--   0        0        0     5323 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/emulation_storage.py
+-rw-r--r--   0        0        0     4947 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/feature_storage.py
+-rw-r--r--   0        0        0     1566 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/feature_tag_storage.py
+-rw-r--r--   0        0        0     2176 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/feature_type_storage.py
+-rw-r--r--   0        0        0     1902 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/scenario_storage.py
+-rw-r--r--   0        0        0      593 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/system_user_group_storage.py
+-rw-r--r--   0        0        0     2464 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/system_user_storage.py
+-rw-r--r--   0        0        0     3054 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/test_run_storage.py
+-rw-r--r--   0        0        0     4451 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/storage/test_user_storage.py
+-rw-r--r--   0        0        0      192 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/synchronization/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/synchronization/abstract.py
+-rw-r--r--   0        0        0     3702 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/synchronization/storage_manager.py
+-rw-r--r--   0        0        0     6973 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/synchronization/synchronizer.py
+-rw-r--r--   0        0        0      307 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/__init__.py
+-rw-r--r--   0        0        0     4256 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/executor.py
+-rw-r--r--   0        0        0     1056 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/objects.py
+-rw-r--r--   0        0        0     1750 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/settings.py
+-rw-r--r--   0        0        0     4106 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/step_collector.py
+-rw-r--r--   0        0        0     1617 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/test_execution/test_runner.py
+-rw-r--r--   0        0        0      983 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/__init__.py
+-rw-r--r--   0        0        0      623 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/__init__.py
+-rw-r--r--   0        0        0      122 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/api_client/__init__.py
+-rw-r--r--   0        0        0     1810 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/api_client/authenticator.py
+-rw-r--r--   0        0        0      237 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/api_client/models.py
+-rw-r--r--   0        0        0      499 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/api_client/settings.py
+-rw-r--r--   0        0        0      208 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/base_client/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/base_client/auth.py
+-rw-r--r--   0        0        0     2139 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/base_client/client.py
+-rw-r--r--   0        0        0      110 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/base_client/objects.py
+-rw-r--r--   0        0        0     1287 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/base_client/settings.py
+-rw-r--r--   0        0        0      258 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/__init__.py
+-rw-r--r--   0        0        0     2003 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/client.py
+-rw-r--r--   0        0        0      609 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/models.py
+-rw-r--r--   0        0        0      144 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/objects.py
+-rw-r--r--   0        0        0      377 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/settings.py
+-rw-r--r--   0        0        0      741 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/gitlab_client/utils.py
+-rw-r--r--   0        0        0      326 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/stash_client/__init__.py
+-rw-r--r--   0        0        0     2115 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/stash_client/client.py
+-rw-r--r--   0        0        0     2757 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/stash_client/models.py
+-rw-r--r--   0        0        0      569 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/http/stash_client/settings.py
+-rw-r--r--   0        0        0      109 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/ldap/__init__.py
+-rw-r--r--   0        0        0     1896 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/ldap/authenticator.py
+-rw-r--r--   0        0        0      420 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/ldap/settings.py
+-rw-r--r--   0        0        0      430 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/__init__.py
+-rw-r--r--   0        0        0     2937 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/consumer.py
+-rw-r--r--   0        0        0     1661 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/deps.py
+-rw-r--r--   0        0        0     2439 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/objects.py
+-rw-r--r--   0        0        0     1319 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/producer.py
+-rw-r--r--   0        0        0     1384 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/runner.py
+-rw-r--r--   0        0        0     1674 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/redis/settings.py
+-rw-r--r--   0        0        0      132 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/s3/__init__.py
+-rw-r--r--   0        0        0     8494 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/s3/manager.py
+-rw-r--r--   0        0        0     2082 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/s3/models.py
+-rw-r--r--   0        0        0      181 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/s3/objects.py
+-rw-r--r--   0        0        0      885 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/transport/s3/settings.py
+-rw-r--r--   0        0        0      103 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/utils/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/utils/mocks.py
+-rw-r--r--   0        0        0      139 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/utils/time.py
+-rw-r--r--   0        0        0      148 2023-07-06 06:26:56.960672 overhave-4.0.5/overhave/utils/url.py
+-rw-r--r--   0        0        0     3522 2023-07-06 06:26:56.960672 overhave-4.0.5/pyproject.toml
+-rw-r--r--   0        0        0    25392 1970-01-01 00:00:00.000000 overhave-4.0.5/PKG-INFO
```

### Comparing `overhave-4.0.4/README.rst` & `overhave-4.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/__init__.py` & `overhave-4.0.5/overhave/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/app.py` & `overhave-4.0.5/overhave/admin/app.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/files/ace-src/ace.js` & `overhave-4.0.5/overhave/admin/files/ace-src/ace.js`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/files/ace-src/mode-gherkin.js` & `overhave-4.0.5/overhave/admin/files/ace-src/mode-gherkin.js`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/files/css/overhave.css` & `overhave-4.0.5/overhave/admin/files/css/overhave.css`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/files/favicon.ico` & `overhave-4.0.5/overhave/admin/files/favicon.ico`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/flask/flask_admin.py` & `overhave-4.0.5/overhave/admin/flask/flask_admin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/flask/login_manager.py` & `overhave-4.0.5/overhave/admin/flask/login_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/templates/emulation_run_detail.html` & `overhave-4.0.5/overhave/admin/templates/emulation_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/templates/feature.html` & `overhave-4.0.5/overhave/admin/templates/feature.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/templates/login.html` & `overhave-4.0.5/overhave/admin/templates/login.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/templates/test_run.html` & `overhave-4.0.5/overhave/admin/templates/test_run.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/templates/test_run_detail.html` & `overhave-4.0.5/overhave/admin/templates/test_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/templates/test_user.html` & `overhave-4.0.5/overhave/admin/templates/test_user.html`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/access.py` & `overhave-4.0.5/overhave/admin/views/access.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/base.py` & `overhave-4.0.5/overhave/admin/views/base.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/draft.py` & `overhave-4.0.5/overhave/admin/views/draft.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/emulation.py` & `overhave-4.0.5/overhave/admin/views/emulation.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/emulation_run.py` & `overhave-4.0.5/overhave/admin/views/emulation_run.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/feature.py` & `overhave-4.0.5/overhave/admin/views/feature.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/formatters/formatters.py` & `overhave-4.0.5/overhave/admin/views/formatters/formatters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/formatters/helpers.py` & `overhave-4.0.5/overhave/admin/views/formatters/helpers.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/formatters/safe_formatter.py` & `overhave-4.0.5/overhave/admin/views/formatters/safe_formatter.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/index/custom_page.py` & `overhave-4.0.5/overhave/admin/views/index/custom_page.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/index/login_form.py` & `overhave-4.0.5/overhave/admin/views/index/login_form.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/index/view.py` & `overhave-4.0.5/overhave/admin/views/index/view.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/scenario_test_run.py` & `overhave-4.0.5/overhave/admin/views/scenario_test_run.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/tag.py` & `overhave-4.0.5/overhave/admin/views/tag.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/admin/views/testing_users.py` & `overhave-4.0.5/overhave/admin/views/testing_users.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/app.py` & `overhave-4.0.5/overhave/api/app.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/auth/regular.py` & `overhave-4.0.5/overhave/api/auth/regular.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/auth/token.py` & `overhave-4.0.5/overhave/api/auth/token.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/deps.py` & `overhave-4.0.5/overhave/api/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/settings.py` & `overhave-4.0.5/overhave/api/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/views/__init__.py` & `overhave-4.0.5/overhave/api/views/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/views/auth_views.py` & `overhave-4.0.5/overhave/api/views/auth_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/views/emulation_views.py` & `overhave-4.0.5/overhave/api/views/emulation_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/views/extra_views.py` & `overhave-4.0.5/overhave/api/views/extra_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/views/feature_views.py` & `overhave-4.0.5/overhave/api/views/feature_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/views/tags_views.py` & `overhave-4.0.5/overhave/api/views/tags_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/views/testrun_views.py` & `overhave-4.0.5/overhave/api/views/testrun_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/api/views/testuser_views.py` & `overhave-4.0.5/overhave/api/views/testuser_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/base_settings.py` & `overhave-4.0.5/overhave/base_settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/cli/admin.py` & `overhave-4.0.5/overhave/cli/admin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/cli/api.py` & `overhave-4.0.5/overhave/cli/api.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/cli/consumers.py` & `overhave-4.0.5/overhave/cli/consumers.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/cli/db_cmds/group.py` & `overhave-4.0.5/overhave/cli/db_cmds/group.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/cli/db_cmds/regular.py` & `overhave-4.0.5/overhave/cli/db_cmds/regular.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/cli/s3.py` & `overhave-4.0.5/overhave/cli/s3.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/cli/synchronizer.py` & `overhave-4.0.5/overhave/cli/synchronizer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/db/base.py` & `overhave-4.0.5/overhave/db/base.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/db/statuses.py` & `overhave-4.0.5/overhave/db/statuses.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/db/tables.py` & `overhave-4.0.5/overhave/db/tables.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/db/users.py` & `overhave-4.0.5/overhave/db/users.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/db/utils.py` & `overhave-4.0.5/overhave/db/utils.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/emulation/emulator.py` & `overhave-4.0.5/overhave/emulation/emulator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/__init__.py` & `overhave-4.0.5/overhave/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/archiver.py` & `overhave-4.0.5/overhave/entities/archiver.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/auth_managers/default.py` & `overhave-4.0.5/overhave/entities/auth_managers/default.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/auth_managers/ldap/manager.py` & `overhave-4.0.5/overhave/entities/auth_managers/ldap/manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/auth_managers/secret_mixin.py` & `overhave-4.0.5/overhave/entities/auth_managers/secret_mixin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/auth_managers/simple.py` & `overhave-4.0.5/overhave/entities/auth_managers/simple.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/feature/extractor.py` & `overhave-4.0.5/overhave/entities/feature/extractor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/file_extractor.py` & `overhave-4.0.5/overhave/entities/file_extractor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/git_initializer.py` & `overhave-4.0.5/overhave/entities/git_initializer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/language/prefixes.py` & `overhave-4.0.5/overhave/entities/language/prefixes.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/report_manager/report_manager.py` & `overhave-4.0.5/overhave/entities/report_manager/report_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/entities/settings.py` & `overhave-4.0.5/overhave/entities/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/__init__.py` & `overhave-4.0.5/overhave/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/base_factory.py` & `overhave-4.0.5/overhave/factory/base_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/components/admin_factory.py` & `overhave-4.0.5/overhave/factory/components/admin_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/components/emulation_factory.py` & `overhave-4.0.5/overhave/factory/components/emulation_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/components/publication_factory.py` & `overhave-4.0.5/overhave/factory/components/publication_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,46 +45,46 @@
     @cached_property
     def _gitlab_client(self) -> GitlabHttpClient:
         return GitlabHttpClient(self.context.client_settings)  # type: ignore
 
     @cached_property
     def _stash_publisher(self) -> StashVersionPublisher:
         return StashVersionPublisher(
-            file_settings=self.context.file_settings,
             project_settings=self.context.project_settings,
             feature_storage=self._feature_storage,
             scenario_storage=self._scenario_storage,
             test_run_storage=self._test_run_storage,
             draft_storage=self._draft_storage,
             file_manager=self._file_manager,
             git_initializer=self._git_initializer,
             stash_publisher_settings=self.context.publisher_settings,  # type: ignore
             stash_client=self._stash_client,
+            metric_container=self.metric_container,
         )
 
     @cached_property
     def _tokenizer_client(self) -> TokenizerClient:
         return TokenizerClient(self.context.tokenizer_client_settings)
 
     @cached_property
     def _gitlab_publisher(self) -> GitlabVersionPublisher:
         if self._tokenizer_client._settings.enabled and self._tokenizer_client._settings.url is None:
             raise UrlGitlabTokenizerNotScepifiedIfEnabled("Please set correct url for gitlab_tokenizer!")
         return GitlabVersionPublisher(
-            file_settings=self.context.file_settings,
             project_settings=self.context.project_settings,
             feature_storage=self._feature_storage,
             scenario_storage=self._scenario_storage,
             test_run_storage=self._test_run_storage,
             draft_storage=self._draft_storage,
             file_manager=self._file_manager,
             git_initializer=self._git_initializer,
             gitlab_publisher_settings=self.context.publisher_settings,  # type: ignore
             gitlab_client=self._gitlab_client,
             tokenizer_client=self._tokenizer_client,
+            metric_container=self.metric_container,
         )
 
     @property
     def publisher(self) -> IVersionPublisher:
         if self.context.publication_settings.publication_manager_type is PublicationManagerType.GITLAB:
             return self._gitlab_publisher
         return self._stash_publisher
```

### Comparing `overhave-4.0.4/overhave/factory/components/synchronizer_factory.py` & `overhave-4.0.5/overhave/factory/components/synchronizer_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/components/test_execution_factory.py` & `overhave-4.0.5/overhave/factory/components/test_execution_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/consumer_factory.py` & `overhave-4.0.5/overhave/factory/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/context/__init__.py` & `overhave-4.0.5/overhave/factory/context/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/context/admin_context.py` & `overhave-4.0.5/overhave/factory/context/admin_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/context/base_context.py` & `overhave-4.0.5/overhave/factory/context/base_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/context/publication_context.py` & `overhave-4.0.5/overhave/factory/context/publication_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/context/synchronizer_context.py` & `overhave-4.0.5/overhave/factory/context/synchronizer_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/context/test_execution_context.py` & `overhave-4.0.5/overhave/factory/context/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/factory/getters.py` & `overhave-4.0.5/overhave/factory/getters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/metrics/client/container.py` & `overhave-4.0.5/overhave/metrics/client/container.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/metrics/getters.py` & `overhave-4.0.5/overhave/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/publication/base_publisher.py` & `overhave-4.0.5/overhave/publication/base_publisher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import logging
 
 import git
 
 from overhave import db
-from overhave.entities import GitPullError, OverhaveFileSettings
+from overhave.entities import GitPullError
 from overhave.metrics import PublicationOverhaveMetricContainer
 from overhave.publication.abstract_publisher import IVersionPublisher
 from overhave.publication.errors import BaseGitVersionPublisherError
 from overhave.scenario import FileManager, OverhaveProjectSettings, generate_task_info
 from overhave.storage import IDraftStorage, IFeatureStorage, IScenarioStorage, ITestRunStorage, PublisherContext
 from overhave.transport import PublicationTask
 
@@ -16,24 +16,22 @@
 
 
 class BaseVersionPublisher(IVersionPublisher, abc.ABC):
     """Class for feature version's pull requests management relative to Atlassian Stash API."""
 
     def __init__(
         self,
-        file_settings: OverhaveFileSettings,
         project_settings: OverhaveProjectSettings,
         feature_storage: IFeatureStorage,
         scenario_storage: IScenarioStorage,
         test_run_storage: ITestRunStorage,
         draft_storage: IDraftStorage,
         file_manager: FileManager,
         metric_container: PublicationOverhaveMetricContainer,
     ) -> None:
-        self._file_settings = file_settings
         self._project_settings = project_settings
         self._feature_storage = feature_storage
         self._scenario_storage = scenario_storage
         self._test_run_storage = test_run_storage
         self._draft_storage = draft_storage
         self._file_manager = file_manager
         self._metric_container = metric_container
```

### Comparing `overhave-4.0.4/overhave/publication/errors.py` & `overhave-4.0.5/overhave/publication/errors.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/publication/git_publisher.py` & `overhave-4.0.5/overhave/publication/git_publisher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import logging
 from typing import Generic, cast
 
 import git
 
-from overhave.entities import GitRepositoryInitializer, OverhaveFileSettings
+from overhave.entities import GitRepositoryInitializer
 from overhave.metrics import PublicationOverhaveMetricContainer
 from overhave.publication.base_publisher import BaseVersionPublisher
 from overhave.publication.errors import (
     BaseGitVersionPublisherError,
     CommitNotCreatedError,
     CurrentBranchEqualToDefaultError,
     CurrentBranchNotEqualToTargetError,
@@ -21,27 +21,25 @@
 
 
 class GitVersionPublisher(Generic[GitPublisherSettings], BaseVersionPublisher, abc.ABC):
     """Class for feature version's management, based on git."""
 
     def __init__(
         self,
-        file_settings: OverhaveFileSettings,
         project_settings: OverhaveProjectSettings,
         feature_storage: IFeatureStorage,
         scenario_storage: IScenarioStorage,
         test_run_storage: ITestRunStorage,
         draft_storage: IDraftStorage,
         file_manager: FileManager,
         git_initializer: GitRepositoryInitializer,
         git_publisher_settings: GitPublisherSettings,
         metric_container: PublicationOverhaveMetricContainer,
     ) -> None:
         super().__init__(
-            file_settings=file_settings,
             project_settings=project_settings,
             feature_storage=feature_storage,
             scenario_storage=scenario_storage,
             test_run_storage=test_run_storage,
             draft_storage=draft_storage,
             file_manager=file_manager,
             metric_container=metric_container,
```

### Comparing `overhave-4.0.4/overhave/publication/gitlab/gitlab_publisher.py` & `overhave-4.0.5/overhave/publication/gitlab/gitlab_publisher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from http import HTTPStatus
 
 import httpx
 from gitlab import GitlabError
 
 from overhave import db
-from overhave.entities import GitRepositoryInitializer, OverhaveFileSettings
+from overhave.entities import GitRepositoryInitializer
 from overhave.metrics import PublicationOverhaveMetricContainer
 from overhave.publication.git_publisher import GitVersionPublisher
 from overhave.publication.gitlab.settings import OverhaveGitlabPublisherSettings
 from overhave.publication.gitlab.tokenizer.client import TokenizerClient
 from overhave.scenario import FileManager, OverhaveProjectSettings
 from overhave.storage import IDraftStorage, IFeatureStorage, IScenarioStorage, ITestRunStorage
 from overhave.transport.http.gitlab_client import GitlabHttpClient, GitlabMrRequest
@@ -18,29 +18,27 @@
 
 
 class GitlabVersionPublisher(GitVersionPublisher[OverhaveGitlabPublisherSettings]):
     """Class for feature version's merge requests management relative to Gitlab API."""
 
     def __init__(
         self,
-        file_settings: OverhaveFileSettings,
         project_settings: OverhaveProjectSettings,
         feature_storage: IFeatureStorage,
         scenario_storage: IScenarioStorage,
         test_run_storage: ITestRunStorage,
         draft_storage: IDraftStorage,
         file_manager: FileManager,
         git_initializer: GitRepositoryInitializer,
         gitlab_publisher_settings: OverhaveGitlabPublisherSettings,
         gitlab_client: GitlabHttpClient,
         tokenizer_client: TokenizerClient,
         metric_container: PublicationOverhaveMetricContainer,
     ):
         super().__init__(
-            file_settings=file_settings,
             project_settings=project_settings,
             feature_storage=feature_storage,
             scenario_storage=scenario_storage,
             test_run_storage=test_run_storage,
             draft_storage=draft_storage,
             file_manager=file_manager,
             git_initializer=git_initializer,
```

### Comparing `overhave-4.0.4/overhave/publication/gitlab/settings.py` & `overhave-4.0.5/overhave/publication/gitlab/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/publication/gitlab/tokenizer/client.py` & `overhave-4.0.5/overhave/publication/gitlab/tokenizer/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/publication/gitlab/tokenizer/settings.py` & `overhave-4.0.5/overhave/publication/gitlab/tokenizer/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/publication/settings.py` & `overhave-4.0.5/overhave/publication/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/publication/stash/settings.py` & `overhave-4.0.5/overhave/publication/stash/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/publication/stash/stash_publisher.py` & `overhave-4.0.5/overhave/publication/stash/stash_publisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 import httpx
 
 from overhave import db
-from overhave.entities import GitRepositoryInitializer, OverhaveFileSettings
+from overhave.entities import GitRepositoryInitializer
 from overhave.metrics import PublicationOverhaveMetricContainer
 from overhave.publication.git_publisher import GitVersionPublisher
 from overhave.publication.stash.settings import OverhaveStashPublisherSettings
 from overhave.scenario import FileManager, OverhaveProjectSettings
 from overhave.storage import IDraftStorage, IFeatureStorage, IScenarioStorage, ITestRunStorage
 from overhave.transport import (
     StashBranch,
@@ -22,28 +22,26 @@
 
 
 class StashVersionPublisher(GitVersionPublisher[OverhaveStashPublisherSettings]):
     """Class for feature version's pull requests management relative to Atlassian Stash API."""
 
     def __init__(
         self,
-        file_settings: OverhaveFileSettings,
         project_settings: OverhaveProjectSettings,
         feature_storage: IFeatureStorage,
         scenario_storage: IScenarioStorage,
         test_run_storage: ITestRunStorage,
         draft_storage: IDraftStorage,
         file_manager: FileManager,
         git_initializer: GitRepositoryInitializer,
         stash_publisher_settings: OverhaveStashPublisherSettings,
         stash_client: StashHttpClient,
         metric_container: PublicationOverhaveMetricContainer,
     ):
         super().__init__(
-            file_settings=file_settings,
             project_settings=project_settings,
             feature_storage=feature_storage,
             scenario_storage=scenario_storage,
             test_run_storage=test_run_storage,
             draft_storage=draft_storage,
             file_manager=file_manager,
             git_initializer=git_initializer,
```

### Comparing `overhave-4.0.4/overhave/pytest_plugin/config_injector.py` & `overhave-4.0.5/overhave/pytest_plugin/config_injector.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/deps.py` & `overhave-4.0.5/overhave/pytest_plugin/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/helpers/__init__.py` & `overhave-4.0.5/overhave/pytest_plugin/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/helpers/allure_utils/description_manager.py` & `overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/description_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/helpers/allure_utils/links.py` & `overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/links.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/helpers/allure_utils/severity.py` & `overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/severity.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py` & `overhave-4.0.5/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/helpers/bdd_item.py` & `overhave-4.0.5/overhave/pytest_plugin/helpers/bdd_item.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/helpers/parsed_info.py` & `overhave-4.0.5/overhave/pytest_plugin/helpers/parsed_info.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/helpers/tag_controller.py` & `overhave-4.0.5/overhave/pytest_plugin/helpers/tag_controller.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/plugin.py` & `overhave-4.0.5/overhave/pytest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/plugin_resolver.py` & `overhave-4.0.5/overhave/pytest_plugin/plugin_resolver.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/pytest_plugin/proxy_manager.py` & `overhave-4.0.5/overhave/pytest_plugin/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/scenario/__init__.py` & `overhave-4.0.5/overhave/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/scenario/compiler/compiler.py` & `overhave-4.0.5/overhave/scenario/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/scenario/compiler/settings.py` & `overhave-4.0.5/overhave/scenario/compiler/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/scenario/file_manager/file_manager.py` & `overhave-4.0.5/overhave/scenario/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/scenario/file_manager/settings.py` & `overhave-4.0.5/overhave/scenario/file_manager/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/scenario/parser/models.py` & `overhave-4.0.5/overhave/scenario/parser/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/scenario/parser/parser.py` & `overhave-4.0.5/overhave/scenario/parser/parser.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/scenario/validator/duplicate_id_mixin.py` & `overhave-4.0.5/overhave/scenario/validator/duplicate_id_mixin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/scenario/validator/validator.py` & `overhave-4.0.5/overhave/scenario/validator/validator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/__init__.py` & `overhave-4.0.5/overhave/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/api_auth_storage.py` & `overhave-4.0.5/overhave/storage/api_auth_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/converters.py` & `overhave-4.0.5/overhave/storage/converters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/draft_storage.py` & `overhave-4.0.5/overhave/storage/draft_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/emulation_storage.py` & `overhave-4.0.5/overhave/storage/emulation_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/feature_storage.py` & `overhave-4.0.5/overhave/storage/feature_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/feature_tag_storage.py` & `overhave-4.0.5/overhave/storage/feature_tag_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/feature_type_storage.py` & `overhave-4.0.5/overhave/storage/feature_type_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/scenario_storage.py` & `overhave-4.0.5/overhave/storage/scenario_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/system_user_group_storage.py` & `overhave-4.0.5/overhave/storage/system_user_group_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/system_user_storage.py` & `overhave-4.0.5/overhave/storage/system_user_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/test_run_storage.py` & `overhave-4.0.5/overhave/storage/test_run_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/storage/test_user_storage.py` & `overhave-4.0.5/overhave/storage/test_user_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/synchronization/storage_manager.py` & `overhave-4.0.5/overhave/synchronization/storage_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/synchronization/synchronizer.py` & `overhave-4.0.5/overhave/synchronization/synchronizer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/test_execution/executor.py` & `overhave-4.0.5/overhave/test_execution/executor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/test_execution/objects.py` & `overhave-4.0.5/overhave/test_execution/objects.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/test_execution/settings.py` & `overhave-4.0.5/overhave/test_execution/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/test_execution/step_collector.py` & `overhave-4.0.5/overhave/test_execution/step_collector.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/test_execution/test_runner.py` & `overhave-4.0.5/overhave/test_execution/test_runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/__init__.py` & `overhave-4.0.5/overhave/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/__init__.py` & `overhave-4.0.5/overhave/transport/http/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/api_client/authenticator.py` & `overhave-4.0.5/overhave/transport/http/api_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/base_client/auth.py` & `overhave-4.0.5/overhave/transport/http/base_client/auth.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/base_client/client.py` & `overhave-4.0.5/overhave/transport/http/base_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/base_client/settings.py` & `overhave-4.0.5/overhave/transport/http/base_client/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/gitlab_client/client.py` & `overhave-4.0.5/overhave/transport/http/gitlab_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/gitlab_client/models.py` & `overhave-4.0.5/overhave/transport/http/gitlab_client/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/gitlab_client/utils.py` & `overhave-4.0.5/overhave/transport/http/gitlab_client/utils.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/stash_client/client.py` & `overhave-4.0.5/overhave/transport/http/stash_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/stash_client/models.py` & `overhave-4.0.5/overhave/transport/http/stash_client/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/http/stash_client/settings.py` & `overhave-4.0.5/overhave/transport/http/stash_client/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/ldap/authenticator.py` & `overhave-4.0.5/overhave/transport/ldap/authenticator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/redis/consumer.py` & `overhave-4.0.5/overhave/transport/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/redis/deps.py` & `overhave-4.0.5/overhave/transport/redis/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/redis/objects.py` & `overhave-4.0.5/overhave/transport/redis/objects.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/redis/producer.py` & `overhave-4.0.5/overhave/transport/redis/producer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/redis/runner.py` & `overhave-4.0.5/overhave/transport/redis/runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/redis/settings.py` & `overhave-4.0.5/overhave/transport/redis/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/s3/manager.py` & `overhave-4.0.5/overhave/transport/s3/manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/s3/models.py` & `overhave-4.0.5/overhave/transport/s3/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/overhave/transport/s3/settings.py` & `overhave-4.0.5/overhave/transport/s3/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.0.4/pyproject.toml` & `overhave-4.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overhave"
-version = "4.0.4"
+version = "4.0.5"
 description = "Overhave - web-framework for BDD"
 readme = "README.rst"
 authors = [
     "Vladislav Mukhamatnurov <livestreamepidemz@yandex.ru>",
     "Tinkoff Backend Dialog System Team <bds-dev@tinkoff.ru>"
 ]
 classifiers = [
```

### Comparing `overhave-4.0.4/PKG-INFO` & `overhave-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overhave
-Version: 4.0.4
+Version: 4.0.5
 Summary: Overhave - web-framework for BDD
 Author: Vladislav Mukhamatnurov
 Author-email: livestreamepidemz@yandex.ru
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

