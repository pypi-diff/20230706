# Comparing `tmp/propan-0.1.5.1.tar.gz` & `tmp/propan-0.1.5.2.tar.gz`

## Comparing `propan-0.1.5.1.tar` & `propan-0.1.5.2.tar`

### file list

```diff
@@ -1,190 +1,191 @@
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 propan-0.1.5.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.5.1/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/dependantbot.yml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 propan-0.1.5.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/redis/pattern.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/scheduling/rocketry.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/serialization/gen_py_code.sh
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/serialization/message.proto
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/serialization/protobuf.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/serialization/requirements.txt
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.5.1/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/__about__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/__main__.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/_compat.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/py.typed
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/security.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/constants.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    19850 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/_model/routing.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/routing.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/routing.pyi
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/consts.py
--rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/nats_js_broker.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/routing.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/routing.pyi
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/logging.py
--rw-r--r--   0        0        0    13869 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/routing.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/routing.pyi
--rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/rabbit/utils.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/routing.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/routing.pyi
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/routing.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/routing.pyi
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/__init__.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/app.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/kafka.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/nats.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/rabbit.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/redis.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/sqs.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/classes.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/context/main.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.5.1/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.1/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.5.1/scripts/publish.sh
--rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 propan-0.1.5.1/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.1/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.5.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.5.1/LICENSE
--rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 propan-0.1.5.1/README.md
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 propan-0.1.5.1/pyproject.toml
--rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 propan-0.1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 propan-0.1.5.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.5.2/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.5.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.5.2/.github/dependantbot.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.5.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.5.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 propan-0.1.5.2/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.5.2/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.5.2/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 propan-0.1.5.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/redis/pattern.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/scheduling/rocketry.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/serialization/gen_py_code.sh
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/serialization/message.proto
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/serialization/protobuf.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/serialization/requirements.txt
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.5.2/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/__about__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/__main__.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/_compat.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/py.typed
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/constants.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/middlewares.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    21080 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/_model/routing.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/kafka/routing.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/kafka/routing.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/nats/consts.py
+-rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0     8331 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/nats/nats_js_broker.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/nats/routing.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/nats/routing.pyi
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/rabbit/logging.py
+-rw-r--r--   0        0        0    13869 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    11287 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/rabbit/routing.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/rabbit/routing.pyi
+-rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/rabbit/utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     8135 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/redis/routing.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/redis/routing.pyi
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/sqs/routing.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/sqs/routing.pyi
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/__init__.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/app.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/test/kafka.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/test/nats.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/test/redis.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/test/sqs.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/utils/classes.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/utils/context/main.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.5.2/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.2/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.5.2/scripts/publish.sh
+-rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 propan-0.1.5.2/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.2/scripts/test.sh
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 propan-0.1.5.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.5.2/LICENSE
+-rw-r--r--   0        0        0    15080 2020-02-02 00:00:00.000000 propan-0.1.5.2/README.md
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 propan-0.1.5.2/pyproject.toml
+-rw-r--r--   0        0        0    19515 2020-02-02 00:00:00.000000 propan-0.1.5.2/PKG-INFO
```

### Comparing `propan-0.1.5.1/CONTRIBUTING.md` & `propan-0.1.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/SECURITY.md` & `propan-0.1.5.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.5.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.5.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.5.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/.github/workflows/documentation.yml` & `propan-0.1.5.2/.github/workflows/documentation.yml`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,17 @@
   push:
     branches:
       - main
     paths:
       - docs/**
       - .github/workflows/documentation.yml
 
+env:
+  CI: true
+
 permissions:
   contents: write
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
@@ -19,10 +22,10 @@
       - uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - uses: actions/cache@v2
         with:
           key: ${{ github.ref }}
           path: .cache
-      - run: pip install mkdocs-material mkdocs-static-i18n mdx-include mkdocs-macros-plugin mkdocs-glightbox
+      - run: pip install mkdocs-material mkdocs-static-i18n mdx-include mkdocs-macros-plugin mkdocs-glightbox pillow cairosvg
       - working-directory: ./docs
         run: mkdocs gh-deploy --force
```

### Comparing `propan-0.1.5.1/.github/workflows/publish_coverage.yml` & `propan-0.1.5.2/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/.github/workflows/publish_pypi.yml` & `propan-0.1.5.2/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/.github/workflows/tests.yml` & `propan-0.1.5.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/3_lifespan_events.py` & `propan-0.1.5.2/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/4_cli_attributes_promotion.py` & `propan-0.1.5.2/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/5_publishing.py` & `propan-0.1.5.2/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/6_arguments_casting.py` & `propan-0.1.5.2/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/7_handler_errors_processing.py` & `propan-0.1.5.2/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/dependencies/1_dependency_injection.py` & `propan-0.1.5.2/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.5.2/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.5.2/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.5.2/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.5.2/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/dependencies/7_annotated.py` & `propan-0.1.5.2/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.5.2/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.5.2/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.5.2/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.5.2/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/http_frameworks_integrations/quart.py` & `propan-0.1.5.2/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.5.2/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.5.2/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/rabbit/direct.py` & `propan-0.1.5.2/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/rabbit/fanout.py` & `propan-0.1.5.2/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/rabbit/header.py` & `propan-0.1.5.2/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/rabbit/topic.py` & `propan-0.1.5.2/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/redis/direct.py` & `propan-0.1.5.2/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/redis/pattern.py` & `propan-0.1.5.2/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/examples/serialization/protobuf.py` & `propan-0.1.5.2/examples/serialization/protobuf.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/__about__.py` & `propan-0.1.5.2/propan/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.5.1"
+__version__ = "0.1.5.2"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.5.1/propan/__init__.py` & `propan-0.1.5.2/propan/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Imports to use at __all__
 from propan import __about__ as about
 from propan.brokers import PropanMessage
+from propan.brokers.middlewares import BaseMiddleware
 from propan.cli.app import *  # noqa: F403
 from propan.log import *  # noqa: F403
 from propan.utils import *  # noqa: F403
 
 try:
     from propan.brokers.rabbit import RabbitBroker, RabbitRouter
 except ImportError:
@@ -46,14 +47,15 @@
     ## context
     "context",
     "Context",
     "ContextRepo",
     "Depends",
     # brokers
     "PropanMessage",
+    "BaseMiddleware",
     ## nats
     "NatsBroker",
     "NatsJSBroker",
     "NatsRouter",
     ## rabbit
     "RabbitBroker",
     "RabbitRouter",
```

### Comparing `propan-0.1.5.1/propan/_compat.py` & `propan-0.1.5.2/propan/_compat.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/annotations.py` & `propan-0.1.5.2/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/types.py` & `propan-0.1.5.2/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/__init__.py` & `propan-0.1.5.2/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/channels.py` & `propan-0.1.5.2/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/info.py` & `propan-0.1.5.2/propan/asyncapi/info.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/main.py` & `propan-0.1.5.2/propan/asyncapi/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/message.py` & `propan-0.1.5.2/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/security.py` & `propan-0.1.5.2/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/subscription.py` & `propan-0.1.5.2/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/bindings/amqp.py` & `propan-0.1.5.2/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/bindings/kafka.py` & `propan-0.1.5.2/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/bindings/main.py` & `propan-0.1.5.2/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/asyncapi/bindings/redis.py` & `propan-0.1.5.2/propan/asyncapi/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/push_back_watcher.py` & `propan-0.1.5.2/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/_model/broker_usecase.py` & `propan-0.1.5.2/propan/brokers/_model/broker_usecase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import warnings
 from abc import ABC, abstractmethod
+from contextlib import AsyncExitStack
 from functools import wraps
 from itertools import chain
 from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
@@ -33,14 +34,15 @@
     get_watcher,
     set_message_context,
     suppress_decor,
     to_send,
 )
 from propan.brokers.constants import ContentType, ContentTypes
 from propan.brokers.exceptions import SkipMessage
+from propan.brokers.middlewares import BaseMiddleware
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import AnyDict, DecodedMessage, SendableMessage
 from propan.utils import apply_types, context
 from propan.utils.functions import get_function_positional_arguments, to_async
 
 T = TypeVar("T", bound=DecodedMessage)
@@ -94,14 +96,15 @@
 
 
 class BrokerUsecase(ABC, Generic[MsgType, ConnectionType]):
     logger: Optional[logging.Logger]
     log_level: int
     handlers: Sequence[BaseHandler]
     dependencies: Sequence[Depends]
+    middlewares: Sequence[Type[BaseMiddleware[MsgType]]]
     started: bool
     _global_parser: CustomParser[MsgType]
     _global_decoder: CustomDecoder[MsgType]
     _connection: Optional[ConnectionType]
     _fmt: Optional[str]
 
     def __init__(
@@ -110,28 +113,30 @@
         apply_types: bool = True,
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = "%(asctime)s %(levelname)s - %(message)s",
         dependencies: Sequence[Depends] = (),
         decode_message: CustomDecoder[MsgType] = None,
         parse_message: CustomParser[MsgType] = None,
+        middlewares: Sequence[Type[BaseMiddleware[MsgType]]] = (),
         # AsyncAPI
         protocol: str = "",
         protocol_version: Optional[str] = None,
         url_: Union[str, List[str]] = "",
         **kwargs: AnyDict,
     ) -> None:
         self.logger = logger
         self.log_level = log_level
         self._fmt = log_fmt
 
         self._connection = None
         self._is_apply_types = apply_types
         self.handlers = []
         self.dependencies = dependencies
+        self.middlewares = middlewares
 
         self._connection_args = args
         self._connection_kwargs = kwargs
 
         self._global_parser = parse_message
         self._global_decoder = decode_message
 
@@ -168,14 +173,17 @@
     def _encode_message(msg: SendableMessage) -> Tuple[bytes, Optional[ContentType]]:
         return to_send(msg)
 
     def include_router(self, router: BrokerRouter[MsgType]) -> None:
         for r in router.handlers:
             r.call = self.handle(*r.args, **r.kwargs)(r.call)
 
+    def include_middleware(self, middleware: Type[BaseMiddleware[MsgType]]) -> None:
+        self.middlewares = (*self.middlewares, middleware)
+
     def _wrap_handler(
         self,
         func: HandlerCallable[T_HandlerReturn],
         *,
         retry: Union[bool, int] = False,
         extra_dependencies: Sequence[Depends] = (),
         decode_message: CustomDecoder[MsgType] = None,
@@ -240,14 +248,16 @@
             params=tuple(chain(dependant.flat_params, extra)),
             decoder=decode_message or self._global_decoder,
         )
 
         if self.logger is not None:
             f = self._log_execution(f, **broker_log_context_kwargs)
 
+        f = self._wrap_middleware(f)
+
         f = self._process_message(
             func=f,
             watcher=get_watcher(self.logger, retry),
         )
 
         f = self._wrap_parse_message(
             func=f,
@@ -375,14 +385,21 @@
         Union[
             T_HandlerReturn,
             Awaitable[T_HandlerReturn],
         ],
     ]:
         raise NotImplementedError()
 
+    @abstractmethod
+    def _wrap_middleware(
+        self,
+        func: Callable[[MsgType], Union[T_HandlerReturn, Awaitable[T_HandlerReturn]]],
+    ) -> Callable[[MsgType], Union[T_HandlerReturn, Awaitable[T_HandlerReturn]]]:
+        raise NotImplementedError()
+
 
 class BrokerAsyncUsecase(BrokerUsecase[MsgType, ConnectionType]):
     _global_parser: AsyncParser[MsgType]
     _global_decoder: AsyncDecoder[MsgType]
 
     @abstractmethod
     async def start(self) -> None:  # type: ignore[override]
@@ -609,14 +626,27 @@
                     raise e
                 else:
                     self._log("Processed", extra=log_context)
                     return r
 
         return log_wrapper
 
+    def _wrap_middleware(
+        self,
+        func: Callable[[PropanMessage[MsgType]], Awaitable[T_HandlerReturn]],
+    ) -> Callable[[PropanMessage[MsgType]], Awaitable[T_HandlerReturn]]:
+        @wraps(func)
+        async def middleware_wrapper(msg: PropanMessage[MsgType]) -> T_HandlerReturn:
+            async with AsyncExitStack() as stack:
+                for m in self.middlewares:
+                    await stack.enter_async_context(m(msg))
+                return await func(msg)
+
+        return middleware_wrapper
+
 
 def extend_dependencies(extra: Sequence[CallModel]) -> Callable[[CallModel], CallModel]:
     def dependant_wrapper(dependant: CallModel) -> CallModel:
         if isinstance(dependant, CallModel):
             dependant.extra_dependencies.extend(extra)
         else:  # FastAPI dependencies
             dependant.dependencies.extend(extra)
```

### Comparing `propan-0.1.5.1/propan/brokers/_model/routing.py` & `propan-0.1.5.2/propan/brokers/_model/routing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/_model/schemas.py` & `propan-0.1.5.2/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/_model/utils.py` & `propan-0.1.5.2/propan/brokers/_model/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         [MsgType],
         Union[
             T_HandlerReturn,
             Awaitable[T_HandlerReturn],
         ],
     ],
     _is_sync: bool = False,
-) -> Callable[[MsgType, bool], Union[T_HandlerReturn, Awaitable[T_HandlerReturn],]]:
+) -> Callable[[MsgType, bool], Union[T_HandlerReturn, Awaitable[T_HandlerReturn]]]:
     if _is_sync:
         func = cast(Callable[[MsgType], T_HandlerReturn], func)
 
         @wraps(func)
         def wrapper(
             message: MsgType, reraise_exc: bool = False
         ) -> Optional[T_HandlerReturn]:
```

### Comparing `propan-0.1.5.1/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.5.2/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.5.2/propan/brokers/kafka/kafka_broker.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     AsyncParser,
     BrokerAsyncUsecase,
     HandlerCallable,
     T_HandlerReturn,
 )
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.kafka.schemas import Handler
+from propan.brokers.middlewares import BaseMiddleware
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import DecodedMessage, SendableMessage
 
 Partition = TypeVar("Partition")
 CorrelationId: TypeAlias = str
 KafkaMessage: TypeAlias = PropanMessage[ConsumerRecord]
@@ -47,14 +48,15 @@
     BrokerAsyncUsecase[ConsumerRecord, Callable[[Tuple[str, ...]], AIOKafkaConsumer]]
 ):
     _publisher: Optional[AIOKafkaProducer]
     __max_topic_len: int
     response_topic: str
     response_callbacks: Dict[CorrelationId, "Future[DecodedMessage]"]
     handlers: List[Handler]
+    middlewares: Sequence[Type[BaseMiddleware[ConsumerRecord]]]
 
     def __init__(
         self,
         bootstrap_servers: Union[str, List[str]] = "localhost",
         *,
         response_topic: str = "",
         # both
@@ -102,14 +104,15 @@
         logger: Optional[logging.Logger] = access_logger,
         decode_message: AsyncDecoder[ConsumerRecord] = None,
         parse_message: AsyncParser[ConsumerRecord] = None,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
         dependencies: Sequence[Depends] = (),
+        middlewares: Sequence[Type[BaseMiddleware[ConsumerRecord]]] = (),
         protocol: str = "kafka",
     ) -> None: ...
     async def connect(
         self,
         *,
         bootstrap_servers: Union[str, List[str]] = "localhost",
         # both
```

### Comparing `propan-0.1.5.1/propan/brokers/kafka/routing.pyi` & `propan-0.1.5.2/propan/brokers/kafka/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/kafka/schemas.py` & `propan-0.1.5.2/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/nats/nats_broker.py` & `propan-0.1.5.2/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.5.2/propan/brokers/nats/nats_broker.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -32,23 +32,25 @@
 from propan.brokers._model.broker_usecase import (
     AsyncDecoder,
     AsyncParser,
     HandlerCallable,
     T_HandlerReturn,
 )
 from propan.brokers._model.schemas import PropanMessage
+from propan.brokers.middlewares import BaseMiddleware
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import DecodedMessage, SendableMessage
 
 NatsMessage: TypeAlias = PropanMessage[Msg]
 
 class NatsBroker(BrokerAsyncUsecase[Msg, Client]):
     logger: logging.Logger
+    middlewares: Sequence[Type[BaseMiddleware[Msg]]]
     handlers: List[Handler]
 
     def __init__(
         self,
         servers: Union[str, List[str]] = ["nats://localhost:4222"],  # noqa: B006
         *,
         error_cb: Optional[ErrorCallback] = None,
@@ -83,14 +85,15 @@
         flush_timeout: Optional[float] = None,
         # broker kwargs
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
         dependencies: Sequence[Depends] = (),
+        middlewares: Sequence[Type[BaseMiddleware[Msg]]] = (),
         decode_message: AsyncDecoder[Msg] = None,
         parse_message: AsyncParser[Msg] = None,
         protocol: str = "nats",
     ) -> None: ...
     async def connect(
         self,
         *,
```

### Comparing `propan-0.1.5.1/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.5.2/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/nats/nats_js_broker.pyi` & `propan-0.1.5.2/propan/brokers/nats/nats_js_broker.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,25 @@
 
 from propan.brokers._model.broker_usecase import (
     AsyncDecoder,
     AsyncParser,
     HandlerCallable,
     T_HandlerReturn,
 )
+from propan.brokers.middlewares import BaseMiddleware
 from propan.brokers.nats import consts as api
 from propan.brokers.nats.nats_broker import NatsBroker, NatsMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import DecodedMessage, SendableMessage
 
 T = TypeVar("T")
 
 class NatsJSBroker(NatsBroker):
+    middlewares: Sequence[Type[BaseMiddleware[Msg]]]
     _raw_connection: Optional[Client]
     _connection: Optional[JetStreamContext]
     _stream_config: api.StreamConfig
 
     @property
     def js(self) -> JetStreamContext:
         """JetStreamContext object to use it with native `nats-py` features"""
@@ -123,14 +125,15 @@
         flush_timeout: Optional[float] = None,
         # broker kwargs
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
         dependencies: Sequence[Depends] = (),
+        middlewares: Sequence[Type[BaseMiddleware[Msg]]] = (),
         decode_message: AsyncDecoder[Msg] = None,
         parse_message: AsyncParser[Msg] = None,
         protocol: str = "nats",
     ) -> None:
         """"""
     async def _connect(
         self,
```

### Comparing `propan-0.1.5.1/propan/brokers/nats/routing.pyi` & `propan-0.1.5.2/propan/brokers/nats/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/nats/schemas.py` & `propan-0.1.5.2/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/rabbit/logging.py` & `propan-0.1.5.2/propan/brokers/rabbit/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.5.2/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.5.2/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from pamqp.common import FieldTable
 from typing_extensions import TypeAlias
 from yarl import URL
 
 from propan.brokers._model import BrokerAsyncUsecase
 from propan.brokers._model.broker_usecase import AsyncDecoder, AsyncParser
 from propan.brokers._model.schemas import PropanMessage
+from propan.brokers.middlewares import BaseMiddleware
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.log import access_logger
 from propan.types import DecodedMessage, SendableMessage
 
 PikaSendableMessage: TypeAlias = Union[aio_pika.message.Message, SendableMessage]
 T_HandlerReturn = TypeVar("T_HandlerReturn", bound=PikaSendableMessage)
@@ -36,14 +37,15 @@
     ..., Union[T_HandlerReturn, Awaitable[T_HandlerReturn]]
 ]
 
 RabbitMessage: TypeAlias = PropanMessage[IncomingMessage]
 
 class RabbitBroker(BrokerAsyncUsecase[IncomingMessage, aio_pika.RobustConnection]):
     handlers: List[Handler]
+    middlewares: Sequence[Type[BaseMiddleware[IncomingMessage]]]
     _channel: Optional[aio_pika.RobustChannel]
 
     __max_queue_len: int
     __max_exchange_len: int
 
     def __init__(
         self,
@@ -62,14 +64,15 @@
         # broker
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
         consumers: Optional[int] = None,
         dependencies: Sequence[Depends] = (),
+        middlewares: Sequence[Type[BaseMiddleware[IncomingMessage]]] = (),
         decode_message: AsyncDecoder[IncomingMessage] = None,
         parse_message: AsyncParser[IncomingMessage] = None,
         # AsyncAPI
         protocol: str = "amqp",
         protocol_version: str = "0.9.1",
     ) -> None:
         """RabbitMQ Propan broker
```

### Comparing `propan-0.1.5.1/propan/brokers/rabbit/routing.pyi` & `propan-0.1.5.2/propan/brokers/rabbit/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/rabbit/schemas.py` & `propan-0.1.5.2/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/rabbit/utils.py` & `propan-0.1.5.2/propan/brokers/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/redis/redis_broker.py` & `propan-0.1.5.2/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.5.2/propan/brokers/redis/redis_broker.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -23,24 +23,26 @@
 from propan.brokers._model.broker_usecase import (
     AsyncDecoder,
     AsyncParser,
     HandlerCallable,
     T_HandlerReturn,
 )
 from propan.brokers._model.schemas import PropanMessage
+from propan.brokers.middlewares import BaseMiddleware
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.redis.schemas import Handler
 from propan.log import access_logger
 from propan.types import AnyDict, DecodedMessage, SendableMessage
 
 T = TypeVar("T")
 RedisMessage: TypeAlias = PropanMessage[AnyDict]
 
 class RedisBroker(BrokerAsyncUsecase[AnyDict, Redis[bytes]]):
     handlers: List[Handler]
+    middlewares: Sequence[Type[BaseMiddleware[AnyDict]]]
     __max_channel_len: int
 
     def __init__(
         self,
         url: str = "redis://localhost:6379",
         *,
         polling_interval: float = 1.0,
@@ -67,14 +69,15 @@
         encoder_class: Type[Encoder] = Encoder,
         # broker kwargs
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
         dependencies: Sequence[Depends] = (),
+        middlewares: Sequence[Type[BaseMiddleware[AnyDict]]] = (),
         decode_message: AsyncDecoder[AnyDict] = None,
         parse_message: AsyncParser[AnyDict] = None,
         protocol: str = "redis",
     ) -> None:
         """Redis Pub/sub Propan broker
 
         URL examples:
```

### Comparing `propan-0.1.5.1/propan/brokers/redis/routing.pyi` & `propan-0.1.5.2/propan/brokers/redis/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/redis/schemas.py` & `propan-0.1.5.2/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/sqs/routing.pyi` & `propan-0.1.5.2/propan/brokers/sqs/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/sqs/schema.py` & `propan-0.1.5.2/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.5.2/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.5.2/propan/brokers/sqs/sqs_broker.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,28 @@
 from propan.brokers._model.broker_usecase import (
     AsyncDecoder,
     AsyncParser,
     HandlerCallable,
     T_HandlerReturn,
 )
 from propan.brokers._model.schemas import PropanMessage
+from propan.brokers.middlewares import BaseMiddleware
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.sqs.schema import Handler, SQSQueue
 from propan.log import access_logger
 from propan.types import AnyDict, DecodedMessage, SendableMessage
 
 T = TypeVar("T")
 QueueUrl: TypeAlias = str
 SQSMessage: TypeAlias = PropanMessage[AnyDict]
 
 class SQSBroker(BrokerAsyncUsecase[AnyDict, AioBaseClient]):
     _queues: Dict[str, QueueUrl]
     response_queue: str
+    middlewares: Sequence[Type[BaseMiddleware[AnyDict]]]
     response_callbacks: Dict[str, "asyncio.Future[DecodedMessage]"]
     handlers: List[Handler]
 
     def __init__(
         self,
         url: str = "http://localhost:9324/",
         *,
@@ -58,14 +60,15 @@
         config: Optional[AioConfig] = None,
         # broker
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
         dependencies: Sequence[Depends] = (),
+        middlewares: Sequence[Type[BaseMiddleware[AnyDict]]] = (),
         decode_message: AsyncDecoder[AnyDict] = None,
         parse_message: AsyncParser[AnyDict] = None,
         protocol: str = "sqs",
     ) -> None:
         """"""
     async def connect(
         self,
```

### Comparing `propan-0.1.5.1/propan/cli/app.py` & `propan-0.1.5.2/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/main.py` & `propan-0.1.5.2/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/docs/app.py` & `propan-0.1.5.2/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/docs/gen.py` & `propan-0.1.5.2/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/docs/serving.py` & `propan-0.1.5.2/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/startproject/core.py` & `propan-0.1.5.2/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/startproject/async_app/app.py` & `propan-0.1.5.2/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/startproject/async_app/core.py` & `propan-0.1.5.2/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.5.2/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/startproject/async_app/nats.py` & `propan-0.1.5.2/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.5.2/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/startproject/async_app/redis.py` & `propan-0.1.5.2/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.5.2/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/supervisors/basereload.py` & `propan-0.1.5.2/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/supervisors/multiprocess.py` & `propan-0.1.5.2/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/supervisors/utils.py` & `propan-0.1.5.2/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/supervisors/watchfiles.py` & `propan-0.1.5.2/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/utils/imports.py` & `propan-0.1.5.2/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/utils/logs.py` & `propan-0.1.5.2/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/cli/utils/parser.py` & `propan-0.1.5.2/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/fastapi/__init__.py` & `propan-0.1.5.2/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/fastapi/core/route.py` & `propan-0.1.5.2/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/fastapi/core/router.py` & `propan-0.1.5.2/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/fastapi/kafka/router.pyi` & `propan-0.1.5.2/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/fastapi/nats/router.pyi` & `propan-0.1.5.2/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/fastapi/rabbit/router.pyi` & `propan-0.1.5.2/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/fastapi/redis/router.pyi` & `propan-0.1.5.2/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/fastapi/sqs/router.pyi` & `propan-0.1.5.2/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/log/formatter.py` & `propan-0.1.5.2/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/log/logging.py` & `propan-0.1.5.2/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/test/__init__.py` & `propan-0.1.5.2/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/test/kafka.py` & `propan-0.1.5.2/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/test/nats.py` & `propan-0.1.5.2/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/test/rabbit.py` & `propan-0.1.5.2/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/test/redis.py` & `propan-0.1.5.2/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/test/sqs.py` & `propan-0.1.5.2/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/test/utils.py` & `propan-0.1.5.2/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/utils/functions.py` & `propan-0.1.5.2/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/utils/context/main.py` & `propan-0.1.5.2/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/propan/utils/context/types.py` & `propan-0.1.5.2/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/LICENSE` & `propan-0.1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.1/README.md` & `propan-0.1.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 | **SQS**           | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **NatsJS**        | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **ZeroMQ**        | :hammer_and_wrench: WIP :hammer_and_wrench:             | :mag: planning :mag:                        |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **ActiveMQ**      | :mag: planning :mag:                                    | :mag: planning :mag:                        |
+| **AzureSB**       | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 
 ---
 
 ### ⭐ Support the project ⭐
 
 If you are interested in this project, please give me feedback by:
```

#### html2text {}

```diff
@@ -34,81 +34,82 @@
 mag: | | **Kafka** | :warning: **beta** :warning: | :mag: planning :mag: | |
 **SQS** | :warning: **beta** :warning: | :mag: planning :mag: | | **NatsJS** |
 :warning: **beta** :warning: | :mag: planning :mag: | | **ZeroMQ** | :
 hammer_and_wrench: WIP :hammer_and_wrench: | :mag: planning :mag: | | **MQTT**
 | :mag: planning :mag: | :mag: planning :mag: | | **Redis Streams** | :mag:
 planning :mag: | :mag: planning :mag: | | **Pulsar** | :mag: planning :mag: | :
 mag: planning :mag: | | **ActiveMQ** | :mag: planning :mag: | :mag: planning :
-mag: | --- ### â­ Support the project â­ If you are interested in this
-project, please give me feedback by: - giving the [repository](https://
-github.com/Lancetnik/Propan) a star - tweet about **Propan** and let me and
-others know why you use it - joining Discord_server Your support helps me to
-stay in touch with you and encourages to continue developing and improving the
-library. Thank you for your support! Really, share information about this
-project with others. The bigger community we have - the better project will be!
---- ## Declarative? With declarative tools you can define **what you need to
-get**. With traditional imperative tools you must write **what you need to
-do**. Take a look at classic imperative tools, such as aio-pika, pika, redis-
-py, nats-py, etc. This is the **Quickstart** with the *aio-pika*: ```python
-import asyncio import aio_pika async def main(): connection = await
-aio_pika.connect_robust( "amqp://guest:guest@127.0.0.1/" ) queue_name =
-"test_queue" async with connection: channel = await connection.channel() queue
-= await channel.declare_queue(queue_name) async with queue.iterator() as
-queue_iter: async for message in queue_iter: async with message.process():
-print(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
-really easy learning curve. But it's still imperative. You need to *connect*,
-declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
-*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
-way, but it can be much easier. ```python from propan import PropanApp,
-RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
-print(body) ``` This is the **Propan** declarative way to write the same code.
-That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
-```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
-nats]" # or pip install "propan[async-redis]" # or pip install "propan[async-
-kafka]" # or pip install "propan[async-sqs]" ``` ### Basic usage Create an
-application with the following code at `serve.py`: ```python from propan import
-PropanApp from propan import RabbitBroker # from propan import RedisBroker #
-from propan import NatsBroker # from propan import SQSBroker # from propan
-import KafkaBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
-# broker = NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://
-localhost:6379") # broker = SQSBroker("http://localhost:9324", ...) # broker =
-KafkaBroker("localhost:9092") app = PropanApp(broker) @broker.handle("test")
-async def base_handler(body): print(body) ``` And just run it: ```shell propan
-run serve:app --workers 3 ``` --- ## Type casting Propan uses `pydantic` to
-cast incoming function arguments to types according to their annotation.
-```python from pydantic import BaseModel from propan import PropanApp,
-RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(broker) class SimpleMessage(BaseModel): key: int @broker.handle
-("test2") async def second_handler(body: SimpleMessage): assert isinstance
-(body.key, int) ``` --- ## Dependencies **Propan** a has dependencies
-management policy close to `pytest fixtures`. You can specify in functions
-arguments which dependencies you would to use. Framework passes them from the
-global Context object. Also, you can specify your own dependencies, call
-dependencies functions (like `FastAPI Depends`) and [more](https://github.com/
-Lancetnik/Propan/tree/main/examples/dependencies). ```python from propan import
-PropanApp, RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") app = PropanApp(rabbit_broker) async def
-dependency(user_id: int) -> bool: return True @rabbit_broker.handle("test")
-async def base_handler(user_id: int, dep: bool = Depends(dependency), broker:
-RabbitBroker = Context()): assert dep is True assert broker is rabbit_broker
-``` --- ## RPC over MQ Also, **Propan** allows you to use **RPC** requests over
-your broker with a simple way: ```python from propan import PropanApp,
-RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(rabbit_broker) @broker.handle("ping") async def base_handler():
-return "pong" @app.after_startup async def self_ping(): assert ( await
-broker.publish("", "ping", callback=True) ) == "pong" ``` --- ## Project
-Documentation **Propan** automatically generates documentation for your project
-according to the **AsyncAPI** specification. You can work with both generated
-artifacts and place a Web view of your documentation on resources available to
-related teams. The availability of such documentation significantly simplifies
-the integration of services: you can immediately see what channels and message
-format the application works with. And most importantly, it doesn't cost you
-anything - **Propan** has already done everything for you! ![HTML-page](https:/
-/lancetnik.github.io/Propan/assets/img/docs-html-short.png) --- ## CLI power
+mag: | | **AzureSB** | :mag: planning :mag: | :mag: planning :mag: | --- ###
+â­ Support the project â­ If you are interested in this project, please give
+me feedback by: - giving the [repository](https://github.com/Lancetnik/Propan)
+a star - tweet about **Propan** and let me and others know why you use it -
+joining Discord_server Your support helps me to stay in touch with you and
+encourages to continue developing and improving the library. Thank you for your
+support! Really, share information about this project with others. The bigger
+community we have - the better project will be! --- ## Declarative? With
+declarative tools you can define **what you need to get**. With traditional
+imperative tools you must write **what you need to do**. Take a look at classic
+imperative tools, such as aio-pika, pika, redis-py, nats-py, etc. This is the
+**Quickstart** with the *aio-pika*: ```python import asyncio import aio_pika
+async def main(): connection = await aio_pika.connect_robust( "amqp://guest:
+guest@127.0.0.1/" ) queue_name = "test_queue" async with connection: channel =
+await connection.channel() queue = await channel.declare_queue(queue_name)
+async with queue.iterator() as queue_iter: async for message in queue_iter:
+async with message.process(): print(message.body) asyncio.run(main()) ```
+**aio-pika** is a great tool with a really easy learning curve. But it's still
+imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by
+yourself. Also, you need to manage *connection*, *message*, *queue* context to
+avoid any troubles. It is not a bad way, but it can be much easier. ```python
+from propan import PropanApp, RabbitBroker broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") app = PropanApp(broker) @broker.handle("test_queue")
+async def base_handler(body): print(body) ``` This is the **Propan**
+declarative way to write the same code. That is so much easier, isn't it? --
+- ## Quickstart Install using `pip`: ```shell pip install "propan[async-
+rabbit]" # or pip install "propan[async-nats]" # or pip install "propan[async-
+redis]" # or pip install "propan[async-kafka]" # or pip install "propan[async-
+sqs]" ``` ### Basic usage Create an application with the following code at
+`serve.py`: ```python from propan import PropanApp from propan import
+RabbitBroker # from propan import RedisBroker # from propan import NatsBroker #
+from propan import SQSBroker # from propan import KafkaBroker broker =
+RabbitBroker("amqp://guest:guest@localhost:5672/") # broker = NatsBroker("nats:
+//localhost:4222") # broker = RedisBroker("redis://localhost:6379") # broker =
+SQSBroker("http://localhost:9324", ...) # broker = KafkaBroker("localhost:
+9092") app = PropanApp(broker) @broker.handle("test") async def base_handler
+(body): print(body) ``` And just run it: ```shell propan run serve:app --
+workers 3 ``` --- ## Type casting Propan uses `pydantic` to cast incoming
+function arguments to types according to their annotation. ```python from
+pydantic import BaseModel from propan import PropanApp, RabbitBroker broker =
+RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp(broker)
+class SimpleMessage(BaseModel): key: int @broker.handle("test2") async def
+second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` --
+- ## Dependencies **Propan** a has dependencies management policy close to
+`pytest fixtures`. You can specify in functions arguments which dependencies
+you would to use. Framework passes them from the global Context object. Also,
+you can specify your own dependencies, call dependencies functions (like
+`FastAPI Depends`) and [more](https://github.com/Lancetnik/Propan/tree/main/
+examples/dependencies). ```python from propan import PropanApp, RabbitBroker,
+Context, Depends rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:
+5672/") app = PropanApp(rabbit_broker) async def dependency(user_id: int) -
+> bool: return True @rabbit_broker.handle("test") async def base_handler
+(user_id: int, dep: bool = Depends(dependency), broker: RabbitBroker = Context
+()): assert dep is True assert broker is rabbit_broker ``` --- ## RPC over MQ
+Also, **Propan** allows you to use **RPC** requests over your broker with a
+simple way: ```python from propan import PropanApp, RabbitBroker broker =
+RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
+(rabbit_broker) @broker.handle("ping") async def base_handler(): return "pong"
+@app.after_startup async def self_ping(): assert ( await broker.publish("",
+"ping", callback=True) ) == "pong" ``` --- ## Project Documentation **Propan**
+automatically generates documentation for your project according to the
+**AsyncAPI** specification. You can work with both generated artifacts and
+place a Web view of your documentation on resources available to related teams.
+The availability of such documentation significantly simplifies the integration
+of services: you can immediately see what channels and message format the
+application works with. And most importantly, it doesn't cost you anything -
+**Propan** has already done everything for you! ![HTML-page](https://
+lancetnik.github.io/Propan/assets/img/docs-html-short.png) --- ## CLI power
 **Propan** has its own CLI tool that provided the following features: * project
 generation * multiprocessing workers * project hot reloading * documentation
 generating and hosting * custom command line arguments passing ### Context
 passing For example: pass your current *.env* project setting to context
 ```bash propan run serve:app --env=.env.dev ``` ```python from propan import
 PropanApp, RabbitBroker from propan.annotations import ContextRepo from
 pydantic import BaseSettings broker = RabbitBroker("amqp://guest:
```

### Comparing `propan-0.1.5.1/pyproject.toml` & `propan-0.1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,16 @@
 
 dev-doc = [
     "mkdocs-material >=8.1.4,<9.0.0",
     "mkdocs-static-i18n",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-macros-plugin",
     "mkdocs-glightbox",
+    "pillow",
+    "cairosvg",
 
     "typer[all]",
 ]
 
 dev = [
     "propan[test]",
     "propan[dev-doc]",
```

### Comparing `propan-0.1.5.1/PKG-INFO` & `propan-0.1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -56,19 +56,21 @@
 Requires-Dist: propan[dev-doc]; extra == 'dev'
 Requires-Dist: propan[test]; extra == 'dev'
 Requires-Dist: ruff==0.0.275; extra == 'dev'
 Requires-Dist: typer[all]; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Requires-Dist: types-redis; extra == 'dev'
 Provides-Extra: dev-doc
+Requires-Dist: cairosvg; extra == 'dev-doc'
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'dev-doc'
 Requires-Dist: mkdocs-glightbox; extra == 'dev-doc'
 Requires-Dist: mkdocs-macros-plugin; extra == 'dev-doc'
 Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'dev-doc'
 Requires-Dist: mkdocs-static-i18n; extra == 'dev-doc'
+Requires-Dist: pillow; extra == 'dev-doc'
 Requires-Dist: typer[all]; extra == 'dev-doc'
 Provides-Extra: doc
 Requires-Dist: email-validator>=2.0.0; extra == 'doc'
 Requires-Dist: fastapi; extra == 'doc'
 Requires-Dist: jsonref; extra == 'doc'
 Requires-Dist: polyfactory>=2.5.0; python_version > '3.7' and extra == 'doc'
 Requires-Dist: pyyaml; extra == 'doc'
@@ -165,14 +167,15 @@
 | **SQS**           | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **NatsJS**        | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **ZeroMQ**        | :hammer_and_wrench: WIP :hammer_and_wrench:             | :mag: planning :mag:                        |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **ActiveMQ**      | :mag: planning :mag:                                    | :mag: planning :mag:                        |
+| **AzureSB**       | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 
 ---
 
 ### ⭐ Support the project ⭐
 
 If you are interested in this project, please give me feedback by:
```

